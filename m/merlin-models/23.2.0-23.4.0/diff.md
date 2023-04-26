# Comparing `tmp/merlin-models-23.2.0.tar.gz` & `tmp/merlin-models-23.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-models-23.2.0.tar", last modified: Wed Mar  8 17:23:25 2023, max compression
+gzip compressed data, was "merlin-models-23.4.0.tar", last modified: Wed Apr 26 20:35:57 2023, max compression
```

## Comparing `merlin-models-23.2.0.tar` & `merlin-models-23.4.0.tar`

### file list

```diff
@@ -1,454 +1,457 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-08 16:24:33.000000 merlin-models-23.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-03-08 16:24:33.000000 merlin-models-23.2.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-03-08 16:24:33.000000 merlin-models-23.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-03-08 16:24:33.000000 merlin-models-23.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-08 16:24:33.000000 merlin-models-23.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-03-08 17:23:25.773296 merlin-models-23.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7606 2023-03-08 16:24:33.000000 merlin-models-23.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.589295 merlin-models-23.2.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.605295 merlin-models-23.2.0/merlin/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.605295 merlin-models-23.2.0/merlin/datasets/advertising/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/advertising/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.605295 merlin-models-23.2.0/merlin/datasets/advertising/criteo/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/advertising/criteo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/advertising/criteo/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.605295 merlin-models-23.2.0/merlin/datasets/advertising/criteo/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/advertising/criteo/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.609295 merlin-models-23.2.0/merlin/datasets/ecommerce/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.609295 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.609295 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.609295 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.613295 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.613295 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.613295 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.613295 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.617295 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/preprocessed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.617295 merlin-models-23.2.0/merlin/datasets/ecommerce/large/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/large/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/large/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.617295 merlin-models-23.2.0/merlin/datasets/ecommerce/small/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/small/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/small/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.617295 merlin-models-23.2.0/merlin/datasets/ecommerce/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.617295 merlin-models-23.2.0/merlin/datasets/entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.621295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.621295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/100k/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/100k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.621295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9494 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.621295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.625295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.625295 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/25m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/25m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/movielens/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.625295 merlin-models-23.2.0/merlin/datasets/entertainment/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/music_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/music_streaming/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.625295 merlin-models-23.2.0/merlin/datasets/entertainment/tenrec_video/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/tenrec_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.625295 merlin-models-23.2.0/merlin/datasets/social/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/social/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.629295 merlin-models-23.2.0/merlin/datasets/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.629295 merlin-models-23.2.0/merlin/datasets/testing/sequence_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/testing/sequence_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/datasets/testing/sequence_testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/merlin/models/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-08 17:23:25.773296 merlin-models-23.2.0/merlin/models/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.633295 merlin-models-23.2.0/merlin/models/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.633295 merlin-models-23.2.0/merlin/models/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.633295 merlin-models-23.2.0/merlin/models/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/lightfm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.633295 merlin-models-23.2.0/merlin/models/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.637295 merlin-models-23.2.0/merlin/models/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.641295 merlin-models-23.2.0/merlin/models/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15357 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.641295 merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18840 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.645295 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/blocks/sampling/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.649295 merlin-models-23.2.0/merlin/models/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28901 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20297 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/core/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.649295 merlin-models-23.2.0/merlin/models/tf/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/distributed/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.649295 merlin-models-23.2.0/merlin/models/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/experimental/sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.653295 merlin-models-23.2.0/merlin/models/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13149 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/inputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/inputs/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    46545 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/inputs/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.653295 merlin-models-23.2.0/merlin/models/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/losses/listwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/losses/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.657295 merlin-models-23.2.0/merlin/models/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/metrics/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20292 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/metrics/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.661296 merlin-models-23.2.0/merlin/models/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86207 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    22994 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    21691 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.661296 merlin-models-23.2.0/merlin/models/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    12343 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.665295 merlin-models-23.2.0/merlin/models/tf/outputs/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/sampling/popularity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/outputs/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.669295 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/prediction_tasks/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.669295 merlin-models-23.2.0/merlin/models/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16399 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transformers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transformers/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.673296 merlin-models-23.2.0/merlin/models/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    39922 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)    34346 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/transforms/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.677296 merlin-models-23.2.0/merlin/models/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/repr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17570 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16036 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/tf/utils/tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.677296 merlin-models-23.2.0/merlin/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.681295 merlin-models-23.2.0/merlin/models/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/block/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/block/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.685296 merlin-models-23.2.0/merlin/models/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/features/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/features/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.685296 merlin-models-23.2.0/merlin/models/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/model/prediction_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.689296 merlin-models-23.2.0/merlin/models/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/tabular/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/tabular/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/tabular/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.689296 merlin-models-23.2.0/merlin/models/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/utils/examples_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/torch/utils/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.693296 merlin-models-23.2.0/merlin/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/example_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8015 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/nvt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/utils/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.693296 merlin-models-23.2.0/merlin/models/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-03-08 16:24:33.000000 merlin-models-23.2.0/merlin/models/xgb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.697296 merlin-models-23.2.0/merlin_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-03-08 17:23:25.000000 merlin-models-23.2.0/merlin_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13952 2023-03-08 17:23:25.000000 merlin-models-23.2.0/merlin_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 17:23:25.000000 merlin-models-23.2.0/merlin_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-08 17:23:25.000000 merlin-models-23.2.0/merlin_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-08 17:23:25.000000 merlin-models-23.2.0/merlin_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-08 16:24:33.000000 merlin-models-23.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.697296 merlin-models-23.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/horovod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/implicit.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/lightfm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/transformers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-08 16:24:33.000000 merlin-models-23.2.0/requirements/xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-03-08 17:23:25.773296 merlin-models-23.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-03-08 16:24:33.000000 merlin-models-23.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.697296 merlin-models-23.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.701296 merlin-models-23.2.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.701296 merlin-models-23.2.0/tests/common/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.705296 merlin-models-23.2.0/tests/common/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_tests_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    29092 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/common/tf/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.705296 merlin-models-23.2.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.709296 merlin-models-23.2.0/tests/integration/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.709296 merlin-models-23.2.0/tests/integration/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/retrieval/test_integration_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.709296 merlin-models-23.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.709296 merlin-models-23.2.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/config/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.713296 merlin-models-23.2.0/tests/unit/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/test_advertising.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/test_ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/test_entertainment.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/test_social.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/datasets/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.713296 merlin-models-23.2.0/tests/unit/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/implicit/test_implicit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.713296 merlin-models-23.2.0/tests/unit/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/lightfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/lightfm/test_lightfm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.717296 merlin-models-23.2.0/tests/unit/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.721296 merlin-models-23.2.0/tests/unit/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.721296 merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.721296 merlin-models-23.2.0/tests/unit/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/sampling/test_in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/test_dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27012 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/blocks/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.729296 merlin-models-23.2.0/tests/unit/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/core/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.737296 merlin-models-23.2.0/tests/unit/tf/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_07_train_traditional_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.737296 merlin-models-23.2.0/tests/unit/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/experimental/test_sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.737296 merlin-models-23.2.0/tests/unit/tf/horovod/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/horovod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5992 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/horovod/test_horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.741296 merlin-models-23.2.0/tests/unit/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7231 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    28763 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/inputs/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.741296 merlin-models-23.2.0/tests/unit/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/layers/test_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.745296 merlin-models-23.2.0/tests/unit/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/losses/test_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.745296 merlin-models-23.2.0/tests/unit/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/metrics/test_metrics_popularity.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/metrics/test_metrics_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.749296 merlin-models-23.2.0/tests/unit/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54929 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/models/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    17411 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/models/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/models/test_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.753296 merlin-models-23.2.0/tests/unit/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31909 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9651 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/outputs/test_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.757296 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/test_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.757296 merlin-models-23.2.0/tests/unit/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transformers/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transformers/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.761296 merlin-models-23.2.0/tests/unit/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    40072 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/transforms/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.761296 merlin-models-23.2.0/tests/unit/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/utils/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/tf/utils/test_tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.765296 merlin-models-23.2.0/tests/unit/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.765296 merlin-models-23.2.0/tests/unit/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/block/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/block/test_mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.769297 merlin-models-23.2.0/tests/unit/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/features/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/features/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/features/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.769297 merlin-models-23.2.0/tests/unit/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/model/test_head.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/model/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/tests/unit/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/tabular/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/tabular/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/tabular/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/test_dataloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/test_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/tests/unit/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/torch/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/utils/test_schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 17:23:25.773296 merlin-models-23.2.0/tests/unit/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/xgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tests/unit/xgb/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-03-08 16:24:33.000000 merlin-models-23.2.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-03-08 16:24:33.000000 merlin-models-23.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-26 19:35:34.000000 merlin-models-23.4.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-26 19:35:34.000000 merlin-models-23.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-04-26 19:35:34.000000 merlin-models-23.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-26 19:35:34.000000 merlin-models-23.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-26 20:35:57.823311 merlin-models-23.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-04-26 19:35:34.000000 merlin-models-23.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.635310 merlin-models-23.4.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.647310 merlin-models-23.4.0/merlin/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/criteo/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.651310 merlin-models-23.4.0/merlin/datasets/ecommerce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.655310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.659310 merlin-models-23.4.0/merlin/datasets/ecommerce/large/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/large/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/large/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/ecommerce/small/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/small/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/small/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.663310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/movielens/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.667310 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/social/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.671310 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/merlin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-26 20:35:57.823311 merlin-models-23.4.0/merlin/models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/lightfm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.675310 merlin-models-23.4.0/merlin/models/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.679310 merlin-models-23.4.0/merlin/models/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.679310 merlin-models-23.4.0/merlin/models/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15357 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.683310 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.683310 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/blocks/sampling/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.687310 merlin-models-23.4.0/merlin/models/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16052 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20972 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/core/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.687310 merlin-models-23.4.0/merlin/models/tf/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/distributed/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/experimental/sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/inputs/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17172 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.691310 merlin-models-23.4.0/merlin/models/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/listwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/losses/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.695310 merlin-models-23.4.0/merlin/models/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11974 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/metrics/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.699310 merlin-models-23.4.0/merlin/models/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100235 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23180 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.699310 merlin-models-23.4.0/merlin/models/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16782 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.703310 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/sampling/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/outputs/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.703310 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/prediction_tasks/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.707310 merlin-models-23.4.0/merlin/models/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transformers/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.707310 merlin-models-23.4.0/merlin/models/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53093 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46929 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/transforms/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/repr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18363 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/tf/utils/tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.711310 merlin-models-23.4.0/merlin/models/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/block/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.715310 merlin-models-23.4.0/merlin/models/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/features/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.715310 merlin-models-23.4.0/merlin/models/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21538 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/model/prediction_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.723311 merlin-models-23.4.0/merlin/models/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21965 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/tabular/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.727311 merlin-models-23.4.0/merlin/models/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/examples_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/torch/utils/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.731311 merlin-models-23.4.0/merlin/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/example_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/nvt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/utils/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.731311 merlin-models-23.4.0/merlin/models/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-04-26 19:35:34.000000 merlin-models-23.4.0/merlin/models/xgb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.735311 merlin-models-23.4.0/merlin_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14045 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 20:35:57.000000 merlin-models-23.4.0/merlin_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-26 19:35:34.000000 merlin-models-23.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 19:35:34.000000 merlin-models-23.4.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/horovod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/implicit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/lightfm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/transformers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 19:35:34.000000 merlin-models-23.4.0/requirements/xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-26 20:35:57.823311 merlin-models-23.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-26 19:35:34.000000 merlin-models-23.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.739311 merlin-models-23.4.0/tests/common/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.743311 merlin-models-23.4.0/tests/common/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_tests_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29117 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/common/tf/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.743311 merlin-models-23.4.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/integration/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/integration/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/retrieval/test_integration_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.747311 merlin-models-23.4.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/config/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.751311 merlin-models-23.4.0/tests/unit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_advertising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_entertainment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/datasets/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.755311 merlin-models-23.4.0/tests/unit/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/implicit/test_implicit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.755311 merlin-models-23.4.0/tests/unit/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/lightfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/lightfm/test_lightfm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.759311 merlin-models-23.4.0/tests/unit/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.763311 merlin-models-23.4.0/tests/unit/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.763311 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.767311 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8397 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/blocks/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.771311 merlin-models-23.4.0/tests/unit/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/core/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.779311 merlin-models-23.4.0/tests/unit/tf/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_07_train_traditional_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.779311 merlin-models-23.4.0/tests/unit/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/experimental/test_sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.783311 merlin-models-23.4.0/tests/unit/tf/horovod/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/horovod/test_horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.787311 merlin-models-23.4.0/tests/unit/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28970 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/inputs/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.787311 merlin-models-23.4.0/tests/unit/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/layers/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.791311 merlin-models-23.4.0/tests/unit/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/losses/test_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.791311 merlin-models-23.4.0/tests/unit/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_popularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.795311 merlin-models-23.4.0/tests/unit/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17376 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36730 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/models/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.799311 merlin-models-23.4.0/tests/unit/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9083 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/outputs/test_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.803311 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/test_public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.803311 merlin-models-23.4.0/tests/unit/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17308 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transformers/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.807311 merlin-models-23.4.0/tests/unit/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39661 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/transforms/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.807311 merlin-models-23.4.0/tests/unit/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/tf/utils/test_tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.811311 merlin-models-23.4.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.811311 merlin-models-23.4.0/tests/unit/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/block/test_mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.815311 merlin-models-23.4.0/tests/unit/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9030 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/features/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.815311 merlin-models-23.4.0/tests/unit/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/test_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/model/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/tabular/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_dataloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/test_public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/torch/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.819311 merlin-models-23.4.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/utils/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:35:57.823311 merlin-models-23.4.0/tests/unit/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/xgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tests/unit/xgb/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-26 19:35:34.000000 merlin-models-23.4.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-04-26 19:35:34.000000 merlin-models-23.4.0/versioneer.py
```

### Comparing `merlin-models-23.2.0/.pre-commit-config.yaml` & `merlin-models-23.4.0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 repos:
   - repo: https://github.com/timothycrosley/isort
-    rev: 5.6.4
+    rev: 5.12.0
     hooks:
       - id: isort
         additional_dependencies: [toml]
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.1.0
     hooks:
       - id: black
   - repo: https://github.com/pycqa/flake8
-    rev: 3.8.4
+    rev: 6.0.0
     hooks:
       - id: flake8
         args: ["--extend-ignore=E203,W503"]
   - repo: https://github.com/MarcoGorelli/absolufy-imports
     rev: v0.3.1
     hooks:
       - id: absolufy-imports
@@ -21,21 +21,21 @@
     rev: 1.5.0
     hooks:
       - id: interrogate
         exclude: ^(docs|examples|tests|setup.py|versioneer.py)
         args: [--config=pyproject.toml]
   # yaml formatting
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.3.0
+    rev: v3.0.0-alpha.4
     hooks:
       - id: prettier
         types: [yaml]
         exclude: ^.github|^conda
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.2
     hooks:
       - id: codespell
         exclude: retrieval-with-hyperparameter-optimization
   - repo: local
     hooks:
       - id: lint-tensorflow
         name: lint-tensorflow
```

### Comparing `merlin-models-23.2.0/CLA.md` & `merlin-models-23.4.0/CLA.md`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/CONTRIBUTING.md` & `merlin-models-23.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/LICENSE` & `merlin-models-23.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/MANIFEST.in` & `merlin-models-23.4.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/PKG-INFO` & `merlin-models-23.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.2.0
+Version: 23.4.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
 Description: ## Merlin Models
         
         [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
@@ -116,15 +116,15 @@
         You can find more details and information about a low-level API in our overview of the
         [Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
         
         ### Notebook Examples and Tutorials
         
         View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
         
-        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repostory.
+        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
         
         ### Feedback and Support
         
         If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
         We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
         To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
```

### Comparing `merlin-models-23.2.0/README.md` & `merlin-models-23.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -109,14 +109,14 @@
 You can find more details and information about a low-level API in our overview of the
 [Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
 
 ### Notebook Examples and Tutorials
 
 View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
 
-The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repostory.
+The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
 
 ### Feedback and Support
 
 If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
 To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
```

### Comparing `merlin-models-23.2.0/merlin/datasets/__init__.py` & `merlin-models-23.4.0/merlin/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/advertising/__init__.py` & `merlin-models-23.4.0/merlin/datasets/advertising/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/advertising/criteo/__init__.py` & `merlin-models-23.4.0/merlin/datasets/advertising/criteo/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/advertising/criteo/dataset.py` & `merlin-models-23.4.0/merlin/datasets/advertising/criteo/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/advertising/criteo/transformed/__init__.py` & `merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/dataset.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/booking/dataset.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
       value: "\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\017\n\tis_ragged\022\002 \000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\024@\n\r\n\007is_list\022\002 \000\n\021\n\013num_buckets\022\002\010\000\n7\n\010cat_path\022+\032).//categories/unique.device_class.parquet\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000"
     }
   }
 }
 feature {
   name: "booker_country"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "booker_country"
     max: 6
     is_categorical: true
@@ -82,15 +82,15 @@
       value: "\n\021\n\013num_buckets\022\002\010\000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\r\n\007is_list\022\002 \001\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\034@\n9\n\010cat_path\022-\032+.//categories/unique.booker_country.parquet\n\017\n\tis_ragged\022\002 \001"
     }
   }
 }
 feature {
   name: "hotel_country"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "hotel_country"
     max: 196
     is_categorical: true
@@ -103,15 +103,15 @@
       value: "\n8\n\010cat_path\022,\032*.//categories/unique.hotel_country.parquet\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \001\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\000?@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\240h@\n\r\n\007is_list\022\002 \001\n\021\n\013num_buckets\022\002\010\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?"
     }
   }
 }
 feature {
   name: "month"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "month"
     max: 13
     is_categorical: true
@@ -124,15 +124,15 @@
       value: "\n\017\n\tis_ragged\022\002 \001\n0\n\010cat_path\022$\032\".//categories/unique.month.parquet\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\021\n\013num_buckets\022\002\010\000\n\r\n\007is_list\022\002 \001\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000,@\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@"
     }
   }
 }
 feature {
   name: "is_weekend"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "is_weekend"
     max: 3
     is_categorical: true
@@ -145,15 +145,15 @@
       value: "\n\r\n\007is_list\022\002 \001\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \001\n5\n\010cat_path\022)\032\'.//categories/unique.is_weekend.parquet\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n\021\n\013num_buckets\022\002\010\000\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\020@\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@"
     }
   }
 }
 feature {
   name: "weekday_checkin"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "weekday_checkin"
     max: 8
     is_categorical: true
@@ -166,15 +166,15 @@
       value: "\n:\n\010cat_path\022.\032,.//categories/unique.weekday_checkin.parquet\n\r\n\007is_list\022\002 \001\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\017\n\tis_ragged\022\002 \001\n\021\n\013num_buckets\022\002\010\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\nG\n\017embedding_sizes\0224*2\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\"@\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@"
     }
   }
 }
 feature {
   name: "weekday_checkout"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "weekday_checkout"
     max: 8
     is_categorical: true
@@ -187,15 +187,15 @@
       value: "\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\r\n\007is_list\022\002 \001\n\017\n\tis_ragged\022\002 \001\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000P@\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\360?\n;\n\010cat_path\022/\032-.//categories/unique.weekday_checkout.parquet\n\021\n\013num_buckets\022\002\010\000\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\0000@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\000\"@"
     }
   }
 }
 feature {
   name: "city_id"
   value_count {
-    min: 1
+    min: 4
     max: 48
   }
   type: INT
   int_domain {
     name: "city_id"
     max: 39902
     is_categorical: true
```

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/dataset.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/large/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/large/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/large/schema.json` & `merlin-models-23.4.0/merlin/datasets/ecommerce/large/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/small/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/small/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/small/schema.json` & `merlin-models-23.4.0/merlin/datasets/ecommerce/small/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/transactions/__init__.py` & `merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/ecommerce/transactions/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/ecommerce/transactions/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/100k/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/100k/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,15 @@
       value: "\n\017\n\tis_ragged\022\002 \000\n\r\n\007is_list\022\002 \000\n\033\n\016freq_threshold\022\t\021\000\000\000\000\000\000\000\000\n\025\n\010max_size\022\t\021\000\000\000\000\000\000\000\000\n\030\n\013start_index\022\t\021\000\000\000\000\000\000\000\000\n\021\n\013num_buckets\022\002\010\000\nG\n\017embedding_sizes\0224*2\n\026\n\tdimension\022\t\021\000\000\000\000\000\340c@\n\030\n\013cardinality\022\t\021\000\000\000\000\000\310\254@\n0\n\010cat_path\022$\032\".//categories/unique.title.parquet\n\034\n\017dtype_item_size\022\t\021\000\000\000\000\000\000@@"
     }
   }
 }
 feature {
   name: "genres"
   value_count {
-    min: 1
-    max: 6
+    min: 1    
   }
   type: INT
   int_domain {
     name: "genres"
     max: 18
     is_categorical: true
   }
```

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/25m/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/movielens/dataset.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/movielens/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/music_streaming/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/music_streaming/schema.json` & `merlin-models-23.4.0/merlin/datasets/entertainment/music_streaming/schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930288461538461%*

 * *Differences: {"'feature'": "{0: {'annotation': {'tag': {delete: [0]}}}, 4: {'valueCount': {'min': '4', delete: "*

 * *              "['max']}}, 8: {'valueCount': {'min': '4', delete: ['max']}}}"}*

```diff
@@ -1,13 +1,12 @@
 {
     "feature": [
         {
             "annotation": {
                 "tag": [
-                    "categorical",
                     "session_id"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
                 "max": "10000",
                 "name": "session_id"
@@ -71,16 +70,15 @@
                 "isCategorical": true,
                 "max": "100",
                 "name": "genres"
             },
             "name": "item_genres",
             "type": "INT",
             "valueCount": {
-                "max": "20",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "categorical",
                     "user_id"
@@ -135,16 +133,15 @@
                 "isCategorical": true,
                 "max": "100",
                 "name": "genres"
             },
             "name": "user_genres",
             "type": "INT",
             "valueCount": {
-                "max": "20",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "bias",
                     "continuous"
```

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/tenrec_video/__init__.py` & `merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt` & `merlin-models-23.4.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/social/__init__.py` & `merlin-models-23.4.0/merlin/datasets/social/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/social/schema.json` & `merlin-models-23.4.0/merlin/datasets/social/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/synthetic.py` & `merlin-models-23.4.0/merlin/datasets/synthetic.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 #
 import difflib
 import logging
 import os
 import pathlib
 from pathlib import Path
 from random import randint
-from typing import Dict, Optional, Sequence, Tuple, Union
+from typing import Dict, Sequence, Tuple, Union
 
 import numpy as np
 
 import merlin.io
 from merlin.models.utils import schema_utils
-from merlin.schema import ColumnSchema, Schema, Tags
+from merlin.schema import Schema, Tags
 from merlin.schema.io.tensorflow_metadata import TensorflowMetadata
 
 LOG = logging.getLogger("merlin-models")
 HERE = pathlib.Path(__file__).parent
 KNOWN_DATASETS: Dict[str, Path] = {
     "e-commerce": HERE / "ecommerce/small",
     "e-commerce-large": HERE / "ecommerce/large",
@@ -52,15 +52,15 @@
 }
 
 
 def generate_data(
     input: Union[Schema, Path, str],
     num_rows: int,
     set_sizes: Sequence[float] = (1.0,),
-    min_session_length=4,
+    min_session_length=None,
     max_session_length=None,
     device="cpu",
 ) -> Union[merlin.io.Dataset, Tuple[merlin.io.Dataset, ...]]:
     """
     Generate synthetic data from a schema or one of the known datasets.
 
     Known fully synthetic datasets:
@@ -88,17 +88,21 @@
     set_sizes: Sequence[float], default=(1.0,)
         This parameter allows outputting multiple datasets, where each
         dataset is a subset of the original dataset.
 
         Example::
             train, valid = generate_data(input, 10000, (0.8, 0.2))
     min_session_length: int
-        The minimum number of events in a session.
+        The minimum number of events in a session. Overrides the
+        min sequence length information from the shape of list columns
+        schema (schema[col].shape.dims[1].min)
     max_session_length: int
-        The maximum number of events in a session.
+        The minimum number of events in a session. Overrides the
+        max sequence length information from the shape of list columns
+        schema (schema[col].shape.dims[1].max)
     device: str
         The device to use for the data generation.
         Supported values: {'cpu', 'gpu'}
 
     Returns
     -------
     merlin.io.Dataset
@@ -115,31 +119,23 @@
         schema = _get_schema(input)
     elif isinstance(input, Schema):
         schema = input
     else:
         raise ValueError(f"Unknown input type: {type(input)}")
 
     for col in schema.column_names:
-        if not schema[col].is_list:
-            continue
-        new_properties = schema[col].properties
-        new_properties["value_count"] = {"min": min_session_length}
-        if max_session_length:
-            new_properties["value_count"]["max"] = max_session_length
-        schema[col] = ColumnSchema(
-            name=schema[col].name,
-            tags=schema[col].tags,
-            properties=new_properties,
-            dtype=schema[col].dtype,
-            is_list=True,
-        )
+        if schema[col].shape.is_list:
+            min_session_length = min_session_length or schema[col].shape.dims[1].min
+            max_session_length = max_session_length or schema[col].shape.dims[1].max
+            # Overriding min and max session length from schema
+            schema[col] = schema[col].with_shape(
+                ((0, None), (min_session_length, max_session_length))
+            )
 
-    df = generate_user_item_interactions(
-        schema, num_rows, min_session_length, max_session_length, device=device
-    )
+    df = generate_user_item_interactions(schema, num_rows, device=device)
 
     if list(set_sizes) != [1.0]:
         num_rows = df.shape[0]
         output_datasets = []
         start_i = 0
         for set_size in set_sizes:
             num_rows_set = int(num_rows * set_size)
@@ -152,16 +148,14 @@
 
     return merlin.io.Dataset(df, schema=schema)
 
 
 def generate_user_item_interactions(
     schema: Schema,
     num_interactions: int,
-    min_session_length: int = 5,
-    max_session_length: Optional[int] = None,
     device: str = "cpu",
 ):
     """
     Util function to generate synthetic data of user-item interactions from a schema object,
     it supports the generation of conditional user, item and session features.
 
     The schema should include a few tags:
@@ -173,18 +167,14 @@
 
     Parameters:
     ----------
     schema: Schema
         schema object describing the columns to generate.
     num_interactions: int
         number of interaction rows to generate.
-    max_session_length: Optional[int]
-        The maximum length of the multi-hot/sequence features
-    min_session_length: int
-        The minimum length of the multi-hot/sequence features
     device: str
         device to use for generating data.
 
     Returns
     -------
     data: DataFrame
        DataFrame with synthetic generated rows,
@@ -211,16 +201,14 @@
         ).astype(str(session_id_col.dtype.to_numpy))
 
         features = list(schema.select_by_tag(Tags.SESSION).remove_by_tag(Tags.SESSION_ID))
         data = generate_conditional_features(
             data,
             features,
             session_id_col,
-            min_session_length=min_session_length,
-            max_session_length=max_session_length,
             device=device,
         )
         processed_cols += [f.name for f in features] + [session_id_col.name]
 
     # get USER cols
     user_id_cols = list(schema.select_by_tag(Tags.USER_ID))
     if user_id_cols:
@@ -231,66 +219,56 @@
             user_id_col.int_domain.max,
         ).astype(str(user_id_col.dtype.to_numpy.name))
         features = list(schema.select_by_tag(Tags.USER).remove_by_tag(Tags.USER_ID))
         data = generate_conditional_features(
             data,
             features,
             user_id_col,
-            min_session_length=min_session_length,
-            max_session_length=max_session_length,
             device=device,
         )
         processed_cols += [f.name for f in features] + [user_id_col.name]
 
     # get ITEM cols
     item_schema = schema.select_by_tag(Tags.ITEM_ID)
     if not len(item_schema) > 0:
         raise ValueError("Item ID column is required")
     item_id_col = item_schema.first
 
-    is_list_feature = item_id_col.is_list
+    is_list_feature = item_id_col.shape.is_list
     if not is_list_feature:
         shape = num_interactions
     else:
-        shape = (num_interactions, max_session_length or min_session_length)  # type: ignore
+        seq_length = item_id_col.shape.dims[1].max or item_id_col.shape.dims[1].min
+        shape = (num_interactions, seq_length)  # type: ignore
     tmp = _array.clip(
         _array.random.lognormal(3.0, 1.0, shape).astype(_array.int32),
         1,
         item_id_col.int_domain.max,
     ).astype(str(item_id_col.dtype.to_numpy.name))
     if isinstance(shape, int):
         data[item_id_col.name] = tmp
     else:
         data[item_id_col.name] = list(tmp)
     features = list(schema.select_by_tag(Tags.ITEM).remove_by_tag(Tags.ITEM_ID))
-    data = generate_conditional_features(
-        data,
-        features,
-        item_id_col,
-        min_session_length=min_session_length,
-        max_session_length=max_session_length,
-        device=device,
-    )
+    data = generate_conditional_features(data, features, item_id_col, device=device)
     processed_cols += [f.name for f in features] + [item_id_col.name]
 
     # Get remaining features
     remaining = schema.without(processed_cols)
 
     for feature in remaining.select_by_tag(Tags.BINARY_CLASSIFICATION):
         data[feature.name] = _array.random.randint(0, 2, num_interactions).astype(
             str(feature.dtype.to_numpy)
         )
 
     for feature in remaining.remove_by_tag(Tags.BINARY_CLASSIFICATION):
         is_int_feature = feature.dtype and np.issubdtype(feature.dtype.to_numpy, np.integer)
         is_list_feature = feature.is_list
         if is_list_feature:
-            data[feature.name] = generate_random_list_feature(
-                feature, num_interactions, min_session_length, max_session_length, device
-            )
+            data[feature.name] = generate_random_list_feature(feature, num_interactions, device)
 
         elif is_int_feature:
             domain = feature.int_domain
             min_value, max_value = (domain.min, domain.max) if domain else (0, 1)
 
             data[feature.name] = _array.random.randint(
                 min_value, max_value, num_interactions, dtype=str(feature.dtype.to_numpy)
@@ -307,16 +285,14 @@
     return data
 
 
 def generate_conditional_features(
     data,
     features,
     parent_feature,
-    min_session_length: int = 5,
-    max_session_length: Optional[int] = None,
     device="cpu",
 ):
     """
     Generate features conditioned by the value of `parent_feature` feature
     """
     if device == "cpu":
         import numpy as _array
@@ -327,17 +303,15 @@
 
     num_interactions = data.shape[0]
     for feature in features:
         is_int_feature = np.issubdtype(feature.dtype.to_numpy, np.integer)
         is_list_feature = feature.is_list
 
         if is_list_feature:
-            data[feature.name] = generate_random_list_feature(
-                feature, num_interactions, min_session_length, max_session_length, device
-            )
+            data[feature.name] = generate_random_list_feature(feature, num_interactions, device)
 
         elif is_int_feature:
             if not feature.int_domain:
                 raise ValueError(
                     "Int domain is required for conditional features, got {}".format(feature)
                 )
 
@@ -360,23 +334,24 @@
 
     return data
 
 
 def generate_random_list_feature(
     feature,
     num_interactions,
-    min_session_length: int = 5,
-    max_session_length: Optional[int] = None,
     device="cpu",
 ):
     if device == "cpu":
         import numpy as _array
     else:
         import cupy as _array
 
+    seq_length_dim = feature.shape.dims[1]
+    min_session_length, max_session_length = seq_length_dim.min, seq_length_dim.max
+
     is_int_feature = np.issubdtype(feature.dtype.to_numpy, np.integer)
     if is_int_feature:
         if max_session_length:
             padded_array = []
             for _ in range(num_interactions):
                 list_length = randint(min_session_length, max_session_length)
                 actual_values = _array.random.randint(
```

### Comparing `merlin-models-23.2.0/merlin/datasets/testing/__init__.py` & `merlin-models-23.4.0/merlin/datasets/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/testing/schema.json` & `merlin-models-23.4.0/merlin/datasets/testing/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/testing/sequence_testing/__init__.py` & `merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/datasets/testing/sequence_testing/schema.json` & `merlin-models-23.4.0/merlin/datasets/testing/sequence_testing/schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9761363636363636%*

 * *Differences: {"'feature'": "{2: {'valueCount': {'min': '4', delete: ['max']}}, 3: {'valueCount': {'min': '4', "*

 * *              "delete: ['max']}}, 4: {'valueCount': {'min': '4', delete: ['max']}}, 5: "*

 * *              "{'valueCount': {'min': '4', delete: ['max']}}, 6: {'valueCount': {'min': '4', "*

 * *              "delete: ['max']}}, 7: {'valueCount': {'min': '4', delete: ['max']}}, 8: "*

 * *              "{'valueCount': {'min': '4', delete: ['max']}}}"}*

```diff
@@ -34,16 +34,15 @@
                 "max": -1.2571640014648438,
                 "min": -2.917728900909424,
                 "name": "item_age_days_norm"
             },
             "name": "item_age_days_norm",
             "type": "FLOAT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "continuous",
                     "item",
@@ -53,16 +52,15 @@
             "floatDomain": {
                 "max": 1.0,
                 "name": "event_hour_sin"
             },
             "name": "event_hour_sin",
             "type": "FLOAT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "continuous",
                     "item",
@@ -72,16 +70,15 @@
             "floatDomain": {
                 "max": 1.0,
                 "name": "event_hour_cos"
             },
             "name": "event_hour_cos",
             "type": "FLOAT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "continuous",
                     "item",
@@ -91,16 +88,15 @@
             "floatDomain": {
                 "max": 1.0,
                 "name": "event_weekday_sin"
             },
             "name": "event_weekday_sin",
             "type": "FLOAT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "continuous",
                     "item",
@@ -110,16 +106,15 @@
             "floatDomain": {
                 "max": 1.0,
                 "name": "event_weekday_cos"
             },
             "name": "event_weekday_cos",
             "type": "FLOAT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "item_id",
                     "categorical",
@@ -132,16 +127,15 @@
                 "max": "51996",
                 "min": "1",
                 "name": "item_id_seq"
             },
             "name": "item_id_seq",
             "type": "INT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "list",
                     "categorical",
@@ -154,16 +148,15 @@
                 "max": "331",
                 "min": "1",
                 "name": "categories"
             },
             "name": "categories",
             "type": "INT",
             "valueCount": {
-                "max": "4",
-                "min": "1"
+                "min": "4"
             }
         },
         {
             "annotation": {
                 "tag": [
                     "categorical",
                     "user"
```

### Comparing `merlin-models-23.2.0/merlin/models/__init__.py` & `merlin-models-23.4.0/merlin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/api.py` & `merlin-models-23.4.0/merlin/models/api.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/config/__init__.py` & `merlin-models-23.4.0/merlin/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/config/schema.py` & `merlin-models-23.4.0/merlin/models/config/schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/io.py` & `merlin-models-23.4.0/merlin/models/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,24 +13,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
 import pathlib
 from typing import Optional, Union
 
-from merlin.models.api import MerlinModel
 from merlin.models.utils.schema_utils import schema_to_tensorflow_metadata_json
 from merlin.schema import Schema
 
 _MERLIN_METADATA_DIR_NAME = ".merlin"
 
 
 def save_merlin_metadata(
     export_path: Union[str, os.PathLike],
-    model: MerlinModel,
     input_schema: Optional[Schema],
     output_schema: Optional[Schema],
 ) -> None:
     """Saves data to Merlin Metadata Directory."""
 
     # When we're asked to save to a path starting with 'ram://'
     # The use-case is for Keras 2.10 and below to serizlize
```

### Comparing `merlin-models-23.2.0/merlin/models/loader/__init__.py` & `merlin-models-23.4.0/merlin/models/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/loader/backend.py` & `merlin-models-23.4.0/merlin/models/loader/backend.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     )
 
 from merlin.models.tf.transforms.features import (
     BroadcastToSequence,
     CategoryEncoding,
     HashedCross,
     HashedCrossAll,
+    PrepareFeatures,
     ToDense,
     ToOneHot,
     ToSparse,
     ToTarget,
 )
 from merlin.models.tf.transforms.noise import StochasticSwapNoise
 from merlin.models.tf.transforms.regularization import L2Norm
@@ -163,15 +164,15 @@
     SequenceMaskLastInference,
     SequenceMaskRandom,
     SequencePredictLast,
     SequencePredictNext,
     SequencePredictRandom,
     SequenceTargetAsInput,
 )
-from merlin.models.tf.transforms.tensor import ExpandDims, ListToDense, ListToRagged, ListToSparse
+from merlin.models.tf.transforms.tensor import ExpandDims
 from merlin.models.tf.utils import repr_utils
 from merlin.models.tf.utils.tf_utils import TensorInitializer
 
 ListWrapper.__repr__ = repr_utils.list_wrapper_repr
 _DictWrapper.__repr__ = repr_utils.dict_wrapper_repr
 
 Dense.repr_extra = repr_utils.dense_extra_repr
@@ -215,17 +216,15 @@
     "Embeddings",
     "FeatureConfig",
     "TableConfig",
     "ParallelPredictionBlock",
     "TwoTowerBlock",
     "MatrixFactorizationBlock",
     "QueryItemIdsEmbeddingsBlock",
-    "ListToDense",
-    "ListToRagged",
-    "ListToSparse",
+    "PrepareFeatures",
     "ToSparse",
     "ToDense",
     "ToTarget",
     "CategoryEncoding",
     "BroadcastToSequence",
     "HashedCross",
     "HashedCrossAll",
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/cross.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/cross.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/dlrm.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/dlrm.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from functools import partial
 from typing import Optional
 
+import tensorflow as tf
+
 from merlin.models.tf.blocks.interaction import DotProductInteraction
+from merlin.models.tf.blocks.mlp import _Dense
 from merlin.models.tf.core.aggregation import StackFeatures
 from merlin.models.tf.core.base import Block, Debug
 from merlin.models.tf.core.combinators import Filter, ParallelBlock, SequentialBlock
 from merlin.models.tf.inputs.continuous import ContinuousFeatures
 from merlin.models.tf.inputs.embedding import EmbeddingOptions, Embeddings
 from merlin.models.utils.schema_utils import infer_embedding_dim
 from merlin.schema import Schema, Tags
@@ -132,23 +135,23 @@
         raise ValueError("The embedding_dim is required")
 
     if embedding_options is not None:
         embedding_options.embedding_dim_default = embedding_dim
     else:
         embedding_options = EmbeddingOptions(embedding_dim_default=embedding_dim)
 
-    if (
-        embedding_dim is not None
-        and bottom_block is not None
-        and embedding_dim != bottom_block.layers[-1].units
-    ):
-        raise ValueError(
-            f"The embedding_dim ({embedding_dim}) needs to match the "
-            "last layer of bottom MLP ({bottom_block.layers[-1].units}) "
-        )
+    if embedding_dim is not None and bottom_block is not None:
+        last_bottom_mlp_layer = list(
+            [k for k in bottom_block.layers if isinstance(k, (_Dense, tf.keras.layers.Dense))]
+        )[-1]
+        if embedding_dim != last_bottom_mlp_layer.units:
+            raise ValueError(
+                f"The embedding_dim ({embedding_dim}) needs to match the "
+                "last layer of bottom MLP ({bottom_block.layers[-1].units}) "
+            )
 
     embeddings_kwargs = dict(
         sequence_combiner=embedding_options.combiner,
         embeddings_initializer=embedding_options.embeddings_initializers,
         dim=embedding_options.embedding_dim_default,
         infer_dim_fn=partial(
             infer_embedding_dim,
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/experts.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/experts.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/interaction.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/interaction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/mlp.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/mlp.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/optimizer.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,52 +17,64 @@
 import collections
 import warnings
 from dataclasses import dataclass
 from typing import Callable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import tensorflow as tf
+from packaging import version
 
 import merlin.models.tf as ml
 from merlin.models.tf.core.base import Block
 from merlin.models.tf.core.combinators import ParallelBlock
 from merlin.models.tf.utils import tf_utils
 
 Tensor = Union[tf.Tensor, tf.SparseTensor, tf.RaggedTensor]
 FloatTensorLike = Union[tf.Tensor, float, np.float16, np.float32, np.float64]
 
 
+if version.parse(tf.__version__) < version.parse("2.11.0"):
+    keras_optimizers = tf.keras.optimizers
+else:
+    keras_optimizers = tf.keras.optimizers.legacy
+
+
 @dataclass
 class OptimizerBlocks:
     """dataclass for a pair of optimizer and blocks that the optimizer should apply to.
     Example:
         ml.OptimizerBlocks("sgd", [user_tower, third_tower])
         ml.OptimizerBlocks("adam", item_tower)
     """
 
-    optimizer: Union[str, tf.keras.optimizers.Optimizer]
+    optimizer: Union[str, keras_optimizers.Optimizer]
     blocks: Sequence[Block]
 
     def get_config(self):
         """return a tuple of serialized keras objects"""
+        optimizer_config = tf.keras.utils.serialize_keras_object(self.optimizer)
+        if version.parse(tf.__version__) >= version.parse("2.11.0") and isinstance(
+            self.optimizer, tf.keras.optimizers.legacy.Optimizer
+        ):
+            optimizer_config["use_legacy_optimizer"] = True
         return (
-            tf.keras.utils.serialize_keras_object(self.optimizer),
+            optimizer_config,
             [tf.keras.utils.serialize_keras_object(block) for block in self.blocks],
         )
 
     @classmethod
     def from_config(cls, config):
         return cls(
             tf.keras.optimizers.deserialize(config[0]),
             [tf.keras.layers.deserialize(block) for block in config[1]],
         )
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
-class MultiOptimizer(tf.keras.optimizers.Optimizer):
+class MultiOptimizer(keras_optimizers.Optimizer):
     """An optimizer that composes multiple individual optimizers.
 
     It allows different optimizers to be applied to different subsets of the model's variables. For
     example, it is possible to apply one optimizer to the blocks which contains the model's
     embeddings (sparse variables) and another optimizer to the rest of its variables (other blocks).
 
     To specify which optimizer should apply to each block, pass a list of pairs of (optimizer
@@ -76,16 +88,16 @@
       third_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([64]))
       three_tower = ml.ParallelBlock({"user": user_tower, "item": item_tower, "third": third_tower})
       model = ml.Model(three_tower,  ml.BinaryClassificationTask("click"))
 
       # The third_tower would be assigned the default_optimizer ("adagrad" in this example)
       optimizer = ml.MultiOptimizer(default_optimizer="adagrad",
         optimizers_and_blocks=[
-          ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
-          ml.OptimizerBlocks(tf.keras.optimizers.Adam(), item_tower),
+          ml.OptimizerBlocks(tf.keras.optimizers.legacy.SGD(), user_tower),
+          ml.OptimizerBlocks(tf.keras.optimizers.legacy.Adam(), item_tower),
         ])
 
       # The string identification of optimizer is also acceptable, here "sgd" for the third_tower
       # The variables of BinaryClassificationTask("click") would still use the default_optimizer
       optimizer = ml.MultiOptimizer(default_optimizer="adam",
         optimizers_and_blocks=[
           ml.OptimizerBlocks("sgd", [user_tower, third_tower]),
@@ -94,49 +106,67 @@
     ```
 
     """
 
     def __init__(
         self,
         optimizers_and_blocks: Sequence[OptimizerBlocks],
-        default_optimizer: Union[str, tf.keras.optimizers.Optimizer] = "rmsprop",
+        default_optimizer: Union[str, keras_optimizers.Optimizer] = "rmsprop",
         name: str = "MultiOptimizer",
         **kwargs,
     ):
         """Initializes an MultiOptimizer instance.
 
         Parameters
         ----------
         optimizers_and_blocks: Sequence[OptimizerBlocks]
             List of OptimizerBlocks(dataclass), the OptimizerBlocks contains two items, one is
             optimizer, another one is a list of blocks or a block that the optimizer should apply
             to. See 'class OptimizerBlocks'
-        default_optimizer: Union[str, tf.keras.optimizers.Optimizer]
+        default_optimizer: Union[str, tf.keras.optimizers.legacy.Optimizer]
             Default optimizer for the rest variables not specified in optimizers_and_blocks, by
             default "rmsprop".
         name:str
             The name of MultiOptimizer.
         """
         super().__init__(name=name)
         self.name = name
         if not optimizers_and_blocks:
             raise ValueError("`optimizers_and_blocks` can't be empty")
-        self.default_optimizer = tf.keras.optimizers.get(default_optimizer)
+        self.default_optimizer = self._get_optimizer(default_optimizer)
         self.optimizers_and_blocks = []
         for i, pair in enumerate(optimizers_and_blocks):
-            pair.optimizer = tf.keras.optimizers.get(pair.optimizer)
+            pair.optimizer = self._get_optimizer(pair.optimizer)
             self._track_trackable(pair.optimizer, name=f"Optimizer{i}")
             pair.blocks = [pair.blocks] if isinstance(pair.blocks, Block) else pair.blocks
             self.optimizers_and_blocks.append(pair)
         if "update_optimizers_and_blocks" in kwargs:
             # only for from_config, where there is already self.update_optimizers_and_blocks
             self.update_optimizers_and_blocks = kwargs.get("update_optimizers_and_blocks")
         else:
             self.update_optimizers_and_blocks = []
 
+    def _get_optimizer(self, optimizer):
+        if version.parse(tf.__version__) < version.parse("2.11.0"):
+            optimizer = tf.keras.optimizers.get(optimizer)
+        else:
+            if not (
+                isinstance(optimizer, str)
+                or isinstance(optimizer, tf.keras.optimizers.legacy.Optimizer)
+            ):
+                raise ValueError(
+                    "Optimizers must be a str or an instance of "
+                    "tf.keras.optimizers.legacy.Optimizer with Tensorflow >= 2.11."
+                )
+            optimizer = tf.keras.optimizers.get(
+                optimizer,
+                use_legacy_optimizer=True,
+            )
+        return optimizer
+
     def _get_trainable_variables_optimizer_dict(self, optimizers_and_blocks, require_disjoint=True):
         attribute = "_trainable_weights"
         for pair in optimizers_and_blocks:
             optimizer = pair.optimizer
             blocks = pair.blocks
             for block in blocks:
                 # Iterate all submodule (BFS) except ModelContext
@@ -201,15 +231,15 @@
 
     def add(
         self,
         optimizer_blocks: OptimizerBlocks,
     ):
         """add another optimzier and specify which block to apply this optimizer to"""
         len_exist_optimizers = len(self.optimizers_and_blocks)
-        optimizer_blocks.optimizer = tf.keras.optimizers.get(optimizer_blocks.optimizer)
+        optimizer_blocks.optimizer = self._get_optimizer(optimizer_blocks.optimizer)
         optimizer = optimizer_blocks.optimizer
         # Check if already track the optimizer
         optimizer_not_exists = True
         for opt_blocks in self.optimizers_and_blocks:
             if optimizer == opt_blocks.optimizer:
                 optimizer_not_exists = False
         if optimizer_not_exists:
@@ -222,19 +252,19 @@
         self,
         optimizer_blocks: OptimizerBlocks,
     ):
         """update the optimzier of a block, which would update the block's optimizer no matter
         what optimizer it used to utilize. If the block is not specified with an optimizer before,
         this functions would have the same functionality as self.add()
 
-        Note: the optimizer_blocks would be kept in self.update_optimizers_and_blockss, instead of
+        Note: the optimizer_blocks would be kept in self.update_optimizers_and_blocks, instead of
         self.optimizers_and_blocks"""
         len_exist_optimizers = len(self.optimizers_and_blocks)
         optimizer = optimizer_blocks.optimizer
-        optimizer = tf.keras.optimizers.get(optimizer)
+        optimizer = self._get_optimizer(optimizer)
         # Check if already track the optimizer
         optimizer_not_exists = True
         for pair in self.optimizers_and_blocks:
             if optimizer == pair.optimizer:
                 optimizer_not_exists = False
         if optimizer_not_exists:
             self._track_trackable(optimizer, name=f"Optimizer{1+len_exist_optimizers}")
@@ -242,14 +272,15 @@
         return
 
     def get_config(self):
         config = dict()
         config = tf_utils.maybe_serialize_keras_objects(self, config, ["default_optimizer"])
         config["name"] = self.name
         config["optimizers_and_blocks"] = []
+        config["update_optimizers_and_blocks"] = []
         for optimizer_blocks in self.optimizers_and_blocks:
             config["optimizers_and_blocks"].append(optimizer_blocks.get_config())
         for optimizer_blocks in self.update_optimizers_and_blocks:
             config["update_optimizers_and_blocks"].append(optimizer_blocks.get_config())
         return config
 
     @classmethod
@@ -285,26 +316,34 @@
         return self.weights
 
     @property
     def weights(self) -> List[tf.Variable]:
         """Returns the optimizer's variables."""
         weights = []
         for optimizer_blocks in self.optimizers_and_blocks:
-            weights += optimizer_blocks.optimizer.weights
+            optimizer = optimizer_blocks.optimizer
+            if hasattr(optimizer, "weights"):  # Tensorflow < 2.11
+                weights += optimizer_blocks.optimizer.weights
+            elif hasattr(optimizer, "variables") and callable(
+                optimizer.variables
+            ):  # Tensorflow >= 2.11
+                weights += optimizer_blocks.optimizer.variables()
+            else:
+                raise AttributeError(f"Unable to get weights from {optimizer.__class__.__name__}")
         return weights
 
     @property
-    def optimizers(self) -> List[tf.keras.optimizers.Optimizer]:
+    def optimizers(self) -> List[keras_optimizers.Optimizer]:
         """Returns the optimizers in MultiOptimizer (in the original order). Note: default_optimizer
         is included here"""
         return [pair.optimizer for pair in self.optimizers_and_blocks] + [self.default_optimizer]
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
-class LazyAdam(tf.keras.optimizers.Adam):
+class LazyAdam(keras_optimizers.Adam):
     """Variant of the Adam optimizer that handles sparse updates more efficiently.
 
     The original Adam algorithm maintains two moving-average accumulators for each trainable
     variable; the accumulators are updated at every step. This class provides lazier handling of
     gradient updates for sparse variables.  It only updates moving-average accumulators for sparse
     variable indices that appear in the current batch, rather than updating the accumulators for all
     indices. Compared with the original Adam optimizer, it can provide large improvements in model
@@ -331,15 +370,15 @@
     ):
         """Constructs a new LazyAdam optimizer.
 
         Parameters
         ----------
         learning_rate: Union[FloatTensorLike, Callable]
             A `Tensor` or a floating point value. or a schedule that is a
-            `tf.keras.optimizers.schedules.LearningRateSchedule` The learning rate.
+            `tf.keras.optimizers.legacy.schedules.LearningRateSchedule` The learning rate.
             FloatTensorLike = Union[tf.Tensor, float, np.float16, np.float32, np.float64]
         beta_1: FloatTensorLike
             A `float` value or a constant `float` tensor. The exponential decay rate for the 1st
             moment estimates.
         beta_2: FloatTensorLike
             A `float` value or a constant `float` tensor.   The exponential decay rate for the 2nd
             moment estimates.
@@ -393,14 +432,17 @@
 
         # \\(variable += -learning_rate * m_t / (epsilon_t + sqrt(v_t))\\)
         var_slice = lr * m_t_slice / (tf.math.sqrt(v_t_slice) + epsilon_t)
         var_update_op = self._resource_scatter_sub(var, indices, var_slice)
 
         return tf.group(*[var_update_op, m_update_op, v_update_op])
 
+    def get_weights(self):
+        return self.variables()
+
     def _resource_scatter_update(self, resource, indices, update):
         return self._resource_scatter_operate(
             resource, indices, update, tf.raw_ops.ResourceScatterUpdate
         )
 
     def _resource_scatter_sub(self, resource, indices, update):
         return self._resource_scatter_operate(
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/base.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,14 @@
         if self.sampled_softmax_mode or isinstance(targets, tf.Tensor):
             positive_item_ids = targets
         else:
             positive_item_ids = tf.squeeze(features[self.item_id_feature_name])
 
         neg_items_ids = None
         if training or testing:
-
             assert (
                 len(self.samplers) > 0
             ), "At least one sampler is required by ItemRetrievalScorer for negative sampling"
 
             if self.sampled_softmax_mode:
                 predictions = self._prepare_query_item_vectors_for_sampled_softmax(
                     predictions, targets
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/retrieval/two_tower.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/retrieval/two_tower.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/sampling/base.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/sampling/cross_batch.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/sampling/in_batch.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/blocks/sampling/queue.py` & `merlin-models-23.4.0/merlin/models/tf/blocks/sampling/queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/aggregation.py` & `merlin-models-23.4.0/merlin/models/tf/core/aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/base.py` & `merlin-models-23.4.0/merlin/models/tf/core/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/combinators.py` & `merlin-models-23.4.0/merlin/models/tf/core/combinators.py`

 * *Files 1% similar despite different names*

```diff
@@ -611,15 +611,19 @@
             self.parallel_layers = pruned
 
         return super().build(input_shape)
 
     def _maybe_filter_layer_inputs_using_schema(self, name, layer, inputs):
         maybe_schema = getattr(layer, "_schema", None)
         if maybe_schema and isinstance(inputs, dict):
-            layer_inputs = {k: v for k, v in inputs.items() if k in maybe_schema.column_names}
+            layer_inputs = {
+                k: v
+                for k, v in inputs.items()
+                if k.replace("__values", "").replace("__offsets", "") in maybe_schema.column_names
+            }
         else:
             layer_inputs = inputs
 
         if isinstance(layer_inputs, dict) and all(
             name in layer_inputs for name in self.parallel_dict
         ):
             layer_inputs = layer_inputs[name]
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/encoder.py` & `merlin-models-23.4.0/merlin/models/tf/core/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 import numpy as np
 import tensorflow as tf
 from packaging import version
 
 import merlin.io
 from merlin.models.io import save_merlin_metadata
 from merlin.models.tf.core import combinators
+from merlin.models.tf.core.base import NoOp
 from merlin.models.tf.core.prediction import TopKPrediction
 from merlin.models.tf.inputs.base import InputBlockV2
 from merlin.models.tf.inputs.embedding import CombinerType, EmbeddingTable
 from merlin.models.tf.models.base import BaseModel, get_output_schema
 from merlin.models.tf.outputs.topk import TopKOutput
-from merlin.models.tf.transforms.tensor import PrepareFeatures
+from merlin.models.tf.transforms.features import PrepareFeatures
 from merlin.models.tf.utils import tf_utils
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class Encoder(tf.keras.Model):
     """Block that can be used for prediction and evaluation but not for training
@@ -45,23 +46,26 @@
         When a schema is provided, a default input block will be created.
     *blocks: tf.keras.layers.Layer
         The blocks to use for encoding.
     pre: Optional[tf.keras.layers.Layer]
         A block to use before the main blocks
     post: Optional[tf.keras.layers.Layer]
         A block to use after the main blocks
-
+    prep_features: Optional[bool]
+        Whether this block should prepare list and scalar features
+        from the dataloader format. By default True.
     """
 
     def __init__(
         self,
         inputs: Union[Schema, tf.keras.layers.Layer],
         *blocks: tf.keras.layers.Layer,
         pre: Optional[tf.keras.layers.Layer] = None,
         post: Optional[tf.keras.layers.Layer] = None,
+        prep_features: Optional[bool] = True,
         **kwargs,
     ):
         super().__init__(**kwargs)
         if isinstance(inputs, Schema):
             input_block = InputBlockV2(inputs)
             self._schema = inputs
         else:
@@ -69,15 +73,18 @@
             if not hasattr(inputs, "schema"):
                 raise ValueError("inputs must have a schema")
             self._schema = inputs.schema
 
         self.blocks = [input_block] + list(blocks) if blocks else [input_block]
         self.pre = pre
         self.post = post
-        self.prepare_features = PrepareFeatures(self._schema)
+
+        self.prep_features = prep_features
+
+        self._prepare_features = PrepareFeatures(self.schema) if self.prep_features else NoOp()
 
     def encode(
         self,
         dataset: merlin.io.Dataset,
         index: Union[str, ColumnSchema, Schema, Tags],
         batch_size: int,
         **kwargs,
@@ -155,19 +162,22 @@
             encode_kwargs["filter_input_columns"] = output_schema.column_names
         predictions = dataset.map_partitions(model_encode, **encode_kwargs)
         if index:
             predictions = predictions.set_index(index)
 
         return merlin.io.Dataset(predictions)
 
-    def call(self, inputs, training=False, testing=False, targets=None, **kwargs):
+    def call(self, inputs, *, targets=None, training=False, testing=False, **kwargs):
+        inputs = self._prepare_features(inputs, targets=targets)
+        if isinstance(inputs, tuple):
+            inputs, targets = inputs
         return combinators.call_sequentially(
             list(self.to_call),
             inputs=inputs,
-            features=self.prepare_features(inputs),
+            features=inputs,
             targets=targets,
             training=training,
             testing=testing,
             **kwargs,
         )
 
     def __call__(self, inputs, **kwargs):
@@ -175,19 +185,23 @@
         # Inside the `call` method, we will add them back by assuming inputs=features
         if "features" in kwargs:
             kwargs.pop("features")
 
         return super().__call__(inputs, **kwargs)
 
     def build(self, input_shape):
+        self._prepare_features.build(input_shape)
+        input_shape = self._prepare_features.compute_output_shape(input_shape)
+
         combinators.build_sequentially(self, list(self.to_call), input_shape=input_shape)
         if not hasattr(self.build, "_is_default"):
             self._build_input_shape = input_shape
 
     def compute_output_shape(self, input_shape):
+        input_shape = self._prepare_features.compute_output_shape(input_shape)
         return combinators.compute_output_shape_sequentially(list(self.to_call), input_shape)
 
     def train_step(self, data):
         """Train step"""
         raise NotImplementedError(
             "This block is not meant to be trained by itself. ",
             "It can only be trained as part of a model.",
@@ -234,15 +248,15 @@
             export_path,
             include_optimizer=include_optimizer,
             save_traces=save_traces,
             save_format="tf",
         )
         input_schema = self.schema
         output_schema = get_output_schema(export_path)
-        save_merlin_metadata(export_path, self, input_schema, output_schema)
+        save_merlin_metadata(export_path, input_schema, output_schema)
 
     @property
     def to_call(self):
         if self.pre:
             yield self.pre
 
         for block in self.blocks:
@@ -536,14 +550,15 @@
         sequence_combiner: Optional[CombinerType] = None,
         trainable=True,
         name=None,
         dtype=None,
         dynamic=False,
         post: Optional[tf.keras.layers.Layer] = None,
         embeddings_l2_batch_regularization: Optional[Union[float, Dict[str, float]]] = 0.0,
+        **kwargs,
     ):
         if isinstance(schema, ColumnSchema):
             col = schema
         else:
             col = schema.first
         col_name = col.name
 
@@ -560,11 +575,11 @@
             trainable=trainable,
             name=name,
             dtype=dtype,
             dynamic=dynamic,
             l2_batch_regularization_factor=embeddings_l2_batch_regularization,
         )
 
-        super().__init__(table, tf.keras.layers.Lambda(lambda x: x[col_name]), post=post)
+        super().__init__(table, tf.keras.layers.Lambda(lambda x: x[col_name]), post=post, **kwargs)
 
     def to_dataset(self, gpu=None) -> merlin.io.Dataset:
         return self.blocks[0].to_dataset(gpu=gpu)
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/index.py` & `merlin-models-23.4.0/merlin/models/tf/core/index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/prediction.py` & `merlin-models-23.4.0/merlin/models/tf/core/prediction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/core/tabular.py` & `merlin-models-23.4.0/merlin/models/tf/core/tabular.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
             sequence_length = list(seq_features_shapes.values())[0][1]
 
         return seq_features_shapes, sequence_length
 
     def _check_concat_shapes(self, inputs: TabularData):
         input_sizes = {k: v.shape for k, v in inputs.items()}
+
         if len(set([tuple(v[:-1]) for v in input_sizes.values()])) > 1:
             raise Exception(
                 "All features dimensions except the last one must match: {}".format(input_sizes)
             )
 
     def _get_agg_output_size(self, input_size, agg_dim, axis=-1):
         batch_size = tf_utils.calculate_batch_size_from_input_shapes(input_size)
@@ -318,14 +319,15 @@
                 self.aggregation.build(output_shapes)
 
     def get_config(self):
         config = super(TabularBlock, self).get_config()
         config = tf_utils.maybe_serialize_keras_objects(
             self, config, ["pre", "post", "aggregation"]
         )
+        config["is_input"] = self._is_input
 
         if self.has_schema:
             config["schema"] = schema_utils.schema_to_tensorflow_metadata_json(self.schema)
 
         return config
 
     @property
@@ -536,15 +538,14 @@
         self.pop = pop
         self.add_to_context = add_to_context
 
         if isinstance(inputs, Schema):
             self.set_schema(schema=inputs)
 
     def set_schema(self, schema=None):
-
         out = super().set_schema(schema)
 
         if isinstance(self.feature_names, Tags):
             self.feature_names = self.schema.select_by_tag(self.feature_names).column_names
 
         return out
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/experimental/sample_weight.py` & `merlin-models-23.4.0/merlin/models/tf/experimental/sample_weight.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/inputs/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/inputs/base.py` & `merlin-models-23.4.0/merlin/models/tf/inputs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 from merlin.models.tf.inputs.embedding import (
     ContinuousEmbedding,
     EmbeddingFeatures,
     EmbeddingOptions,
     Embeddings,
     SequenceEmbeddingFeatures,
 )
-from merlin.models.tf.transforms.tensor import ListToDense, PrepareFeatures
 from merlin.schema import Schema, Tags, TagsType
 
 LOG = logging.getLogger("merlin-models")
 
 
 def InputBlock(
     schema: Schema,
     branches: Optional[Dict[str, Block]] = None,
+    pre: Optional[BlockType] = None,
     post: Optional[BlockType] = None,
     aggregation: Optional[TabularAggregationType] = None,
     seq: bool = False,
     max_seq_length: Optional[int] = None,
     add_continuous_branch: bool = True,
     continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
     continuous_projection: Optional[Block] = None,
@@ -139,15 +139,14 @@
         agg = aggregation
         sparse_interactions = InputBlock(
             sparse_schema,
             branches,
             post,
             aggregation=agg,
             seq=True,
-            max_seq_length=max_seq_length,
             add_continuous_branch=add_continuous_branch,
             continuous_tags=continuous_tags,
             continuous_projection=continuous_projection,
             add_embedding_branch=add_embedding_branch,
             embedding_options=embedding_options,
             categorical_tags=categorical_tags,
             split_sparse=False,
@@ -175,44 +174,37 @@
             split_sparse=False,
         )
 
     if (
         add_continuous_branch
         and schema.select_by_tag(continuous_tags).excluding_by_tag(Tags.TARGET).column_schemas
     ):
-        pre = None
-        if max_seq_length and seq:
-            pre = ListToDense(max_seq_length)
         branches["continuous"] = ContinuousFeatures.from_schema(  # type: ignore
-            schema,
-            tags=continuous_tags,
-            pre=pre,
+            schema, tags=continuous_tags
         )
     if (
         add_embedding_branch
         and schema.select_by_tag(categorical_tags).excluding_by_tag(Tags.TARGET).column_schemas
     ):
         emb_cls: Type[EmbeddingFeatures] = SequenceEmbeddingFeatures if seq else EmbeddingFeatures
-        emb_kwargs = {}
-        if max_seq_length and seq:
-            emb_kwargs["max_seq_length"] = max_seq_length
 
         branches["categorical"] = emb_cls.from_schema(  # type: ignore
-            schema, tags=categorical_tags, embedding_options=embedding_options, **emb_kwargs
+            schema, tags=categorical_tags, embedding_options=embedding_options
         )
     if continuous_projection:
         return ContinuousEmbedding(
             ParallelBlock(branches),
             continuous_projection,
             aggregation=aggregation,
             post=post,
             name="continuous_projection",
         )
 
-    return ParallelBlock(branches, aggregation=aggregation, post=post, is_input=True, **kwargs)
+    kwargs["is_input"] = kwargs.get("is_input", True)
+    return ParallelBlock(branches, pre=pre, aggregation=aggregation, post=post, **kwargs)
 
 
 INPUT_TAG_TO_BLOCK: Dict[Tags, Callable[[Schema], Layer]] = {
     Tags.CONTINUOUS: Continuous,
     Tags.CATEGORICAL: Embeddings,
 }
 
@@ -321,19 +313,15 @@
             branch_schema: Schema = schema.select_by_tag(branch)
             if branch_schema:
                 parsed[name] = tag_to_block[branch](branch_schema)
 
     if not parsed:
         raise ValueError("No columns selected for the input block")
 
-    _pre = PrepareFeatures(schema)
-    if pre:
-        _pre = _pre.connect(pre)
-
     return ParallelBlock(
         parsed,
-        pre=_pre,
+        pre=pre,
         post=post,
         aggregation=aggregation,
         is_input=True,
         schema=schema,
     )
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/inputs/continuous.py` & `merlin-models-23.4.0/merlin/models/tf/inputs/continuous.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,22 +86,17 @@
         pre: Optional[BlockType] = None,
         post: Optional[BlockType] = None,
         aggregation: Optional[TabularAggregationType] = None,
         schema: Optional[Schema] = None,
         name: Optional[str] = None,
         **kwargs
     ):
+        kwargs["is_input"] = kwargs.get("is_input", True)
         super().__init__(
-            pre=pre,
-            post=post,
-            aggregation=aggregation,
-            schema=schema,
-            name=name,
-            is_input=True,
-            **kwargs
+            pre=pre, post=post, aggregation=aggregation, schema=schema, name=name, **kwargs
         )
         self.filter_features = Filter(features)
 
     @classmethod
     def from_features(cls, features, **kwargs):
         return cls(features, **kwargs)
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/inputs/embedding.py` & `merlin-models-23.4.0/merlin/models/tf/inputs/embedding.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,26 +32,20 @@
 from merlin.models.tf.core.combinators import ParallelBlock, SequentialBlock
 from merlin.models.tf.core.tabular import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     Filter,
     TabularAggregationType,
     TabularBlock,
 )
-from merlin.models.tf.transforms.tensor import ListToDense, ListToSparse
 
 # pylint has issues with TF array ops, so disable checks until fixed:
 # https://github.com/PyCQA/pylint/issues/3613
 # pylint: disable=no-value-for-parameter, unexpected-keyword-arg
 from merlin.models.tf.typing import TabularData
-from merlin.models.tf.utils.tf_utils import (
-    call_layer,
-    df_to_tensor,
-    list_col_to_ragged,
-    tensor_to_df,
-)
+from merlin.models.tf.utils.tf_utils import call_layer, df_to_tensor, tensor_to_df
 from merlin.models.utils import schema_utils
 from merlin.models.utils.doc_utils import docstring_parameter
 from merlin.models.utils.schema_utils import (
     create_categorical_column,
     infer_embedding_dim,
     schema_to_tensorflow_metadata_json,
     tensorflow_metadata_json_to_schema,
@@ -153,14 +147,17 @@
 
 CombinerType = Union[str, tf.keras.layers.Layer]
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class EmbeddingTable(EmbeddingTableBase):
     """Embedding table that is backed by a standard Keras Embedding Layer.
+    It accepts as input features for lookup tf.Tensor, tf.RaggedTensor,
+    and tf.SparseTensor which might be 2D (batch_size, 1) for scalars
+    or 3d (batch_size, seq_length, 1) for sequential features
 
      Parameters
      ----------
      dim: Dimension of the dense embedding.
      col_schema: ColumnSchema
          Schema of the column. This is used to infer the cardinality.
      embeddings_initializer: Initializer for the `embeddings`
@@ -217,14 +214,15 @@
         sequence_combiner: Optional[CombinerType] = None,
         trainable=True,
         name=None,
         dtype=None,
         dynamic=False,
         table=None,
         l2_batch_regularization_factor=0.0,
+        weights=None,
         **kwargs,
     ):
         """Create an EmbeddingTable."""
         super(EmbeddingTable, self).__init__(
             dim,
             *col_schemas,
             trainable=trainable,
@@ -240,14 +238,15 @@
                 embeddings_initializer=embeddings_initializer,
                 embeddings_regularizer=embeddings_regularizer,
                 activity_regularizer=activity_regularizer,
                 embeddings_constraint=embeddings_constraint,
                 mask_zero=mask_zero,
                 input_length=input_length,
                 trainable=trainable,
+                weights=weights,
             )
             self.table = tf.keras.layers.Embedding(
                 input_dim=self.input_dim,
                 output_dim=self.dim,
                 name=self.table_name,
                 **table_kwargs,
             )
@@ -309,22 +308,29 @@
         num_items, dim = tuple(embeddings.shape)
 
         if not col_schema:
             if not name:
                 raise ValueError("`name` is required when not using a ColumnSchema")
             col_schema = create_categorical_column(name, num_items - 1)
 
-        return cls(
+        embedding_table = cls(
             dim,
             col_schema,
             name=name,
-            embeddings_initializer=tf.keras.initializers.constant(embeddings),
+            weights=[embeddings],
+            embeddings_initializer=None,
             trainable=trainable,
             **kwargs,
         )
+        # trigger build of table to make sure that weights are configured
+        # without this line the weights are not initialized correctly with
+        # the provided values
+        embedding_table.table(0)
+
+        return embedding_table
 
     @classmethod
     def from_dataset(
         cls,
         data: Union[Dataset, DataFrameType],
         trainable=True,
         name=None,
@@ -384,44 +390,48 @@
                     out[feature_name] = self._call_table(inputs[feature_name], **kwargs)
         else:
             out = self._call_table(inputs, **kwargs)
 
         return out
 
     def _call_table(self, inputs, **kwargs):
-        if isinstance(inputs, tuple) and len(inputs) == 2:
-            inputs = list_col_to_ragged(inputs)
-
-        # Eliminating the last dim==1 of dense tensors before embedding lookup
-        if isinstance(inputs, tf.Tensor) or (
-            isinstance(inputs, tf.RaggedTensor) and inputs.shape[-1] == 1
-        ):
-            inputs = tf.squeeze(inputs, axis=-1)
-
         if isinstance(inputs, (tf.RaggedTensor, tf.SparseTensor)):
             if self.sequence_combiner and isinstance(self.sequence_combiner, str):
                 if isinstance(inputs, tf.RaggedTensor):
                     inputs = inputs.to_sparse()
-                if len(inputs.dense_shape) == 3 and inputs.dense_shape[-1] == 1:
-                    inputs = tf.sparse.reshape(inputs, inputs.dense_shape[:-1])
+
+                inputs = tf.sparse.reshape(inputs, tf.shape(inputs)[:-1])
+
                 out = tf.nn.safe_embedding_lookup_sparse(
                     self.table.embeddings, inputs, None, combiner=self.sequence_combiner
                 )
+
             else:
                 if isinstance(inputs, tf.SparseTensor):
                     raise ValueError(
                         "Sparse tensors are not supported without sequence_combiner ",
                         "please convert the tensor to a ragged or dense.",
                     )
 
+                inputs = tf.squeeze(inputs, axis=-1)
+
                 out = call_layer(self.table, inputs, **kwargs)
-                if isinstance(self.sequence_combiner, tf.keras.layers.Layer):
+                if len(out.get_shape()) > 2 and isinstance(
+                    self.sequence_combiner, tf.keras.layers.Layer
+                ):
                     out = call_layer(self.sequence_combiner, out, **kwargs)
         else:
+            if inputs.shape.as_list()[-1] == 1:
+                inputs = tf.squeeze(inputs, axis=-1)
             out = call_layer(self.table, inputs, **kwargs)
+            if len(out.get_shape()) > 2 and self.sequence_combiner is not None:
+                if isinstance(self.sequence_combiner, tf.keras.layers.Layer):
+                    out = call_layer(self.sequence_combiner, out, **kwargs)
+                elif isinstance(self.sequence_combiner, str):
+                    out = process_str_sequence_combiner(out, self.sequence_combiner, **kwargs)
 
         if self.l2_batch_regularization_factor > 0:
             self.add_loss(self.l2_batch_regularization_factor * tf.reduce_sum(tf.square(out)))
 
         if self._dtype_policy.compute_dtype != self._dtype_policy.variable_dtype:
             # Instead of casting the variable as in most layers, cast the output, as
             # this is mathematically equivalent but is faster.
@@ -443,17 +453,14 @@
             output_shapes = self._compute_output_shape_table(input_shape)
 
         return output_shapes
 
     def _compute_output_shape_table(
         self, input_shape: Union[tf.TensorShape, tuple]
     ) -> tf.TensorShape:
-        if isinstance(input_shape, tuple) and isinstance(input_shape[1], tf.TensorShape):
-            input_shape = tf.TensorShape([input_shape[1][0], None])
-
         first_dims = input_shape
 
         if input_shape.rank > 1:
             if self.sequence_combiner is not None:
                 first_dims = [input_shape[0]]
 
             elif input_shape[-1] == 1:
@@ -744,15 +751,15 @@
         schema: Optional[Schema] = None,
         name=None,
         add_default_pre=True,
         l2_reg: Optional[float] = 0.0,
         **kwargs,
     ):
         if add_default_pre:
-            embedding_pre = [Filter(list(feature_config.keys())), ListToSparse()]
+            embedding_pre = [Filter(list(feature_config.keys()))]
             pre = [embedding_pre, pre] if pre else embedding_pre  # type: ignore
         self.feature_config = feature_config
         self.l2_reg = l2_reg
 
         self.embedding_tables = {}
         tables: Dict[str, TableConfig] = {}
         for _, feature in self.feature_config.items():
@@ -764,21 +771,21 @@
             self.embedding_tables[table_name] = tf.keras.layers.Embedding(
                 table.vocabulary_size,
                 table.dim,
                 name=table_name,
                 embeddings_initializer=table.initializer,
             )
 
+        kwargs["is_input"] = kwargs.get("is_input", True)
         super().__init__(
             pre=pre,
             post=post,
             aggregation=aggregation,
             name=name,
             schema=schema,
-            is_input=True,
             **kwargs,
         )
 
     @classmethod
     def from_schema(  # type: ignore
         cls,
         schema: Schema,
@@ -903,29 +910,32 @@
     def lookup_feature(self, name, val, output_sequence=False):
         dtype = backend.dtype(val)
         if dtype != "int32" and dtype != "int64":
             val = tf.cast(val, "int32")
 
         table: TableConfig = self.feature_config[name].table
         table_var = self.embedding_tables[table.name].embeddings
-        if isinstance(val, tf.SparseTensor):
-            if len(val.dense_shape) == 3 and val.dense_shape[-1] == 1:
-                val = tf.sparse.reshape(val, val.dense_shape[:-1])
+        if isinstance(val, (tf.RaggedTensor, tf.SparseTensor)):
+            if isinstance(val, tf.RaggedTensor):
+                val = val.to_sparse()
+
+            val = tf.sparse.reshape(val, tf.shape(val)[:-1])
 
             out = tf.nn.safe_embedding_lookup_sparse(table_var, val, None, combiner=table.combiner)
         else:
             if output_sequence:
                 out = tf.gather(table_var, tf.cast(val, tf.int32))
             else:
-                if len(val.shape) > 1:
-                    # TODO: Check if it is correct to retrieve only the 1st element
-                    # of second dim for non-sequential multi-hot categ features
-                    out = tf.gather(table_var, tf.cast(val, tf.int32)[:, 0])
-                else:
-                    out = tf.gather(table_var, tf.cast(val, tf.int32))
+                if len(val.shape) > 1 and val.shape.as_list()[-1] == 1:
+                    val = tf.squeeze(val, axis=-1)
+                out = tf.gather(table_var, tf.cast(val, tf.int32))
+
+            if len(out.get_shape()) > 2 and table.combiner is not None:
+                out = process_str_sequence_combiner(out, table.combiner)
+
         if self._dtype_policy.compute_dtype != self._dtype_policy.variable_dtype:
             # Instead of casting the variable as in most layers, cast the output, as
             # this is mathematically equivalent but is faster.
             out = tf.cast(out, self._dtype_policy.compute_dtype)
 
         return out
 
@@ -1090,27 +1100,26 @@
         The symbol to use for padding.
     {tabular_module_parameters}
     """
 
     def __init__(
         self,
         feature_config: Dict[str, FeatureConfig],
-        max_seq_length: Optional[int] = None,
         mask_zero: bool = True,
         padding_idx: int = 0,
         pre: Optional[BlockType] = None,
         post: Optional[BlockType] = None,
         aggregation: Optional[TabularAggregationType] = None,
         schema: Optional[Schema] = None,
         name: Optional[str] = None,
         add_default_pre=True,
         **kwargs,
     ):
         if add_default_pre:
-            embedding_pre = [Filter(list(feature_config.keys())), ListToDense(max_seq_length)]
+            embedding_pre = [Filter(list(feature_config.keys()))]
             pre = [embedding_pre, pre] if pre else embedding_pre  # type: ignore
 
         super().__init__(
             feature_config=feature_config,
             pre=pre,
             post=post,
             aggregation=aggregation,
@@ -1200,7 +1209,39 @@
 
     for key, val in feature_config.items():
         feature_config_dict = dict(name=val.name, max_sequence_length=val.max_sequence_length)
         feature_config_dict["table"] = serialize_table_config(feature_config_dict["table"])
         outputs[key] = feature_config_dict
 
     return outputs
+
+
+def process_str_sequence_combiner(
+    inputs: Union[tf.Tensor, tf.RaggedTensor], combiner: str, **kwargs
+) -> tf.Tensor:
+    """Process inputs with str sequence combiners ("mean" or "sum")
+
+    Parameters
+    ----------
+    inputs : Union[tf.Tensor, tf.RaggedTensor]
+        Input 3D tensor (batch size, seq length, embedding dim)
+    combiner : str
+        The combiner: "mean" or "sum"
+
+    Returns
+    -------
+    tf.Tensor
+        A 2D tensor with values combined on axis=1
+    """
+    if not combiner or len(inputs.get_shape()) <= 2:
+        return inputs
+    if combiner == "mean":
+        combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1))
+    elif combiner == "sum":
+        combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_sum(x, axis=1))
+    else:
+        raise ValueError(
+            "Only 'mean' and 'sum' str combiners is implemented for dense"
+            " list/multi-hot embedded features. You can also"
+            " provide a tf.keras.layers.Layer instance as a sequence combiner."
+        )
+    return call_layer(combiner, inputs, **kwargs)
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/loader.py` & `merlin-models-23.4.0/merlin/models/tf/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -361,70 +361,61 @@
     KerasSequenceValidator
 ) = merlin.dataloader.tensorflow.KerasSequenceValidater
 
 
 def sample_batch(
     dataset_or_loader: Union[Dataset, Loader],
     batch_size: Optional[int] = None,
-    shuffle: bool = False,
-    include_targets: bool = True,
-    to_ragged: bool = False,
-    to_dense: bool = False,
-    prepare_features=False,
+    shuffle: Optional[bool] = False,
+    include_targets: Optional[bool] = True,
+    prepare_features: Optional[bool] = True,
 ):
     """Util function to generate a batch of input tensors from a merlin.io.Dataset instance
 
     Parameters
     ----------
     data: merlin.io.dataset
         A Dataset object.
     batch_size: int
         Number of samples to return.
     shuffle: bool
         Whether to sample a random batch or not, by default False.
     include_targets: bool
         Whether to include the targets in the returned batch, by default True.
-    to_ragged: bool
-        Whether to convert the tuple of sparse tensors into ragged tensors, by default False.
-    to_dense: bool
-        Whether to convert the tuple of sparse tensors into dense tensors, by default False.
     prepare_features: bool
         Whether to prepare features from dataloader for the model, by default False.
         If enabled, it converts multi-hot/list features to dense or ragged based on the schema.
         It also ensures that scalar features are converted to 2D (batch size, 1).
         P.s. The features are automatically prepared by InputBlockV2 if it is used
     Returns:
     -------
     batch: Dict[tf.tensor]
         dictionary of input tensors.
     """
-    if to_ragged and to_dense:
-        raise ValueError(
-            "Sparse values cannot be converted to both ragged tensors and dense tensors"
-        )
 
-    from merlin.models.tf.transforms.tensor import ListToDense, ListToRagged, PrepareFeatures
+    from merlin.models.tf.transforms.features import PrepareFeatures
 
     if isinstance(dataset_or_loader, Dataset):
         if not batch_size:
             raise ValueError("Either use 'Loader' or specify 'batch_size'")
         loader = Loader(dataset_or_loader, batch_size=batch_size, shuffle=shuffle)
     else:
         loader = dataset_or_loader
 
     batch = loader.peek()
     # batch could be of type Prediction, so we can't unpack directly
     inputs, targets = batch[0], batch[1]
 
-    if to_ragged:
-        inputs = ListToRagged()(inputs)
-    elif to_dense:
-        inputs = ListToDense()(inputs)
     if prepare_features:
-        inputs = PrepareFeatures(loader.schema)(inputs)
+        pf = PrepareFeatures(loader.schema)
+        if targets is not None:
+            inputs, targets = pf(inputs, targets=targets)
+        else:
+            inputs = pf(inputs)
+
     if not include_targets:
         return inputs
     return inputs, targets
 
 
 def get_default_hvd_seed_fn(seed=None):
     """
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/losses/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/losses/base.py` & `merlin-models-23.4.0/merlin/models/tf/losses/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/losses/listwise.py` & `merlin-models-23.4.0/merlin/models/tf/losses/listwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/losses/pairwise.py` & `merlin-models-23.4.0/merlin/models/tf/losses/pairwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/metrics/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/metrics/evaluation.py` & `merlin-models-23.4.0/merlin/models/tf/metrics/evaluation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/metrics/topk.py` & `merlin-models-23.4.0/merlin/models/tf/metrics/topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 def dcg_at(
     y_true: tf.Tensor,
     y_pred: tf.Tensor,
     label_relevant_counts: Optional[tf.Tensor] = None,
     k: int = 5,
     log_base: int = 2,
 ) -> tf.Tensor:
-
     """
     Compute discounted cumulative gain @K (ignoring ties)
     Parameters
     ----------
     {METRIC_PARAMETERS_DOCSTRING}
     """
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/models/base.py` & `merlin-models-23.4.0/merlin/models/tf/models/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,32 +29,42 @@
 from keras.engine.compile_utils import MetricsContainer
 from keras.utils.losses_utils import cast_losses_to_common_dtype
 from packaging import version
 from tensorflow.keras.losses import Loss
 from tensorflow.keras.metrics import Metric
 from tensorflow.keras.utils import unpack_x_y_sample_weight
 
+# This is to handle TensorFlow 2.11/2.12 Saving V3 triggering with model pickle
+try:
+    from keras.saving.experimental import saving_lib  # 2.11
+except ImportError:
+    try:
+        from keras.saving import saving_lib  # 2.12
+    except ImportError:
+        saving_lib = None
+
 import merlin.io
 from merlin.models.io import save_merlin_metadata
-from merlin.models.tf.core.base import Block, ModelContext, PredictionOutput, is_input_block
+from merlin.models.tf.core.base import Block, ModelContext, NoOp, PredictionOutput, is_input_block
 from merlin.models.tf.core.combinators import ParallelBlock, SequentialBlock
 from merlin.models.tf.core.prediction import Prediction, PredictionContext, TensorLike
 from merlin.models.tf.core.tabular import TabularBlock
 from merlin.models.tf.distributed.backend import hvd, hvd_installed
 from merlin.models.tf.inputs.base import InputBlock
 from merlin.models.tf.loader import Loader
 from merlin.models.tf.losses.base import loss_registry
 from merlin.models.tf.metrics import metrics_registry
 from merlin.models.tf.metrics.evaluation import MetricType
 from merlin.models.tf.metrics.topk import TopKMetricsAggregator, filter_topk_metrics, split_metrics
 from merlin.models.tf.models.utils import parse_prediction_blocks
 from merlin.models.tf.outputs.base import ModelOutput, ModelOutputType
 from merlin.models.tf.outputs.contrastive import ContrastiveOutput
 from merlin.models.tf.prediction_tasks.base import ParallelPredictionBlock, PredictionTask
-from merlin.models.tf.transforms.tensor import PrepareFeatures
+from merlin.models.tf.transforms.features import PrepareFeatures, expected_input_cols_from_schema
+from merlin.models.tf.transforms.sequence import SequenceTransform
 from merlin.models.tf.typing import TabularData
 from merlin.models.tf.utils.search_utils import find_all_instances_in_layers
 from merlin.models.tf.utils.tf_utils import (
     call_layer,
     get_sub_blocks,
     maybe_serialize_keras_objects,
 )
@@ -138,49 +148,51 @@
     model = tf.keras.models.load_model(export_path)
     signature = model.signatures["serving_default"]
 
     output_schema = Schema()
     for output_name, output_spec in signature.structured_outputs.items():
         col_schema = ColumnSchema(output_name, dtype=output_spec.dtype.as_numpy_dtype)
         shape = output_spec.shape
-        if shape.rank > 1 and (shape[1] is None or shape[1] > 1):
-            is_ragged = shape[1] is None
-            properties = {}
-            if not is_ragged:
-                properties["value_count"] = {"min": shape[1], "max": shape[1]}
+        if shape.rank > 1 and (shape[1] is not None and shape[1] > 1):
             col_schema = ColumnSchema(
                 output_name,
                 dtype=output_spec.dtype.as_numpy_dtype,
-                is_list=True,
-                is_ragged=is_ragged,
-                properties=properties,
+                dims=(None, shape[1]),
             )
+
         output_schema.column_schemas[output_name] = col_schema
 
     return output_schema
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class ModelBlock(Block, tf.keras.Model):
     """Block that extends `tf.keras.Model` to make it saveable."""
 
-    def __init__(self, block: Block, **kwargs):
+    def __init__(self, block: Block, prep_features: Optional[bool] = True, **kwargs):
         super().__init__(**kwargs)
         self.block = block
         if hasattr(self, "set_schema"):
             block_schema = getattr(block, "schema", None)
             self.set_schema(block_schema)
 
+        self.prep_features = prep_features
+        self._prepare_features = PrepareFeatures(self.schema) if self.prep_features else NoOp()
+
     def call(self, inputs, **kwargs):
+        inputs = self._prepare_features(inputs)
         if "features" not in kwargs:
             kwargs["features"] = inputs
         outputs = call_layer(self.block, inputs, **kwargs)
         return outputs
 
     def build(self, input_shapes):
+        self._prepare_features.build(input_shapes)
+        input_shapes = self._prepare_features.compute_output_shape(input_shapes)
+
         self.block.build(input_shapes)
 
         if not hasattr(self.build, "_is_default"):
             self._build_input_shape = input_shapes
         self.built = True
 
     def fit(
@@ -204,14 +216,15 @@
         max_queue_size=10,
         workers=1,
         use_multiprocessing=False,
         train_metrics_steps=1,
         **kwargs,
     ):
         x = _maybe_convert_merlin_dataset(x, batch_size, **kwargs)
+
         validation_data = _maybe_convert_merlin_dataset(
             validation_data, batch_size, shuffle=shuffle, **kwargs
         )
         callbacks = self._add_metrics_callback(callbacks, train_metrics_steps)
         fit_kwargs = {
             k: v
             for k, v in locals().items()
@@ -249,14 +262,15 @@
             workers,
             use_multiprocessing,
             return_dict,
             **kwargs,
         )
 
     def compute_output_shape(self, input_shape):
+        input_shape = self._prepare_features.compute_output_shape(input_shape)
         return self.block.compute_output_shape(input_shape)
 
     @property
     def schema(self) -> Schema:
         return self.block.schema
 
     @classmethod
@@ -276,14 +290,26 @@
             # Keras will interpret kwargs like `features` & `targets` as
             # required args, which is wrong. This is a workaround.
             _arg_spec = self._saved_model_arg_spec
             self._saved_model_arg_spec = ([_arg_spec[0][0]], _arg_spec[1])
 
 
 class BaseModel(tf.keras.Model):
+    def __init__(self, **kwargs):
+        super(BaseModel, self).__init__(**kwargs)
+
+        # Initializing model control flags controlled by MetricsComputeCallback()
+        self._should_compute_train_metrics_for_batch = tf.Variable(
+            dtype=tf.bool,
+            name="should_compute_train_metrics_for_batch",
+            trainable=False,
+            synchronization=tf.VariableSynchronization.NONE,
+            initial_value=lambda: True,
+        )
+
     def compile(
         self,
         optimizer="rmsprop",
         loss: Optional[Union[str, Loss, Dict[str, Union[str, Loss]]]] = None,
         metrics: Optional[
             Union[
                 MetricType,
@@ -386,23 +412,14 @@
               [XLA documentation](https://www.tensorflow.org/xla).
               Also refer to
               [known XLA issues](https://www.tensorflow.org/xla/known_issues) for
               more details.
             **kwargs: Arguments supported for backwards compatibility only.
         """
 
-        # Initializing model control flags controlled by MetricsComputeCallback()
-        self._should_compute_train_metrics_for_batch = tf.Variable(
-            dtype=tf.bool,
-            name="should_compute_train_metrics_for_batch",
-            trainable=False,
-            synchronization=tf.VariableSynchronization.NONE,
-            initial_value=lambda: True,
-        )
-
         num_v1_blocks = len(self.prediction_tasks)
         num_v2_blocks = len(self.model_outputs)
 
         if num_v1_blocks > 1 and num_v2_blocks > 1:
             raise ValueError(
                 "You cannot use both `prediction_tasks` and `prediction_blocks` at the same time.",
                 "`prediction_tasks` is deprecated and will be removed in a future version.",
@@ -445,15 +462,18 @@
             else:
                 opt_config["lr"] = opt.learning_rate * hvd.size()
 
             opt = opt.__class__.from_config(opt_config)
 
             return hvd.DistributedOptimizer(opt)
 
-        optimizer = tf.keras.optimizers.get(optimizer)
+        if version.parse(tf.__version__) < version.parse("2.11.0"):
+            optimizer = tf.keras.optimizers.get(optimizer)
+        else:
+            optimizer = tf.keras.optimizers.get(optimizer, use_legacy_optimizer=True)
 
         if hvd_installed and hvd.size() > 1:
             if optimizer.__module__.startswith("horovod"):
                 # do nothing if the optimizer is already wrapped in hvd.DistributedOptimizer
                 pass
             elif isinstance(optimizer, merlin.models.tf.MultiOptimizer):
                 for pair in (
@@ -772,15 +792,15 @@
                     task_y = y[task.target_name] if isinstance(y, dict) and y else y
                     task_sample_weight = sample_weight
 
                 targets[task.task_name] = task_y
                 predictions[task.task_name] = task_x
                 sample_weights[task.task_name] = task_sample_weight
 
-            self.adjust_predictions_and_targets(predictions, targets)
+            self.adjust_predictions_and_targets(predictions, targets, sample_weights)
 
             if len(predictions) == 1 and len(targets) == 1:
                 predictions = list(predictions.values())[0]
                 targets = list(targets.values())[0]
                 sample_weights = list(sample_weights.values())[0]
 
             if output:
@@ -804,72 +824,275 @@
                 task_y = y[task.target] if isinstance(y, dict) and y else y
                 task_sample_weight = sample_weight
 
             targets[task.full_name] = task_y
             predictions[task.full_name] = task_x
             sample_weights[task.full_name] = task_sample_weight
 
-        self.adjust_predictions_and_targets(predictions, targets)
+        self.adjust_predictions_and_targets(predictions, targets, sample_weights)
 
         return Prediction(predictions, targets, sample_weights)
 
+    def _extract_masked_predictions(self, prediction: TensorLike):
+        """Extracts the prediction scores corresponding to masked positions (targets).
+
+        This method assumes that the input predictions tensor is 3-D and contains a mask
+        indicating the positions of the targets. It requires that the mask information has
+        exactly one masked position per input sequence. The method returns a 2-D dense tensor
+        containing the prediction score corresponding to each masked position.
+
+        Parameters
+        ----------
+        prediction : TensorLike
+            A 3-D dense tensor of predictions, with a mask indicating the positions of the targets.
+
+        Returns
+        -------
+        tf.Tensor
+            A 2-D dense tensor of prediction scores, with one score per input.
+
+        Raises
+        ------
+        ValueError
+            If the mask does not have exactly one masked position per input sequence.
+        """
+        num_preds_per_example = tf.reduce_sum(tf.cast(prediction._keras_mask, tf.int32), axis=-1)
+        with tf.control_dependencies(
+            [
+                tf.debugging.assert_equal(
+                    num_preds_per_example,
+                    1,
+                    message="If targets are scalars (1-D) and predictions are"
+                    " sequential (3-D), the predictions mask should contain"
+                    " one masked position per example",
+                )
+            ]
+        ):
+            return tf.boolean_mask(prediction, prediction._keras_mask)
+
+    def _adjust_dense_predictions_and_targets(
+        self,
+        prediction: tf.Tensor,
+        target: TensorLike,
+        sample_weight: TensorLike,
+    ):
+        """Adjusts the dense predictions tensor, the target tensor and sample_weight tensor
+        to ensure compatibility with most Keras losses and metrics.
+
+        This method applies the following transformations to the target and prediction tensors:
+        - Converts ragged targets and their masks to dense format.
+        - Copies the target mask to the prediction mask, if defined.
+        - If predictions are sequential (3-D) and targets are scalar (1-D), extracts the predictions
+        at target positions using the predictions mask.
+        - One-hot encodes targets if their rank is one less than the rank of predictions.
+        - Ensures that targets have the same shape and dtype as predictions.
+
+        Parameters
+        ----------
+        prediction : tf.Tensor
+            The prediction tensor as a dense tensor.
+        target : TensorLike
+            The target tensor that can be either a dense or ragged tensor.
+        sample_weight : TensorLike
+            The sample weight tensor that can be either a dense or ragged tensor.
+
+        Returns:
+        --------
+            A tuple of the adjusted prediction, target, and sample_weight tensors,
+            with the same dtype and shape.
+        """
+        if isinstance(target, tf.RaggedTensor):
+            # Converts ragged targets (and ragged mask) to dense
+            dense_target_mask = None
+            if getattr(target, "_keras_mask", None) is not None:
+                dense_target_mask = target._keras_mask.to_tensor()
+            target = target.to_tensor()
+            if dense_target_mask is not None:
+                target._keras_mask = dense_target_mask
+
+        if isinstance(sample_weight, tf.RaggedTensor):
+            sample_weight = sample_weight.to_tensor()
+
+        if prediction.shape.ndims == 2:
+            # Removes the mask information as the sequence is summarized into
+            # a single vector.
+            prediction._keras_mask = None
+
+        elif getattr(target, "_keras_mask", None) is not None:
+            # Copies the mask from the targets to the predictions
+            # because Keras considers the prediction mask in loss
+            # and metrics computation
+            if isinstance(target._keras_mask, tf.RaggedTensor):
+                target._keras_mask = target._keras_mask.to_tensor()
+            prediction._keras_mask = target._keras_mask
+
+        # Ensuring targets and preds have the same dtype
+        target = tf.cast(target, prediction.dtype)
+
+        # If targets are scalars (1-D) and predictions are sequential (3-D),
+        # extract predictions at target position because Keras expects
+        # predictions and targets to have the same shape.
+        if getattr(prediction, "_keras_mask", None) is not None:
+            rank_check = tf.logical_and(
+                tf.logical_and(tf.rank(target) > 0, tf.shape(target)[-1] == 1),
+                tf.equal(tf.rank(prediction), 3),
+            )
+            prediction = tf.cond(
+                rank_check, lambda: self._extract_masked_predictions(prediction), lambda: prediction
+            )
+
+        # Ensuring targets are one-hot encoded if they are not
+        condition = tf.logical_and(
+            tf.logical_and(tf.rank(target) > 0, tf.shape(target)[-1] == 1),
+            tf.shape(prediction)[-1] > 1,
+        )
+        target = tf.cond(
+            condition,
+            lambda: tf.one_hot(
+                tf.cast(target, tf.int32),
+                tf.shape(prediction)[-1],
+                dtype=prediction.dtype,
+            ),
+            lambda: target,
+        )
+        # Makes target shape equal to the predictions tensor, as shape is lost after tf.cond
+        target = tf.reshape(target, tf.shape(prediction))
+
+        return prediction, target, sample_weight
+
+    def _adjust_ragged_predictions_and_targets(
+        self,
+        prediction: tf.RaggedTensor,
+        target: TensorLike,
+        sample_weight: TensorLike,
+    ):
+        """Adjusts the prediction (ragged tensor), target and sample weight
+        to ensure compatibility with most Keras losses and metrics.
+
+        This methods applies the following transformations to the target and prediction tensors:
+        - Select ragged targets based on the mask information, if defined.
+        - Remove mask information from the ragged targets and predictions.
+        - One-hot encode targets if their rank is one less than the rank of predictions.
+        - Ensure that targets have the same shape and dtype as predictions.
+
+        Parameters
+        ----------
+        prediction : tf.RaggedTensor
+            The prediction tensor as a ragged tensor.
+        target : TensorLike
+            The target tensor that can be either a dense or ragged tensor.
+        sample_weight : TensorLike
+            The sample weight tensor that can be either a dense or ragged tensor.
+
+        Returns
+        -------
+        Tuple[tf.Tensor, tf.Tensor]
+            A tuple containing the adjusted prediction, target and sample_weight tensors.
+        """
+        target_mask = None
+        if getattr(target, "_keras_mask", None) is not None:
+            target_mask = target._keras_mask
+
+        if isinstance(target, tf.RaggedTensor) and target_mask is not None:
+            # Select targets at masked positions and return
+            # a ragged tensor.
+            target = tf.ragged.boolean_mask(
+                target, target_mask.with_row_splits_dtype(target.row_splits.dtype)
+            )
+
+        # Ensuring targets and preds have the same dtype
+        target = tf.cast(target, prediction.dtype)
+
+        # Align sample_weight with the ragged target tensor
+        if isinstance(target, tf.RaggedTensor) and sample_weight is not None:
+            if isinstance(sample_weight, tf.RaggedTensor):
+                # sample_weight is a 2-D tensor, weights in the same sequence are different
+                if target_mask is not None:
+                    # Select sample weights at masked positions and return a ragged tensor.
+                    sample_weight = tf.ragged.boolean_mask(
+                        sample_weight,
+                        target_mask.with_row_splits_dtype(sample_weight.row_splits.dtype),
+                    )
+            else:
+                # sample_weight is a 1-D tensor, one weight value per sequence
+                # repeat the weight value for each masked target position
+                row_lengths = tf.constant(target.row_lengths(), dtype=tf.int64)
+                sample_weight = tf.repeat(sample_weight, row_lengths)
+
+        # Take the flat values of predictions, targets and sample weihts as Keras
+        # losses does not support RaggedVariantTensor on GPU:
+        prediction = prediction.flat_values
+        if isinstance(target, tf.RaggedTensor):
+            target = target.flat_values
+        if isinstance(sample_weight, tf.RaggedTensor):
+            sample_weight = sample_weight.flat_values
+
+        # Ensuring targets are one-hot encoded if they are not
+        condition = tf.logical_and(
+            tf.logical_and(tf.rank(target) > 0, tf.shape(target)[-1] == 1),
+            tf.shape(prediction)[-1] > 1,
+        )
+        target = tf.cond(
+            condition,
+            lambda: tf.one_hot(
+                tf.cast(target, tf.int32),
+                tf.shape(prediction)[-1],
+                dtype=prediction.dtype,
+            ),
+            lambda: target,
+        )
+
+        # Makes target shape equal to the predictions tensor, as shape is lost after tf.cond
+        target = tf.reshape(target, tf.shape(prediction))
+
+        return prediction, target, sample_weight
+
     def adjust_predictions_and_targets(
         self,
         predictions: Dict[str, TensorLike],
-        targets: Optional[Union[tf.Tensor, Dict[str, tf.Tensor]]],
+        targets: Optional[Union[TensorLike, Dict[str, TensorLike]]],
+        sample_weights: Optional[Union[TensorLike, Dict[str, TensorLike]]],
     ):
-        """Adjusts the predctions and targets, doing the following transformations
-        if the target is provided:
-        - Converts ragged targets (and their masks) to dense, so that they are compatible
-        with most losses and metrics
-        - Copies the targets mask to predictions mask, if defined
-        - One-hot encode targets if their tf.rank(targets) == tf.rank(predictions)-1
-        - Ensures targets has the same shape and dtype as predicitnos
+        """Adjusts the predictions and targets to ensure compatibility with
+        most Keras losses and metrics.
+
+        If the predictions are ragged tensors, `_adjust_ragged_predictions_and_targets` is called,
+        otherwise `_adjust_dense_predictions_and_targets` is called.
 
         Parameters
         ----------
         predictions : Dict[str, TensorLike]
-            A dict with predictions for the tasks
+            A dictionary with predictions for the tasks.
         targets : Optional[Union[tf.Tensor, Dict[str, tf.Tensor]]]
-            A dict with targets for the tasks
+            A dictionary with targets for the tasks, or None if targets are not provided.
+        sample_weights : Optional[Union[tf.Tensor, Dict[str, tf.Tensor]]]
+            A dictionary with sample weights for the tasks,
+            or None if sample_weights are not provided.
+
         """
         if targets is None:
             return
 
         for k in targets:
-            # Convert ragged targets (and ragged mask) to dense
-            if isinstance(targets[k], tf.RaggedTensor):
-                dense_target_mask = None
-                if getattr(targets[k], "_keras_mask", None) is not None:
-                    dense_target_mask = targets[k]._keras_mask.to_tensor()
-                targets[k] = targets[k].to_tensor()
-                if dense_target_mask is not None:
-                    targets[k]._keras_mask = dense_target_mask
-
-            if getattr(targets[k], "_keras_mask", None) is not None:
-                # Copies the mask from the targets to the predictions
-                # because Keras considers the prediction mask in loss
-                # and metrics computation
-                predictions[k]._keras_mask = targets[k]._keras_mask
-
-            # Ensuring targets and preds have the same dtype
-            targets[k] = tf.cast(targets[k], predictions[k].dtype)
-
-            # Ensuring targets are one-hot encoded if they are not
-            targets[k] = tf.cond(
-                tf.rank(targets[k]) == tf.rank(predictions[k]) - 1,
-                lambda: tf.one_hot(
-                    tf.cast(targets[k], tf.int32),
-                    tf.shape(predictions[k])[-1],
-                    dtype=predictions[k].dtype,
-                ),
-                lambda: targets[k],
-            )
-            # Makes target shape equal to the predictions tensor, as shape is lost after tf.cond
-            targets[k] = tf.reshape(targets[k], tf.shape(predictions[k]))
+            if isinstance(predictions[k], tf.RaggedTensor):
+                (
+                    predictions[k],
+                    targets[k],
+                    sample_weights[k],
+                ) = self._adjust_ragged_predictions_and_targets(
+                    predictions[k], targets[k], sample_weights[k]
+                )
+            else:
+                (
+                    predictions[k],
+                    targets[k],
+                    sample_weights[k],
+                ) = self._adjust_dense_predictions_and_targets(
+                    predictions[k], targets[k], sample_weights[k]
+                )
 
     def train_step(self, data):
         """Custom train step using the `compute_loss` method."""
 
         with tf.GradientTape() as tape:
             x, y, sample_weight = unpack_x_y_sample_weight(data)
 
@@ -1064,15 +1287,16 @@
         Returns
         -------
         Optional[Schema]
             Schema corresponding to the inputs of the model
         """
         schema = getattr(self, "schema", None)
         if isinstance(schema, Schema) and schema.column_names:
-            return schema
+            target_tags = [Tags.TARGET, Tags.BINARY_CLASSIFICATION, Tags.REGRESSION]
+            return schema.excluding_by_tag(target_tags)
 
     def _maybe_set_schema(self, maybe_loader):
         """Try to set the correct schema on the model or loader.
 
         Parameters
         ----------
         maybe_loader : Union[Loader, Any]
@@ -1129,14 +1353,17 @@
         train_metrics_steps=1,
         pre=None,
         **kwargs,
     ):
         x = _maybe_convert_merlin_dataset(x, batch_size, **kwargs)
         self._maybe_set_schema(x)
 
+        if hasattr(x, "batch_size"):
+            self._batch_size = x.batch_size
+
         validation_data = _maybe_convert_merlin_dataset(
             validation_data, batch_size, shuffle=shuffle, **kwargs
         )
 
         callbacks = self._add_metrics_callback(callbacks, train_metrics_steps)
         if hvd_installed and hvd.size() > 1:
             callbacks = self._add_horovod_callbacks(callbacks)
@@ -1150,14 +1377,16 @@
             for k, v in locals().items()
             if k not in ["self", "kwargs", "train_metrics_steps", "pre"] and not k.startswith("__")
         }
 
         if pre:
             self._reset_compile_cache()
             self.train_pre = pre
+            if isinstance(self.train_pre, SequenceTransform):
+                self.train_pre.configure_for_train()
 
         out = super().fit(**fit_kwargs)
 
         if pre:
             del self.train_pre
 
         return out
@@ -1236,14 +1465,16 @@
         **kwargs,
     ):
         x = _maybe_convert_merlin_dataset(x, batch_size, shuffle=False, **kwargs)
 
         if pre:
             self._reset_compile_cache()
             self.test_pre = pre
+            if isinstance(self.test_pre, SequenceTransform):
+                self.test_pre.configure_for_test()
 
         out = super().evaluate(
             x,
             y,
             batch_size,
             verbose,
             sample_weight,
@@ -1331,47 +1562,71 @@
         if hvd_installed and hvd.rank() != 0:
             return
         super().save(*args, **kwargs)
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class Model(BaseModel):
+    """Merlin Model class
+
+    Parameters
+    ----------
+    context : Optional[ModelContext], optional
+        ModelContext is used to store/retrieve public variables across blocks,
+        by default None.
+    pre : Optional[BlockType], optional
+        Optional `Block` instance to apply before the `call` method of the Two-Tower block
+    post : Optional[BlockType], optional
+        Optional `Block` instance to apply on both outputs of Two-tower model
+        to output a single Tensor.
+    schema : Optional[Schema], optional
+        The `Schema` object with the input features.
+    prep_features: Optional[bool]
+        Whether this block should prepare list and scalar features
+        from the dataloader format. By default True.
+    """
+
     def __init__(
         self,
         *blocks: Block,
         context: Optional[ModelContext] = None,
         pre: Optional[tf.keras.layers.Layer] = None,
         post: Optional[tf.keras.layers.Layer] = None,
         schema: Optional[Schema] = None,
+        prep_features: Optional[bool] = True,
         **kwargs,
     ):
         super(Model, self).__init__(**kwargs)
+
         context = context or ModelContext()
         if len(blocks) == 1 and isinstance(blocks[0], SequentialBlock):
             blocks = blocks[0].layers
 
         self.blocks = blocks
         for block in self.submodules:
             if hasattr(block, "_set_context"):
                 block._set_context(context)
 
         self.pre = pre
         self.post = post
         self.context = context
         self._is_fitting = False
+        self._batch_size = None
 
         if schema is not None:
             self.schema = schema
         else:
             input_block_schemas = [
                 block.schema for block in self.submodules if getattr(block, "is_input", False)
             ]
             self.schema = sum(input_block_schemas, Schema())
 
-        self.prepare_features = PrepareFeatures(self.schema)
+        self.prep_features = prep_features
+
+        self._prepare_features = PrepareFeatures(self.schema)
         self._frozen_blocks = set()
 
     def save(
         self,
         export_path: Union[str, os.PathLike],
         include_optimizer=True,
         save_traces=True,
@@ -1396,49 +1651,54 @@
             export_path,
             include_optimizer=include_optimizer,
             save_traces=save_traces,
             save_format="tf",
         )
         input_schema = self.schema
         output_schema = get_output_schema(export_path)
-        save_merlin_metadata(export_path, self, input_schema, output_schema)
+        save_merlin_metadata(export_path, input_schema, output_schema)
 
     @classmethod
     def load(cls, export_path: Union[str, os.PathLike]) -> "Model":
         """Loads a model that was saved with `model.save()`.
 
         Parameters
         ----------
         export_path : Union[str, os.PathLike]
             The path to the saved model.
         """
         return tf.keras.models.load_model(export_path)
 
-    def _maybe_build(self, inputs):
-        if isinstance(inputs, dict):
-            if isinstance(self.input_schema, Schema) and set(inputs.keys()) != set(
-                self.input_schema.column_names
-            ):
-                model_input_features = set(self.input_schema.column_names)
-                call_input_features = set(inputs.keys())
+    def _check_schema_and_inputs_matching(self, inputs):
+        if isinstance(self.input_schema, Schema):
+            model_expected_features = set(
+                expected_input_cols_from_schema(self.input_schema, inputs)
+            )
+            call_input_features = set(inputs.keys())
+            if model_expected_features != call_input_features:
                 raise ValueError(
                     "Model called with a different set of features "
                     "compared with the input schema it was configured with. "
                     "Please check that the inputs passed to the model are only  "
                     "those required by the model. If you're using a Merlin Dataset, "
                     "the `schema` property can be changed to control the features being returned. "
-                    f"\nModel input features:\n\t{model_input_features}"
+                    f"\nModel expected features:\n\t{model_expected_features}"
                     f"\nCall input features:\n\t{call_input_features}"
-                    f"\nFeatures in model only:"
-                    f"\n\t{model_input_features.difference(call_input_features)}"
-                    f"\nFeatures in call only:"
-                    f"\n\t{call_input_features.difference(model_input_features)}"
+                    f"\nFeatures expected by model input schema only:"
+                    f"\n\t{model_expected_features.difference(call_input_features)}"
+                    f"\nFeatures provided in inputs only:"
+                    f"\n\t{call_input_features.difference(model_expected_features)}"
                 )
 
-            _ragged_inputs = self.prepare_features(inputs)
+    def _maybe_build(self, inputs):
+        if isinstance(inputs, dict):
+            self._check_schema_and_inputs_matching(inputs)
+            _ragged_inputs = inputs
+            if self.prep_features:
+                _ragged_inputs = self._prepare_features(inputs)
             feature_shapes = {k: v.shape for k, v in _ragged_inputs.items()}
             feature_dtypes = {k: v.dtype for k, v in _ragged_inputs.items()}
 
             for block in self.blocks:
                 block._feature_shapes = feature_shapes
                 block._feature_dtypes = feature_dtypes
                 for child in block.submodules:
@@ -1452,15 +1712,17 @@
         Parameters
         ----------
         input_shape : tf.TensorShape, optional
             The input shape, by default None
         """
         last_layer = None
 
-        input_shape = self.prepare_features.compute_output_shape(input_shape)
+        if self.prep_features:
+            self._prepare_features.build(input_shape)
+            input_shape = self._prepare_features.compute_output_shape(input_shape)
 
         if self.pre is not None:
             self.pre.build(input_shape)
             input_shape = self.pre.compute_output_shape(input_shape)
 
         for layer in self.blocks:
             try:
@@ -1478,22 +1740,26 @@
 
         if self.post is not None:
             self.post.build(input_shape)
 
         self.built = True
 
     def call(self, inputs, targets=None, training=False, testing=False, output_context=False):
+        outputs = inputs
+        features = self._prepare_features(inputs, targets=targets)
+        if isinstance(features, tuple):
+            features, targets = features
+        if self.prep_features:
+            outputs = features
         context = self._create_context(
-            self.prepare_features(inputs),
+            features,
             targets=targets,
             training=training,
             testing=testing,
         )
-
-        outputs = inputs
         if self.pre:
             outputs, context = self._call_child(self.pre, outputs, context)
 
         for block in self.blocks:
             outputs, context = self._call_child(block, outputs, context)
 
         if self.post:
@@ -1589,14 +1855,15 @@
         return cls(_input_block, block, prediction_tasks)
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
         pre = config.pop("pre", None)
         post = config.pop("post", None)
         schema = config.pop("schema", None)
+        batch_size = config.pop("batch_size", None)
 
         layers = [
             tf.keras.layers.deserialize(conf, custom_objects=custom_objects)
             for conf in config.values()
         ]
 
         if pre is not None:
@@ -1604,21 +1871,81 @@
 
         if post is not None:
             post = tf.keras.layers.deserialize(post, custom_objects=custom_objects)
 
         if schema is not None:
             schema = schema_utils.tensorflow_metadata_json_to_schema(schema)
 
-        return cls(*layers, pre=pre, post=post, schema=schema)
+        model = cls(*layers, pre=pre, post=post, schema=schema)
+
+        # For TF/Keras 2.11 calling the model with sample inputs to trigger build
+        # so that variable restore works correctly.
+        # TODO: review if this needs changing for 2.12
+        if (
+            saving_lib
+            and hasattr(saving_lib, "_SAVING_V3_ENABLED")
+            and saving_lib._SAVING_V3_ENABLED.value
+        ):
+            inputs = model.get_sample_inputs(batch_size=batch_size)
+            if inputs:
+                model(inputs)
+
+        return model
+
+    def get_sample_inputs(self, batch_size=None):
+        batch_size = batch_size or 2
+        if self.input_schema is not None:
+            inputs = {}
+            for column in self.input_schema:
+                shape = [batch_size]
+                try:
+                    dtype = column.dtype.to("tensorflow")
+                except ValueError:
+                    dtype = tf.float32
+
+                if column.int_domain:
+                    maxval = column.int_domain.max
+                elif column.float_domain:
+                    maxval = column.float_domain.max
+                else:
+                    maxval = 1
+
+                if column.is_list and column.is_ragged:
+                    row_length = (
+                        int(column.value_count.max)
+                        if column.value_count and column.value_count.max
+                        else 3
+                    )
+                    values = tf.random.uniform(
+                        [batch_size * row_length],
+                        dtype=dtype,
+                        maxval=maxval,
+                    )
+                    offsets = tf.cumsum([0] + [row_length] * batch_size)
+                    inputs[f"{column.name}__values"] = values
+                    inputs[f"{column.name}__offsets"] = offsets
+                elif column.is_list:
+                    row_length = (
+                        int(column.value_count.max)
+                        if column.value_count and column.value_count.max
+                        else 3
+                    )
+                    inputs[column.name] = tf.random.uniform(
+                        shape + [row_length], dtype=dtype, maxval=maxval
+                    )
+                else:
+                    inputs[column.name] = tf.random.uniform(shape, dtype=dtype, maxval=maxval)
+            return inputs
 
     def get_config(self):
         config = maybe_serialize_keras_objects(self, {}, ["pre", "post"])
         config["schema"] = schema_utils.schema_to_tensorflow_metadata_json(self.schema)
         for i, layer in enumerate(self.blocks):
             config[i] = tf.keras.utils.serialize_keras_object(layer)
+        config["batch_size"] = self._batch_size
 
         return config
 
     def _set_save_spec(self, inputs, args=None, kwargs=None):
         # We need to overwrite this in order to fix a Keras-bug in TF<2.9
         super()._set_save_spec(inputs, args, kwargs)
 
@@ -1784,14 +2111,18 @@
         ...
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class RetrievalModel(Model):
     """Embedding-based retrieval model."""
 
+    def __init__(self, *args, **kwargs):
+        kwargs["prep_features"] = False
+        super().__init__(*args, **kwargs)
+
     def evaluate(
         self,
         x=None,
         y=None,
         item_corpus: Optional[Union[merlin.io.Dataset, TopKIndexBlock]] = None,
         batch_size=None,
         verbose=1,
@@ -2019,15 +2350,15 @@
             candidate_name = output.candidate_name
 
         if query and candidate:
             encoder = ParallelBlock({query_name: query, candidate_name: candidate})
         else:
             encoder = query
 
-        super().__init__(encoder, output, pre=pre, post=post, **kwargs)
+        super().__init__(encoder, output, pre=pre, post=post, prep_features=False, **kwargs)
 
         self._query_name = query_name
         self._candidate_name = candidate_name
         self._encoder = encoder
         self._output = output
 
     def query_embeddings(
@@ -2194,22 +2525,26 @@
     outputs: Union[List[str], List[PredictionTask], ParallelPredictionBlock, List[ParallelBlock]]
 ):
     "Extracts tasks names from outputs"
     if isinstance(outputs, ParallelPredictionBlock):
         output_names = outputs.task_names
     elif isinstance(outputs, ParallelBlock):
         if all(isinstance(x, ModelOutput) for x in outputs.parallel_values):
-            output_names = [o.full_name for o in outputs.parallel_values]
+            output_names = [o.task_name for o in outputs.parallel_values]
         else:
             raise ValueError("The blocks within ParallelBlock must be ModelOutput.")
     elif isinstance(outputs, (list, tuple)):
         if all(isinstance(x, PredictionTask) for x in outputs):
             output_names = [o.task_name for o in outputs]  # type: ignore
         elif all(isinstance(x, ModelOutput) for x in outputs):
-            output_names = [o.full_name for o in outputs]  # type: ignore
+            output_names = [o.task_name for o in outputs]  # type: ignore
         else:
             raise ValueError(
                 "The blocks within the list/tuple must be ModelOutput or PredictionTask."
             )
+    elif isinstance(outputs, PredictionTask):
+        output_names = [outputs.task_name]
+    elif isinstance(outputs, ModelOutput):
+        output_names = [outputs.task_name]
     else:
-        raise ValueError("Invalid outputs")
+        raise ValueError("Invalid model outputs")
     return output_names
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/models/benchmark.py` & `merlin-models-23.4.0/merlin/models/tf/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/models/ranking.py` & `merlin-models-23.4.0/merlin/models/tf/models/ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import warnings
 from typing import List, Optional, Union
 
+import tensorflow as tf
+
 from merlin.models.tf.blocks.cross import CrossBlock
 from merlin.models.tf.blocks.dlrm import DLRMBlock
 from merlin.models.tf.blocks.interaction import FMBlock
 from merlin.models.tf.blocks.mlp import MLPBlock, RegularizerType
 from merlin.models.tf.core.aggregation import ConcatFeatures
-from merlin.models.tf.core.base import Block
+from merlin.models.tf.core.base import Block, BlockType
 from merlin.models.tf.core.combinators import ParallelBlock, TabularBlock
 from merlin.models.tf.inputs.base import InputBlockV2
 from merlin.models.tf.inputs.embedding import EmbeddingOptions, Embeddings
 from merlin.models.tf.models.base import Model
 from merlin.models.tf.models.utils import parse_prediction_blocks
 from merlin.models.tf.outputs.base import ModelOutputType
 from merlin.models.tf.prediction_tasks.base import ParallelPredictionBlock, PredictionTask
@@ -281,14 +283,15 @@
     deep_regularizer: Optional[RegularizerType] = None,
     wide_regularizer: Optional[RegularizerType] = None,
     deep_dropout: Optional[float] = None,
     wide_dropout: Optional[float] = None,
     prediction_tasks: Optional[
         Union[PredictionTask, List[PredictionTask], ParallelPredictionBlock, ModelOutputType]
     ] = None,
+    pre: Optional[BlockType] = None,
     **wide_body_kwargs,
 ) -> Model:
     """
     The Wide&Deep architecture [1] was proposed by Google
     in 2016 to balance between the ability of neural networks to generalize and capacity
     of linear models to memorize relevant feature interactions. The deep part is an MLP
     model, with categorical features represented as embeddings, which are concatenated
@@ -367,16 +370,15 @@
         (with maximum size defined) where the missing values are padded with zeros, as in the
         following example.
 
         ```python
         # Multi-hot features
         multi_hot_encoding = mm.SequentialBlock(
                 mm.Filter(multi_hot_schema),
-                # Assuming max size of multi-hot features is 5
-                ml.AsDenseFeatures(max_seq_length=5),
+                ml.ToDense(multi_hot_schema),
                 mm.CategoryEncoding(multi_hot_schema, sparse=True, output_mode="multi_hot")
         )
         ```
         Linear models are not able to compute feature interaction (like MLPs).
         So to give the wide part more power we perform paired feature interactions
         as a preprocessing step, so that every possible combination of the values of
         two categorical features is mapped to a single id. That way, the model is be
@@ -392,16 +394,15 @@
         single item category. You can explicitly ignore those combinations to reduce a bit
         the feature space.
 
         ```python
         # 2nd-level features interaction
         features_crossing = mm.SequentialBlock(
                     mm.Filter(wide_schema),
-                    # Assuming max size of multi-hot features is 5
-                    ml.AsDenseFeatures(max_seq_length=5),
+                    ml.ToDense(wide_schema),
                     mm.HashedCrossAll(
                         wide_schema,
                         # The crossed features will be hashed to this number of bins
                         num_bins=100,
                         # Performs 2nd feature interactions, typically max is 3rd level
                         max_level=2,
                         output_mode="multi_hot",
@@ -505,15 +506,22 @@
     if not deep_schema:
         deep_schema = schema
 
     branches = dict()
 
     if not deep_input_block:
         if deep_schema is not None and len(deep_schema) > 0:
-            deep_input_block = InputBlockV2(deep_schema)
+            deep_input_block = InputBlockV2(
+                deep_schema,
+                categorical=Embeddings(
+                    deep_schema.select_by_tag(Tags.CATEGORICAL),
+                    sequence_combiner=tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1)),
+                ),
+            )
+
     if deep_input_block:
         deep_body = deep_input_block.connect(deep_block).connect(
             MLPBlock(
                 [1],
                 no_activation_last_layer=True,
                 kernel_regularizer=deep_regularizer,
                 bias_regularizer=deep_regularizer,
@@ -549,11 +557,11 @@
 
     if len(branches) == 0:
         raise ValueError(
             "At least the deep part (deep_schema/deep_input_block)"
             " or wide part (wide_schema/wide_input_block) must be provided."
         )
 
-    wide_and_deep_body = ParallelBlock(branches, aggregation="element-wise-sum")
+    wide_and_deep_body = ParallelBlock(branches, pre=pre, aggregation="element-wise-sum")
     model = Model(wide_and_deep_body, prediction_blocks)
 
     return model
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/models/retrieval.py` & `merlin-models-23.4.0/merlin/models/tf/models/retrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,10 +575,11 @@
         outputs = ContrastiveOutput(
             to_call=candidate_table,
             logits_temperature=logits_temperature,
             post=post,
             negative_samplers=PopularityBasedSamplerV2(
                 max_num_samples=num_sampled, max_id=num_classes - 1, min_id=min_sampled_id
             ),
+            logq_sampling_correction=True,
         )
 
     return RetrievalModelV2(query=query, output=outputs)
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/models/utils.py` & `merlin-models-23.4.0/merlin/models/tf/models/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/base.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         pre: Optional[Layer] = None,
         post: Optional[Layer] = None,
         logits_temperature: float = 1.0,
         **kwargs,
     ):
         logits_scaler = kwargs.pop("logits_scaler", None)
         self.target = target
-        self.full_name = self.task_name(self.target)
+        self.full_name = self.get_task_name(self.target)
 
         super().__init__(name=name or self.full_name, **kwargs)
         self.to_call = to_call
         self.default_loss = default_loss
         self.default_metrics_fn = default_metrics_fn
         self.pre = pre
         self.post = post
@@ -88,14 +88,18 @@
             self.logits_scaler = logits_scaler
             self.logits_temperature = logits_scaler.temperature
         else:
             self.logits_temperature = logits_temperature
             if logits_temperature != 1.0:
                 self.logits_scaler = LogitsTemperatureScaler(logits_temperature)
 
+    @property
+    def task_name(self) -> str:
+        return self.full_name
+
     def build(self, input_shape=None):
         """Builds the PredictionBlock.
 
         Parameters
         ----------
         input_shape : tf.TensorShape, optional
             The input shape, by default None
@@ -126,14 +130,17 @@
 
         if self.post is not None:
             output_shape = self.post.compute_output_shape(output_shape)
 
         return output_shape
 
     def __call__(self, inputs, *args, **kwargs):
+        training = kwargs.get("training", False)
+        testing = kwargs.get("testing", False)
+
         # call pre
         if self.pre:
             inputs = tf_utils.call_layer(self.pre, inputs, **kwargs)
 
         # super call
         outputs = super(ModelOutput, self).__call__(inputs, *args, **kwargs)
 
@@ -141,15 +148,16 @@
             outputs = tf_utils.call_layer(self.post, outputs, target_name=self.target, **kwargs)
 
         if getattr(self, "logits_scaler", None):
             if isinstance(outputs, tf.Tensor):
                 targets = kwargs.pop("targets", None)
                 if isinstance(targets, dict) and self.target in targets:
                     targets = targets[self.target]
-                outputs = Prediction(outputs, targets)
+                if training or testing:
+                    outputs = Prediction(outputs, targets)
             outputs = tf_utils.call_layer(self.logits_scaler, outputs, **kwargs)
 
         return outputs
 
     def create_default_metrics(self):
         metrics = self.get_default_metrics()
         for metric in metrics:
@@ -241,15 +249,15 @@
             objects.append("default_loss")
 
         config = tf_utils.maybe_serialize_keras_objects(self, config, objects)
 
         return config
 
     @classmethod
-    def task_name(cls, target_name):
+    def get_task_name(cls, target_name):
         base_name = to_snake_case(cls.__name__)
         return name_fn(target_name, base_name) if target_name else base_name
 
     @classmethod
     def from_config(cls, config):
         config["default_metrics_fn"] = cls._parse_function_from_config(
             config, "default_metrics_fn", "module", "function_type"
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/block.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             model_output_cls = BinaryOutput
         elif col.name in cat:
             if col.int_domain.max == 1:
                 model_output_cls = BinaryOutput
             else:
                 model_output_cls = CategoricalOutput
 
-        task_name = model_output_cls.task_name(col.name)
+        task_name = model_output_cls.get_task_name(col.name)
 
         if task_name in outputs:
             output_block = outputs[task_name]
         else:
             # Creates outputs only for the tasks not provided in model_outputs
             output_block = model_output_cls(col)
             outputs[task_name] = output_block
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/classification.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -242,15 +242,14 @@
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
         **kwargs,
     ):
-
         if feature is not None:
             if isinstance(feature, Schema):
                 assert len(feature) == 1, "Schema can have max 1 feature"
                 col_schema = feature.first
             else:
                 col_schema = feature
 
@@ -321,21 +320,26 @@
 
     def build(self, input_shape):
         self.bias = self.add_weight(
             name="output_layer_bias",
             shape=(self.num_classes,),
             initializer=self.bias_initializer,
         )
-
+        self.table.build(input_shape)
         return super().build(input_shape)
 
     def call(self, inputs, training=False, **kwargs) -> tf.Tensor:
+        is_ragged = isinstance(inputs, tf.RaggedTensor)
+        if is_ragged:
+            original_inputs = inputs
+            inputs = inputs.flat_values
         logits = tf.matmul(inputs, self.table.table.embeddings, transpose_b=True)
         logits = tf.nn.bias_add(logits, self.bias)
-
+        if is_ragged:
+            logits = original_inputs.with_flat_values(logits)
         return logits
 
     @property
     def embeddings(self):
         return self.table.table.embeddings
 
     def embedding_lookup(self, inputs, **kwargs):
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/contrastive.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/contrastive.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import logging
-from typing import List, Optional, Protocol, Union, runtime_checkable
+import warnings
+from typing import List, Optional, Protocol, Tuple, Union, runtime_checkable
 
 import tensorflow as tf
 from tensorflow.keras.layers import Layer
 
 import merlin.io
 from merlin.models.tf.core.prediction import Prediction
 from merlin.models.tf.inputs.embedding import EmbeddingTable
@@ -73,14 +74,28 @@
         by default 'categorical_crossentropy'
     get_default_metrics: Callable, optional
         A function returning the list of default metrics
         to use for categorical-classification
     store_negative_ids: bool, optional
         Whether to store negative ids for post-processing
         by default False
+    logq_sampling_correction: bool, optional
+        The LogQ correction is a standard technique for
+        sampled softmax and popularity-biased sampling.
+        It subtracts from the logits the
+        log expected count/prob of the positive and
+        negative samples in order to not overpenalize the
+        popular items for being sampled more often as negatives.
+        It can be enabled if a single negative sampler is provided
+        and if it provides the sampler provides the
+        sampling probabilities (i.e. implements with_sampling_probs()).
+        Another alternative for performing logQ correction is using
+        ContrastiveOutput(..., post=PopularityLogitsCorrection(item_frequencies)),
+        where you need to provide the items frequency probability distribution (prior).
+        Default is False.
 
     References:
     ----------
     [1] Hakan Inan, Khashayar Khosravi, and Richard Socher. 2016. Tying word vectors
     and word classifiers: A loss framework for language modeling. arXiv preprint
     arXiv:1611.01462 (2016).
 
@@ -128,14 +143,15 @@
         default_loss: Union[str, tf.keras.losses.Loss] = "categorical_crossentropy",
         default_metrics_fn: MetricsFn = default_categorical_prediction_metrics,
         downscore_false_negatives=True,
         false_negative_score: float = MIN_FLOAT,
         query_name: str = "query",
         candidate_name: str = "candidate",
         store_negative_ids: bool = False,
+        logq_sampling_correction: Optional[bool] = False,
         **kwargs,
     ):
         self.col_schema = None
         _to_call = None
         if to_call is not None:
             if isinstance(to_call, (Schema, ColumnSchema)):
                 if isinstance(to_call, Schema):
@@ -164,14 +180,15 @@
 
         self.negative_samplers = parse_negative_samplers(negative_samplers)
         self.downscore_false_negatives = downscore_false_negatives
         self.false_negative_score = false_negative_score
         self.query_name = query_name
         self.candidate_name = candidate_name
         self.store_negative_ids = store_negative_ids
+        self.logq_sampling_correction = logq_sampling_correction
 
         self.target_name = kwargs.pop("target", target_name)
         super().__init__(
             to_call=_to_call,
             default_loss=default_loss,
             default_metrics_fn=default_metrics_fn,
             name=name,
@@ -216,16 +233,20 @@
             if isinstance(targets, dict):
                 positive_id = targets[self.col_schema.name]
             positive_embedding = self.embedding_lookup(positive_id)
         else:
             positive_id = features[self.col_schema.name]
             positive_embedding = inputs[self.candidate_name]
 
-        positive = Candidate(positive_id, {**features}).with_embedding(positive_embedding)
-        negative = self.sample_negatives(positive, features, training=training, testing=testing)
+        positive = Candidate(id=positive_id, metadata={**features}).with_embedding(
+            positive_embedding
+        )
+        negative, positive = self.sample_negatives(
+            positive, features, training=training, testing=testing
+        )
         if self.has_candidate_weights and (
             positive.id.shape != negative.id.shape or positive != negative
         ):
             negative = negative.with_embedding(self.embedding_lookup(negative.id))
 
         return self.outputs(query_embedding, positive, negative)
 
@@ -258,14 +279,26 @@
         # Apply dot-product
         negative_scores = tf.linalg.matmul(query_embedding, negative.embedding, transpose_b=True)
 
         positive_scores = tf.reduce_sum(
             tf.multiply(query_embedding, positive.embedding), keepdims=True, axis=-1
         )
 
+        if self.logq_sampling_correction:
+            if positive.sampling_prob is None or negative.sampling_prob is None:
+                warnings.warn(
+                    "The logQ sampling correction is enabled, but sampling probs were not found "
+                    "for both positive and negative candidates",
+                    RuntimeWarning,
+                )
+
+            epsilon = 1e-16
+            positive_scores -= tf.math.log(positive.sampling_prob + epsilon)
+            negative_scores -= tf.math.log(tf.transpose(negative.sampling_prob + epsilon))
+
         if self.downscore_false_negatives:
             negative_scores, _ = tf_utils.rescore_false_negatives(
                 positive.id, negative.id, negative_scores, self.false_negative_score
             )
 
         outputs = tf.concat([positive_scores, negative_scores], axis=-1)
 
@@ -289,15 +322,15 @@
 
     def sample_negatives(
         self,
         positive: Candidate,
         features: TabularData,
         training=False,
         testing=False,
-    ) -> Candidate:
+    ) -> Tuple[Candidate, Candidate]:
         """Method to sample negatives from `self.negative_samplers`
 
         Parameters
         ----------
         positive_items : Items
             Positive items (ids and metadata)
         features : TabularData
@@ -305,24 +338,36 @@
         training : bool, optional
             Flag for train mode, by default False
         testing : bool, optional
             Flag for test mode, by default False
 
         Returns
         -------
-        Items
-            Class containing the sampled negative ids
+        Tuple[Candidate, Candidate]
+            Tuple of candidates with sampled negative ids and the provided positive ids
+            added with the sampling probability
         """
         sampling_kwargs = {"training": training, "testing": testing, "features": features}
         candidates: List[Candidate] = []
+
+        if self.logq_sampling_correction and len(self.negative_samplers) > 1:
+            raise ValueError(
+                "It is only possible to apply logQ sampling correction "
+                "(logq_sampling_correction=True) when only one negative sampler is provided."
+            )
+
         for sampler in self.negative_samplers:
-            sampled: Candidate = tf_utils.call_layer(sampler, positive, **sampling_kwargs)
+            neg_samples: Candidate = tf_utils.call_layer(sampler, positive, **sampling_kwargs)
+
+            # Adds to the positive and negative candidates their sampling probs from the sampler
+            positive = sampler.with_sampling_probs(positive)
+            neg_samples = sampler.with_sampling_probs(neg_samples)
 
-            if sampled.id is not None:
-                candidates.append(sampled)
+            if neg_samples.id is not None:
+                candidates.append(neg_samples)
             else:
                 LOG.warn(
                     f"The sampler {type(sampler).__name__} returned no samples for this batch."
                 )
 
         if len(candidates) == 0:
             raise Exception(
@@ -330,15 +375,15 @@
             )
 
         negatives = candidates[0]
         if len(candidates) > 1:
             for neg in candidates[1:]:
                 negatives += neg
 
-        return negatives
+        return negatives, positive
 
     def embedding_lookup(self, ids: tf.Tensor):
         return self.to_call.embedding_lookup(tf.squeeze(ids))
 
     def to_dataset(self, gpu=None) -> merlin.io.Dataset:
         return merlin.io.Dataset(tf_utils.tensor_to_df(self.to_call.embeddings, gpu=gpu))
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/regression.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/sampling/base.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/sampling/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,78 +26,85 @@
 class Candidate(NamedTuple):
     """Store candidate id and their metadata
 
     Parameters
     ----------
     id : tf.Tensor
         The tensor of item ids
+    sampling_prob : tf.Tensor
+        Useful for logQ correction, based on the sampling distribution
     metadata:
         dictionary of tensors containing meta information
         about items such as item embeddings and item category
     """
 
     id: tf.Tensor
     metadata: Dict[str, tf.Tensor]
+    sampling_prob: Optional[tf.Tensor] = None
 
     @property
     def embedding(self) -> tf.Tensor:
         return self.metadata[EMBEDDING_KEY]
 
     @property
     def has_embedding(self) -> bool:
         return EMBEDDING_KEY in self.metadata
 
     def with_embedding(self, embedding: tf.Tensor) -> "Candidate":
         self.metadata[EMBEDDING_KEY] = embedding
 
         return self
 
+    def with_sampling_prob(self, sampling_prob: tf.Tensor) -> "Candidate":
+        return Candidate(id=self.id, metadata=self.metadata, sampling_prob=sampling_prob)
+
     def __add__(self, other):
         metadata = {}
         for key in self.metadata:
             if key in other.metadata:
                 metadata[key] = _list_to_tensor([self.metadata[key], other.metadata[key]])
 
-        return Candidate(
-            id=_list_to_tensor([self.id, other.id]),
-            metadata=metadata,
-        )
+        return Candidate(id=_list_to_tensor([self.id, other.id]), metadata=metadata)
 
     @property
     def shape(self) -> "Candidate":
-        return Candidate(self.id.shape, {key: val.shape for key, val in self.metadata.items()})
+        return Candidate(
+            id=self.id.shape, metadata={key: val.shape for key, val in self.metadata.items()}
+        )
 
     def __repr__(self):
         metadata = {key: str(val) for key, val in self.metadata.items()}
 
-        return f"Candidate({self.id}, {metadata})"
+        return f"Candidate({self.id}, {self.sampling_prob}, {metadata})"
 
     def __str__(self):
         metadata = {key: str(val) for key, val in self.metadata.items()}
 
-        return f"Candidate({self.id}, {metadata})"
+        return f"Candidate({self.id}, {self.sampling_prob}, {metadata})"
 
     def __eq__(self, other) -> bool:
         if self.id.shape != other.id.shape:
             return False
 
         return self.id.ref() == other.id.ref()
 
     def get_config(self):
         return {
-            "ids": self.id.as_list() if self.id else None,
-            "metadata": {key: val.as_list() for key, val in self.metadata.items()},
+            "id": self.id,
+            "sampling_prob": self.sampling_prob,
+            "metadata": self.metadata,
         }
 
     @classmethod
     def from_config(cls, config):
-        ids = tf.TensorShape(config["config"]["id"])
-        metadata = {key: tf.TensorShape(val) for key, val in config["config"]["metadata"].items()}
+        ids = config["config"]["id"]
+        sampling_prob = config["config"]["sampling_prob"]
+        metadata = config["config"]["metadata"]
 
-        return cls(ids, metadata)
+        return cls(ids, sampling_prob, metadata)
 
 
 negative_sampling_registry: Registry = Registry.class_registry("tf.negative_sampling")
 
 
 class CandidateSampler(tf.keras.layers.Layer, RegistryMixin["CandidateSampler"], abc.ABC):
     """Base-class for negative sampling
@@ -136,14 +143,17 @@
     def add(self, items: Candidate):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def sample(self) -> Candidate:
         raise NotImplementedError()
 
+    def with_sampling_probs(self, items: Candidate) -> Candidate:
+        return items
+
     @property
     def max_num_samples(self) -> int:
         return self._max_num_samples
 
     def set_max_num_samples(self, value) -> None:
         self._max_num_samples = value
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/sampling/in_batch.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/sampling/in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/outputs/topk.py` & `merlin-models-23.4.0/merlin/models/tf/outputs/topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,15 +140,14 @@
             Name of the layer. By default None
         """
 
         super().__init__(k=k, name=name, **kwargs)
         self._candidates = kwargs.pop("_candidates", None)
 
     def index(self, candidates: tf.Tensor, identifiers: Optional[tf.Tensor] = None) -> "BruteForce":
-
         tf.assert_equal(
             tf.rank(candidates), 2, f"candidates must be 2-D tensor (got {candidates.shape})"
         )
 
         if identifiers is None:
             identifiers = tf.range(candidates.shape[0])
 
@@ -276,15 +275,14 @@
         post: Optional[Layer] = None,
         logits_temperature: float = 1.0,
         name: Optional[str] = None,
         default_loss: Union[str, tf.keras.losses.Loss] = "categorical_crossentropy",
         default_metrics_fn: MetricsFn = default_categorical_prediction_metrics,
         **kwargs,
     ):
-
         if isinstance(to_call, str):
             if candidates is None:
                 raise ValueError(
                     "You should provide the dataset of pre-trained embeddings"
                     " when `to_call` is the top-k strategy name "
                 )
             if isinstance(candidates, merlin.io.Dataset):
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/base.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/classification.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/multi.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/multi.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/next_item.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/next_item.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/regression.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/prediction_tasks/retrieval.py` & `merlin-models-23.4.0/merlin/models/tf/prediction_tasks/retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/transformers/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/transformers/block.py` & `merlin-models-23.4.0/merlin/models/tf/transformers/block.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,17 @@
     ]
     return main_layer
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class TransformerBlock(Block):
     """
-    Class to support HF Transformers for session-based and sequential-based recommendation models.
+    Base class to support HuggingFace Transformers for session-based and
+    sequential-based recommendation models.
+
     Parameters
     ----------
     transformer: TransformerBody
         One of the following HuggingFace classes:
         Pretrained Config or model, or the custom keras layer `TF*MainLayer`,
         related to a specific transformer architecture.
     transformer_pre: tf.keras.layers.Layer
@@ -67,23 +69,31 @@
         Layer to extract the desired tensors from the HuggingFace dataclass
         `TFBaseModelOutputWithPoolingAndCrossAttentions`
         by default `last_hidden_state`
     pre: Optional[Union[str, tf.keras.layers.Layer]]
         A block to use before the main transformer block, by default None
     post: Optional[Union[str, tf.keras.layers.Layer]]
         A block to use after the main transformer block, by default None
+    masking_post:
+        A block to use to postprocess the output of the transformer block based on
+        keras mask information, by default None
+    masking_pre:
+        A block to use to prepare the inputs to the transformer block based on
+        keras mask information, by default None
     """
 
     def __init__(
         self,
         transformer: TransformerBody,
         pre: Optional[Union[str, tf.keras.layers.Layer]] = None,
         post: Optional[Union[str, tf.keras.layers.Layer]] = None,
         transformer_pre=PrepareTransformerInputs(),
         transformer_post: Optional[Union[str, tf.keras.layers.Layer]] = "last_hidden_state",
+        masking_post: Optional[tf.keras.layers.Layer] = None,
+        masking_pre: Optional[tf.keras.layers.Layer] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         if isinstance(transformer, PretrainedConfig):
             model_cls = transformers.TF_MODEL_MAPPING[transformer.__class__]
             self.transformer = get_tf_main_layer(model_cls(transformer))
@@ -103,14 +113,32 @@
             pre = block_registry.parse(pre)
 
         if isinstance(post, str):
             post = block_registry.parse(post)
 
         self.post = post
         self.pre = pre
+        self._masking_post = masking_post
+        self._masking_pre = masking_pre
+
+    @property
+    def masking_post(self):
+        return self._masking_post
+
+    @masking_post.setter
+    def masking_post(self, block):
+        self._masking_post = block
+
+    @property
+    def masking_pre(self):
+        return self._masking_pre
+
+    @masking_pre.setter
+    def masking_pre(self, block):
+        self._masking_pre = block
 
     def build(self, input_shape=None):
         """Builds the sequential block
 
         Parameters
         ----------
         input_shape : tf.TensorShape, optional
@@ -131,40 +159,62 @@
         transformer = self.transformer(pre)
         out = combinators.call_sequentially(list(self.to_call_post), transformer, **kwargs)
 
         return out
 
     @property
     def to_call_pre(self):
+        if self.masking_pre:
+            yield self.masking_pre
+
         if self.pre:
             yield self.pre
 
         yield self.transformer_pre
 
     @property
     def to_call_post(self):
         yield self.transformer_post
 
+        if self.masking_post:
+            yield self.masking_post
+
         if self.post:
             yield self.post
 
     def get_config(self):
         config = super().get_config()
         config = maybe_serialize_keras_objects(
             self,
             config,
-            ["transformer", "pre", "post", "transformer_pre", "transformer_post"],
+            [
+                "transformer",
+                "pre",
+                "post",
+                "transformer_pre",
+                "transformer_post",
+                "masking_pre",
+                "masking_post",
+            ],
         )
         return config
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
         config = maybe_deserialize_keras_objects(
             config,
-            ["transformer", "pre", "post", "transformer_pre", "transformer_post"],
+            [
+                "transformer",
+                "pre",
+                "post",
+                "transformer_pre",
+                "transformer_post",
+                "masking_post",
+                "masking_pre",
+            ],
         )
 
         output = TransformerBlock(**config)
         output.__class__ = cls
 
         return output
 
@@ -223,15 +273,14 @@
         initializer_range=0.01,
         layer_norm_eps=0.03,
         dropout=0.3,
         pad_token=0,
         log_attention_weights=False,
         **kwargs,
     ) -> BertConfig:
-
         return BertConfig(
             hidden_size=d_model,
             num_attention_heads=n_head,
             num_hidden_layers=n_layer,
             max_position_embeddings=max_position_embeddings,
             hidden_act=hidden_act,
             intermediate_size=d_model * 4,
@@ -300,15 +349,14 @@
         initializer_range=0.01,
         layer_norm_eps=0.03,
         dropout=0.3,
         pad_token=0,
         log_attention_weights=False,
         **kwargs,
     ) -> AlbertConfig:
-
         return AlbertConfig(
             hidden_size=d_model,
             num_attention_heads=n_head,
             num_hidden_layers=n_layer,
             hidden_act=hidden_act,
             intermediate_size=d_model * 4,
             hidden_dropout_prob=dropout,
@@ -377,15 +425,14 @@
         initializer_range=0.01,
         layer_norm_eps=0.03,
         dropout=0.3,
         pad_token=0,
         log_attention_weights=False,
         **kwargs,
     ) -> RobertaConfig:
-
         return RobertaConfig(
             hidden_size=d_model,
             num_hidden_layers=n_layer,
             num_attention_heads=n_head,
             max_position_embeddings=max_position_embeddings + 8,
             hidden_act=hidden_act,
             initializer_range=initializer_range,
@@ -458,15 +505,14 @@
         layer_norm_eps=0.03,
         dropout=0.3,
         pad_token=0,
         log_attention_weights=False,
         mem_len=1,
         **kwargs,
     ) -> XLNetConfig:
-
         return XLNetConfig(
             d_model=d_model,
             d_inner=d_model * 4,
             n_layer=n_layer,
             n_head=n_head,
             attn_type=attn_type,
             ff_activation=hidden_act,
@@ -536,15 +582,14 @@
         initializer_range=0.01,
         layer_norm_eps=0.03,
         dropout=0.3,
         pad_token=0,
         log_attention_weights=False,
         **kwargs,
     ) -> GPT2Config:
-
         return GPT2Config(
             n_embd=d_model,
             n_inner=d_model * 4,
             n_layer=n_layer,
             n_head=n_head,
             activation_function=hidden_act,
             initializer_range=initializer_range,
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/transformers/transforms.py` & `merlin-models-23.4.0/merlin/models/tf/transformers/transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,27 +77,34 @@
 
         Returns
         -------
         tf.Tensor
             If inference, returns a 2-D tensor with the hidden states of
             the target position
         """
-        batch_size = tf.shape(inputs)[0]
+        if isinstance(inputs, tf.RaggedTensor):
+            batch_size = tf.shape(inputs.row_lengths())[0]
+        else:
+            batch_size = tf.shape(inputs)[0]
         if not training and not testing:
-            if getattr(inputs, "_keras_mask", None) is not None:
+            if isinstance(inputs, tf.RaggedTensor):
+                inputs = inputs[:, -1:, :]
+                inputs = tf.squeeze(tf.sparse.to_dense(inputs.to_sparse()), axis=1)
+
+            elif getattr(inputs, "_keras_mask", None) is not None:
                 inputs = tf.reshape(
                     tf.boolean_mask(inputs, inputs._keras_mask), (-1, inputs.shape[-1])
                 )
-        tf.debugging.assert_equal(
-            tf.shape(inputs)[0],
-            batch_size,
-            f"The resulting tensor has {tf.shape(inputs)[0]} rows, which does not match"
-            f" the inputs batch-size {batch_size}. During inference only one position "
-            "candidate (the last one) should be masked per example",
-        )
+            tf.debugging.assert_equal(
+                tf.shape(inputs)[0],
+                batch_size,
+                f"The resulting tensor has {tf.shape(inputs)[0]} rows, which does not match"
+                f" the inputs batch-size {batch_size}. During inference only one position "
+                "candidate (the last one) should be masked per example",
+            )
         return inputs
 
 
 @Block.registry.register("pooler_output")
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class PoolerOutput(Layer):
     """Select the pooled representation of the sequence
@@ -228,7 +235,34 @@
 
 
 @Block.registry.register("sequence_cls_index")
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class SequenceClsIndex(SequenceSummary):
     def __init__(self, initializer_range: float = 0.02, **kwargs):
         super().__init__("cls_index", initializer_range=initializer_range, **kwargs)
+
+
+@tf.keras.utils.register_keras_serializable(package="merlin.models")
+class TransformerOutputToRagged(Block):
+    """Converts the dense outputs returned by the transformer layer to
+    a ragged tensor using masking information.
+
+    This layer takes dense inputs from the transformer layer and
+    applies the masking information (in the `_keras_mask` attribute)
+    to produce a ragged tensor output. The resulting tensor contains predictions
+    only at masked positions (targets).
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.supports_masking = True
+
+    def call(self, inputs: tf.Tensor) -> Dict[str, tf.Tensor]:
+        if isinstance(inputs, tf.RaggedTensor):
+            return input
+
+        if getattr(inputs, "_keras_mask", None) is not None:
+            mask = inputs._keras_mask
+            if isinstance(mask, tf.RaggedTensor):
+                mask = mask.to_tensor()
+            inputs = tf.ragged.boolean_mask(inputs, mask)
+        return inputs
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/bias.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/bias.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,16 @@
 class PopularityLogitsCorrection(Block):
     """Correct the predicted logit scores based on the item frequency,
     using the logQ correction proposed in sampled softmax [1]_ [2]_.
     The correction is done as `logits -= log(item_prob)`,
     where `item_prob = item_freq_count / sum(item_freq_count)` is
     a probability distribution of the item frequency. In a nutshell,
     the logQ correction aims to increase the prediction scores (logits)
-    for infrequent items and decrease the ones for frequent items.
+    for infrequent items and decrease the ones for frequent items, so
+    that they are not much more penalized for being sampled more often.
 
     References
     ----------
     .. [1] Yoshua Bengio and Jean-Sébastien Sénécal. 2003. Quick Training of Probabilistic
        Neural Nets by Importance Sampling. In Proceedings of the conference on Artificial
        Intelligence and Statistics (AISTATS).
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/negative_sampling.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/negative_sampling.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 # limitations under the License.
 #
 from typing import Optional, Tuple, Union
 
 import tensorflow as tf
 
 from merlin.models.tf.core.prediction import Prediction
+from merlin.models.tf.transforms.features import PrepareFeatures
 from merlin.models.tf.typing import TabularData
-from merlin.models.tf.utils.tf_utils import list_col_to_ragged
+from merlin.models.tf.utils.tf_utils import calculate_batch_size_from_inputs
 from merlin.models.utils import schema_utils
 from merlin.schema import Schema, Tags
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class InBatchNegatives(tf.keras.layers.Layer):
     """Random in-batch negative sampling.
@@ -36,50 +37,57 @@
         The schema
     n_per_positive : int
         Number of negatives for each positive
     seed : Optional[int], optional
         The random seed, by default None
     run_when_testing : bool, optional
         Whether the negative sampling should happen when testing=True, by default True
+    prep_features: Optional[bool]
+        Whether this block should prepare list and scalar features
+        from the dataloader format. By default False.
     """
 
     def __init__(
         self,
         schema: Schema,
         n_per_positive: int,
         seed: Optional[int] = None,
         run_when_testing: bool = True,
+        prep_features: Optional[bool] = False,
         **kwargs
     ):
-
-        super(InBatchNegatives, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.n_per_positive = n_per_positive
         self.item_id_col = schema.select_by_tag(Tags.ITEM_ID).column_names[0]
         self.schema = schema.select_by_tag(Tags.ITEM)
         self.seed = seed
         self.run_when_testing = run_when_testing
+        self.prep_features = prep_features
+        self._prepare_features = PrepareFeatures(schema)
 
     def call(
         self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs
     ) -> Union[Prediction, Tuple]:
         """Extend batch of inputs and targets with negatives."""
 
         def get_tuple(x, y):
             if training or testing or y is None:
                 return Prediction(x, y)
             return (x, y)
 
         if targets is None or (testing and not self.run_when_testing):
             return get_tuple(inputs, targets)
 
+        if self.prep_features:
+            inputs = self._prepare_features(inputs, targets=targets)
+            if isinstance(inputs, tuple):
+                inputs, targets = inputs
+
         # 1. Select item-features
-        fist_input = list(inputs.values())[0]
-        batch_size = (
-            fist_input.shape[0] if not isinstance(fist_input, tuple) else fist_input[1].shape[0]
-        )
+        batch_size = calculate_batch_size_from_inputs(inputs)
 
         if batch_size is None:
             return get_tuple(inputs, targets)
 
         sampled_num_negatives = self.n_per_positive * batch_size
         # 2. Sample `n_per_positive * batch_size` items at random
         sampled_positive_idx = tf.random.uniform(
@@ -103,17 +111,14 @@
 
         # 3. Loop through all features:
         #   - For item-feature: append from item-collection
         #   - For user-feature: repeat `n_per_positive` times
         item_cols = self.schema.column_names
         outputs = {}
         for name, val in inputs.items():
-            if isinstance(val, tuple):
-                val = list_col_to_ragged(val)
-
             if name in item_cols:
                 negatives = tf.gather(val, sampled_positive_idx)
             else:
                 if isinstance(val, tf.RaggedTensor):
                     negatives = tf.concat([val] * self.n_per_positive, axis=0)
                 else:
                     negatives = tf.repeat(val, self.n_per_positive, axis=0)
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/noise.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/regularization.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/regularization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/transforms/sequence.py` & `merlin-models-23.4.0/merlin/models/tf/transforms/sequence.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 # limitations under the License.
 #
 from typing import Optional, Tuple, Union
 
 import tensorflow as tf
 from tensorflow.keras.backend import random_bernoulli
 
+from merlin.models.tf.core import combinators
 from merlin.models.tf.core.base import Block, BlockType, PredictionOutput
 from merlin.models.tf.core.combinators import TabularBlock
-from merlin.models.tf.transforms.tensor import ListToRagged
+from merlin.models.tf.transforms.features import PrepareFeatures
 from merlin.models.tf.typing import TabularData
 from merlin.models.tf.utils import tf_utils
 from merlin.models.utils import schema_utils
+from merlin.models.utils.dependencies import is_transformers_available
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 @Block.registry.register_with_multiple_names("remove_pad_3d")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class RemovePad3D(Block):
     """
@@ -81,33 +83,38 @@
     ----------
     schema : Schema
         The schema with the sequential columns to be truncated
     target : Union[str, Tags, ColumnSchema]
         The sequential input column that will be used to extract the target
     pre : Optional[BlockType], optional
         A block that is called before this method call().
-        If not set, the ListToRagged() block is applied to convert
+        P.s. The PrepareFeatures() block is applied to convert
         the tuple representation of sequential features to RaggedTensors,
         so that the tensors sequences can be shifted/truncated
+    transformer:  Optional[TransformerBlock]
+        The transformer block that leverages the group of sequences returned
+        by the given SequenceTransform, by default None.
     """
 
     def __init__(
         self,
         schema: Schema,
         target: Union[str, Tags, ColumnSchema],
         pre: Optional[BlockType] = None,
+        transformer=None,
         **kwargs,
     ):
-        _pre = ListToRagged()
+        _pre = PrepareFeatures(schema)
         if pre:
             _pre = _pre.connect(pre)
         super().__init__(pre=_pre, schema=schema, **kwargs)
 
         self.target = target
         self.target_name = self._get_target(target)
+        self.transformer = transformer
 
     def _get_target(self, target):
         if (
             (isinstance(target, str) and target not in self.schema.column_names)
             or (isinstance(target, Tags) and len(self.schema.select_by_tag(target)) > 0)
             or (isinstance(target, ColumnSchema) and target not in self.schema)
         ):
@@ -152,15 +159,15 @@
         seq_inputs_shapes = {
             col: inputs[col].get_shape().as_list() for col in self.schema.column_names
         }
 
         seq_shapes = list(seq_inputs_shapes.values())
         if not all(x == seq_shapes[0] for x in seq_shapes):
             raise ValueError(
-                "The sequential inputs must have the same shape, but the shapes"
+                "The sequential inputs must have the same shape, but the shapes "
                 f"are different: {seq_inputs_shapes}"
             )
 
     def compute_output_shape(self, input_shape):
         new_input_shapes = dict()
         for k, v in input_shape.items():
             new_input_shapes[k] = v
@@ -185,14 +192,26 @@
         """Creates layer from its config. Returning the instance."""
         config = tf_utils.maybe_deserialize_keras_objects(config, ["pre", "post", "aggregation"])
         config["schema"] = schema_utils.tensorflow_metadata_json_to_schema(config["schema"])
         schema = config.pop("schema")
         target = config.pop("target")
         return cls(schema, target, **config)
 
+    def configure_for_train(self):
+        """Method called by the model.fit() to set additional model's
+        configuration before calling keras parent class `fit()`
+        """
+        pass
+
+    def configure_for_test(self):
+        """Method called by the model.evaluate() to check any custom model's
+        configuration before calling keras parent class `evaluate()`
+        """
+        pass
+
 
 @Block.registry.register_with_multiple_names("seq_predict_next")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class SequencePredictNext(SequenceTransform):
     """Prepares sequential inputs and targets for next-item prediction.
     The target is extracted from the shifted sequence of item ids and
     the sequential input features are truncated in the last position.
@@ -201,17 +220,16 @@
     ----------
     schema : Schema
         The schema with the sequential columns to be truncated
     target : Union[str, Tags, ColumnSchema]
         The sequential input column that will be used to extract the target
     pre : Optional[BlockType], optional
         A block that is called before this method call().
-        If not set, the ListToRagged() block is applied to convert
-        the tuple representation of sequential features to RaggedTensors,
-        so that the tensors sequences can be shifted/truncated
+        P.s. The PrepareFeatures() is called automatically before the pre
+        to convert the list features representation
     """
 
     def call(
         self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs
     ) -> Tuple:
         self._check_seq_inputs_targets(inputs)
 
@@ -244,14 +262,83 @@
                     new_input_shapes[k] = tf.TensorShape([v[1][0], None])
                 else:
                     # Reducing 1 position of the seq length
                     new_input_shapes[k] = tf.TensorShape([v[0], v[1] - 1])
 
         return new_input_shapes
 
+    def compute_mask(self, inputs, mask=None):
+        new_item_id_seq = inputs[self.target_name][:, :-1]
+        target_mask = tf.RaggedTensor.from_row_lengths(
+            values=tf.ones_like(new_item_id_seq.flat_values, dtype=tf.bool),
+            row_lengths=new_item_id_seq.row_lengths(),
+        )
+        self.target_mask = tf.squeeze(target_mask, axis=-1)
+
+        targets_mask = dict({self.target_name: self.target_mask})
+        inputs_mask = dict()
+        for k, v in inputs.items():
+            if k in self.schema.column_names:
+                inputs_mask[k] = self.target_mask
+            else:
+                inputs_mask[k] = None
+        return (inputs_mask, targets_mask)
+
+    def configure_for_train(self):
+        """Method called by the model.fit() to set the specialized
+        `masking_post` and `masking_pre` needed by the TransformerBlock
+        to align with the SequencePredictNext outputs.
+        """
+        if self.transformer is not None:
+            if not is_transformers_available():
+                raise ImportError("HuggingFace library `transformers` is required")
+            from merlin.models.tf.transformers.transforms import (
+                TransformerInferenceHiddenState,
+                TransformerOutputToRagged,
+            )
+
+            # set the tansformer block with the correct masking block
+            self.transformer.masking_post = combinators.SequentialBlock(
+                [TransformerOutputToRagged(), TransformerInferenceHiddenState()]
+            )
+            self.transformer.masking_pre = combinators.SequentialBlock(
+                [SequenceCausalLastInference(), ExtractMaskFromTargets()]
+            )
+
+    def configure_for_test(self):
+        """Method called by the model.evaluate() to check that the
+        `masking_post` and `masking_pre` set in the TransformerBlock
+        are aligned with the evaluation strategy of SequencePredictNext
+        """
+        if self.transformer is not None:
+            if self.transformer.masking_pre is None:
+                raise ValueError(
+                    "To evaluate using `SequencePredictNext`, ensure that your TransformerBlock has"
+                    " `masking_pre` set as"
+                    " `combinators.SequentialBlock("
+                    "    [SequenceCausalLastInference(), ExtractMaskFromTargets()]"
+                    ")`."
+                    " You can automatically set `masking_pre` by passing `SequencePredictNext`"
+                    " as the `pre` argument to the `fit` method: "
+                    "`model.fit(..., pre=SequencePredictNext(...))`."
+                )
+
+            if any(
+                isinstance(layer, ReplaceMaskedEmbeddings)
+                for layer in self.transformer.masking_pre.layers
+            ):
+                ValueError(
+                    "You cannot use `ReplaceMaskedEmbeddings` as `masking_pre`"
+                    " of your TransformerBlock with the `SequencePredictNext`"
+                    " evaluation strategy. Please ensure that your Transformer"
+                    " model has been trained with `SequencePredictNext`"
+                    " by passing it as the `pre` argument to the `fit` method: "
+                    "`model.fit(..., pre=SequencePredictNext(...))`."
+                )
+
 
 @Block.registry.register_with_multiple_names("seq_predict_last")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class SequencePredictLast(SequenceTransform):
     """Prepares sequential inputs and targets for last-item prediction.
     The target is extracted from the last element of sequence of item ids and
     the sequential input features are truncated before the last position.
@@ -260,28 +347,26 @@
     ----------
     schema : Schema
         The schema with the sequential columns to be truncated
     target : Union[str, Tags, ColumnSchema]
         The sequential input column that will be used to extract the target
     pre : Optional[BlockType], optional
         A block that is called before this method call().
-        If not set, the ListToRagged() block is applied to convert
-        the tuple representation of sequential features to RaggedTensors,
-        so that the tensors sequences can be processed
+        P.s. The PrepareFeatures() is called automatically before the pre
+        to convert the list features representation
     """
 
     @tf.function
     def call(
         self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs
     ) -> Tuple:
         self._check_seq_inputs_targets(inputs)
 
         # Shifts the target column to be the next item of corresponding input column
-        new_target = inputs[self.target_name][:, -1:]
-        new_target = tf.squeeze(tf.sparse.to_dense(new_target.to_sparse()), axis=1)
+        new_target = tf.squeeze(inputs[self.target_name][:, -1:], axis=1)
         if targets is None:
             targets = dict({self.target_name: new_target})
         elif isinstance(targets, dict):
             targets[self.target_name] = new_target
         else:
             raise ValueError("Targets should be None or a dict of tensors")
 
@@ -305,14 +390,49 @@
                     new_input_shapes[k] = tf.TensorShape([v[1][0], None])
                 else:
                     # Reducing 1 position of the seq length
                     new_input_shapes[k] = tf.TensorShape([v[0], v[1] - 1])
 
         return new_input_shapes
 
+    def compute_mask(self, inputs, mask=None):
+        new_item_id_seq = inputs[self.target_name][:, :-1]
+        self.target_mask = self._generate_target_mask(new_item_id_seq)
+        inputs_mask = dict()
+        for k, v in inputs.items():
+            if k in self.schema.column_names:
+                inputs_mask[k] = self.target_mask
+            else:
+                inputs_mask[k] = None
+
+        return (inputs_mask, self.target_mask)
+
+    def _generate_target_mask(self, ids_seq: tf.RaggedTensor) -> tf.RaggedTensor:
+        """Returns a bool ragged tensor with the last positions of the sequence masked
+
+        Parameters
+        ----------
+        ids_seq : tf.RaggedTensor
+            Sequence of ids, which are used to infer how many values
+            each sequence contains
+
+        Returns
+        -------
+        tf.RaggedTensor
+            Mask tensor, with True at the last positions
+        """
+        row_lengths = ids_seq.row_lengths(1)
+        max_seq_length = tf.cast(tf.reduce_max(row_lengths), tf.int32)
+
+        padding_mask = tf.sequence_mask(row_lengths)
+        targets_mask = tf.ragged.boolean_mask(
+            tf.cast(tf.one_hot(row_lengths - 1, max_seq_length), tf.bool), padding_mask
+        )
+        return targets_mask
+
 
 @Block.registry.register_with_multiple_names("seq_predict_random")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class SequencePredictRandom(SequenceTransform):
     """Prepares sequential inputs and targets for random-item prediction.
     A random element in the sequence (except the first one) is selected
     as target and all elements before the selected target as used as
@@ -322,17 +442,16 @@
     ----------
     schema : Schema
         The schema with the sequential columns to be truncated
     target : Union[str, Tags, ColumnSchema]
         The sequential input column that will be used to extract the target
     pre : Optional[BlockType], optional
         A block that is called before this method call().
-        If not set, the ListToRagged() block is applied to convert
-        the tuple representation of sequential features to RaggedTensors,
-        so that the tensors sequences can be shifted/truncated
+        P.s. The PrepareFeatures() is called automatically before the pre
+        to convert the list features representation
     """
 
     def call(
         self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs
     ) -> Tuple:
         self._check_seq_inputs_targets(inputs)
 
@@ -354,51 +473,88 @@
             ),
             1,
         )
 
         positions_matrix = tf.tile(
             tf.expand_dims(tf.range(0, max_length, dtype=tf.int32), 0), [batch_size, 1]
         )
-        input_mask = positions_matrix < random_targets_indices
+        self.random_mask = positions_matrix < random_targets_indices
         target_mask = positions_matrix == random_targets_indices
 
-        new_target = tf.squeeze(tf.ragged.boolean_mask(inputs[self.target_name], target_mask), 1)
+        new_target = tf.squeeze(
+            tf.ragged.boolean_mask(inputs[self.target_name], target_mask), axis=1
+        )
         if targets is None:
             targets = dict({self.target_name: new_target})
         elif isinstance(targets, dict):
             targets[self.target_name] = new_target
         else:
             raise ValueError("Targets should be None or a dict of tensors")
 
         new_inputs = dict()
         for k, v in inputs.items():
             if k in self.schema.column_names:
-                new_inputs[k] = tf.ragged.boolean_mask(v, input_mask)
+                new_inputs[k] = tf.ragged.boolean_mask(v, self.random_mask)
             else:
                 new_inputs[k] = v
 
         return (new_inputs, targets)
 
+    def compute_mask(self, inputs, mask=None):
+        new_item_id_seq = tf.ragged.boolean_mask(inputs[self.target_name], self.random_mask)
+
+        self.target_mask = self._generate_target_mask(new_item_id_seq)
+        inputs_mask = dict()
+        for k, v in inputs.items():
+            if k in self.schema.column_names:
+                inputs_mask[k] = self.target_mask
+            else:
+                inputs_mask[k] = None
+
+        return (inputs_mask, self.target_mask)
+
+    def _generate_target_mask(self, ids_seq: tf.RaggedTensor) -> tf.RaggedTensor:
+        """Returns a bool ragged tensor with the last positions of the sequence masked
+
+        Parameters
+        ----------
+        ids_seq : tf.RaggedTensor
+            Sequence of ids, which are used to infer how many values
+            each sequence contains
+
+        Returns
+        -------
+        tf.RaggedTensor
+            Mask tensor, with True at the last positions
+        """
+        row_lengths = ids_seq.row_lengths(1)
+        max_seq_length = tf.cast(tf.reduce_max(row_lengths), tf.int32)
+
+        padding_mask = tf.sequence_mask(row_lengths)
+        targets_mask = tf.ragged.boolean_mask(
+            tf.cast(tf.one_hot(row_lengths - 1, max_seq_length), tf.bool), padding_mask
+        )
+        return targets_mask
+
 
 @Block.registry.register_with_multiple_names("seq_target_as_input")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class SequenceTargetAsInput(SequenceTransform):
     """Creates targets to be equal to one of the sequential input features.
 
     Parameters
     ----------
     schema : Schema
         The schema with the sequential columns to be truncated
     target : Union[str, Tags, ColumnSchema]
         The sequential input column that will be used to extract the target
     pre : Optional[BlockType], optional
         A block that is called before this method call().
-        If not set, the ListToRagged() block is applied to convert
-        the tuple representation of sequential features to RaggedTensors,
-        so that the tensors sequences can be processed
+        P.s. The PrepareFeatures() is called automatically before the pre
+        to convert the list features representation
     """
 
     @tf.function
     def call(
         self, inputs: TabularData, targets=None, training=False, testing=False, **kwargs
     ) -> Tuple:
         self._check_seq_inputs_targets(inputs)
@@ -574,14 +730,71 @@
     def from_config(cls, config):
         config = tf_utils.maybe_deserialize_keras_objects(config, ["pre", "post", "aggregation"])
         schema = schema_utils.tensorflow_metadata_json_to_schema(config.pop("schema"))
         target = config.pop("target")
         masking_prob = config.pop("masking_prob")
         return cls(schema, target, masking_prob, **config)
 
+    def configure_for_train(self):
+        """Method called by the model.fit() to set the specialized
+        `masking_post` and `masking_pre` needed by the TransformerBlock
+        to align with the SequencePredictNext outputs.
+        """
+        if self.transformer is not None:
+            if not is_transformers_available():
+                raise ImportError("HuggingFace library `transformers` is required")
+            from merlin.models.tf.transformers.transforms import (
+                TransformerInferenceHiddenState,
+                TransformerOutputToRagged,
+            )
+
+            # set the tansformer block with the correct masking blocks
+            self.transformer.masking_post = combinators.SequentialBlock(
+                [TransformerOutputToRagged(), TransformerInferenceHiddenState()]
+            )
+            self.transformer.masking_pre = combinators.SequentialBlock(
+                [SequenceMaskLastInference(), ExtractMaskFromTargets(), ReplaceMaskedEmbeddings()]
+            )
+
+    def configure_for_test(self):
+        """Method called by the model.evaluate() to check that the
+        `masking_pre` set in the TransformerBlock is aligned with
+        the evaluation strategy of SequenceMaskRandom
+        """
+        if self.transformer is not None:
+            if self.transformer.masking_pre is None:
+                raise ValueError(
+                    "To evaluate using `SequenceMaskRandom`, ensure that your TransformerBlock has"
+                    " `masking_pre` set as"
+                    " `combinators.SequentialBlock("
+                    "   ["
+                    "        SequenceMaskLastInference(),"
+                    "        ExtractMaskFromTargets(),"
+                    "        ReplaceMaskedEmbeddings()"
+                    "   ]"
+                    ")`"
+                    " You can automatically set `masking_pre` by passing `SequenceMaskRandom`"
+                    " as the `pre` argument to the `fit` method:"
+                    " `model.fit(..., pre=SequenceMaskRandom(...))`."
+                )
+
+            if not any(
+                isinstance(layer, ReplaceMaskedEmbeddings)
+                for layer in self.transformer.masking_pre.layers
+            ):
+                ValueError(
+                    " The block `ReplaceMaskedEmbeddings` must be part of the `masking_pre`"
+                    " of your TransformerBlock to be able to use `SequenceMaskRandom`"
+                    " evaluation strategy."
+                    " Please ensure that your Transformer model has been trained with"
+                    " `SequenceMaskRandom` or `SequenceMaskLast`"
+                    " by passing it as the `pre` argument to the `fit` method: "
+                    "`model.fit(..., pre=SequenceMaskRandom(...))`."
+                )
+
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class SequenceMaskLast(SequenceTargetAsInput):
     """This block copies one of the sequence input features to be
     the target feature. The last item of the target (and corresponding
     sequences) is selected (masked) to be predicted
     The input and target masks are returned by using Keras Masking
@@ -645,28 +858,85 @@
     @classmethod
     def from_config(cls, config):
         config = tf_utils.maybe_deserialize_keras_objects(config, ["pre", "post", "aggregation"])
         schema = schema_utils.tensorflow_metadata_json_to_schema(config.pop("schema"))
         target = config.pop("target")
         return cls(schema, target, **config)
 
+    def configure_for_train(self):
+        """Method called by the model.fit() to set the specialized
+        `masking_post` and `masking_pre` needed by the TransformerBlock
+        to align with the SequencePredictNext outputs.
+        """
+        if self.transformer is not None:
+            if not is_transformers_available():
+                raise ImportError("HuggingFace library `transformers` is required")
+            from merlin.models.tf.transformers.transforms import (
+                TransformerInferenceHiddenState,
+                TransformerOutputToRagged,
+            )
+
+            # set the tansformer block with the correct masking blocks
+            self.transformer.masking_post = combinators.SequentialBlock(
+                [TransformerOutputToRagged(), TransformerInferenceHiddenState()]
+            )
+            self.transformer.masking_pre = combinators.SequentialBlock(
+                [SequenceMaskLastInference(), ExtractMaskFromTargets(), ReplaceMaskedEmbeddings()]
+            )
+
+    def configure_for_test(self):
+        """Method called by the model.evaluate() to check that the
+        `masking_pre` set in the TransformerBlock is aligned with
+        the evaluation strategy of SequenceMaskRandom
+        """
+        if self.transformer is not None:
+            if self.transformer.masking_pre is None:
+                raise ValueError(
+                    "To evaluate using `SequenceMaskLast`, ensure that your TransformerBlock has"
+                    " `masking_pre` set as"
+                    " `combinators.SequentialBlock("
+                    "   ["
+                    "        SequenceMaskLastInference(),"
+                    "        ExtractMaskFromTargets(),"
+                    "        ReplaceMaskedEmbeddings()"
+                    "   ]"
+                    ")`"
+                    " You can automatically set `masking_pre` by passing `SequenceMaskRandom`"
+                    " or `SequenceMaskLast` as the `pre` argument to the `fit` method:"
+                    " `model.fit(..., pre=SequenceMaskRandom(...))`."
+                )
+
+            if not any(
+                isinstance(layer, ReplaceMaskedEmbeddings)
+                for layer in self.transformer.masking_pre.layers
+            ):
+                ValueError(
+                    "The block `ReplaceMaskedEmbeddings` must be part of the `masking_pre`"
+                    " of your TransformerBlock to be able to use `SequenceMaskRandom`"
+                    " evaluation strategy."
+                    " Please ensure that your Transformer model has been trained with"
+                    " `SequenceMaskRandom` or `SequenceMaskLast`"
+                    " by passing it as the `pre` argument to the `fit` method: "
+                    "`model.fit(..., pre=SequenceMaskLast(...))`."
+                )
+
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class SequenceMaskLastInference(Block):
     def call(self, inputs, training=False, testing=False):
         self.inference_mode = not training and not testing
         if self.inference_mode:
             # Extending sequences in one position by copying the last embedding
             repeat = inputs[:, -1:, :]
             # repeat = tf.expand_dims(repeat, 1)
             inputs = tf.concat([inputs, repeat], axis=1)
         return inputs
 
     def compute_mask(self, inputs, mask=None):
-        """Selects (masks) the nex position after the
+        """Selects (masks) the next position after the
         last valid (non-padded) position of the sequential targets
         to be predicted.
         This method is called by Keras after call()
         and returns the mask that is going to be assigned
         to the input tensors, being accessible
         by tensor._keras_mask
         """
@@ -684,31 +954,26 @@
 
         return targets_mask
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class ReplaceMaskedEmbeddings(Block):
     """Takes a 3D input tensor (batch size x seq. length x embedding dim) and replaces
-     by a dummy trainable single embedding at the positions to be masked.
-     This block looks for the Keras mask (`._keras_mask`) in the following order:
-       1. Checks if the input tensor has a mask
-       2. Checks if there is a single target and if it has a mask
-       3. If there are multiple targets (dict) returns the mask of the target
-       that matches the first 2 dims of the input
-     This is useful to be used when PredictMasked() transformation is used in
-     the Loader, which randomly selects some targets to be predicted and uses
-     Keras Masking to cascade the `_keras_mask`. By replacing input embeddings
-     at masked positions we avoid target leakage when training models with
-     Masked Language Modeling (BERT-like)
-
-     **Note:** To support inference, the input sequence and its corresponding mask should be
-     extended by one position at the end to account for the next-item (`target`) position.
-     To do this, you should set `SequenceMaskLastInference` as a pre-layer of
-    `ReplaceMaskedEmbeddings()` using the sequential-block:
-    ```mm.SequentialBlock([mm.SequenceMaskLastInference(), mm.ReplaceMaskedEmbeddings()])```
+    by a dummy trainable single embedding at the positions to be masked.
+
+    This is useful to be used when PredictMasked() transformation is used in
+    the fit()/eval() methods, which randomly selects some targets to be predicted and uses
+    Keras Masking to cascade the `_keras_mask`. By replacing input embeddings
+    at masked positions we avoid target leakage when training models with
+    Masked Language Modeling (BERT-like).
+
+    To support masked training approach in Transformer-based model,
+    SequenceMaskRandom and SequenceLastRandom implements `configure_for_train` method
+    that sets `ReplaceMaskedEmbeddings` as part of the `masking_pre` of
+    the transformer block.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.supports_masking = True
 
     def build(self, input_shape):
@@ -720,41 +985,87 @@
         self.masked_embedding = tf.Variable(initializer(shape=[self.hidden_size], dtype=tf.float32))
 
         return super().build(input_shape)
 
     def call(
         self,
         inputs: Union[tf.Tensor, tf.RaggedTensor],
-        targets: Optional[Union[tf.Tensor, tf.RaggedTensor, TabularData]] = None,
     ) -> Union[tf.Tensor, tf.RaggedTensor]:
-        """If the sequence of input embeddings or the corresponding sequential
-        targets is masked (with `tensor._keras_mask` defined),
+        """If the sequence of input embeddings is masked (with `tensor._keras_mask` defined),
         replaces the input embeddings for masked elements
         Parameters
         ----------
         inputs : Union[tf.Tensor, tf.RaggedTensor]
             A tensor with sequences of vectors.
             Needs to be 3D (batch_size, sequence_length, embeddings dim).
             If inputs._keras_mask is defined uses it to infer the mask
-        targets : Union[tf.Tensor, tf.RaggedTensor, TabularData], optional
-            The target values, from which the mask can be extracted
-            if targets inputs._keras_mask is defined.
+
         Returns
         -------
         Union[tf.Tensor, tf.RaggedTensor]
-            If training, returns a tensor with the masked inputs replaced by the dummy embedding
+            returns a tensor with the masked inputs replaced by the dummy embedding
         """
         outputs = inputs
-        # Infers the mask from the inputs or targets
-        mask = self._infer_mask_from_inputs_or_targets(inputs, targets)
-        if mask is not None:
+        if getattr(inputs, "_keras_mask", None) is not None:
             # Replaces the embeddings at masked positions by a dummy trainable embedding
-            outputs = self._replace_masked_embeddings(inputs, mask)
+            outputs = self._replace_masked_embeddings(inputs, inputs._keras_mask)
         return outputs
 
+    def _replace_masked_embeddings(
+        self, inputs: Union[tf.Tensor, tf.RaggedTensor], mask: Union[tf.Tensor, tf.RaggedTensor]
+    ) -> tf.RaggedTensor:
+        """
+        Replaces in the inputs tensors the values masked as targets by a common trainable
+        embedding
+        """
+
+        tf.Assert(
+            tf_utils.check_inputs_mask_compatible_shape(inputs, mask),
+            [
+                "The inputs and mask need to be compatible: have the same dtype "
+                "(tf.Tensor or tf.RaggedTensor) and the tf.rank(mask) == tf.rank(inputs)-1"
+            ],
+        )
+
+        if isinstance(mask, tf.RaggedTensor):
+            mask = mask.with_row_splits_dtype(inputs.row_splits.dtype)
+
+        output = tf.where(
+            tf.cast(tf.expand_dims(mask, -1), tf.bool),
+            tf.cast(self.masked_embedding, dtype=inputs.dtype),
+            inputs,
+        )
+        return output
+
+
+@tf.keras.utils.register_keras_serializable(package="merlin.models")
+class ExtractMaskFromTargets(Block):
+    """
+    Recovers the mask information for the inputs from the mask information
+    stored in the targets.
+
+    This block looks for the Keras mask (`._keras_mask`) in the following order:
+        1. Checks if the input tensor has a mask.
+        2. Checks if there is a single target and if it has a mask.
+        3. If there are multiple targets (dictionary), returns the mask of the target
+        that matches the first two dimensions of the input.
+
+    This is useful to use when the mask information for the inputs may be lost in
+    previous non-mask-aware Merlin blocks.
+    """
+
+    def call(
+        self,
+        inputs: Union[tf.Tensor, tf.RaggedTensor],
+        targets: Optional[Union[tf.Tensor, tf.RaggedTensor, TabularData]] = None,
+    ) -> Union[tf.Tensor, tf.RaggedTensor]:
+        mask = self._infer_mask_from_inputs_or_targets(inputs, targets)
+        inputs._keras_mask = mask
+        return inputs
+
     def _infer_mask_from_inputs_or_targets(
         self,
         inputs: Union[tf.Tensor, tf.RaggedTensor],
         targets: Optional[Union[tf.Tensor, tf.RaggedTensor]] = None,
     ):
         mask = None
         if getattr(inputs, "_keras_mask", None) is not None:
@@ -768,15 +1079,15 @@
                         mask = single_target._keras_mask
                 elif len(targets) > 1:
                     # If there is more than 1 target, checks if only one
                     # target matches the shape sequence of the inputs
                     for _, v in targets.items():
                         if getattr(
                             v, "_keras_mask", None
-                        ) is not None and self._check_inputs_mask_compatible_shape(
+                        ) is not None and tf_utils.check_inputs_mask_compatible_shape(
                             inputs, v._keras_mask
                         ):
                             if mask is None:
                                 mask = v._keras_mask
                             else:
                                 raise ValueError(
                                     "It is not possible to infer the mask "
@@ -785,45 +1096,32 @@
                                     "the inputs shape (batch_size x seq_length)"
                                 )
             elif getattr(targets, "_keras_mask", None) is not None:
                 mask = targets._keras_mask
 
         return mask
 
-    def _check_inputs_mask_compatible_shape(
-        self, inputs: Union[tf.Tensor, tf.RaggedTensor], mask: Union[tf.Tensor, tf.RaggedTensor]
-    ):
-        result = False
-        if type(inputs) == type(mask) and (inputs.shape.as_list()[:-1] == mask.shape.as_list()):
-            if isinstance(inputs, tf.RaggedTensor):
-                result = tf.reduce_all(
-                    tf.cast(inputs.row_lengths(), tf.int32) == tf.cast(mask.row_lengths(), tf.int32)
-                )
-            else:
-                result = True
-        return result
-
-    def _replace_masked_embeddings(
-        self, inputs: Union[tf.Tensor, tf.RaggedTensor], mask: Union[tf.Tensor, tf.RaggedTensor]
-    ) -> tf.RaggedTensor:
-        """
-        Replaces in the inputs tensors the values masked as targets by a common trainable
-        embedding
-        """
 
-        tf.Assert(
-            self._check_inputs_mask_compatible_shape(inputs, mask),
-            [
-                "The inputs and mask need to be compatible: have the same dtype "
-                "(tf.Tensor or tf.RaggedTensor) and the tf.rank(mask) == tf.rank(inputs)-1"
-            ],
-        )
+@tf.keras.utils.register_keras_serializable(package="merlin.models")
+class SequenceCausalLastInference(Block):
+    def call(self, inputs, training=False, testing=False):
+        self.inference_mode = not training and not testing
+        return inputs
 
-        if isinstance(mask, tf.RaggedTensor):
-            mask = mask.with_row_splits_dtype(inputs.row_splits.dtype)
+    def compute_mask(self, inputs, mask=None):
+        """Selects (masks) the last non padded position of the
+        input sequence to be predicted.
+        This method is called by Keras after call()
+        and returns the mask that is going to be assigned
+        to the input tensors, being accessible
+        by tensor._keras_mask
+        """
+        if self.inference_mode:
+            if isinstance(inputs, tf.RaggedTensor):
+                row_lengths = inputs.row_lengths(1)
+                max_seq_length = tf.cast(tf.reduce_max(row_lengths), tf.int32)
 
-        output = tf.where(
-            tf.cast(tf.expand_dims(mask, -1), tf.bool),
-            tf.cast(self.masked_embedding, dtype=inputs.dtype),
-            inputs,
-        )
-        return output
+                padding_mask = tf.sequence_mask(row_lengths)
+                mask = tf.ragged.boolean_mask(
+                    tf.cast(tf.one_hot(row_lengths - 1, max_seq_length), tf.bool), padding_mask
+                )
+        return mask
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/typing.py` & `merlin-models-23.4.0/merlin/models/tf/typing.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/__init__.py` & `merlin-models-23.4.0/merlin/models/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/batch_utils.py` & `merlin-models-23.4.0/merlin/models/tf/utils/batch_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import tensorflow as tf
 
 from merlin.core.dispatch import DataFrameType, concat_columns, get_lib
 from merlin.models.tf.core.base import Block
 from merlin.models.tf.loader import Loader
-from merlin.models.tf.models.base import Model, RetrievalModel
+from merlin.models.tf.models.base import Model, RetrievalModel, get_task_names_from_outputs
 from merlin.models.utils.schema_utils import select_targets
 from merlin.schema import Schema, Tags
 
 
 class ModelEncode:
     def __init__(
         self,
@@ -76,18 +76,18 @@
         schema: tp.Optional[Schema] = None,
         output_concat_func=None,
     ):
         save_path = save_path or tempfile.mkdtemp()
         model.save(save_path)
 
         model_load_func = block_load_func if block_load_func else tf.keras.models.load_model
-        if not output_names:
+        if not output_names and isinstance(model, Model):
             try:
-                output_names = model.last.task_names
-            except AttributeError:
+                output_names = get_task_names_from_outputs(model.last)
+            except ValueError:
                 pass
         if not output_concat_func:
             if output_names and len(output_names) == 1:  # type: ignore
                 output_concat_func = np.concatenate
             else:
                 output_concat_func = get_lib().concat  # type: ignore
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/repr_utils.py` & `merlin-models-23.4.0/merlin/models/tf/utils/repr_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/search_utils.py` & `merlin-models-23.4.0/merlin/models/tf/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/testing_utils.py` & `merlin-models-23.4.0/merlin/models/tf/utils/testing_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import pathlib
 import platform
 import tempfile
-from typing import Any, Optional, Sequence, Tuple, Union
+from typing import Any, Tuple, Union
 
 import numpy as np
 import pytest
 import tensorflow as tf
 from keras.utils import tf_inspect
 from tensorflow.python.framework.test_util import disable_cudnn_autotune
 
 import merlin.io
 from merlin.models.tf.loader import Loader, sample_batch
 from merlin.models.tf.models.base import Model
-from merlin.schema import Schema
+from merlin.models.tf.transforms.features import PrepareFeatures, expected_input_cols_from_schema
+from merlin.schema import Tags
 
 
 def mark_run_eagerly_modes(*args, **kwargs):
     modes = [True, False]
 
     # As of TF 2.5 there's a bug that our EmbeddingFeatures don't work on M1 Macs
     if "macOS" in platform.platform() and "arm64-arm-64bit" in platform.platform():
@@ -99,15 +100,15 @@
     if reload_model:
         with tempfile.TemporaryDirectory() as tmpdir:
             model.save(tmpdir)
             loaded_model = tf.keras.models.load_model(tmpdir)
 
         assert isinstance(loaded_model, type(model))
 
-        x, y = sample_batch(dataloader, batch_size=50, to_ragged=False, prepare_features=False)
+        x, y = sample_batch(dataloader, batch_size=50, prepare_features=False)
         batch = [(x, y)]
 
         model_preds = model.predict(iter(batch))
         loaded_model_preds = loaded_model.predict(iter(batch))
 
         if isinstance(model_preds, dict):
             for task_name in model_preds:
@@ -120,48 +121,27 @@
         loaded_model.compile(run_eagerly=run_eagerly, optimizer=optimizer, **kwargs)
         loaded_model.fit(iter(batch))
 
         if model.input_schema:
             signature = loaded_model.signatures["serving_default"]
             signature_input_names = set(signature.structured_input_signature[1].keys())
 
-            model_input_names = []
-            for col in model.input_schema:
-                if col.is_list:
-                    # list columns are currently always passed
-                    # in as a tuple of (values, row_lengths)
-                    for i in ["1", "2"]:
-                        model_input_names.append(f"{col.name}_{i}")
-                else:
-                    model_input_names.append(col.name)
+            model_input_names = expected_input_cols_from_schema(model.input_schema)
 
             assert signature_input_names == set(model_input_names)
 
         return loaded_model, losses
 
     dataloader.stop()
 
     assert isinstance(model.from_config(model.get_config()), type(model))
 
     return model, losses
 
 
-def get_model_inputs(schema: Schema, list_cols: Optional[Sequence[str]] = None):
-    list_cols = list_cols or []
-    features = schema.column_names
-
-    # Right now the model expects a tuple for each list-column
-    for list_col in list_cols:
-        features.pop(features.index(list_col))
-        for i in ["1", "2"]:
-            features.append(f"{list_col}_{i}")
-
-    return features
-
-
 def test_model_signature(model, input_names, output_names):
     """Test that the model signature is correct."""
 
     signatures = getattr(model, "signatures", {}) or {}
     default_signature = signatures.get("serving_default")
 
     if not default_signature:
@@ -477,7 +457,43 @@
     if isinstance(expected_output_shape, dict):
         for key in expected_output_shape.keys():
             output_shape = _get_shape(output[key])
             assert list(output_shape) == list(expected_output_shape[key])
     else:
         output_shape = _get_shape(output)
         assert list(output_shape) == list(expected_output_shape)
+
+
+def loader_for_last_item_prediction(sequence_testing_data: merlin.io.Dataset, to_one_hot=True):
+    schema = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL)
+    prepare_features = PrepareFeatures(schema)
+
+    class LastInteractionAsTarget:
+        def compute_output_schema(self, input_schema):
+            return input_schema
+
+        @tf.function
+        def __call__(self, inputs, targets=None):
+            inputs = prepare_features(inputs)
+
+            seq_item_id_col = schema.select_by_tag(Tags.ITEM_ID).column_names[0]
+            targets = tf.squeeze(inputs[seq_item_id_col][:, -1:].flat_values, -1)
+            if to_one_hot:
+                targets = tf.one_hot(targets, schema[seq_item_id_col].int_domain.max + 1)
+
+            for name in schema.select_by_tag(Tags.SEQUENCE).column_names:
+                inputs[name] = inputs[name][:, :-1]
+
+            col_names = list(inputs.keys())
+            for k in col_names:
+                if isinstance(inputs[k], tf.RaggedTensor):
+                    inputs[f"{k}__values"] = inputs[k].values
+                    inputs[f"{k}__offsets"] = inputs[k].row_splits
+                    del inputs[k]
+
+            return inputs, targets
+
+    sequence_testing_data.schema = schema
+    dataloader = Loader(sequence_testing_data, batch_size=50)
+    _last_interaction_as_target = LastInteractionAsTarget()
+    dataloader = dataloader.map(_last_interaction_as_target)
+    return dataloader, schema
```

### Comparing `merlin-models-23.2.0/merlin/models/tf/utils/tf_utils.py` & `merlin-models-23.4.0/merlin/models/tf/utils/tf_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import numpy as np
 import tensorflow as tf
 from keras.utils.tf_inspect import getfullargspec
 from packaging import version
 from tensorflow.python import to_dlpack
 
+from merlin.core.compat import cudf, cupy
 from merlin.core.dispatch import DataFrameType
 from merlin.io import Dataset
 from merlin.models.tf.core.base import Block, ModelContext
 from merlin.models.tf.typing import TabularData
 from merlin.models.utils.misc_utils import filter_kwargs
 
 if version.parse(tf.__version__) < version.parse("2.3.0"):
@@ -43,30 +44,47 @@
     sizes = {}
     for feature in schema:
         name = feature.name
         if feature.is_list:
             sizes[name] = tf.TensorShape(
                 [
                     batch_size,
-                    max_sequence_length if max_sequence_length else feature.value_count.max,
+                    max_sequence_length if max_sequence_length else feature.shape.dims[1].max,
                 ]
             )
         elif feature.HasField("shape"):
             sizes[name] = tf.TensorShape([batch_size] + [d.size for d in feature.shape.dim])
         else:
             sizes[name] = tf.TensorShape([batch_size, 1])
 
     return sizes
 
 
+def calculate_batch_size_from_inputs(inputs):
+    input_shapes = {k: v.shape for k, v in inputs.items()}
+    batch_size = calculate_batch_size_from_input_shapes(input_shapes)
+    return batch_size
+
+
 def calculate_batch_size_from_input_shapes(input_shapes):
-    val = list(input_shapes.values())[0]
-    if isinstance(val, tuple) and isinstance(val[1], tf.TensorShape):
-        val = val[1]
-    return val[0]
+    non_ragged_features = list(
+        [k for k in input_shapes if not k.endswith("__values") and not k.endswith("__offsets")]
+    )
+    if len(non_ragged_features) > 0:
+        batch_size = input_shapes[non_ragged_features[0]][0]
+        return batch_size
+
+    ragged_features_offsets = list([k for k in input_shapes if k.endswith("__offsets")])
+    if len(ragged_features_offsets) > 0:
+        batch_size = input_shapes[ragged_features_offsets[0]][0]
+        if batch_size is not None:
+            batch_size -= 1
+        return batch_size
+
+    return None
 
 
 def maybe_serialize_keras_objects(
     self,
     config,
     maybe_serialize_keys,
 ):
@@ -194,15 +212,14 @@
 
 
 def create_output_placeholder(scores, ks):
     return tf.Variable(tf.zeros([tf.shape(scores)[0], len(ks)], tf.float32))
 
 
 def gather_torch_like(labels, indices, max_k):
-
     row_idxs = tf.repeat(tf.range(tf.shape(labels)[0]), max_k)
     col_idx = tf.reshape(indices, tf.shape(row_idxs))
     all_indices = tf.transpose(tf.stack([row_idxs, col_idx]))
 
     labels = tf.reshape(tf.gather_nd(labels, all_indices), (tf.shape(labels)[0], max_k))
     return labels
 
@@ -278,21 +295,15 @@
         return tf.cast(x, dtype)
 
     return x
 
 
 def tensor_to_df(tensor, index=None, gpu=None):
     if gpu is None:
-        try:
-            import cudf  # noqa: F401
-            import cupy
-
-            gpu = True
-        except ImportError:
-            gpu = False
+        gpu = cudf
 
     if gpu:
         # Note: It is not possible to convert Tensorflow tensors to the cudf dataframe
         # directly using dlPack (as the example commented below) because cudf.from_dlpack()
         # expects the 2D tensor to be in Fortran order (column-major), which is not
         # supported by TF (https://github.com/rapidsai/cudf/issues/10754).
         # df = cudf.from_dlpack(to_dlpack(tf.convert_to_tensor(embeddings)))
@@ -457,15 +468,44 @@
                 # filter out modelcontext
                 if type(sub_module) != ModelContext:
                     deque.append(sub_module)
     return list(result_blocks)
 
 
 @tf.function
-def list_col_to_ragged(col: Tuple[tf.Tensor, tf.Tensor]):
-    values = col[0][:, 0]
-    row_lengths = col[1][:, 0]
+def list_col_to_ragged(values: tf.Tensor, offsets: tf.Tensor):
+    if offsets.dtype.is_floating:
+        offsets = tf.cast(offsets, tf.int32)
+
+    return tf.RaggedTensor.from_row_splits(values, offsets)
+
+
+def check_inputs_mask_compatible_shape(
+    inputs: Union[tf.Tensor, tf.RaggedTensor], mask: Union[tf.Tensor, tf.RaggedTensor]
+):
+    """Check if the shape and the type of the input and mask tensors are compatible.
+    Parameters
+    ----------
+    inputs : Union[tf.Tensor, tf.RaggedTensor]
+        The input tensor, which can be either a dense or ragged tensor.
+    mask : Union[tf.Tensor, tf.RaggedTensor]
+        The mask tensor, which can be either a dense or ragged tensor.
 
-    if row_lengths.dtype.is_floating:
-        row_lengths = tf.cast(row_lengths, tf.int32)
+    Returns
+    -------
+    bool:
+        Returns True if the shape of the input and mask tensors are compatible, False otherwise.
 
-    return tf.RaggedTensor.from_row_lengths(values, row_lengths)
+    Notes
+    -----
+       The function assumes that the `inputs` tensor has one more dimension than the `mask` tensor,
+       with the extra dimension typically related to the embeddings dimension.
+    """
+    result = False
+    if type(inputs) == type(mask) and (inputs.shape.as_list()[:-1] == mask.shape.as_list()):
+        if isinstance(inputs, tf.RaggedTensor):
+            result = tf.reduce_all(
+                tf.cast(inputs.row_lengths(), tf.int32) == tf.cast(mask.row_lengths(), tf.int32)
+            )
+        else:
+            result = True
+    return result
```

### Comparing `merlin-models-23.2.0/merlin/models/torch/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/block/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/block/base.py` & `merlin-models-23.4.0/merlin/models/torch/block/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/block/mlp.py` & `merlin-models-23.4.0/merlin/models/torch/block/mlp.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/features/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/features/base.py` & `merlin-models-23.4.0/merlin/models/torch/features/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/features/continuous.py` & `merlin-models-23.4.0/merlin/models/torch/features/continuous.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/features/embedding.py` & `merlin-models-23.4.0/merlin/models/torch/features/embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/features/tabular.py` & `merlin-models-23.4.0/merlin/models/torch/features/tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/losses.py` & `merlin-models-23.4.0/merlin/models/torch/losses.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/model/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/model/base.py` & `merlin-models-23.4.0/merlin/models/torch/model/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/model/prediction_task.py` & `merlin-models-23.4.0/merlin/models/torch/model/prediction_task.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/tabular/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/tabular/aggregation.py` & `merlin-models-23.4.0/merlin/models/torch/tabular/aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/tabular/base.py` & `merlin-models-23.4.0/merlin/models/torch/tabular/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/tabular/transformations.py` & `merlin-models-23.4.0/merlin/models/torch/tabular/transformations.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/typing.py` & `merlin-models-23.4.0/merlin/models/torch/typing.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/utils/__init__.py` & `merlin-models-23.4.0/merlin/models/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/utils/data_utils.py` & `merlin-models-23.4.0/merlin/models/torch/utils/data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,14 @@
 class ShuffleDataset(IterableDataset):
     def __init__(self, dataset, buffer_size):
         super().__init__()
         self.dataset = dataset
         self.buffer_size = buffer_size
 
     def __iter__(self):
-
         logger.info("[SHUFFLE] INITIALIZING BUFFER_SIZE: {}".format(self.buffer_size))
 
         raise StopIteration()
         # TODO define The shuffle method for pyarrow dataloader
 
     def __len__(self):
         return len(self.dataset)
```

### Comparing `merlin-models-23.2.0/merlin/models/torch/utils/examples_utils.py` & `merlin-models-23.4.0/merlin/models/torch/utils/examples_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/torch/utils/torch_utils.py` & `merlin-models-23.4.0/merlin/models/torch/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/__init__.py` & `merlin-models-23.4.0/merlin/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/constants.py` & `merlin-models-23.4.0/merlin/models/utils/constants.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/dataset.py` & `merlin-models-23.4.0/merlin/models/utils/dataset.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,51 +10,82 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import warnings
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
 import pandas as pd
 from scipy.sparse import coo_matrix
 
 from merlin.io import Dataset
-from merlin.schema import Tags
+from merlin.schema import Schema, Tags
 
 
-def dataset_to_coo(dataset: Dataset):
+def dataset_to_coo(
+    dataset: Dataset,
+    target_column: Optional[str] = None,
+):
     """Converts a merlin.io.Dataset object to a scipy coo matrix"""
-    user_id_column = dataset.schema.select_by_tag(Tags.USER_ID).first.name
-    item_id_column = dataset.schema.select_by_tag(Tags.ITEM_ID).first.name
+    user_id_column = get_user_id_column_name(dataset)
+    item_id_column = get_item_id_column_name(dataset)
 
     columns = [user_id_column, item_id_column]
-    target_column = None
-    target = dataset.schema.select_by_tag(Tags.TARGET)
 
-    if len(target) > 1:
-        raise ValueError(
-            "Found more than one column tagged Tags.TARGET in the dataset schema."
-            f" Expected a single target column but found  {target.column_names}"
-        )
+    if not target_column:
+        target_column = get_target_column_name(dataset)
 
-    elif len(target) == 1:
-        target_column = target.first.name
+    if target_column:
         columns.append(target_column)
 
     df = dataset.to_ddf()[columns].compute(scheduler="synchronous")
 
     userids = _to_numpy(df[user_id_column])
     itemids = _to_numpy(df[item_id_column])
     targets = _to_numpy(df[target_column]) if target_column else np.ones(len(userids))
     return coo_matrix((targets.astype("float32"), (userids, itemids)))
 
 
+def get_schema(dataset_or_schema: Union[Dataset, Schema]) -> Schema:
+    if isinstance(dataset_or_schema, Dataset):
+        schema = dataset_or_schema.schema
+    elif isinstance(dataset_or_schema, Schema):
+        schema = dataset_or_schema
+    else:
+        raise ValueError(f"Cannot get schema from {type(dataset_or_schema)}.")
+    return schema
+
+
+def get_user_id_column_name(dataset_or_schema: Union[Dataset, Schema]) -> str:
+    schema = get_schema(dataset_or_schema)
+    return schema.select_by_tag(Tags.USER_ID).first.name
+
+
+def get_item_id_column_name(dataset_or_schema: Union[Dataset, Schema]) -> str:
+    schema = get_schema(dataset_or_schema)
+    return schema.select_by_tag(Tags.ITEM_ID).first.name
+
+
+def get_target_column_name(dataset_or_schema: Union[Dataset, Schema]) -> Optional[str]:
+    target_column = None
+    schema = get_schema(dataset_or_schema)
+    target = schema.select_by_tag(Tags.TARGET)
+    if len(target) > 1:
+        raise ValueError(
+            "Found more than one column tagged Tags.TARGET in the dataset schema."
+            f" Expected a single target column but found  {target.column_names}"
+        )
+    elif len(target) == 1:
+        target_column = target.first.name
+    return target_column
+
+
 def unique_rows_by_features(
     dataset: Dataset, features_tag: Union[str, Tags], grouping_tag: Union[str, Tags] = Tags.ID
 ) -> Dataset:
     """
     Select unique rows from a Dataset. Returns columns specified by `features_tag`
      that are unique based on the columns specified by the `grouping_tag`.
```

### Comparing `merlin-models-23.2.0/merlin/models/utils/dependencies.py` & `merlin-models-23.4.0/merlin/models/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/doc_utils.py` & `merlin-models-23.4.0/merlin/models/utils/doc_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/example_utils.py` & `merlin-models-23.4.0/merlin/models/utils/example_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/misc_utils.py` & `merlin-models-23.4.0/merlin/models/utils/misc_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 import itertools
 import logging
 import os
 import sys
 import time
 from typing import Any, Dict
 
+from merlin.io.dataset import Dataset
+
 logger = logging.getLogger(__name__)
 
 
 def filter_kwargs(
     kwargs, thing_with_kwargs, cascade_kwargs_if_possible=False, argspec_fn=inspect.getfullargspec
 ):
     arg_spec = argspec_fn(thing_with_kwargs)
@@ -189,19 +191,14 @@
         to load at once.
     engine: str
         parameter to specify the file format,
         possible values are: ["parquet", "csv", "csv-no-header"].
     reader_kwargs: dict
         Additional arguments of the specified reader.
     """
-    try:
-        from nvtabular.io.dataset import Dataset
-    except ImportError:
-        raise ValueError("NVTabular is necessary for this function, please install: " "nvtabular.")
-
     # TODO: put this in parent class and allow
     # torch dataset to leverage as well?
 
     # if a dataset was passed, just return it
     if isinstance(paths_or_dataset, Dataset):
         return paths_or_dataset
```

### Comparing `merlin-models-23.2.0/merlin/models/utils/nvt_utils.py` & `merlin-models-23.4.0/merlin/models/utils/nvt_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import logging
 
+from merlin.core.compat import cudf
+
 
 def require_nvt():
     try:
         import nvtabular as nvt  # noqa
 
         backend = None
         try:
@@ -32,15 +34,13 @@
         raise ImportError(
             "nvtabular is required for this feature.",
             "Please install it with `pip install nvtabular`.",
         )
 
 
 def _check_nvt_gpu():
-    try:
-        import cudf  # noqa
-    except ImportError:
+    if not cudf:
         logging.warning(
             "A GPU was detected but rapids is not installed.",
             "NVTabular will not be able to use GPU.",
             "Look at the documentation for more information at rapids.ai",
         )
```

### Comparing `merlin-models-23.2.0/merlin/models/utils/registry.py` & `merlin-models-23.4.0/merlin/models/utils/registry.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/merlin/models/utils/schema_utils.py` & `merlin-models-23.4.0/merlin/models/utils/schema_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,37 +60,23 @@
 ):
     properties = properties or {}
     if not domain_name:
         domain_name = name
     if num_items:
         properties["domain"] = {"name": domain_name, "min": 0, "max": num_items}
 
-    is_list, is_ragged = False, False
-    value_count = {}
-    if min_value_count is not None:
-        value_count["min"] = min_value_count
-    if max_value_count is not None:
-        value_count["max"] = max_value_count
-    if value_count:
-        properties["value_count"] = value_count
-        is_list = True
-        is_ragged = min_value_count != max_value_count
-
     tags = tags or []
     if Tags.CATEGORICAL not in tags:
         tags.append(Tags.CATEGORICAL)
 
-    return ColumnSchema(
-        name=name,
-        tags=tags,
-        dtype=dtype,
-        properties=properties,
-        is_list=is_list,
-        is_ragged=is_ragged,
-    )
+    kwargs = {}
+    if min_value_count is not None:
+        kwargs = {"dims": ((0, None), (min_value_count, max_value_count))}
+
+    return ColumnSchema(name=name, tags=tags, dtype=dtype, properties=properties, **kwargs)
 
 
 def create_continuous_column(
     name,
     dtype=np.float32,
     tags=None,
     properties=None,
```

### Comparing `merlin-models-23.2.0/merlin/models/xgb/__init__.py` & `merlin-models-23.4.0/merlin/models/xgb/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,14 @@
         export_dir = Path(path)
         export_dir.mkdir(parents=True)
         self.booster.save_model(export_dir / "model.json")
         schema_to_tensorflow_metadata_json(self.schema, export_dir / "schema.json")
 
         save_merlin_metadata(
             export_dir,
-            self,
             self.schema.select_by_name(self.feature_columns),
             self.schema.select_by_name(self.target_columns),
         )
 
         with open(export_dir / "params.json", "w") as f:
             json.dump(self.params, f, indent=4)
         with open(export_dir / "config.json", "w") as f:
```

### Comparing `merlin-models-23.2.0/merlin_models.egg-info/PKG-INFO` & `merlin-models-23.4.0/merlin_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.2.0
+Version: 23.4.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
 Description: ## Merlin Models
         
         [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
@@ -116,15 +116,15 @@
         You can find more details and information about a low-level API in our overview of the
         [Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
         
         ### Notebook Examples and Tutorials
         
         View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
         
-        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repostory.
+        The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
         
         ### Feedback and Support
         
         If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
         We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
         To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
```

### Comparing `merlin-models-23.2.0/merlin_models.egg-info/SOURCES.txt` & `merlin-models-23.4.0/merlin_models.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .pre-commit-config.yaml
 CLA.md
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
+pytest.ini
 setup.cfg
 setup.py
 tox.ini
 versioneer.py
 merlin/datasets/__init__.py
 merlin/datasets/synthetic.py
 merlin/datasets/advertising/__init__.py
@@ -97,14 +98,15 @@
 merlin/models/tf/core/combinators.py
 merlin/models/tf/core/encoder.py
 merlin/models/tf/core/index.py
 merlin/models/tf/core/prediction.py
 merlin/models/tf/core/tabular.py
 merlin/models/tf/distributed/__init__.py
 merlin/models/tf/distributed/backend.py
+merlin/models/tf/distributed/embedding.py
 merlin/models/tf/experimental/sample_weight.py
 merlin/models/tf/inputs/__init__.py
 merlin/models/tf/inputs/base.py
 merlin/models/tf/inputs/continuous.py
 merlin/models/tf/inputs/embedding.py
 merlin/models/tf/losses/__init__.py
 merlin/models/tf/losses/base.py
@@ -276,14 +278,15 @@
 tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
 tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
 tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
 tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
 tests/unit/tf/experimental/__init__.py
 tests/unit/tf/experimental/test_sample_weight.py
 tests/unit/tf/horovod/__init__.py
+tests/unit/tf/horovod/test_embedding.py
 tests/unit/tf/horovod/test_horovod.py
 tests/unit/tf/inputs/__init__.py
 tests/unit/tf/inputs/test_base.py
 tests/unit/tf/inputs/test_block.py
 tests/unit/tf/inputs/test_continuous.py
 tests/unit/tf/inputs/test_embedding.py
 tests/unit/tf/inputs/test_tabular.py
```

### Comparing `merlin-models-23.2.0/merlin_models.egg-info/requires.txt` & `merlin-models-23.4.0/merlin_models.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-merlin-core>=0.2.0
-merlin-dataloader>=0.0.2
+merlin-core>=23.4.0
+merlin-dataloader>=23.4.0
 
 [all]
-merlin-core>=0.2.0
-merlin-dataloader>=0.0.2
+merlin-core>=23.4.0
+merlin-dataloader>=23.4.0
 tensorflow>=2.8
 torch>=1.0
 torchmetrics>=0.10.0
 lightfm>=1.0.0
 implicit>=0.5.2
 xgboost>=1.0.0
-transformers
+transformers<5,>=4.23
 horovod
+sparse_operation_kit
 nvtabular>=1.0.0
 bokeh
 check-manifest
 pytest>=5
 pytest-cov>=2
 pytest-xdist
 black==20.8b1
@@ -41,16 +42,16 @@
 sphinx-external-toc==0.2.4
 sphinx-multiversion@ git+https://github.com/mikemckiernan/sphinx-multiversion.git
 Sphinx==3.5.4
 sphinxcontrib-copydirs@ git+https://github.com/mikemckiernan/sphinxcontrib-copydirs.git
 ipython==8.2.0
 
 [base]
-merlin-core>=0.2.0
-merlin-dataloader>=0.0.2
+merlin-core>=23.4.0
+merlin-dataloader>=23.4.0
 
 [dev]
 bokeh
 check-manifest
 pytest>=5
 pytest-cov>=2
 pytest-xdist
@@ -80,14 +81,15 @@
 sphinx-multiversion@ git+https://github.com/mikemckiernan/sphinx-multiversion.git
 Sphinx==3.5.4
 sphinxcontrib-copydirs@ git+https://github.com/mikemckiernan/sphinxcontrib-copydirs.git
 ipython==8.2.0
 
 [horovod]
 horovod
+sparse_operation_kit
 
 [implicit]
 implicit>=0.5.2
 
 [implicit-dev]
 implicit>=0.5.2
 bokeh
@@ -166,15 +168,15 @@
 nvtabular>=1.0.0
 
 [tensorflow]
 tensorflow>=2.8
 
 [tensorflow-dev]
 tensorflow>=2.8
-transformers
+transformers<5,>=4.23
 bokeh
 check-manifest
 pytest>=5
 pytest-cov>=2
 pytest-xdist
 black==20.8b1
 flake8
@@ -188,15 +190,15 @@
 fiddle==0.2.2
 wandb
 optuna
 plotly
 nvtabular>=1.0.0
 
 [transformers]
-transformers
+transformers<5,>=4.23
 
 [xgboost]
 xgboost>=1.0.0
 
 [xgboost-dev]
 xgboost>=1.0.0
 bokeh
```

### Comparing `merlin-models-23.2.0/pyproject.toml` & `merlin-models-23.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/setup.cfg` & `merlin-models-23.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/setup.py` & `merlin-models-23.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/__init__.py` & `merlin-models-23.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/__init__.py` & `merlin-models-23.4.0/tests/common/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/tf/__init__.py` & `merlin-models-23.4.0/tests/common/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/tf/retrieval/__init__.py` & `merlin-models-23.4.0/tests/common/tf/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_config.py` & `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_config.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_tests_common.py` & `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_tests_common.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/common/tf/retrieval/retrieval_utils.py` & `merlin-models-23.4.0/tests/common/tf/retrieval/retrieval_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -400,15 +400,14 @@
     else:
         raise ValueError(f"Invalid model_type: {model_type}")
     return model
 
 
 def get_youtube_dnn_model(
     schema,
-    max_seq_length,
     item_id_emb_size=32,
     emb_init_distr="truncated_normal",
     emb_init_range=0.05,
     two_tower_mlp_layers="64",
     youtubednn_sampled_softmax_n_candidates=100,
     youtubednn_sampled_softmax=True,
     logits_temperature=0.1,
@@ -439,17 +438,17 @@
 
     layers_dims = []
 
     layers_dims = list([int(v.strip()) for v in two_tower_mlp_layers.split(",") if v != ""])
     # Appends the top MLP layer with the same size as the item id embedding
     layers_dims.append(item_id_emb_size)
 
+    # TODO: Update test to use YoutubeDNNRetrievalModelV2, as this one is deprecated
     model = mm.YoutubeDNNRetrievalModel(
         schema=schema_selected,
-        max_seq_length=max_seq_length,
         num_sampled=youtubednn_sampled_softmax_n_candidates,
         sampled_softmax=youtubednn_sampled_softmax,
         logits_temperature=logits_temperature,
         embedding_options=mm.EmbeddingOptions(
             embedding_dims=embedding_dims,
             infer_embedding_sizes=True,
             infer_embedding_sizes_multiplier=two_tower_embedding_sizes_multiplier,
@@ -583,15 +582,14 @@
     callbacks = [
         ExamplesPerSecondCallback(
             train_batch_size, every_n_steps=metrics_log_frequency, wandb_logger=wandb_logger
         )
     ]
 
     if wandb_logger:
-
         wandb_callback = wandb_logger.get_callback(metrics_log_frequency=metrics_log_frequency)
         if wandb_callback:
             callbacks.append(wandb_callback)
 
     return callbacks
```

### Comparing `merlin-models-23.2.0/tests/common/tf/tests_utils.py` & `merlin-models-23.4.0/tests/common/tf/tests_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/conftest.py` & `merlin-models-23.4.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/__init__.py` & `merlin-models-23.4.0/tests/integration/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/retrieval/__init__.py` & `merlin-models-23.4.0/tests/integration/tf/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/retrieval/test_integration_retrieval.py` & `merlin-models-23.4.0/tests/integration/tf/retrieval/test_integration_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_01_getting_started.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_02_dataschema.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_03_exploring_different_models.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_04_export_ranking_models.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_05_export_retrieval_model.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py` & `merlin-models-23.4.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/config/test_schema.py` & `merlin-models-23.4.0/tests/unit/config/test_schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/datasets/test_advertising.py` & `merlin-models-23.4.0/tests/unit/datasets/test_advertising.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/datasets/test_ecommerce.py` & `merlin-models-23.4.0/tests/unit/datasets/test_ecommerce.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from pathlib import Path
 
 import pytest
 
 import merlin.io
 from merlin.datasets import ecommerce
 from merlin.datasets.synthetic import generate_data
 
@@ -52,17 +53,39 @@
         "user_item_intentions",
         "user_item_shops",
         "user_profile",
         "user_shops",
     ]
 
     ecommerce.transform_aliccp((dataset, dataset), tmp_path)
-    output_files = list(tmp_path.glob("*/*"))
 
-    assert len(output_files) == 13
+    output_files = set(sorted(tmp_path.glob("*/*")))
+    assert {
+        Path(f"{tmp_path}/train/.merlin"),
+        Path(f"{tmp_path}/train/_file_list.txt"),
+        Path(f"{tmp_path}/train/_metadata"),
+        Path(f"{tmp_path}/train/_metadata.json"),
+        Path(f"{tmp_path}/train/part_0.parquet"),
+        Path(f"{tmp_path}/train/schema.pbtxt"),
+        Path(f"{tmp_path}/valid/.merlin"),
+        Path(f"{tmp_path}/valid/_file_list.txt"),
+        Path(f"{tmp_path}/valid/_metadata"),
+        Path(f"{tmp_path}/valid/_metadata.json"),
+        Path(f"{tmp_path}/valid/part_0.parquet"),
+        Path(f"{tmp_path}/valid/schema.pbtxt"),
+        Path(f"{tmp_path}/workflow/categories"),
+        Path(f"{tmp_path}/workflow/metadata.json"),
+        Path(f"{tmp_path}/workflow/workflow.pkl"),
+    }.issubset(output_files)
+
+    metadata_files = tmp_path.glob("*/*.merlin/*")
+    assert sorted(metadata_files) == [
+        Path(f"{tmp_path}/train/.merlin/schema.json"),
+        Path(f"{tmp_path}/valid/.merlin/schema.json"),
+    ]
 
 
 @pytest.mark.skipif(
     MAYBE_ALICCP_DATA is None,
     reason="ALI-CCP data is not available, pass it through env variable $DATA_PATH_ALICCP",
 )
 def test_get_alliccp():
```

### Comparing `merlin-models-23.2.0/tests/unit/datasets/test_entertainment.py` & `merlin-models-23.4.0/tests/unit/datasets/test_entertainment.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/datasets/test_synthetic.py` & `merlin-models-23.4.0/tests/unit/datasets/test_synthetic.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import numpy as np
 import pytest
 
+from merlin.core.compat import cudf
 from merlin.datasets.synthetic import generate_data, generate_user_item_interactions
 from merlin.io import Dataset
 from merlin.models.utils.schema_utils import filter_dict_by_schema
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 def test_synthetic_sequence_testing_data():
@@ -44,17 +45,17 @@
     data = generate_data("testing", num_rows=100, min_session_length=5, max_session_length=50)
     schema = data.schema
 
     from merlin.models.tf import sample_batch
 
     tensors, _ = sample_batch(data, batch_size=100)
     assert tensors["user_id"].shape == (100, 1)
-    assert tensors["user_age"].dtype == tf.float64
-    for name, val in filter_dict_by_schema(tensors, schema.select_by_tag(Tags.LIST)).items():
-        assert len(val) == 2
+    assert tensors["user_age"].dtype == tf.float32
+    for val in filter_dict_by_schema(tensors, schema.select_by_tag(Tags.LIST)).values():
+        len(val.shape) == 3
 
 
 @pytest.mark.parametrize(
     ["generate_data_kwargs", "expected_sequence_length"],
     [
         [{}, 4],  # this is the default value in the generate_data kwargs
         [{"min_session_length": 6}, 6],
@@ -67,15 +68,15 @@
     data = generate_data("sequence-testing", num_rows=10, **generate_data_kwargs)
 
     from merlin.models.tf import sample_batch
 
     tensors, y = sample_batch(data, batch_size=1)
 
     for col in ["item_id_seq", "categories"]:
-        assert all(tensors[col][1] == expected_sequence_length)
+        assert tensors[col].row_lengths().numpy()[0] == expected_sequence_length
 
 
 def test_generate_user_item_interactions_dtypes():
     schema = Schema(
         [
             ColumnSchema(
                 "item_id",
@@ -133,16 +134,16 @@
     }
 
     assert all(
         val == expected_dtypes[key] for key, val in dict(data.dtypes).items() if key != "categories"
     )
 
 
+@pytest.mark.skipif(not cudf, reason="cudf could not be imported")
 def test_generate_item_interactions_gpu(testing_data: Dataset):
-    cudf = pytest.importorskip("cudf")
     data = generate_user_item_interactions(testing_data.schema, num_interactions=500, device="cuda")
 
     assert isinstance(data, cudf.DataFrame)
     assert len(data) == 500
     assert list(data.columns) == [
         "user_id",
         "user_country",
```

### Comparing `merlin-models-23.2.0/tests/unit/implicit/__init__.py` & `merlin-models-23.4.0/tests/unit/implicit/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/lightfm/__init__.py` & `merlin-models-23.4.0/tests/unit/lightfm/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/lightfm/test_lightfm.py` & `merlin-models-23.4.0/tests/unit/torch/features/test_continuous.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-import numpy as np
 
-from merlin.datasets.synthetic import generate_data
-from merlin.models.lightfm import LightFM
+import merlin.models.torch as ml
 from merlin.schema import Tags
 
 
-def test_warp():
-    np.random.seed(0)
-    train, valid = generate_data("music-streaming", 100, (0.95, 0.05))
-    train.schema = train.schema.remove_by_tag(Tags.TARGET)
-    valid.schema = valid.schema.remove_by_tag(Tags.TARGET)
+def test_continuous_features(torch_con_features):
+    features = ["con_a", "con_b"]
+    con = ml.ContinuousFeatures(features)(torch_con_features)
 
-    model = LightFM(learning_rate=0.05, loss="warp", epochs=10)
-    model.fit(train)
+    assert list(con.keys()) == features
 
-    model.predict(train)
 
-    metrics = model.evaluate(valid, k=10)
-    assert metrics["auc"] > 0.01
+def test_continuous_features_yoochoose(tabular_schema, torch_tabular_data):
+    cont_cols = tabular_schema.select_by_tag(Tags.CONTINUOUS)
+
+    con = ml.ContinuousFeatures.from_schema(cont_cols)
+    outputs = con(torch_tabular_data)
+
+    assert set(outputs.keys()) == set(cont_cols.column_names)
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/_conftest.py` & `merlin-models-23.4.0/tests/unit/tf/_conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_base.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 #
 import os
 
 import tensorflow as tf
 
 import merlin.models.tf as ml
+from merlin.core.compat import cudf
 from merlin.io import Dataset
 from merlin.schema import Tags
 
 
 def test_matrix_factorization_block(music_streaming_data: Dataset):
     mf = ml.QueryItemIdsEmbeddingsBlock(music_streaming_data.schema, dim=128)
 
@@ -67,18 +68,14 @@
 
     df = mf.embedding_table_df(Tags.ITEM_ID, gpu=False)
     assert isinstance(df, pd.DataFrame)
     assert len(df) == 10001
     assert os.path.exists(item_embedding_parquet)
 
     # Test GPU export if available
-    try:
-        import cudf  # noqa: F401
-
+    if cudf:
         user_embedding_parquet = str(tmp_path / "users.parquet")
         mf.export_embedding_table(Tags.USER_ID, user_embedding_parquet, gpu=True)
         assert os.path.exists(user_embedding_parquet)
         df = mf.embedding_table_df(Tags.USER_ID, gpu=True)
         assert isinstance(df, cudf.DataFrame)
         assert len(df) == 10001
-    except ImportError:
-        pass
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/retrieval/test_two_tower.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/retrieval/test_two_tower.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 
 import numpy as np
 import pytest
 import tensorflow as tf
 
 import merlin.models.tf as ml
+from merlin.core.compat import cudf
 from merlin.datasets.synthetic import generate_data
 from merlin.io import Dataset
 from merlin.models.tf.core.aggregation import ElementWiseMultiply
 from merlin.models.tf.utils import testing_utils
 from merlin.schema import Tags
 
 
@@ -55,25 +56,21 @@
 
     df = mf.embedding_table_df(Tags.ITEM_ID, gpu=False)
     assert isinstance(df, pd.DataFrame)
     assert len(df) == 10001
     assert os.path.exists(item_embedding_parquet)
 
     # Test GPU export if available
-    try:
-        import cudf  # noqa: F401
-
+    if cudf:
         user_embedding_parquet = str(tmp_path / "users.parquet")
         mf.export_embedding_table(Tags.USER_ID, user_embedding_parquet, gpu=True)
         assert os.path.exists(user_embedding_parquet)
         df = mf.embedding_table_df(Tags.USER_ID, gpu=True)
         assert isinstance(df, cudf.DataFrame)
         assert len(df) == 10001
-    except ImportError:
-        pass
 
 
 def test_elementwisemultiply():
     emb1 = np.random.uniform(-1, 1, size=(5, 10))
     emb2 = np.random.uniform(-1, 1, size=(5, 10))
     x = ElementWiseMultiply()({"emb1": tf.constant(emb1), "emb2": tf.constant(emb2)})
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/sampling/test_cross_batch.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/sampling/test_in_batch.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/sampling/test_in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/test_cross.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/test_cross.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     cross = mm.CrossBlock(depth=1, inputs=inputs)
     output = cross(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
 
     assert list(output.shape) == [100, 518]
 
 
 def test_dcn_v2_stacked(testing_data: Dataset):
-
     dcn_body = (
         mm.InputBlock(
             testing_data.schema,
             embedding_options=mm.EmbeddingOptions(embedding_dim_default=128),
             aggregation="concat",
         )
         .connect(mm.CrossBlock(3))
@@ -90,15 +89,14 @@
 
     output = dcn_body(mm.sample_batch(testing_data, batch_size=100, include_targets=False))
 
     assert list(output.shape) == [100, 256]
 
 
 def test_dcn_v2_stacked_low_rank(testing_data: Dataset):
-
     dcn_body = (
         mm.InputBlock(
             testing_data.schema,
             embedding_options=mm.EmbeddingOptions(embedding_dim_default=128),
             aggregation="concat",
         )
         .connect(mm.CrossBlock(3, low_rank_dim=64))
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/test_dlrm.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/test_dlrm.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/test_interactions.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/test_interactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     wide_input_block = mm.ParallelBlock(
         {
             "categorical_ohe": mm.Filter(cat_schema_onehot).connect(
                 mm.CategoryEncoding(cat_schema_onehot, sparse=True, output_mode="one_hot"),
             ),
             "categorical_mhe": mm.SequentialBlock(
                 mm.Filter(cat_schema_multihot),
-                mm.ListToDense(max_seq_length=cat_schema_multihot["categories"].int_domain.max),
+                mm.ToDense(cat_schema_multihot),
                 mm.CategoryEncoding(cat_schema_multihot, sparse=True, output_mode="multi_hot"),
             ),
             "continuous": mm.SequentialBlock(
                 mm.Filter(schema.select_by_tag(Tags.CONTINUOUS)), mm.ToSparse()
             ),
         },
         aggregation="concat",
@@ -83,11 +83,11 @@
     fm_block = mm.FMBlock(
         schema,
         fm_input_block=input_block,
         wide_input_block=wide_input_block,
         factors_dim=32,
     )
 
-    batch, _ = mm.sample_batch(testing_data, batch_size=16)
+    batch, _ = mm.sample_batch(testing_data, batch_size=16, prepare_features=True)
 
     output = fm_block(batch)
     assert output.shape.as_list() == [16, 1]
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/test_mlp.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/test_mlp.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/blocks/test_optimizer.py` & `merlin-models-23.4.0/tests/unit/tf/blocks/test_optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,29 +9,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import numpy as np
 import pytest
 import tensorflow as tf
+from packaging import version
 from tensorflow.test import TestCase
 
 import merlin.models.tf as ml
 from merlin.core.dispatch import HAS_GPU
 from merlin.datasets.synthetic import generate_data
 from merlin.models.tf.core.combinators import ParallelBlock, SequentialBlock, TabularBlock
 from merlin.models.tf.utils import testing_utils
 from merlin.models.utils import schema_utils
 from merlin.models.utils.schema_utils import create_categorical_column
 from merlin.schema import Schema, Tags
 
+if version.parse(tf.__version__) < version.parse("2.11.0"):
+    keras_optimizers = tf.keras.optimizers
+else:
+    keras_optimizers = tf.keras.optimizers.legacy
+
 
 def generate_two_layers():
     initializer_first_layer = tf.constant_initializer(np.ones((3, 4)))
     initializer_second_layer = tf.constant_initializer(np.ones((4, 1)))
     first_layer = ml.MLPBlock(
         [4], use_bias=False, kernel_initializer=initializer_first_layer, block_name="first_mlp"
     )
@@ -40,22 +45,45 @@
         use_bias=False,
         kernel_initializer=initializer_second_layer,
         block_name="second_mlp",
     )
     return first_layer, second_layer
 
 
+@pytest.mark.skipif
+@pytest.mark.parametrize(
+    "optimizers",
+    [
+        ("sgd", keras_optimizers.Adagrad()),
+        (keras_optimizers.SGD(), "adam"),
+    ],
+)
+def test_new_optimizers_raise_error(optimizers):
+    layers = generate_two_layers()
+    with pytest.raises(ValueError) as excinfo:
+        ml.MultiOptimizer(
+            default_optimizer=optimizers[0],
+            optimizers_and_blocks=[
+                ml.OptimizerBlocks(optimizers[0], layers[0]),
+                ml.OptimizerBlocks(optimizers[1], layers[1]),
+            ],
+        )
+        assert "Optimizers must be an instance of tf.keras.optimizers.legacy.Optimizer" in str(
+            excinfo.value
+        )
+
+
 @pytest.mark.parametrize(
     "optimizers",
     [
         ("sgd", "adam"),
         ("rmsprop", "sgd"),
         ("adam", "adagrad"),
         ("adagrad", "rmsprop"),
-        (tf.keras.optimizers.SGD(), tf.keras.optimizers.Adagrad()),
+        (keras_optimizers.SGD(), keras_optimizers.Adagrad()),
     ],
 )
 def test_optimizers(optimizers):
     testing_data = generate_data("e-commerce", num_rows=5)
     train_schema = testing_data.schema.select_by_name(
         names=["user_categories", "user_brands", "user_shops", "user_intensions"]
     )
@@ -116,16 +144,16 @@
     user_tower = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     item_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([256, 128]))
     two_tower = ml.ParallelBlock({"user": user_tower, "item": item_tower}, aggregation="concat")
     model = ml.Model(two_tower, ml.BinaryClassificationTask("click"))
     multi_optimizers = ml.MultiOptimizer(
         default_optimizer="adam",
         optimizers_and_blocks=[
-            ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
-            ml.OptimizerBlocks(tf.keras.optimizers.Adam(), item_tower),
+            ml.OptimizerBlocks(keras_optimizers.SGD(), user_tower),
+            ml.OptimizerBlocks(keras_optimizers.Adam(), item_tower),
         ],
     )
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizers
     )
 
 
@@ -137,16 +165,16 @@
     third_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([128, 64]))
     two_tower = ml.ParallelBlock(
         {"user": user_tower, "item": item_tower, "third": third_tower}, aggregation="concat"
     )
     model = ml.Model(two_tower, ml.BinaryClassificationTask("click"))
     multi_optimizers = ml.MultiOptimizer(
         optimizers_and_blocks=[
-            ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
-            ml.OptimizerBlocks(tf.keras.optimizers.Adam(), [item_tower, third_tower]),
+            ml.OptimizerBlocks(keras_optimizers.SGD(), user_tower),
+            ml.OptimizerBlocks(keras_optimizers.Adam(), [item_tower, third_tower]),
         ],
     )
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizers
     )
 
 
@@ -159,16 +187,16 @@
     two_tower = ml.ParallelBlock(
         {"user": user_tower, "item": item_tower, "third": third_tower}, aggregation="concat"
     )
     model = ml.Model(two_tower, ml.BinaryClassificationTask("click"))
     multi_optimizers = ml.MultiOptimizer(
         default_optimizer="adam",
         optimizers_and_blocks=[
-            ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
-            ml.OptimizerBlocks(tf.keras.optimizers.Adam(), item_tower),
+            ml.OptimizerBlocks(keras_optimizers.SGD(), user_tower),
+            ml.OptimizerBlocks(keras_optimizers.Adam(), item_tower),
         ],
     )
     multi_optimizers.add(ml.OptimizerBlocks("adagrad", third_tower))
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizers
     )
 
@@ -176,15 +204,15 @@
 @pytest.mark.parametrize(
     "optimizers",
     [
         ("sgd", "adam"),
         ("rmsprop", "sgd"),
         ("adam", "adagrad"),
         ("adagrad", "rmsprop"),
-        (tf.keras.optimizers.SGD(), tf.keras.optimizers.Adagrad()),
+        (keras_optimizers.SGD(), keras_optimizers.Adagrad()),
     ],
 )
 def test_multi_optimizers_from_config(ecommerce_data, optimizers):
     test_case = TestCase()
     schema = ecommerce_data.schema
     user_tower = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     item_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([256, 128]))
@@ -206,15 +234,15 @@
     )
 
 
 @pytest.mark.parametrize(
     "optimizers",
     [
         ("sgd", "adam"),
-        (tf.keras.optimizers.SGD(), tf.keras.optimizers.Adagrad()),
+        (keras_optimizers.SGD(), keras_optimizers.Adagrad()),
     ],
 )
 def test_multi_optimizers_from_config_list_input(ecommerce_data, optimizers):
     test_case = TestCase()
     schema = ecommerce_data.schema
     user_tower = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     item_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([256, 128]))
@@ -250,16 +278,16 @@
     model = ml.Model(three_tower, ml.BinaryClassificationTask("click"))
 
     # The third_tower would be assigned the default_optimizer ("adagrad" in this example)
     if use_default:
         optimizer = ml.MultiOptimizer(
             default_optimizer="adagrad",
             optimizers_and_blocks=[
-                ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
-                ml.OptimizerBlocks(tf.keras.optimizers.Adam(), item_tower),
+                ml.OptimizerBlocks(keras_optimizers.SGD(), user_tower),
+                ml.OptimizerBlocks(keras_optimizers.Adam(), item_tower),
             ],
         )
     else:
         # The string identification of optimizer is also acceptable, here "sgd" for the third_tower
         # the variables of BinaryClassificationTask("click") would still use the default_optimizer
         optimizer = ml.MultiOptimizer(
             default_optimizer="adam",
@@ -279,29 +307,32 @@
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_update_optimizer(ecommerce_data, run_eagerly):
     schema = ecommerce_data.schema
     user_tower_0 = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     user_tower_1 = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     two_tower = ml.ParallelBlock({"user": user_tower_0, "item": user_tower_1}, aggregation="concat")
     model = ml.Model(two_tower, ml.BinaryClassificationTask("click"))
-    sgd = tf.keras.optimizers.SGD()
-    adam = tf.keras.optimizers.Adam()
+    sgd = keras_optimizers.SGD()
+    adam = keras_optimizers.Adam()
     multi_optimizers = ml.MultiOptimizer(
         optimizers_and_blocks=[
             ml.OptimizerBlocks(adam, user_tower_0),
             ml.OptimizerBlocks(sgd, user_tower_1),
         ],
     )
 
     lazy_adam = ml.LazyAdam()
     multi_optimizers.update(ml.OptimizerBlocks(lazy_adam, user_tower_1))
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizers
     )
-    assert len(lazy_adam.get_weights()) == len(adam.get_weights())
+    if version.parse(tf.__version__) < version.parse("2.11.0"):
+        assert len(lazy_adam.get_weights()) == len(adam.get_weights())
+    else:
+        assert len(lazy_adam.get_weights()) == len(adam.variables())
 
 
 def adam_update_numpy(param, g_t, t, m, v, lr=0.001, beta1=0.9, beta2=0.999, epsilon=1e-7):
     lr_t = lr * np.sqrt(1 - beta2 ** (t + 1)) / (1 - beta1 ** (t + 1))
 
     m_t = beta1 * m + (1 - beta1) * g_t
     v_t = beta2 * v + (1 - beta2) * g_t * g_t
@@ -361,15 +392,14 @@
         # Validate updated params
         testing_utils.assert_allclose_according_to_type(var0_np, var0.numpy())
         testing_utils.assert_allclose_according_to_type(var1_np, var1.numpy())
 
 
 @pytest.mark.parametrize("dtype", [tf.int32, tf.int64])
 def test_lazy_adam_sparse_device_placement(dtype):
-
     # If a GPU is available, tests that all optimizer ops can be placed on it (i.e. they have GPU
     # kernels).
     if HAS_GPU:
         with tf.device("/GPU:0"):
             var = tf.Variable([[1.0], [2.0]])
             indices = tf.constant([0, 1], dtype=dtype)
 
@@ -554,15 +584,15 @@
     user_tower = ml.InputBlock(schema.select_by_tag(Tags.USER)).connect(ml.MLPBlock([256, 128]))
     item_tower = ml.InputBlock(schema.select_by_tag(Tags.ITEM)).connect(ml.MLPBlock([256, 128]))
     two_tower = ml.ParallelBlock({"user": user_tower, "item": item_tower}, aggregation="concat")
     model = ml.Model(two_tower, ml.BinaryClassificationTask("click"))
     multi_optimizers = ml.MultiOptimizer(
         default_optimizer="adam",
         optimizers_and_blocks=[
-            ml.OptimizerBlocks(tf.keras.optimizers.SGD(), user_tower),
+            ml.OptimizerBlocks(keras_optimizers.SGD(), user_tower),
             ml.OptimizerBlocks(ml.LazyAdam(), item_tower),
         ],
     )
     testing_utils.model_test(
         model, ecommerce_data, run_eagerly=run_eagerly, optimizer=multi_optimizers
     )
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_aggregation.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_base.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,18 @@
 
 import merlin.models.tf as ml
 from merlin.io.dataset import Dataset
 from merlin.models.tf.utils import testing_utils
 
 
 def test_sequential_block_yoochoose(testing_data: Dataset):
-    body = ml.InputBlock(testing_data.schema).connect(ml.MLPBlock([64]))
+    body = ml.InputBlockV2(testing_data.schema).connect(ml.MLPBlock([64]))
 
-    outputs = body(ml.sample_batch(testing_data, batch_size=100, include_targets=False))
+    batch = ml.sample_batch(testing_data, batch_size=100, include_targets=False)
+    outputs = body(batch)
 
     assert list(outputs.shape) == [100, 64]
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class DummyFeaturesBlock(ml.Block):
     def call(self, inputs, features, **kwargs):
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_combinators.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_combinators.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,15 @@
         layer = mm.Cond(condition, true)
 
         model = mm.Model(
             tf.keras.layers.Lambda(lambda x: x["item_recency"]),
             layer,
             tf.keras.layers.Dense(1),
             mm.BinaryClassificationTask("click"),
+            schema=music_streaming_data.schema.select_by_name("item_recency"),
         )
 
         testing_utils.model_test(model, music_streaming_data, run_eagerly=run_eagerly)
 
 
 class TestMapValues:
     def test_map_values_tensor(self):
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_encoder.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import tempfile
 
 import pytest
 import tensorflow as tf
 
 import merlin.models.tf as mm
 from merlin.io import Dataset
+from merlin.models.tf.transforms.features import expected_input_cols_from_schema
 from merlin.models.tf.utils import testing_utils
 from merlin.models.utils.dataset import unique_by_tag
 from merlin.schema import Tags
 
 
 def test_encoder_block(music_streaming_data: Dataset):
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(
@@ -20,32 +21,33 @@
     user_encoder = mm.Encoder(user_schema, mm.MLPBlock([4]), name="query")
     item_schema = schema.select_by_name(["item_id"])
     item_encoder = mm.Encoder(item_schema, mm.MLPBlock([4]), name="candidate")
 
     model = mm.Model(
         mm.ParallelBlock(user_encoder, item_encoder),
         mm.ContrastiveOutput(item_schema, "in-batch"),
+        prep_features=False,
     )
 
     assert model.blocks[0]["query"] == user_encoder
     assert model.blocks[0]["candidate"] == item_encoder
 
     loader = mm.Loader(music_streaming_data, batch_size=50)
     testing_utils.model_test(model, loader, reload_model=True)
 
     with pytest.raises(Exception) as excinfo:
         user_encoder.compile("adam")
         user_encoder.fit(loader)
 
     assert "This block is not meant to be trained by itself" in str(excinfo.value)
 
-    user_features = testing_utils.get_model_inputs(user_schema, ["user_genres"])
+    user_features = expected_input_cols_from_schema(user_schema)
     testing_utils.test_model_signature(user_encoder, user_features, ["output_1"])
 
-    item_features = testing_utils.get_model_inputs(item_schema)
+    item_features = expected_input_cols_from_schema(item_schema)
     testing_utils.test_model_signature(item_encoder, item_features, ["output_1"])
 
 
 def test_topk_encoder(music_streaming_data: Dataset):
     TOP_K = 10
     BATCH_SIZE = 32
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_index.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_prediction.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_prediction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/core/test_tabular.py` & `merlin-models-23.4.0/tests/unit/tf/core/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_01_getting_started.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_02_dataschema.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_03_exploring_different_models.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_04_export_ranking_models.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_05_export_retrieval_model.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_07_train_traditional_models.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_07_train_traditional_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py` & `merlin-models-23.4.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+import shutil
+
 import pytest
 from testbook import testbook
 
+from merlin.systems.triton.utils import run_triton_server
 from tests.conftest import REPO_ROOT
 
 pytest.importorskip("transformers")
 
+TRITON_SERVER_PATH = shutil.which("tritonserver")
+
 
+@pytest.mark.skipif(not TRITON_SERVER_PATH, reason="triton server not found")
 @testbook(
     REPO_ROOT / "examples/usecases/transformers-next-item-prediction.ipynb",
-    timeout=180,
+    timeout=720,
     execute=False,
 )
 @pytest.mark.notebook
 def test_next_item_prediction(tb):
     tb.inject(
         """
         import os, random
@@ -30,9 +36,13 @@
         df.to_csv('/tmp/train_set.csv')
         """
     )
     tb.cells[4].source = tb.cells[4].source.replace("get_booking('/workspace/data')", "")
     tb.cells[4].source = tb.cells[4].source.replace(
         "read_csv('/workspace/data/train_set.csv'", "read_csv('/tmp/train_set.csv'"
     )
-    tb.cells[30].source = tb.cells[30].source.replace("epochs=5", "epochs=1")
-    tb.execute()
+    tb.cells[31].source = tb.cells[31].source.replace("epochs=5", "epochs=1")
+    tb.cells[37].source = tb.cells[37].source.replace("/workspace/ensemble", "/tmp/ensemble")
+    tb.execute_cell(list(range(0, 38)))
+
+    with run_triton_server("/tmp/ensemble", grpc_port=8001):
+        tb.execute_cell(list(range(38, len(tb.cells))))
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/experimental/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/experimental/test_sample_weight.py` & `merlin-models-23.4.0/tests/unit/tf/experimental/test_sample_weight.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 )
 @pytest.mark.parametrize("neg_class_weight", [0.1, tf.random.uniform(shape=(1000,))])
 def test_two_tower_v2_with_contrastive_sample_weight(
     ecommerce_data: Dataset,
     pos_class_weight,
     neg_class_weight,
 ):
-
     tower_dim = 64
     data = ecommerce_data
     input_features = ["user_categories", "item_id"]
     if isinstance(pos_class_weight, str):
         input_features += [pos_class_weight]
     data.schema = data.schema.select_by_name(input_features)
 
@@ -69,15 +68,14 @@
         pos_class_weight=pos_class_weight, neg_class_weight=neg_class_weight, schema=data.schema
     )
     model.compiled_metrics.reset_state()
     metrics3 = model.test_step(batch)
 
     assert metrics3["loss"] != metrics2["loss"]
     for m in metrics3:
-
         if m.startswith("weighted_"):
             assert metrics3[m] <= 1
             if isinstance(pos_class_weight, tf.Tensor):
                 assert metrics3[m] != metrics2[m]
 
 
 @testing_utils.mark_run_eagerly_modes
@@ -91,19 +89,21 @@
     user_inputs = mm.InputBlockV2(user_schema)
     query = mm.Encoder(user_inputs, mm.MLPBlock([128, tower_dim]))
 
     item_schema = data.schema.select_by_tag(Tags.ITEM)
     item_inputs = mm.InputBlockV2(item_schema)
     candidate = mm.Encoder(item_inputs, mm.MLPBlock([128, tower_dim]))
 
+    item_id_cardinality = item_schema["item_id"].int_domain.max + 1
+
     output = mm.ContrastiveOutput(
         DotProduct(),
         post=ContrastiveSampleWeight(
-            pos_class_weight=tf.random.uniform(shape=(1000,)),
-            neg_class_weight=tf.random.uniform(shape=(1000,)),
+            pos_class_weight=tf.random.uniform(shape=(item_id_cardinality,)),
+            neg_class_weight=tf.random.uniform(shape=(item_id_cardinality,)),
             schema=data.schema,
         ),
         schema=data.schema.select_by_tag(Tags.ITEM_ID),
         negative_samplers="in-batch",
         store_negative_ids=True,
     )
     model = mm.TwoTowerModelV2(query, candidate, outputs=output, schema=data.schema)
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/horovod/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/transformers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import pytest
 
-pytest.importorskip("horovod")
+pytest.importorskip("transformers")
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/horovod/test_horovod.py` & `merlin-models-23.4.0/tests/unit/tf/horovod/test_horovod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 import pytest
 import tensorflow as tf
+from packaging import version
 from tensorflow.keras.utils import set_random_seed
 
 import merlin.models.tf as mm
 from merlin.datasets.advertising.criteo.dataset import default_criteo_transform
 from merlin.io.dataset import Dataset
 from merlin.models.tf.distributed.backend import hvd, hvd_installed
 from merlin.models.utils.example_utils import workflow_fit_transform
@@ -65,21 +66,26 @@
         train.schema,
         embedding_dim=16,
         bottom_block=mm.MLPBlock([32, 16]),
         top_block=mm.MLPBlock([32, 16]),
         prediction_tasks=mm.BinaryClassificationTask(target_column),
     )
 
+    if version.parse(tf.__version__) < version.parse("2.11.0"):
+        keras_optimizers = tf.keras.optimizers
+    else:
+        keras_optimizers = tf.keras.optimizers.legacy
+
     if custom_distributed_optimizer:
         # Test for a case when the user uses a custom DistributedOptimizer.
         # With a custom hvd.DistributedOptimzer, users have to adjust the learning rate.
-        opt = tf.keras.optimizers.Adagrad(learning_rate=learning_rate * hvd.size())
+        opt = keras_optimizers.Adagrad(learning_rate=learning_rate * hvd.size())
         opt = hvd.DistributedOptimizer(opt, compression=hvd.Compression.fp16)
     else:
-        opt = tf.keras.optimizers.Adagrad(learning_rate=learning_rate)
+        opt = keras_optimizers.Adagrad(learning_rate=learning_rate)
 
     model.compile(optimizer=opt, run_eagerly=False, metrics=[tf.keras.metrics.AUC()])
 
     # model.fit() will hang or terminate with error if all workers don't have
     # the same number of batches.
     losses = model.fit(
         train_loader,
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/test_base.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/test_block.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/test_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         categorical=ml.Embeddings(
             sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
         ),
         aggregation=None,
     )
 
     batch = ml.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     outputs = tab_module(batch)
 
     con = sequence_testing_data.schema.select_by_tag(Tags.CONTINUOUS).column_names
     cat = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL).column_names
     seq = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE).column_names
@@ -80,15 +80,15 @@
             sequence_combiner=seq_combiner,
         ),
         continuous=ml.Continuous(con2d),
         aggregation=None,
     )
 
     batch = ml.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     outputs = input_block(batch)
 
     cat = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL).column_names
 
     assert all(isinstance(val, tf.Tensor) for name, val in outputs.items())
@@ -98,15 +98,15 @@
 
 def test_tabular_seq_features_ragged_custom_emb_combiner(sequence_testing_data: Dataset):
     schema = sequence_testing_data.schema
     schema = schema + Schema([ColumnSchema("item_id_seq_weights")])
     assert "item_id_seq_weights" in schema.column_names
 
     batch = ml.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
     batch["item_id_seq_weights"] = tf.ragged.constant(
         [[1.0, 2.0, 3.0, 4.0] for _ in range(batch["item_id_seq"].shape[0])],
         row_splits_dtype=batch["item_id_seq"].row_splits.dtype,
     )
 
     input_block_weighed_avg = ml.InputBlockV2(
@@ -145,15 +145,15 @@
     assert all(tf.rank(val) == 2 for name, val in outputs_weighted_avg.items() if name in cat)
 
 
 def test_tabular_seq_features_avg_embeddings_with_mapvalues(sequence_testing_data: Dataset):
     cat_schema = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL)
 
     batch = ml.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     input_block = ml.InputBlockV2(
         cat_schema,
         categorical=ml.Embeddings(
             cat_schema,
         ),
@@ -181,15 +181,15 @@
         cat_schema.select_by_tag(Tags.CATEGORICAL),
         dim={"item_id_seq": 15, "test_user_id": 21},
         embeddings_initializer="truncated_normal",
     )
     input_block = ml.InputBlockV2(cat_schema, categorical=embeddings_block, aggregation=aggregation)
 
     batch = ml.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     outputs = input_block(batch)
 
     if aggregation == "concat":
         assert outputs.shape[-1] == 60
     elif aggregation is None:
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/test_continuous.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/test_continuous.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 def test_inputv2_without_categorical_features(music_streaming_data: Dataset, run_eagerly):
     schema = music_streaming_data.schema.select_by_tag(Tags.CONTINUOUS)
     music_streaming_data.schema = schema
 
     inputs = ml.InputBlockV2(schema)
 
     batch = ml.sample_batch(
-        music_streaming_data, batch_size=100, include_targets=False, to_ragged=True
+        music_streaming_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     assert inputs(batch).shape == (100, 3)
 
 
 def test_continuous_features_ragged(sequence_testing_data: Dataset):
     schema = sequence_testing_data.schema.select_by_tag(Tags.CONTINUOUS)
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/test_embedding.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/test_embedding.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import numpy as np
 import pandas as pd
 import pytest
 import tensorflow as tf
 from tensorflow.keras.initializers import RandomUniform
 
 import merlin.models.tf as mm
+from merlin.core.compat import cudf
 from merlin.io import Dataset
 from merlin.models.tf.utils import testing_utils
 from merlin.models.tf.utils.testing_utils import assert_output_shape, model_test
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 def test_embedding_features(tf_cat_features):
@@ -67,22 +68,33 @@
             mm.EmbeddingTable(16, column_schema)
         assert "needs to have an int-domain" in str(exc_info.value)
 
     @pytest.mark.parametrize(
         ["dim", "kwargs", "inputs", "expected_output_shape"],
         [
             (32, {}, tf.constant([[1]]), [1, 32]),
-            (16, {}, tf.ragged.constant([[1, 2, 3], [4, 5]]), [2, None, 16]),
-            (16, {"sequence_combiner": "mean"}, tf.ragged.constant([[1, 2, 3], [4, 5]]), [2, 16]),
+            (16, {}, tf.ragged.constant([[[1], [2], [3]], [[4], [5]]]), [2, None, 16]),
             (
                 16,
                 {"sequence_combiner": "mean"},
-                tf.sparse.from_dense(tf.constant([[1, 2, 3]])),
+                tf.ragged.constant([[[1], [2], [3]], [[4], [5]]]),
+                [2, 16],
+            ),
+            (
+                16,
+                {"sequence_combiner": "mean"},
+                tf.sparse.from_dense(tf.constant([[[1], [2], [3]]])),
                 [1, 16],
             ),
+            (
+                16,
+                {"sequence_combiner": "mean"},
+                tf.constant([[[1], [2], [3]], [[4], [5], [6]]]),
+                [2, 16],
+            ),
             (12, {}, {"item_id": tf.constant([[1]])}, {"item_id": [1, 12]}),
         ],
     )
     def test_layer(self, dim, kwargs, inputs, expected_output_shape):
         column_schema = self.sample_column_schema
         layer = mm.EmbeddingTable(dim, column_schema, **kwargs)
 
@@ -230,23 +242,19 @@
 
         embedding_table = mm.EmbeddingTable(dim, col_schema_a, col_schema_b)
         embedding_table.add_feature(col_schema_c)
 
         assert embedding_table.schema == Schema([col_schema_a, col_schema_b, col_schema_c])
 
         result = embedding_table(
-            {
-                "a": tf.constant([[1]]),
-                "b": tf.ragged.constant([[1]]),
-                "c": tf.constant([1]),
-            }
+            {"a": tf.constant([[[1]]]), "b": tf.ragged.constant([[[1]]]), "c": tf.constant([1])}
         )
 
         assert set(result.keys()) == {"a", "b", "c"}
-        np.testing.assert_array_equal(result["a"].numpy(), result["b"].numpy()[0])
+        np.testing.assert_array_equal(result["a"].numpy(), result["b"].numpy())
 
     def test_incompatible_features(self):
         dim = 4
         col_schema_a = ColumnSchema(
             "a", dtype=np.int32, properties={"domain": {"min": 0, "max": 10}}
         )
         col_schema_b = ColumnSchema(
@@ -712,29 +720,24 @@
         item_id_embeddings.numpy(), items_embeddings_dataset.to_ddf().compute().values
     )
 
     emb_init = mm.TensorInitializer.from_dataset(items_embeddings_dataset)
     assert np.allclose(item_id_embeddings.numpy(), emb_init(item_id_embeddings.shape).numpy())
 
     # Test GPU export if available
-    try:
-        import cudf  # noqa: F401
-
+    if cudf:
         items_embeddings_dataset = emb_module.embedding_table_dataset(Tags.ITEM_ID, gpu=True)
         assert np.allclose(
             item_id_embeddings.numpy(),
             items_embeddings_dataset.to_ddf().compute().to_pandas().values,
         )
 
         emb_init = mm.TensorInitializer.from_dataset(items_embeddings_dataset)
         assert np.allclose(item_id_embeddings.numpy(), emb_init(item_id_embeddings.shape).numpy())
 
-    except ImportError:
-        pass
-
 
 def test_shared_embeddings(music_streaming_data: Dataset):
     inputs = mm.InputBlock(music_streaming_data.schema)
 
     embeddings = inputs.select_by_name(Tags.CATEGORICAL.value)
 
     assert embeddings.table_config("item_genres") == embeddings.table_config("user_genres")
@@ -764,15 +767,15 @@
             "item_id_embedding",
             "item_feature_a",
         }
         assert set(embeddings.parallel_layers.keys()) == {"item_id_embedding", "item_feature_a"}
 
         outputs = embeddings(
             {
-                "item_id": tf.constant([1]),
-                "user_item_history": tf.ragged.constant([[1], [2, 3]]),
-                "item_feature_a": tf.constant([2]),
+                "item_id": tf.constant([[1]]),
+                "user_item_history": tf.ragged.constant([[[1]], [[2], [3]]]),
+                "item_feature_a": tf.constant([[2]]),
             }
         )
 
         assert set(outputs.keys()) == {"item_id", "user_item_history", "item_feature_a"}
-        np.testing.assert_array_equal(outputs["item_id"], outputs["user_item_history"][0])
+        np.testing.assert_array_equal(outputs["item_id"], outputs["user_item_history"][:1])
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/inputs/test_tabular.py` & `merlin-models-23.4.0/tests/unit/tf/inputs/test_tabular.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         categorical=mm.Embeddings(
             sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
         ),
         aggregation=None,
     )
 
     loader = mm.Loader(sequence_testing_data, batch_size=100)
-    batch = mm.sample_batch(loader, include_targets=False, to_ragged=True)
+    batch = mm.sample_batch(loader, include_targets=False, prepare_features=True)
 
     outputs = tab_module(batch)
 
     con = sequence_testing_data.schema.select_by_tag(Tags.CONTINUOUS).column_names
     cat = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL).column_names
     seq = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE).column_names
 
@@ -128,15 +128,15 @@
             sequence_combiner=seq_combiner,
         ),
         continuous=mm.Continuous(con2d),
         aggregation=None,
     )
 
     loader = mm.Loader(sequence_testing_data, batch_size=100)
-    batch = mm.sample_batch(loader, include_targets=False, to_ragged=True)
+    batch = mm.sample_batch(loader, include_targets=False, prepare_features=True)
 
     outputs = input_block(batch)
 
     cat = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL).column_names
 
     assert all(isinstance(val, tf.Tensor) for name, val in outputs.items())
     assert all(tf.rank(val) == 2 for name, val in outputs.items() if name in cat)
@@ -145,15 +145,15 @@
 
 def test_tabular_seq_features_ragged_custom_emb_combiner(sequence_testing_data: Dataset):
     schema = sequence_testing_data.schema
     schema = schema + Schema([ColumnSchema("item_id_seq_weights")])
     assert "item_id_seq_weights" in schema.column_names
 
     loader = mm.Loader(sequence_testing_data, batch_size=100)
-    batch = mm.sample_batch(loader, include_targets=False, to_ragged=True)
+    batch = mm.sample_batch(loader, include_targets=False, prepare_features=True)
     batch["item_id_seq_weights"] = tf.ragged.constant(
         [[1.0, 2.0, 3.0, 4.0] for _ in range(batch["item_id_seq"].shape[0])],
         row_splits_dtype=batch["item_id_seq"].row_splits.dtype,
     )
 
     input_block_weighed_avg = mm.InputBlockV2(
         schema,
@@ -191,15 +191,15 @@
     assert all(tf.rank(val) == 2 for name, val in outputs_weighted_avg.items() if name in cat)
 
 
 def test_tabular_seq_features_avg_embeddings_with_mapvalues(sequence_testing_data: Dataset):
     cat_schema = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL)
 
     batch = mm.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
 
     input_block = mm.InputBlockV2(
         cat_schema,
         categorical=mm.Embeddings(
             cat_schema,
         ),
@@ -227,15 +227,15 @@
         cat_schema.select_by_tag(Tags.CATEGORICAL),
         dim={"item_id_seq": 15, "test_user_id": 21},
         embeddings_initializer="truncated_normal",
     )
     input_block = mm.InputBlockV2(cat_schema, categorical=embeddings_block, aggregation=aggregation)
 
     loader = mm.Loader(sequence_testing_data, batch_size=100)
-    batch = mm.sample_batch(loader, include_targets=False, to_ragged=True)
+    batch = mm.sample_batch(loader, include_targets=False, prepare_features=True)
 
     outputs = input_block(batch)
 
     if aggregation == "concat":
         assert outputs.shape[-1] == 60
     elif aggregation is None:
         assert {k: v.shape[-1] for k, v in outputs.items()} == {
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/layers/test_queue.py` & `merlin-models-23.4.0/tests/unit/tf/layers/test_queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/losses/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/losses/test_losses.py` & `merlin-models-23.4.0/tests/unit/tf/losses/test_losses.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/metrics/test_metrics_popularity.py` & `merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_popularity.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/metrics/test_metrics_topk.py` & `merlin-models-23.4.0/tests/unit/tf/metrics/test_metrics_topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         (PrecisionAt(k=4), 0.25),
         (AvgPrecisionAt(k=4), 0.20833333),
         (MRRAt(k=4), 0.25),
         (NDCGAt(k=4), 0.30499637),
     ],
 )
 def test_topk_metrics_classes(topk_metrics_test_data_pre_sorted, metric_exp_result):
-
     labels, predictions, label_relevant_counts = topk_metrics_test_data_pre_sorted
     metric, expected_result = metric_exp_result
     metric.label_relevant_counts = label_relevant_counts
     metric.update_state(labels, predictions)
     result = metric.result()
     tf.debugging.assert_near(result, expected_result)
 
@@ -227,15 +226,14 @@
     reloaded_metric.update_state(labels, predictions)
     reloaded_result = reloaded_metric.result()
 
     tf.assert_equal(result, reloaded_result)
 
 
 def test_topk_metrics_sequential_3d_with_sample_weights():
-
     labels = tf.convert_to_tensor(
         [
             [[0, 1, 0, 1, 0], [0, 0, 0, 1, 1], [0, 0, 0, 0, 1]],
             [[0, 1, 0, 1, 0], [0, 0, 0, 1, 1], [0, 0, 0, 0, 1]],
         ],
         tf.float32,
     )
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/models/test_base.py` & `merlin-models-23.4.0/tests/unit/tf/models/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 from merlin.datasets.synthetic import generate_data
 from merlin.io.dataset import Dataset
 from merlin.models.tf.models.base import get_output_schema
 from merlin.models.tf.utils import testing_utils, tf_utils
 from merlin.models.utils import schema_utils
 from merlin.schema import ColumnSchema, Schema, Tags
 
+# import pickle
+
 
 class TestGetOutputSchema:
     def test_scalar(self, tmpdir):
         inputs = tf.keras.Input(shape=(1), name="my_input")
         outputs = tf.keras.layers.Dense(1, name="my_output")(inputs)
         model = tf.keras.models.Model(inputs=inputs, outputs=outputs)
         _ = model({"my_input": tf.constant([[1]])})
@@ -48,15 +50,15 @@
         inputs = tf.keras.Input(shape=(1), name="my_input")
         outputs = tf.keras.layers.Dense(4, name="my_output")(inputs)
         model = tf.keras.models.Model(inputs=inputs, outputs=outputs)
         _ = model({"my_input": tf.constant([[1]])})
         model.save(tmpdir)
         output_schema = get_output_schema(tmpdir)
         output_col = output_schema["my_output"]
-        assert output_col.value_count.min == output_col.value_count.max == 4
+        assert output_col.shape.dims[1].min == output_col.shape.dims[1].max == 4
         assert output_col.is_list is True
         assert output_col.is_ragged is False
 
 
 @pytest.mark.parametrize("run_eagerly", [False])
 def test_simple_model(ecommerce_data: Dataset, run_eagerly):
     model = mm.Model(
@@ -80,14 +82,15 @@
         ]
     )
     loader = mm.Loader(dataset, batch_size=2, shuffle=False)
     model = mm.Model(
         tf.keras.layers.Lambda(lambda x: x["feature"]),
         tf.keras.layers.Dense(1),
         mm.BinaryClassificationTask("target"),
+        schema=dataset.schema,
     )
     model.compile()
     model.fit(loader, epochs=2)
     model.compile()
     model.fit(loader, epochs=2)
 
 
@@ -156,15 +159,15 @@
         input_block_weighed_avg_model,
         mm.MLPBlock([4]),
         mm.BinaryClassificationTask("click"),
     )
 
     testing_utils.model_test(model, loader, run_eagerly=run_eagerly, reload_model=True)
 
-    batch = mm.sample_batch(loader, include_targets=False, to_ragged=True)
+    batch = mm.sample_batch(loader, include_targets=False, prepare_features=True)
     out = model(batch)
     assert out.shape == (100, 1)
 
     predictions = model.predict(loader, batch_size=8, steps=1)
     assert predictions.shape == (100, 1)
 
 
@@ -220,15 +223,15 @@
             self.call_count.assign(tf.constant([0.0]))
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 @pytest.mark.parametrize(
     ["num_rows", "batch_size", "train_metrics_steps", "expected_steps", "expected_metrics_steps"],
     [
-        (1, 1, 1, 1, 1),
+        (2, 2, 1, 1, 1),
         (60, 10, 2, 6, 3),
         (60, 10, 3, 6, 2),
         (120, 10, 4, 12, 3),
     ],
 )
 def test_train_metrics_steps(
     run_eagerly, num_rows, batch_size, train_metrics_steps, expected_steps, expected_metrics_steps
@@ -916,19 +919,19 @@
     )
 
     reloaded_model, _ = testing_utils.model_test(model, ecommerce_data, reload_model=True)
 
     assert isinstance(reloaded_model.query_encoder, mm.EmbeddingEncoder)
     assert isinstance(reloaded_model.candidate_encoder, mm.EmbeddingEncoder)
 
-    queries = model.query_embeddings(ecommerce_data, batch_size=10, index=Tags.USER_ID).compute()
+    queries = model.query_embeddings(ecommerce_data, batch_size=16, index=Tags.USER_ID).compute()
     _check_embeddings(queries, 100, "user_id")
 
     candidates = model.candidate_embeddings(
-        ecommerce_data, batch_size=10, index=candidate
+        ecommerce_data, batch_size=16, index=candidate
     ).compute()
     _check_embeddings(candidates, 100, "item_id")
 
 
 def _check_embeddings(embeddings, extected_len, index_name=None):
     if not isinstance(embeddings, pd.DataFrame):
         embeddings = embeddings.to_pandas()
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/models/test_benchmark.py` & `merlin-models-23.4.0/tests/unit/tf/models/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/models/test_ranking.py` & `merlin-models-23.4.0/tests/unit/tf/models/test_ranking.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import pytest
 import tensorflow as tf
 from tensorflow.keras import regularizers
 
 import merlin.models.tf as mm
 from merlin.datasets.synthetic import generate_data
 from merlin.io import Dataset
+from merlin.models.tf.transforms.features import expected_input_cols_from_schema
 from merlin.models.tf.utils import testing_utils
 from merlin.schema import Tags
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_mf_model_single_binary_task(ecommerce_data, run_eagerly):
     model = mm.MatrixFactorizationModel(
@@ -40,36 +41,34 @@
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 @pytest.mark.parametrize(
     "prediction_blocks", [None, mm.BinaryOutput("click"), mm.BinaryClassificationTask("click")]
 )
 def test_dlrm_model(music_streaming_data, run_eagerly, prediction_blocks):
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(
-        ["item_id", "user_age", "click", "item_genres"]
+        ["item_id", "user_id", "user_age", "item_genres", "click"]
     )
     model = mm.DLRMModel(
         music_streaming_data.schema,
         embedding_dim=2,
-        bottom_block=mm.MLPBlock([2]),
+        bottom_block=mm.MLPBlock([5, 2], dropout=0.05),
         prediction_tasks=prediction_blocks,
     )
 
     loaded_model, _ = testing_utils.model_test(
         model, music_streaming_data, run_eagerly=run_eagerly, reload_model=True
     )
 
-    features = testing_utils.get_model_inputs(
-        music_streaming_data.schema.remove_by_tag(Tags.TARGET), ["item_genres"]
-    )
+    expected_features = expected_input_cols_from_schema(music_streaming_data.schema)
     expected_output_signature = (
         "click/binary_classification_task"
         if isinstance(prediction_blocks, mm.PredictionTask)
         else "click/binary_output"
     )
-    testing_utils.test_model_signature(loaded_model, features, [expected_output_signature])
+    testing_utils.test_model_signature(loaded_model, expected_features, [expected_output_signature])
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_dlrm_model_with_embeddings(music_streaming_data, run_eagerly):
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(
         ["item_id", "user_age", "click"]
     )
@@ -248,15 +247,14 @@
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 @pytest.mark.parametrize(
     "prediction_blocks", [None, mm.BinaryOutput("click"), mm.BinaryClassificationTask("click")]
 )
 def test_wide_deep_model(music_streaming_data, run_eagerly, prediction_blocks):
-
     # prepare wide_schema
     wide_schema = music_streaming_data.schema.select_by_name(["country"])
     deep_schema = music_streaming_data.schema.select_by_name(["country", "user_age"])
 
     model = mm.WideAndDeepModel(
         music_streaming_data.schema,
         wide_schema=wide_schema,
@@ -266,15 +264,14 @@
     )
 
     testing_utils.model_test(model, music_streaming_data, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_wide_deep_model_wide_categorical_one_hot(ecommerce_data, run_eagerly):
-
     wide_schema = ecommerce_data.schema.select_by_name(names=["user_categories", "item_category"])
     deep_schema = ecommerce_data.schema
 
     model = mm.WideAndDeepModel(
         ecommerce_data.schema,
         wide_schema=wide_schema,
         deep_schema=deep_schema,
@@ -284,15 +281,14 @@
     )
 
     testing_utils.model_test(model, ecommerce_data, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_wide_deep_model_hashed_cross(ecommerce_data, run_eagerly):
-
     wide_schema = ecommerce_data.schema.select_by_name(names=["user_categories", "item_category"])
     deep_schema = ecommerce_data.schema
 
     model = mm.WideAndDeepModel(
         ecommerce_data.schema,
         wide_schema=wide_schema,
         deep_schema=deep_schema,
@@ -302,15 +298,14 @@
     )
 
     testing_utils.model_test(model, ecommerce_data, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_wide_deep_embedding_custom_inputblock(music_streaming_data, run_eagerly):
-
     schema = music_streaming_data.schema
     # prepare wide_schema
     wide_schema = schema.select_by_name(["country", "user_age"])
     deep_embedding = mm.Embeddings(schema.select_by_tag(Tags.CATEGORICAL), dim=16)
 
     model = mm.WideAndDeepModel(
         schema,
@@ -325,18 +320,16 @@
         prediction_tasks=mm.BinaryOutput("click"),
     )
 
     testing_utils.model_test(model, music_streaming_data, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_wide_deep_model_wide_onehot_multihot_feature_interaction(ecommerce_data, run_eagerly):
-    ml_dataset = generate_data("movielens-1m", 100)
-    # data_ddf = ml_dataset.to_ddf()
-    # data_ddf = data_ddf[[c for c in list(data_ddf.columns) if c != "rating"]]
+def test_wide_deep_model_wide_onehot_multihot_feature_interaction(run_eagerly):
+    ml_dataset = generate_data("movielens-1m", 100, max_session_length=4)
 
     # Removing the rating regression target
     schema = ml_dataset.schema.remove_col("rating")
     target_col = schema.select_by_tag(Tags.TARGET).column_names[0]
 
     cat_schema = schema.select_by_tag(Tags.CATEGORICAL)
     cat_schema_onehot = cat_schema.remove_col("genres")
@@ -349,34 +342,33 @@
         mm.SequentialBlock(
             mm.Filter(cat_schema_onehot),
             mm.CategoryEncoding(cat_schema_onehot, sparse=True, output_mode="one_hot"),
         ),
         # Multi-hot features
         mm.SequentialBlock(
             mm.Filter(cat_schema_multihot),
-            mm.ListToDense(max_seq_length=6),
+            mm.ToDense(cat_schema_multihot),
             mm.CategoryEncoding(cat_schema_multihot, sparse=True, output_mode="multi_hot"),
         ),
         # 2nd level feature interactions of one-hot features
         mm.SequentialBlock(
             mm.Filter(cat_schema),
-            mm.ListToDense(max_seq_length=6),
+            mm.ToDense(cat_schema),
             mm.HashedCrossAll(
                 cat_schema,
                 num_bins=100,
                 max_level=2,
                 output_mode="multi_hot",
                 sparse=True,
                 ignore_combinations=ignore_combinations,
             ),
         ),
     ]
 
-    batch, _ = mm.sample_batch(ml_dataset, batch_size=100)
-
+    batch, _ = mm.sample_batch(ml_dataset, batch_size=100, prepare_features=True)
     output_wide_features = mm.ParallelBlock(wide_preprocessing_blocks)(batch)
     assert set(output_wide_features.keys()) == set(
         [
             "userId",
             "movieId",
             "title",
             "gender",
@@ -440,15 +432,14 @@
     )
 
     testing_utils.model_test(model, ml_dataset, run_eagerly=run_eagerly)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_wide_deep_model_wide_feature_interaction_multi_optimizer(ecommerce_data, run_eagerly):
-
     deep_schema = ecommerce_data.schema.select_by_name(
         names=["user_categories", "item_category", "user_brands", "item_brand"]
     )
     wide_schema = ecommerce_data.schema.select_by_name(
         names=["user_categories", "item_category", "user_brands", "item_brand"]
     )
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/models/test_retrieval.py` & `merlin-models-23.4.0/tests/unit/tf/models/test_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     MRRAt,
     NDCGAt,
     PrecisionAt,
     RecallAt,
     TopKMetricsAggregator,
 )
 from merlin.models.tf.outputs.base import DotProduct
+from merlin.models.tf.transforms.features import expected_input_cols_from_schema
 from merlin.models.tf.utils import testing_utils
 from merlin.models.utils.dataset import unique_rows_by_features
 from merlin.schema import Tags
 from tests.common.tf.retrieval import retrieval_tests_common
 
 
 def test_two_tower_shared_embeddings():
@@ -117,15 +118,14 @@
 
     assert len(losses.epoch) == 1
     assert all(measure >= 0 for metric in losses.history for measure in losses.history[metric])
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_matrix_factorization_topk_evaluation(music_streaming_data: Dataset, run_eagerly):
-
     music_streaming_data.schema = music_streaming_data.schema.select_by_name(["user_id", "item_id"])
     model = mm.MatrixFactorizationModelV2(
         music_streaming_data.schema, negative_samplers="in-batch", dim=4
     )
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
     _, losses = testing_utils.model_test(model, music_streaming_data, reload_model=False)
 
@@ -207,20 +207,20 @@
     model = mm.TwoTowerModel(music_streaming_data.schema, query_tower=mm.MLPBlock([2]))
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
     losses = model.fit(music_streaming_data, batch_size=50, epochs=num_epochs, steps_per_epoch=1)
     assert len(losses.epoch) == num_epochs
     assert all(measure >= 0 for metric in losses.history for measure in losses.history[metric])
 
-    query_features = testing_utils.get_model_inputs(
-        music_streaming_data.schema.select_by_tag(Tags.USER), ["user_genres"]
+    query_features = expected_input_cols_from_schema(
+        music_streaming_data.schema.select_by_tag(Tags.USER),
     )
     testing_utils.test_model_signature(model.first.query_block(), query_features, ["output_1"])
 
-    item_features = testing_utils.get_model_inputs(
+    item_features = expected_input_cols_from_schema(
         music_streaming_data.schema.select_by_tag(Tags.ITEM),
     )
     testing_utils.test_model_signature(model.first.item_block(), item_features, ["output_1"])
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_two_tower_retrieval_model_evaluate_after_fit_validation_should_raise(
@@ -271,20 +271,20 @@
     model = mm.TwoTowerModelV2(query, candidate)
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
     losses = model.fit(music_streaming_data, batch_size=50, epochs=num_epochs, steps_per_epoch=1)
     assert len(losses.epoch) == num_epochs
     assert all(measure >= 0 for metric in losses.history for measure in losses.history[metric])
 
-    query_features = testing_utils.get_model_inputs(
-        music_streaming_data.schema.select_by_tag(Tags.USER), ["user_genres"]
+    query_features = expected_input_cols_from_schema(
+        music_streaming_data.schema.select_by_tag(Tags.USER)
     )
     testing_utils.test_model_signature(model.query_encoder, query_features, ["output_1"])
 
-    item_features = testing_utils.get_model_inputs(
+    item_features = expected_input_cols_from_schema(
         music_streaming_data.schema.select_by_tag(Tags.ITEM),
     )
     testing_utils.test_model_signature(model.candidate_encoder, item_features, ["output_1"])
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 @pytest.mark.parametrize(
@@ -797,21 +797,26 @@
 #     with pytest.raises(ValueError) as exc_info:
 #         model.evaluate(ecommerce_data, batch_size=10)
 #         assert "You need to specify the set of negatives to use for evaluation" in str(
 #             exc_info.value
 #         )
 
 
+@pytest.mark.skip(
+    reason="The YoutubeDNNRetrievalModel is outdated, "
+    "was never officially released and is going to be deprecated in favor "
+    "of YoutubeDNNRetrievalModelV2"
+)
 def test_youtube_dnn_retrieval(sequence_testing_data: Dataset):
     """This test works both for eager mode and graph mode when
     ran individually. But when both tests are run by pytest
     the last one fails. So somehow pytest is sharing some
     graph state between tests. I keep now only the graph mode test"""
 
-    to_remove = (
+    to_remove = ["event_timestamp"] + (
         sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
         .select_by_tag(Tags.CONTINUOUS)
         .column_names
     )
     sequence_testing_data.schema = sequence_testing_data.schema.excluding_by_name(to_remove)
 
     model = mm.YoutubeDNNRetrievalModel(
@@ -822,22 +827,22 @@
         num_sampled=100,
         embedding_options=mm.EmbeddingOptions(
             embedding_dim_default=2,
         ),
     )
     model.compile(optimizer="adam", run_eagerly=False)
 
-    as_ragged = mm.ListToRagged()
+    prepare_features = mm.PrepareFeatures(sequence_testing_data.schema)
 
     class LastInteractionAsTarget(tf.keras.layers.Layer):
         def call(self, inputs, **kwargs):
-            inputs = as_ragged(inputs)
+            inputs = prepare_features(inputs)
             items = inputs["item_id_seq"]
             _items = items[:, :-1]
-            targets = items[:, -1:].flat_values
+            targets = tf.reshape(items[:, -1:].to_tensor(), (1, -1))
 
             inputs["item_id_seq"] = _items
 
             return inputs, targets
 
     dataloader = mm.Loader(sequence_testing_data, batch_size=50)
 
@@ -889,19 +894,19 @@
     candidate = mm.Encoder(candidate_schema, mm.MLPBlock([8]))
     model = mm.TwoTowerModelV2(
         query_tower=query, candidate_tower=candidate, negative_samplers=["in-batch"]
     )
 
     model, _ = testing_utils.model_test(model, ecommerce_data, reload_model=False)
 
-    queries = model.query_embeddings(ecommerce_data, batch_size=10, index=Tags.USER_ID).compute()
+    queries = model.query_embeddings(ecommerce_data, batch_size=16, index=Tags.USER_ID).compute()
     _check_embeddings(queries, 100, 8, "user_id")
 
     candidates = model.candidate_embeddings(
-        ecommerce_data, batch_size=10, index=Tags.ITEM_ID
+        ecommerce_data, batch_size=16, index=Tags.ITEM_ID
     ).compute()
     _check_embeddings(candidates, 100, 8, "item_id")
 
 
 def test_mf_v2_export_embeddings(
     ecommerce_data: Dataset,
 ):
@@ -909,19 +914,19 @@
         ecommerce_data.schema,
         dim=8,
         negative_samplers="in-batch",
     )
 
     model, _ = testing_utils.model_test(model, ecommerce_data, reload_model=False)
 
-    queries = model.query_embeddings(ecommerce_data, batch_size=10, index=Tags.USER_ID).compute()
+    queries = model.query_embeddings(ecommerce_data, batch_size=16, index=Tags.USER_ID).compute()
     _check_embeddings(queries, 100, 8, "user_id")
 
     candidates = model.candidate_embeddings(
-        ecommerce_data, batch_size=10, index=Tags.ITEM_ID
+        ecommerce_data, batch_size=16, index=Tags.ITEM_ID
     ).compute()
     _check_embeddings(candidates, 100, 8, "item_id")
 
 
 def _check_embeddings(embeddings, extected_len, num_dim=8, index_name=None):
     import pandas as pd
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_base.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_block.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_block.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,17 @@
     music_streaming_data: Dataset, task_blocks, run_eagerly: bool
 ):
     inputs = mm.InputBlockV2(music_streaming_data.schema)
     output_block = mm.OutputBlock(music_streaming_data.schema, task_blocks=task_blocks)
     model = mm.Model(inputs, mm.MLPBlock([64]), output_block)
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
     assert set(list(metrics.keys())) == set(
         [
             "loss",
             "loss_batch",
             "regularization_loss",
@@ -290,15 +292,17 @@
     model.compile(
         optimizer="adam",
         run_eagerly=True,
         metrics=metrics,
         weighted_metrics=weighted_metrics,
     )
 
-    metrics_results = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics_results = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics_results["loss"] >= 0
     assert set(metrics_results.keys()) == set(expected_metrics)
 
 
 @testing_utils.mark_run_eagerly_modes
 def test_model_with_multi_output_blocks_loss_weights_and_weighted_metrics(
@@ -827,15 +831,14 @@
     inputs = mm.InputBlockV2(schema)
     output_block = mm.OutputBlock(music_streaming_data.schema, task_blocks=task_blocks)
     cgc = mm.CGCBlock(
         output_block,
         expert_block=mm.MLPBlock([64]),
         num_task_experts=2,
         num_shared_experts=3,
-        schema=schema,
     )
     model = mm.Model(inputs, cgc, output_block)
 
     _, losses = testing_utils.model_test(
         model,
         music_streaming_data,
         run_eagerly=run_eagerly,
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_classification.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_classification.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import pytest
 import tensorflow as tf
 
 import merlin.models.tf as mm
 from merlin.io import Dataset
 from merlin.models.tf.outputs.classification import CategoricalTarget, EmbeddingTablePrediction
 from merlin.models.tf.utils import testing_utils
-from merlin.schema import Tags
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_binary_output(ecommerce_data: Dataset, run_eagerly):
     model = mm.Model(
         mm.InputBlock(ecommerce_data.schema),
         mm.MLPBlock([8]),
@@ -43,15 +42,14 @@
         "regularization_loss",
     }
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 @pytest.mark.parametrize("use_output_block", [True, False])
 def test_binary_output_two_tasks(ecommerce_data: Dataset, run_eagerly, use_output_block):
-
     if use_output_block:
         output_block = mm.OutputBlock(ecommerce_data.schema)
     else:
         output_block = mm.ParallelBlock(mm.BinaryOutput("click"), mm.BinaryOutput("conversion"))
 
     model = mm.Model(mm.InputBlock(ecommerce_data.schema), mm.MLPBlock([8]), output_block)
 
@@ -74,17 +72,17 @@
         "conversion/binary_output/auc",
         "regularization_loss",
     }
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_categorical_output(sequence_testing_data: Dataset, run_eagerly):
-    dataloader, schema = _next_item_loader(sequence_testing_data)
+    dataloader, schema = testing_utils.loader_for_last_item_prediction(sequence_testing_data)
     model = mm.Model(
-        mm.InputBlock(schema),
+        mm.InputBlockV2(schema),
         mm.MLPBlock([8]),
         mm.CategoricalOutput(schema["item_id_seq"]),
     )
 
     _, history = testing_utils.model_test(model, dataloader, run_eagerly=run_eagerly)
 
     assert set(history.history.keys()) == {
@@ -96,16 +94,16 @@
         "mrr_at_10",
         "recall_at_10",
         "regularization_loss",
     }
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_next_item_prediction(sequence_testing_data: Dataset, run_eagerly):
-    dataloader, schema = _next_item_loader(sequence_testing_data)
+def test_last_item_prediction(sequence_testing_data: Dataset, run_eagerly):
+    dataloader, schema = testing_utils.loader_for_last_item_prediction(sequence_testing_data)
     embeddings = mm.Embeddings(
         schema,
         sequence_combiner=tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1)),
     )
 
     predictions = [
         schema.select_by_name("item_id_seq"),
@@ -118,36 +116,7 @@
     for target in predictions:
         model = mm.Model(
             mm.InputBlockV2(schema, categorical=embeddings),
             mm.MLPBlock([32]),
             mm.CategoricalOutput(target),
         )
         testing_utils.model_test(model, dataloader, run_eagerly=run_eagerly)
-
-
-def _next_item_loader(sequence_testing_data: Dataset):
-    class LastInteractionAsTarget:
-        def compute_output_schema(self, input_schema):
-            return input_schema
-
-        def __call__(self, inputs, targets):
-            inputs = mm.ListToRagged()(inputs)
-            items = inputs["item_id_seq"]
-            _items = items[:, :-1]
-            targets = tf.one_hot(items[:, -1:].flat_values, 51997)
-            inputs["item_id_seq"] = _items
-
-            for k in inputs:
-                if isinstance(inputs[k], tf.RaggedTensor):
-                    inputs[k] = (
-                        tf.expand_dims(inputs[k].values, 1),
-                        tf.expand_dims(inputs[k].row_lengths(), 1),
-                    )
-
-            return inputs, targets
-
-    schema = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL)
-    sequence_testing_data.schema = schema
-    dataloader = mm.Loader(sequence_testing_data, batch_size=50)
-    _last_interaction_as_target = LastInteractionAsTarget()
-    dataloader = dataloader.map(_last_interaction_as_target)
-    return dataloader, schema
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_contrastive.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_contrastive.py`

 * *Files 7% similar despite different names*

```diff
@@ -97,26 +97,27 @@
         ),
     )
 
     testing_utils.model_test(model, ecommerce_data, reload_model=True)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_contrastive_output(ecommerce_data: Dataset, run_eagerly):
+def test_contrastive_output_with_sampled_softmax(ecommerce_data: Dataset, run_eagerly):
     schema = ecommerce_data.schema
     schema["item_category"] = schema["item_category"].with_tags(
         schema["item_category"].tags + "target"
     )
     ecommerce_data.schema = schema
     model = mm.Model(
         mm.InputBlock(schema),
         mm.MLPBlock([8]),
         mm.ContrastiveOutput(
             schema["item_category"],
-            negative_samplers=PopularityBasedSamplerV2(max_id=100, max_num_samples=20),
+            negative_samplers=PopularityBasedSamplerV2(max_id=100, max_num_samples=20, min_id=1),
+            logq_sampling_correction=True,
         ),
     )
 
     _, history = testing_utils.model_test(model, ecommerce_data, run_eagerly=run_eagerly)
 
     assert set(history.history.keys()) == {
         "loss",
@@ -127,15 +128,17 @@
         "mrr_at_10",
         "recall_at_10",
         "regularization_loss",
     }
 
 
 def test_setting_negative_sampling_strategy(sequence_testing_data: Dataset):
-    dataloader, schema = _next_item_loader(sequence_testing_data, to_one_hot=False)
+    dataloader, schema = testing_utils.loader_for_last_item_prediction(
+        sequence_testing_data, to_one_hot=False
+    )
     model_out = mm.ContrastiveOutput(schema["item_id_seq"], "in-batch")
     model = mm.Model(mm.InputBlockV2(schema), mm.MLPBlock([32]), model_out)
     model.compile(optimizer="adam")
 
     batch = next(iter(dataloader))
     output = model(batch[0], batch[1], training=True)
     assert output[1].shape == (batch[1].shape[0], 51)
@@ -240,26 +243,7 @@
     items_embeddings = tf.random.uniform(shape=(batch_size, 5), dtype=tf.float32)
     positive_items = tf.random.uniform(
         shape=(batch_size,), minval=1, maxval=1000000, dtype=tf.int32
     )
     inputs = {"query": users_embeddings, "candidate": items_embeddings}
     features = {"item_id": positive_items, "user_id": None}
     return inputs, features
-
-
-def _next_item_loader(sequence_testing_data: Dataset, to_one_hot=True):
-    def _last_interaction_as_target(inputs, targets):
-        inputs = mm.ListToRagged()(inputs)
-        items = inputs["item_id_seq"]
-        _items = items[:, :-1]
-
-        targets = items[:, -1:].flat_values
-        if to_one_hot:
-            targets = tf.one_hot(targets, 51997)
-        inputs["item_id_seq"] = _items
-        return inputs, targets
-
-    schema = sequence_testing_data.schema.select_by_tag(Tags.CATEGORICAL)
-    sequence_testing_data.schema = schema
-    loader = mm.Loader(sequence_testing_data, batch_size=50)
-    loader = loader.map(_last_interaction_as_target)
-    return loader, schema
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_regression.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_sampling.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_sampling.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,58 +19,59 @@
 
 import merlin.models.tf as mm
 from merlin.models.tf.outputs.sampling.popularity import PopularityBasedSamplerV2
 
 
 def test_inbatch_sampler():
     item_embeddings = tf.random.uniform(shape=(10, 5), dtype=tf.float32)
-    item_ids = tf.random.uniform(shape=(10,), minval=1, maxval=10000, dtype=tf.int32)
+    item_ids = tf.random.uniform(shape=(10, 1), minval=1, maxval=10000, dtype=tf.int32)
 
     inbatch_sampler = mm.InBatchSamplerV2()
 
-    input_data = mm.Candidate(item_ids, {"item_ids": item_ids}).with_embedding(item_embeddings)
+    input_data = mm.Candidate(id=item_ids, metadata={"item_ids": item_ids}).with_embedding(
+        item_embeddings
+    )
     output_data = inbatch_sampler(input_data)
 
     tf.assert_equal(input_data.embedding, output_data.embedding)
     for feat_name in output_data.metadata:
         tf.assert_equal(input_data.metadata[feat_name], output_data.metadata[feat_name])
 
 
 def test_inbatch_sampler_no_metadata_features():
-    item_ids = tf.random.uniform(shape=(10,), minval=1, maxval=10000, dtype=tf.int32)
+    item_ids = tf.random.uniform(shape=(10, 1), minval=1, maxval=10000, dtype=tf.int32)
 
     inbatch_sampler = mm.InBatchSamplerV2()
 
-    input_data = mm.Candidate(item_ids, {})
+    input_data = mm.Candidate(id=item_ids, metadata={})
     output_data = inbatch_sampler(input_data)
 
     tf.assert_equal(input_data.id, output_data.id)
     assert output_data.metadata == {}
 
 
 def test_popularity_sampler():
     num_classes = 1000
     min_id = 2
     num_sampled = 10
-    item_ids = tf.random.uniform(shape=(10,), minval=1, maxval=num_classes, dtype=tf.int32)
+    item_ids = tf.random.uniform(shape=(10, 1), minval=1, maxval=num_classes, dtype=tf.int32)
 
     popularity_sampler = PopularityBasedSamplerV2(
         max_num_samples=num_sampled, max_id=num_classes - 1, min_id=min_id
     )
 
-    input_data = mm.Candidate(item_ids, {})
+    input_data = mm.Candidate(id=item_ids, metadata={})
     output_data = popularity_sampler(input_data)
 
-    assert len(tf.unique_with_counts(output_data.id)[0]) == num_sampled
+    assert len(tf.unique_with_counts(tf.squeeze(output_data.id))[0]) == num_sampled
 
     tf.assert_equal(tf.reduce_all(output_data.id >= min_id), True)
 
 
 def test_popularity_sampler_with_num_samples_greater_than_cardinality():
-
     num_classes = 50
     min_id = 2
     num_sampled = 100
 
     with pytest.raises(Exception) as excinfo:
         _ = PopularityBasedSamplerV2(
             max_num_samples=num_sampled, max_id=num_classes - 1, min_id=min_id
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/outputs/test_topk.py` & `merlin-models-23.4.0/tests/unit/tf/outputs/test_topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_classification.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_multi_task.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_multi_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,17 @@
     music_streaming_data: Dataset, task_blocks, run_eagerly: bool
 ):
     inputs = mm.InputBlockV2(music_streaming_data.schema)
     prediction_tasks = mm.PredictionTasks(music_streaming_data.schema, task_blocks=task_blocks)
     model = mm.Model(inputs, mm.MLPBlock([64]), prediction_tasks)
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
     assert set(list(metrics.keys())) == set(
         [
             "loss",
             "loss_batch",
             "regularization_loss",
@@ -165,15 +167,17 @@
         optimizer="adam",
         run_eagerly=run_eagerly,
         metrics=metrics,
         weighted_metrics=weighted_metrics,
         from_serialized=False,
     )
 
-    metrics_results = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics_results = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics_results["loss"] >= 0
     assert set(metrics_results.keys()) == set(expected_metrics)
 
 
 @testing_utils.mark_run_eagerly_modes
 def test_model_with_multiple_tasks_loss_weights_and_weighted_metrics(
@@ -210,15 +214,15 @@
     model.compile(
         optimizer="adam",
         run_eagerly=run_eagerly,
         loss_weights=loss_weights,
         weighted_metrics=weighted_metrics,
     )
 
-    batch = mm.sample_batch(music_streaming_data, batch_size=50)
+    batch = mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
 
     metrics = model.test_step(batch)
 
     assert metrics["loss"] >= 0
     assert set(metrics.keys()) == set(
         [
             "loss",
@@ -299,15 +303,17 @@
         "click/binary_classification_task": 1.0,
         "like/binary_classification_task": 2.0,
         "play_percentage/regression_task": 3.0,
     }
 
     model.compile(optimizer="adam", run_eagerly=run_eagerly, loss_weights=loss_weights)
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
 
     expected_metrics = [
         "loss",
         "loss_batch",
         "click/binary_classification_task_loss",
@@ -344,15 +350,17 @@
             features: Dict[str, tf.Tensor] = None,
             targets: tf.Tensor = None,
             training=True,
             testing=False,
             **kwargs,
         ) -> PredictionOutput:
             # Computes loss for the like loss only for clicked items
-            outputs = outputs.copy_with_updates(sample_weight=targets)
+            outputs = outputs.copy_with_updates(
+                sample_weight=tf.expand_dims(targets["click"], -1),
+            )
             return outputs
 
     inputs = mm.InputBlockV2(music_streaming_data.schema)
     prediction_tasks = mm.PredictionTasks(
         music_streaming_data.schema, task_pre_dict={"like": CustomSampleWeight()}
     )
     mmoe = mm.MMOEBlock(prediction_tasks, expert_block=mm.MLPBlock([64]), num_experts=4)
@@ -385,15 +393,17 @@
     model.compile(
         optimizer="adam",
         run_eagerly=run_eagerly,
         loss_weights=loss_weights,
         weighted_metrics=weighted_metrics,
     )
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
     assert set(metrics.keys()) == set(
         [
             "loss",
             "loss_batch",
             "regularization_loss",
@@ -457,20 +467,21 @@
     inputs = mm.InputBlockV2(schema)
     prediction_tasks = mm.PredictionTasks(schema, task_blocks=task_blocks)
     cgc = mm.CGCBlock(
         prediction_tasks,
         expert_block=mm.MLPBlock([64]),
         num_task_experts=2,
         num_shared_experts=3,
-        schema=schema,
     )
     model = mm.Model(inputs, cgc, prediction_tasks)
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
     assert set(metrics.keys()) == set(
         [
             "loss",
             "loss_batch",
             "click/binary_classification_task_loss",
@@ -505,15 +516,17 @@
         expert_block=mm.MLPBlock([64]),
         num_task_experts=2,
         num_shared_experts=3,
     )
     model = mm.Model(inputs, cgc, prediction_tasks)
     model.compile(optimizer="adam", run_eagerly=run_eagerly)
 
-    metrics = model.train_step(mm.sample_batch(music_streaming_data, batch_size=50))
+    metrics = model.train_step(
+        mm.sample_batch(music_streaming_data, batch_size=50, prepare_features=False)
+    )
 
     assert metrics["loss"] >= 0
     assert set(metrics.keys()) == set(
         [
             "loss",
             "click/binary_classification_task_loss",
             "like/binary_classification_task_loss",
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_next_item.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_next_item.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_regression.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_retrieval.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/prediction_tasks/test_sampling.py` & `merlin-models-23.4.0/tests/unit/tf/prediction_tasks/test_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/test_core.py` & `merlin-models-23.4.0/tests/unit/tf/test_core.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/test_loader.py` & `merlin-models-23.4.0/tests/unit/tf/test_loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import pytest
 import tensorflow as tf
 from sklearn.metrics import roc_auc_score
 
 import merlin.models.tf as mm
 from merlin.core.dispatch import make_df
 from merlin.io.dataset import Dataset
+from merlin.models.tf.utils.tf_utils import list_col_to_ragged
 from merlin.models.utils.schema_utils import create_categorical_column
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 def test_lazy_dataset_map():
     dataset_size = 100
     data_df = pd.DataFrame({"feature": np.random.randint(100, size=dataset_size)})
@@ -69,36 +70,29 @@
         label_names=["label"],
         batch_size=batch_size,
         shuffle=False,
     )
 
     batch = next(iter(loader))
 
-    # [[1,2,3],[3,1],[...],[]]
     @tf.function
-    def _ragged_for_nested_data_col():
-        nested_data_col = tf.RaggedTensor.from_row_lengths(
-            batch[0]["data"][0][:, 0], tf.cast(batch[0]["data"][1][:, 0], tf.int32)
+    def _ragged_to_dense(col_name):
+        result = list_col_to_ragged(
+            batch[0][f"{col_name}__values"], batch[0][f"{col_name}__offsets"]
         ).to_tensor()
-        return nested_data_col
+        return result
 
-    nested_data_col = _ragged_for_nested_data_col()
+    # [[1,2,3],[3,1],[...],[]]
+    nested_data_col = _ragged_to_dense("data")
     true_data_col = tf.reshape(
         tf.ragged.constant(df.iloc[:batch_size, 0].tolist()).to_tensor(), [batch_size, -1]
     )
 
     # [1,2,3]
-    @tf.function
-    def _ragged_for_multihot_data_col():
-        multihot_data2_col = tf.RaggedTensor.from_row_lengths(
-            batch[0]["data2"][0][:, 0], tf.cast(batch[0]["data2"][1][:, 0], tf.int32)
-        ).to_tensor()
-        return multihot_data2_col
-
-    multihot_data2_col = _ragged_for_multihot_data_col()
+    multihot_data2_col = _ragged_to_dense("data2")
     true_data2_col = tf.reshape(
         tf.ragged.constant(df.iloc[:batch_size, 1].tolist()).to_tensor(), [batch_size, -1]
     )
     assert nested_data_col.shape == true_data_col.shape
     assert np.allclose(nested_data_col.numpy(), true_data_col.numpy())
     assert multihot_data2_col.shape == true_data2_col.shape
     assert np.allclose(multihot_data2_col.numpy(), true_data2_col.numpy())
@@ -275,30 +269,30 @@
 
     validator = mm.KerasSequenceValidator(loader)
     model.fit(loader, epochs=2, verbose=0, callbacks=[validator])
 
     predictions, labels = [], []
     for X, y_true in loader:
         y_pred = model(X)
-        labels.extend(y_true.numpy()[:, 0])
+        labels.extend(y_true.numpy())
         predictions.extend(y_pred.numpy()[:, 0])
     predictions = np.array(predictions)
     labels = np.array(labels)
 
     logs = {}
     validator.on_epoch_end(0, logs)
     auc_key = [i for i in logs if i.startswith("val_auc")][0]
 
     true_accuracy = (labels == (predictions > 0.5)).mean()
     estimated_accuracy = logs["val_accuracy"]
-    assert np.isclose(true_accuracy, estimated_accuracy, rtol=1e-6)
+    assert np.isclose(true_accuracy, estimated_accuracy, rtol=1e-1)
 
     true_auc = roc_auc_score(labels, predictions)
     estimated_auc = logs[auc_key]
-    assert np.isclose(true_auc, estimated_auc, rtol=1e-6)
+    assert np.isclose(true_auc, estimated_auc, rtol=1e-1)
 
 
 def test_block_with_sparse_inputs(music_streaming_data: Dataset):
     item_id_schema = music_streaming_data.schema.select_by_name(["user_id", "item_genres"])
 
     inputs = mm.InputBlock(item_id_schema)
     block = inputs.connect(mm.MLPBlock([64]), context=mm.ModelContext())
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/test_public_api.py` & `merlin-models-23.4.0/tests/unit/tf/test_public_api.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/transformers/__init__.py` & `merlin-models-23.4.0/tests/unit/xgb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import pytest
 
-pytest.importorskip("transformers")
+pytest.importorskip("xgboost")
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transformers/test_block.py` & `merlin-models-23.4.0/tests/unit/tf/transformers/test_block.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,42 +108,38 @@
         transformer_post="pooler_output",
     )
     outputs = transformer_encod(inputs)
 
     assert list(outputs.shape) == [NUM_ROWS, EMBED_DIM]
 
 
-@pytest.mark.parametrize("max_seq_length", [None, 5, 20])
-def test_transformer_encoder_with_list_to_dense(max_seq_length):
+def test_transformer_encoder_with_list_to_dense():
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
     inputs = tf.RaggedTensor.from_tensor(tf.random.uniform((NUM_ROWS, SEQ_LENGTH, EMBED_DIM)))
 
     transformer_encod = mm.TransformerBlock(
         transformer=BertConfig(hidden_size=EMBED_DIM, num_attention_heads=16),
-        pre=mm.ListToDense(max_seq_length=max_seq_length),
+        pre=mm.ToDense(),
     )
     outputs = transformer_encod(inputs)
 
-    if max_seq_length is not None:
-        assert list(outputs.shape) == [NUM_ROWS, max_seq_length, EMBED_DIM]
-    else:
-        assert list(outputs.shape) == [NUM_ROWS, SEQ_LENGTH, EMBED_DIM]
+    assert list(outputs.shape) == [NUM_ROWS, SEQ_LENGTH, EMBED_DIM]
 
 
 def test_transformer_encoder_with_post():
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
     inputs = tf.RaggedTensor.from_tensor(tf.random.uniform((NUM_ROWS, SEQ_LENGTH, EMBED_DIM)))
 
     transformer_encod = mm.TransformerBlock(
         transformer=BertConfig(hidden_size=EMBED_DIM, num_attention_heads=16),
-        pre=mm.ListToDense(max_seq_length=5),
+        pre=mm.ToDense(),
         post="sequence_mean",
     )
     outputs = transformer_encod(inputs)
     testing_utils.assert_serialization(transformer_encod)
     assert list(outputs.shape) == [NUM_ROWS, EMBED_DIM]
 
 
@@ -182,15 +178,15 @@
             to_call=schema["user_country"],
         ),
     )
 
     batch = loader.peek()[0]
 
     outputs = model(batch)
-    assert list(outputs.shape) == [50, 63]
+    assert list(outputs.shape) == [64, 63]
     testing_utils.model_test(model, loader, run_eagerly=run_eagerly)
 
 
 def test_tranformer_with_prepare_module(sequence_testing_data):
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
@@ -223,165 +219,215 @@
 def classification_loader(sequence_testing_data: Dataset):
     schema = sequence_testing_data.schema.select_by_name(
         ["item_id_seq", "categories", "user_country"]
     )
     sequence_testing_data.schema = schema
     dataloader = mm.Loader(
         sequence_testing_data,
-        batch_size=50,
+        batch_size=64,
     ).map(mm.ToTarget(schema, "user_country", one_hot=True))
     return dataloader, dataloader.output_schema
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_transformer_with_causal_language_modeling(sequence_testing_data: Dataset, run_eagerly):
-
+def test_transformer_with_predict_random(sequence_testing_data: Dataset, run_eagerly):
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE).select_by_tag(
         Tags.CATEGORICAL
     )
     target_schema = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID)
     target = target_schema.column_names[0]
 
     sequence_testing_data.schema = seq_schema + target_schema
+    model_schema = sequence_testing_data.schema
 
-    predict_next = mm.SequencePredictNext(schema=seq_schema, target=target)
+    transformer_input_dim = 48
+    transformer_block = GPT2Block(d_model=transformer_input_dim, n_head=8, n_layer=2)
+    model = mm.Model(
+        mm.InputBlockV2(
+            model_schema,
+            categorical=mm.Embeddings(
+                model_schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
+            ),
+        ),
+        mm.MLPBlock([transformer_input_dim]),
+        transformer_block,
+        mm.CategoricalOutput(
+            model_schema.select_by_name(target), default_loss="categorical_crossentropy"
+        ),
+    )
+
+    predict_next = mm.SequencePredictRandom(
+        schema=seq_schema, target=target, transformer=transformer_block
+    )
     loader = Loader(sequence_testing_data, batch_size=8, shuffle=False)
+
+    testing_utils.model_test(
+        model, loader, run_eagerly=run_eagerly, reload_model=True, fit_kwargs={"pre": predict_next}
+    )
+
+    predict_last = mm.SequencePredictLast(
+        schema=seq_schema, target=target, transformer=transformer_block
+    )
+    metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=predict_last)
+    assert len(metrics) > 0
+
+
+@pytest.mark.parametrize("run_eagerly", [True, False])
+def test_transformer_with_causal_language_modeling(sequence_testing_data: Dataset, run_eagerly):
+    seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE).select_by_tag(
+        Tags.CATEGORICAL
+    )
+    target_schema = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID)
+    target = target_schema.column_names[0]
+
+    sequence_testing_data.schema = seq_schema + target_schema
     model_schema = sequence_testing_data.schema
 
     transformer_input_dim = 48
+    transformer_block = GPT2Block(d_model=transformer_input_dim, n_head=8, n_layer=2)
     model = mm.Model(
         mm.InputBlockV2(
             model_schema,
             categorical=mm.Embeddings(
                 model_schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
             ),
         ),
         mm.MLPBlock([transformer_input_dim]),
-        GPT2Block(d_model=transformer_input_dim, n_head=8, n_layer=2),
+        transformer_block,
         mm.CategoricalOutput(
             model_schema.select_by_name(target), default_loss="categorical_crossentropy"
         ),
     )
 
-    batch = next(iter(loader))[0]
-    outputs = model(batch)
-    assert list(outputs.shape) == [8, 4, 51997]
+    predict_next = mm.SequencePredictNext(
+        schema=seq_schema, target=target, transformer=transformer_block
+    )
+    loader = Loader(sequence_testing_data, batch_size=8, shuffle=False)
+
     testing_utils.model_test(
         model, loader, run_eagerly=run_eagerly, reload_model=True, fit_kwargs={"pre": predict_next}
     )
 
+    batch = next(iter(loader))[0]
+    outputs = model(batch)
+    assert list(outputs.shape) == [8, 51997]
+
     metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=predict_next)
     assert len(metrics) > 0
 
     predictions = model.predict(loader, batch_size=8, steps=1)
-    assert predictions.shape == (8, 4, 51997)
+    assert predictions.shape == (8, 51997)
+
+    predict_last = mm.SequencePredictLast(
+        schema=seq_schema, target=target, transformer=transformer_block
+    )
+    metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=predict_last)
+    assert len(metrics) > 0
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_transformer_with_masked_language_modeling(sequence_testing_data: Dataset, run_eagerly):
-
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
 
     target_schema = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID)
     model_schema = seq_schema + target_schema
     target = target_schema.column_names[0]
 
     sequence_testing_data.schema = model_schema
 
     loader = Loader(sequence_testing_data, batch_size=8, shuffle=False)
     transformer_input_dim = 48
+    transformer_block = XLNetBlock(d_model=transformer_input_dim, n_head=8, n_layer=2)
     model = mm.Model(
         mm.InputBlockV2(
             seq_schema,
             categorical=mm.Embeddings(
                 seq_schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
             ),
         ),
         mm.MLPBlock([transformer_input_dim]),
-        XLNetBlock(
-            d_model=transformer_input_dim,
-            n_head=8,
-            n_layer=2,
-            pre=mm.SequentialBlock([mm.SequenceMaskLastInference(), mm.ReplaceMaskedEmbeddings()]),
-            post="inference_hidden_state",
-        ),
+        transformer_block,
         mm.CategoricalOutput(
             seq_schema.select_by_name(target),
             default_loss="categorical_crossentropy",
         ),
     )
-    seq_mask_random = mm.SequenceMaskRandom(schema=seq_schema, target=target, masking_prob=0.3)
+    seq_mask_random = mm.SequenceMaskRandom(
+        schema=seq_schema, target=target, masking_prob=0.3, transformer=transformer_block
+    )
 
     inputs, targets = loader.peek()
 
     outputs = model(inputs, targets=targets, training=True)
     assert list(outputs.shape) == [8, 4, 51997]
     testing_utils.model_test(
         model,
         loader,
         run_eagerly=run_eagerly,
         reload_model=True,
         fit_kwargs={"pre": seq_mask_random},
     )
 
-    seq_mask_last = mm.SequenceMaskLast(schema=seq_schema, target=target)
+    seq_mask_last = mm.SequenceMaskLast(
+        schema=seq_schema, target=target, transformer=transformer_block
+    )
     metrics = model.evaluate(loader, batch_size=8, steps=1, return_dict=True, pre=seq_mask_last)
     assert len(metrics) > 0
 
     # Get predictions for next-item position
     predictions = model.predict(loader, batch_size=8, steps=1)
     assert predictions.shape == (8, 51997)
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
 def test_transformer_with_masked_language_modeling_check_eval_masked(
     sequence_testing_data: Dataset, run_eagerly
 ):
-
     seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE)
 
     target_schema = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID)
     target = target_schema.column_names[0]
     model_schema = seq_schema + target_schema
     sequence_testing_data.schema = model_schema
 
     loader = Loader(sequence_testing_data, batch_size=8, shuffle=False)
 
     transformer_input_dim = 48
+    transformer_block = BertBlock(d_model=transformer_input_dim, n_head=8, n_layer=2)
     model = mm.Model(
         mm.InputBlockV2(
             seq_schema,
             categorical=mm.Embeddings(
                 seq_schema.select_by_tag(Tags.CATEGORICAL), sequence_combiner=None
             ),
         ),
         mm.MLPBlock([transformer_input_dim]),
-        BertBlock(
-            d_model=transformer_input_dim, n_head=8, n_layer=2, pre=mm.ReplaceMaskedEmbeddings()
-        ),
+        transformer_block,
         mm.CategoricalOutput(
             seq_schema.select_by_name(target),
             default_loss="categorical_crossentropy",
         ),
     )
-    seq_mask_random = mm.SequenceMaskRandom(schema=seq_schema, target=target, masking_prob=0.3)
-
-    inputs = itertools.islice(iter(loader), 1)
-    outputs = model.predict(inputs, pre=seq_mask_random)
-    assert list(outputs.shape) == [8, 4, 51997]
+    seq_mask_random = mm.SequenceMaskRandom(
+        schema=seq_schema, target=target, masking_prob=0.3, transformer=transformer_block
+    )
 
     testing_utils.model_test(
         model,
         loader,
         run_eagerly=run_eagerly,
         reload_model=True,
         fit_kwargs={"pre": seq_mask_random},
         metrics=[mm.RecallAt(5000), mm.NDCGAt(5000, seed=4)],
     )
 
+    inputs = itertools.islice(iter(loader), 1)
+    outputs = model.predict(inputs, pre=seq_mask_random)
+    assert list(outputs.shape) == [8, 51997]
+
     # This transform only extracts targets, but without applying mask
     seq_target_as_input_no_mask = mm.SequenceTargetAsInput(schema=seq_schema, target=target)
 
     with Loader(sequence_testing_data, batch_size=8, shuffle=False) as loader:
         metrics_all_positions1 = model.evaluate(
             loader, batch_size=8, steps=1, return_dict=True, pre=seq_target_as_input_no_mask
         )
@@ -432,35 +478,32 @@
             sequence_combiner=None,
         ),
         post=mm.BroadcastToSequence(context_schema, seq_schema),
     )
 
     dmodel = 32
     mlp_block = mm.MLPBlock([128, dmodel], activation="relu")
-
-    dense_block = mm.SequentialBlock(
-        input_block,
-        mlp_block,
-        mm.GPT2Block(
-            d_model=dmodel,
-            n_head=4,
-            n_layer=2,
-            pre=mm.ReplaceMaskedEmbeddings(),
-            post="inference_hidden_state",
-        ),
+    transformer_block = mm.GPT2Block(
+        d_model=dmodel,
+        n_head=4,
+        n_layer=2,
     )
 
+    dense_block = mm.SequentialBlock(input_block, mlp_block, transformer_block)
+
     mlp_block2 = mm.MLPBlock([128, dmodel], activation="relu")
 
     prediction_task = mm.CategoricalOutput(
         to_call=input_block["categorical"][item_id_name],
     )
     model = mm.Model(dense_block, mlp_block2, prediction_task)
 
-    fit_pre = mm.SequenceMaskRandom(schema=seq_schema, target=target, masking_prob=0.3)
+    fit_pre = mm.SequenceMaskRandom(
+        schema=seq_schema, target=target, masking_prob=0.3, transformer=transformer_block
+    )
     testing_utils.model_test(
         model,
         sequence_testing_data,
         run_eagerly=run_eagerly,
         reload_model=False,
         fit_kwargs={"pre": fit_pre},
     )
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transformers/test_transforms.py` & `merlin-models-23.4.0/tests/unit/tf/transformers/test_transforms.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_bias.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_bias.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_features.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,16 @@
     schema = Schema(
         [
             create_categorical_column("cat1", tags=[Tags.CATEGORICAL], num_items=3),
             create_categorical_column("cat2", tags=[Tags.CATEGORICAL], num_items=3),
         ]
     )
     inputs = {}
-    inputs["cat1"] = tf.constant(["A", "B"])
-    inputs["cat2"] = tf.constant([101, 102])
+    inputs["cat1"] = tf.constant([["A"], ["B"]])
+    inputs["cat2"] = tf.constant([[101], [102]])
     hashed_cross_op = mm.HashedCross(schema=schema, num_bins=10, output_mode="int")
     outputs = hashed_cross_op(inputs)
     output_name, output_value = outputs.popitem()
 
     assert output_name == "cross_cat1_cat2"
     assert output_value.shape.as_list() == [2, 1]
     test_case.assertAllClose(output_value, [[1], [6]])
@@ -99,16 +99,16 @@
     schema = Schema(
         [
             create_categorical_column("cat1", tags=[Tags.CATEGORICAL], num_items=20),
             create_categorical_column("cat2", tags=[Tags.CATEGORICAL], num_items=20),
         ]
     )
     inputs = {}
-    inputs["cat1"] = tf.constant(["A", "B", "A", "B", "A"])
-    inputs["cat2"] = tf.constant([101, 101, 101, 102, 102])
+    inputs["cat1"] = tf.constant([["A"], ["B"], ["A"], ["B"], ["A"]])
+    inputs["cat2"] = tf.constant([[101], [101], [101], [102], [102]])
     hashed_cross_op = mm.HashedCross(schema=schema, num_bins=10, output_mode="int")
     outputs = hashed_cross_op(inputs)
     _, output_value = outputs.popitem()
 
     assert output_value.shape.as_list() == [5, 1]
     test_case.assertAllClose(output_value, [[1], [4], [1], [6], [3]])
 
@@ -360,17 +360,17 @@
     schema = Schema(
         [
             create_categorical_column("dense_feature", tags=[Tags.CATEGORICAL], num_items=4),
             create_categorical_column("sparse_feature", tags=[Tags.CATEGORICAL], num_items=5),
         ]
     )
     inputs = {}
-    inputs["dense_feature"] = tf.constant([[1, 2, 3], [3, 3, 0]])
-    inputs["sparse_feature"] = tf.sparse.from_dense(
-        np.array([[1, 2, 3, 0], [0, 3, 1, 0]], dtype=np.int64)
+    inputs["dense_feature"] = tf.expand_dims(tf.constant([[1, 2, 3], [3, 3, 0]]), -1)
+    inputs["sparse_feature"] = tf.sparse.expand_dims(
+        tf.sparse.from_dense(np.array([[1, 2, 3, 0], [0, 3, 1, 0]], dtype=np.int64)), -1
     )
 
     # 1. Sparse output
     category_encoding = mm.CategoryEncoding(
         schema=schema,
         output_mode="count",
         sparse=True,
@@ -417,15 +417,15 @@
         output_mode="count",
         sparse=False,
     )
     with test_case.assertRaisesRegex(ValueError, "inputs should not contain a RaggedTensor"):
         category_encoding(inputs)
 
 
-@pytest.mark.parametrize("input", [np.array([[1, 2, 3, 4], [4, 3, 1, 4]])])
+@pytest.mark.parametrize("input", [np.expand_dims(np.array([[1, 2, 3, 4], [4, 3, 1, 4]]), -1)])
 @pytest.mark.parametrize("weight", [np.array([[0.1, 0.2, 0.3, 0.4], [0.2, 0.1, 0.4, 0.3]])])
 def test_category_encoding_weightd_count_dense(input, weight):
     test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
         ]
@@ -442,15 +442,18 @@
     inputs = {}
     inputs["feature"] = input
     outputs = category_encoding(inputs)
     test_case.assertAllEqual(expected_output_shape, outputs["feature"].shape.as_list())
     test_case.assertAllClose(expected_output, outputs["feature"])
 
 
-@pytest.mark.parametrize("input", [tf.sparse.from_dense(np.array([[1, 2, 3, 4], [4, 3, 1, 4]]))])
+@pytest.mark.parametrize(
+    "input",
+    [tf.sparse.expand_dims(tf.sparse.from_dense(np.array([[1, 2, 3, 4], [4, 3, 1, 4]])), -1)],
+)
 @pytest.mark.parametrize(
     "weight", [tf.sparse.from_dense(np.array([[0.1, 0.2, 0.3, 0.4], [0.2, 0.1, 0.4, 0.3]]))]
 )
 def test_category_encoding_weightd_count_sparse(input, weight):
     test_case = TestCase()
     schema = Schema(
         [
@@ -469,15 +472,18 @@
     inputs = {}
     inputs["feature"] = input
     outputs = category_encoding(inputs)
     test_case.assertAllEqual(expected_output_shape, outputs["feature"].shape.as_list())
     test_case.assertAllClose(expected_output, outputs["feature"])
 
 
-@pytest.mark.parametrize("input", [tf.sparse.from_dense(np.array([[1, 2, 3, 4], [4, 3, 1, 4]]))])
+@pytest.mark.parametrize(
+    "input",
+    [tf.sparse.expand_dims(tf.sparse.from_dense(np.array([[1, 2, 3, 4], [4, 3, 1, 4]])), -1)],
+)
 @pytest.mark.parametrize("weight", [np.array([[0.1, 0.2, 0.3, 0.4], [0.2, 0.1, 0.4, 0.3]])])
 def test_category_encoding_weightd_count_not_match(input, weight):
     test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
         ]
@@ -492,16 +498,16 @@
     ):
         category_encoding(inputs)
 
 
 @pytest.mark.parametrize(
     "input",
     [
-        tf.convert_to_tensor([[1, 2, 3, 0], [0, 3, 1, 0]]),
-        tf.sparse.from_dense(np.array([[1, 2, 3, 0], [0, 3, 1, 0]])),
+        tf.expand_dims(tf.convert_to_tensor([[1, 2, 3, 0], [0, 3, 1, 0]]), -1),
+        tf.sparse.expand_dims(tf.sparse.from_dense(np.array([[1, 2, 3, 0], [0, 3, 1, 0]])), -1),
     ],
 )
 def test_category_encoding_multi_hot_2d_input(input):
     test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
@@ -524,18 +530,18 @@
     test_case.assertAllEqual(expected_output_shape, outputs["feature"].shape.as_list())
     test_case.assertAllClose(expected_output, outputs["feature"])
 
 
 @pytest.mark.parametrize(
     "input",
     [
-        tf.convert_to_tensor([1, 2, 0]),
-        tf.sparse.from_dense([1, 2, 0]),
         tf.convert_to_tensor([[1], [2], [0]]),
         tf.sparse.from_dense([[1], [2], [0]]),
+        tf.convert_to_tensor([[[1]], [[2]], [[0]]]),
+        tf.sparse.from_dense([[[1]], [[2]], [[0]]]),
     ],
 )
 def test_category_encoding_multi_hot_single_value(input):
     test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
@@ -558,18 +564,18 @@
     test_case.assertAllEqual(expected_output_shape, outputs["feature"].shape.as_list())
     test_case.assertAllClose(expected_output, outputs["feature"])
 
 
 @pytest.mark.parametrize(
     "input",
     [
-        tf.convert_to_tensor([1, 2, 3, 0]),
-        tf.sparse.from_dense(np.array([1, 2, 3, 0])),
         tf.convert_to_tensor([[1], [2], [3], [0]]),
         tf.sparse.from_dense(np.array([[1], [2], [3], [0]])),
+        tf.convert_to_tensor([[[1]], [[2]], [[3]], [[0]]]),
+        tf.sparse.from_dense(np.array([[[1]], [[2]], [[3]], [[0]]])),
     ],
 )
 def test_category_encoding_one_hot(input):
     test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
@@ -601,15 +607,18 @@
     outputs = category_encoding(inputs)
     test_case.assertAllEqual(expected_output_shape, outputs["feature"].shape.as_list())
     test_case.assertAllClose(expected_output, outputs["feature"])
 
 
 @pytest.mark.parametrize(
     "input",
-    [tf.convert_to_tensor([[1, 2], [2, 0]]), tf.sparse.from_dense(np.array([[1, 2], [2, 0]]))],
+    [
+        tf.convert_to_tensor([[[1], [2]], [[2], [0]]]),
+        tf.sparse.from_dense(np.array([[[1], [2]], [[2], [0]]])),
+    ],
 )
 def test_category_encoding_one_hot_2D_input_should_raise(input):
     test_case = TestCase()
     schema = Schema([create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5)])
     category_encoding = mm.CategoryEncoding(schema=schema, output_mode="one_hot")
     inputs = {}
     inputs["feature"] = input
@@ -618,32 +627,31 @@
     ):
         category_encoding(inputs)
 
 
 @pytest.mark.parametrize(
     "input",
     [
-        tf.convert_to_tensor([[[1], [2]], [[2], [0]]]),
-        tf.sparse.from_dense(np.array([[[1], [2]], [[2], [0]]])),
+        tf.convert_to_tensor([0, 1, 2, 3]),
+        tf.convert_to_tensor([[[[1]]], [[[2]]], [[[2]]], [[[0]]]]),
+        tf.sparse.from_dense(np.array([[[[1]]], [[[2]]], [[[2]]], [[[0]]]])),
     ],
 )
 def test_category_encoding_should_raise_if_input_3D(input):
-    test_case = TestCase()
     schema = Schema(
         [
             create_categorical_column("feature", tags=[Tags.CATEGORICAL], num_items=5),
         ]
     )
     category_encoding = mm.CategoryEncoding(schema=schema, output_mode="multi_hot")
     inputs = {}
     inputs["feature"] = input
-    with test_case.assertRaisesRegex(
-        Exception, r"`CategoryEncoding` only accepts 1D or 2D-shaped inputs"
-    ):
+    with pytest.raises(Exception) as excinfo:
         category_encoding(inputs)
+    assert "`CategoryEncoding` only accepts 2D (batch_size,1) or 3D" in str(excinfo.value)
 
 
 def test_hashedcrossall():
     schema = Schema(
         [
             # num_items: 0, 1, 2 thus cardinality = 3
             create_categorical_column("cat1", tags=[Tags.CATEGORICAL], num_items=2),
@@ -803,30 +811,14 @@
 
         broadcast_layer = BroadcastToSequence(context_schema, sequence_schema)
         outputs = broadcast_layer(partially_masked_inputs)
 
         self.assertAllEqual(outputs["a"]._keras_mask, tf.ragged.constant([[True], [False, True]]))
         self.assertAllEqual(outputs["b"]._keras_mask, tf.ragged.constant([[True], [False, True]]))
 
-    def test_in_model(self):
-        masking_layer = tf.keras.layers.Masking(mask_value=0)
-        partially_masked_inputs = {
-            "a": tf.constant([[1], [2]]),
-            "b": masking_layer(tf.ragged.constant([[[1]], [[0], [1]]])),
-        }
-        context_schema = Schema([ColumnSchema("a")])
-        sequence_schema = Schema([ColumnSchema("b")])
-
-        broadcast_layer = BroadcastToSequence(context_schema, sequence_schema)
-        model = mm.Model(broadcast_layer, schema=context_schema + sequence_schema)
-        outputs = model(partially_masked_inputs)
-
-        self.assertAllEqual(outputs["a"]._keras_mask, tf.ragged.constant([[True], [False, True]]))
-        self.assertAllEqual(outputs["b"]._keras_mask, tf.ragged.constant([[True], [False, True]]))
-
     def test_compute_output_shape(self):
         masking_layer = tf.keras.layers.Masking(mask_value=0)
         partially_masked_inputs = {
             "a": tf.constant([[1], [2]]),
             "b": masking_layer(tf.ragged.constant([[[1]], [[0], [1]]])),
             "c": masking_layer(tf.ragged.constant([[[1, 2]], [[3, 4], [4, 5]]], ragged_rank=1)),
         }
@@ -874,15 +866,15 @@
             sequence_combiner=None,
         ),
         post=mm.BroadcastToSequence(context_schema, seq_schema),
         aggregation=None,
     )
 
     batch = mm.sample_batch(
-        sequence_testing_data, batch_size=100, include_targets=False, to_ragged=True
+        sequence_testing_data, batch_size=100, include_targets=False, prepare_features=True
     )
     input_batch = input_block(batch)
     assert set(input_batch.keys()) == set(
         ["item_id_seq", "categories", "item_age_days_norm", "user_age", "user_country"]
     )
     assert set([len(v.shape) for v in input_batch.values()]) == set([3])
     assert set([tuple(list(v.shape)[:-1]) for v in input_batch.values()]) == set(
@@ -1003,40 +995,40 @@
     input_df = input_df[sorted(input_df.columns)]
     dataset = Dataset(input_df, schema=schema)
 
     # target is passed as a string.
     loader0 = mm.Loader(dataset, batch_size=10).map(mm.ToTarget(schema, "c"))
     inputs0, targets0 = next(iter(loader0))
     assert sorted(inputs0.keys()) == ["a", "b"]
-    assert targets0.numpy().tolist() == [[3], [6]]
+    assert targets0.numpy().tolist() == [3, 6]
     assert loader0.output_schema.select_by_tag(Tags.TARGET).column_names == ["c"]
 
     # target is passed as a ColumnSchema
     target_column_schema = ColumnSchema("c", tags=[Tags.CATEGORICAL])
     assert Tags.TARGET not in target_column_schema.tags
     loader1 = mm.Loader(dataset, batch_size=10).map(mm.ToTarget(schema, target_column_schema))
     inputs1, targets1 = next(iter(loader1))
     assert sorted(inputs1.keys()) == ["a", "b"]
-    assert targets1.numpy().tolist() == [[3], [6]]
+    assert targets1.numpy().tolist() == [3, 6]
     assert loader1.output_schema.select_by_tag(Tags.TARGET).column_names == ["c"]
 
     # target is passed as a Schema
     target_schema = schema.select_by_name("c")
     assert not target_schema.select_by_tag(Tags.TARGET)
     loader2 = mm.Loader(dataset, batch_size=10).map(mm.ToTarget(schema, target_schema))
     inputs2, targets2 = next(iter(loader2))
     assert sorted(inputs2.keys()) == ["a", "b"]
-    assert targets2.numpy().tolist() == [[3], [6]]
+    assert targets2.numpy().tolist() == [3, 6]
     assert loader2.output_schema.select_by_tag(Tags.TARGET).column_names == ["c"]
 
     # target is passed as a Tag
     loader3 = mm.Loader(dataset, batch_size=10).map(mm.ToTarget(schema, Tags.ITEM))
     inputs3, targets3 = next(iter(loader3))
     assert sorted(inputs3.keys()) == ["a", "b"]
-    assert targets3.numpy().tolist() == [[3], [6]]
+    assert targets3.numpy().tolist() == [3, 6]
     assert loader3.output_schema.select_by_tag(Tags.TARGET).column_names == ["c"]
 
 
 def test_to_target_compute_output_schema():
     schema = Schema(
         [
             ColumnSchema("a", tags=[Tags.ITEM, Tags.CATEGORICAL]),
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_negative_sampling.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_negative_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import tensorflow as tf
 
 import merlin.models.tf as mm
 from merlin.io import Dataset
 from merlin.models.tf.core.prediction import Prediction
 from merlin.models.tf.transforms.negative_sampling import InBatchNegatives
 from merlin.models.tf.utils import testing_utils
+from merlin.models.tf.utils.tf_utils import calculate_batch_size_from_inputs
 from merlin.schema import ColumnSchema, Schema, Tags
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class ExampleIsTraining(tf.keras.layers.Layer):
     def call(self, inputs, training=False):
         return training
@@ -53,15 +54,15 @@
                     "user_id", tags=[Tags.USER, Tags.USER_ID, Tags.CATEGORICAL], dtype="int64"
                 ),
                 ColumnSchema("user_feature", tags=[Tags.USER, Tags.CATEGORICAL]),
                 ColumnSchema("label", tags=[Tags.TARGET]),
             ]
         )
         n_per_positive = 5
-        sampler = InBatchNegatives(schema, n_per_positive)
+        sampler = InBatchNegatives(schema, n_per_positive, prep_features=True)
 
         input_df = pd.DataFrame(
             [
                 {"user_id": 1, "item_id": 1, "item_feature": 2, "user_feature": 10, "label": 1},
                 {"user_id": 2, "item_id": 3, "item_feature": 6, "user_feature": 5, "label": 1},
             ]
         )
@@ -86,72 +87,74 @@
 
         input_user_item_pairs = user_item_pairs(input_df)
         negatives_df = output_df[len(input_df) :]
         negatives_user_item_pairs = user_item_pairs(negatives_df)
 
         assert input_user_item_pairs.intersection(negatives_user_item_pairs) == set()
 
-    def assert_outputs_batch_size(self, assert_fn, *outputs):
-        for values in zip(*outputs):
-            for value in values:
-                if isinstance(value, tuple):
-                    assert_fn(value[1].shape[0])
-                else:
-                    assert_fn(value.shape[0])
-
-    @pytest.mark.parametrize("to_dense", [True, False])
-    def test_calling_without_targets(
-        self, music_streaming_data: Dataset, to_dense: bool, tf_random_seed: int
-    ):
+    def assert_outputs_batch_size(self, assert_fn, outputs, targets=None):
+        batch_size = calculate_batch_size_from_inputs(outputs)
+        assert_fn(batch_size)
+
+        if targets is not None:
+            batch_size = calculate_batch_size_from_inputs(targets)
+            assert_fn(batch_size)
+
+    def test_calling_without_targets(self, music_streaming_data: Dataset, tf_random_seed: int):
         schema = music_streaming_data.schema
         batch_size, n_per_positive = 10, 5
         features = mm.sample_batch(
-            music_streaming_data, batch_size=batch_size, include_targets=False, to_dense=to_dense
+            music_streaming_data,
+            batch_size=batch_size,
+            include_targets=False,
+            prepare_features=True,
         )
 
         sampler = InBatchNegatives(schema, n_per_positive, seed=tf_random_seed)
 
         outputs = sampler(features).outputs
 
         def assert_fn(output_batch_size):
             assert output_batch_size == batch_size
 
-        self.assert_outputs_batch_size(assert_fn, outputs.values())
+        self.assert_outputs_batch_size(assert_fn, outputs)
 
-    @pytest.mark.parametrize("to_dense", [True, False])
-    def test_calling(self, music_streaming_data: Dataset, to_dense: bool, tf_random_seed: int):
+    def test_calling(self, music_streaming_data: Dataset, tf_random_seed: int):
         schema = music_streaming_data.schema
         batch_size, n_per_positive = 10, 5
         inputs, targets = mm.sample_batch(
-            music_streaming_data, batch_size=batch_size, include_targets=True, to_dense=to_dense
+            music_streaming_data,
+            batch_size=batch_size,
+            include_targets=True,
+            prepare_features=True,
         )
 
         sampler = InBatchNegatives(schema, 5, seed=tf_random_seed)
 
         outputs, targets = sampler(inputs, targets=targets)
 
         max_batch_size = batch_size + batch_size * n_per_positive
 
         def assert_fn(output_batch_size):
             assert batch_size < output_batch_size <= max_batch_size
 
         self.assert_outputs_batch_size(
             assert_fn,
-            outputs.values(),
-            targets.values(),
+            outputs,
+            targets,
         )
 
-    @pytest.mark.parametrize("to_dense", [True, False])
-    def test_run_when_testing(
-        self, music_streaming_data: Dataset, to_dense: bool, tf_random_seed: int
-    ):
+    def test_run_when_testing(self, music_streaming_data: Dataset, tf_random_seed: int):
         schema = music_streaming_data.schema
         batch_size, n_per_positive = 10, 5
         inputs, targets = mm.sample_batch(
-            music_streaming_data, batch_size=batch_size, include_targets=True, to_dense=to_dense
+            music_streaming_data,
+            batch_size=batch_size,
+            include_targets=True,
+            prepare_features=True,
         )
 
         sampler = InBatchNegatives(
             schema, n_per_positive, seed=tf_random_seed, run_when_testing=False
         )
 
         with_negatives = sampler(inputs, targets=targets, testing=True)
@@ -159,16 +162,16 @@
         targets = with_negatives.targets
 
         def assert_fn(output_batch_size):
             assert output_batch_size == batch_size
 
         self.assert_outputs_batch_size(
             assert_fn,
-            outputs.values(),
-            targets.values(),
+            outputs,
+            targets,
         )
 
     # The sampling layer currnetly only works correctly as part of the model when run in eager mode
     @pytest.mark.parametrize("run_eagerly", [True])
     def test_in_model(self, run_eagerly, music_streaming_data: Dataset, tf_random_seed: int):
         dataset = music_streaming_data
         schema = dataset.schema
@@ -196,21 +199,21 @@
         preds = model.predict(features)
         assert preds.shape[0] == batch_size
 
     def test_model_with_dataloader(self, music_streaming_data: Dataset, tf_random_seed: int):
         dataset = music_streaming_data
         schema = dataset.schema
 
-        add_negatives = InBatchNegatives(schema, 5, seed=tf_random_seed)
+        add_negatives = InBatchNegatives(schema, 5, seed=tf_random_seed, prep_features=True)
 
         batch_size, n_per_positive = 10, 5
         loader = mm.Loader(dataset, batch_size=batch_size)
 
         features, targets = next(loader)
-        features, targets = add_negatives(features, targets)
+        features, targets = add_negatives(features, targets=targets)
 
         expected_batch_size = batch_size + batch_size * n_per_positive
 
         assert features["item_category"].shape[0] > batch_size
         assert features["item_category"].shape[0] <= expected_batch_size
         assert all(
             f.shape[0] > batch_size and f.shape[0] <= expected_batch_size for f in features.values()
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_noise.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_noise.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
 #         replacement_rate = tf.reduce_mean(
 #             tf.cast(replaced_mask_non_padded, dtype=tf.float32)
 #         ).numpy()
 #         assert replacement_rate == pytest.approx(replacement_prob, abs=0.15)
 
 
 def test_stochastic_swap_noise_raise_exception_not_2d_item_id():
-
     s = Schema(
         [
             create_categorical_column("item_id_feat", num_items=1000, tags=[Tags.ITEM_ID]),
         ]
     )
 
     NUM_SEQS = 100
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_sequence.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_sequence.py`

 * *Files 11% similar despite different names*

```diff
@@ -81,15 +81,14 @@
     output = predict_random(batch)
     output_x, output_y = output
     output_y = output_y[target]
 
     batch_size = batch[target].shape[0]
 
     for k, v in batch.items():
-
         if k in seq_schema.column_names:
             # Check if output sequences length is smaller than input sequences length
             tf.Assert(
                 tf.reduce_all(output_x[k].row_lengths(1) < v.row_lengths(1)), [output_x[k], v]
             )
             # Check if first position of input and output sequence matches
             tf.Assert(
@@ -191,68 +190,75 @@
 
 
 @pytest.mark.parametrize("dense", [False, True])
 @pytest.mark.parametrize("target_as_dict", [False, True])
 def test_seq_mask_random_replace_embeddings(
     sequence_testing_data: Dataset, dense: bool, target_as_dict: bool
 ):
-    seq_schema = sequence_testing_data.schema.select_by_tag(Tags.SEQUENCE).select_by_name(
-        ["item_id_seq", "categories"]
-    )
+    from merlin.models.tf.transforms.sequence import ExtractMaskFromTargets
 
+    sequence_testing_data.schema = sequence_testing_data.schema.select_by_tag(
+        Tags.SEQUENCE
+    ).select_by_name(["item_id_seq", "categories"])
     target = sequence_testing_data.schema.select_by_tag(Tags.ITEM_ID).column_names[0]
-    predict_masked = mm.SequenceMaskRandom(schema=seq_schema, target=target, masking_prob=0.3)
+    predict_masked = mm.SequenceMaskRandom(
+        schema=sequence_testing_data.schema, target=target, masking_prob=0.3
+    )
 
     batch, _ = mm.sample_batch(sequence_testing_data, batch_size=8, prepare_features=False)
 
     inputs, targets = predict_masked(batch)
     targets = targets[target]
 
     emb = tf.keras.layers.Embedding(1000, 16)
-    item_id_emb_seq = emb(inputs["item_id_seq"])
+    item_id_emb_seq = emb(tf.squeeze(inputs["item_id_seq"], axis=-1))
     targets_mask = targets._keras_mask
     if dense:
         item_id_emb_seq = item_id_emb_seq.to_tensor()
         targets = targets.to_tensor()
         targets_mask = targets_mask.to_tensor()
         targets._keras_mask = targets_mask
 
     if target_as_dict:
         # Making targets different in dict, the valid one is "target2" which is 2D
         targets = {"target1": tf.ragged.constant([1, 2, 3, 4, 5, 6, 7, 8]), "target2": targets}
 
-    masked_embeddings = mm.ReplaceMaskedEmbeddings()
+    masked_embeddings = mm.SequentialBlock(ExtractMaskFromTargets(), mm.ReplaceMaskedEmbeddings())
     output = masked_embeddings(item_id_emb_seq, targets=targets, training=True)
 
     replaced_mask = tf.logical_not(tf.reduce_all(output == item_id_emb_seq, axis=2))
 
     if not dense:
         replaced_mask = replaced_mask.with_row_splits_dtype(tf.int64)
     tf.Assert(tf.reduce_all(replaced_mask == targets_mask), [])
     asserts_mlm_target_mask(replaced_mask)
 
 
 def test_replace_masked_input_embeddings_no_target():
+    from merlin.models.tf.transforms.sequence import ExtractMaskFromTargets
+
     item_id_emb_seq = tf.random.uniform((8, 10), dtype=tf.float32)
     item_id_emb_seq._keras_mask = tf.cast(
         tf.random.uniform((8,), minval=0, maxval=2, dtype=tf.int32), tf.bool
     )
     targets = None
 
-    masked_embeddings = mm.ReplaceMaskedEmbeddings()
+    masked_embeddings = mm.SequentialBlock(ExtractMaskFromTargets(), mm.ReplaceMaskedEmbeddings())
     output = masked_embeddings(item_id_emb_seq, targets=targets, training=True)
     # Checks that no input embedding was replaced, as there was no masking defined
     tf.Assert(tf.logical_not(tf.reduce_all(output == item_id_emb_seq)), [])
 
 
 def test_not_replace_unmasked_sequence_embeddings():
+    from merlin.models.tf.transforms.sequence import ExtractMaskFromTargets
+
     item_id_emb_seq = tf.random.uniform((8, 10), dtype=tf.float32)
     targets = tf.random.uniform((8, 10), dtype=tf.float32)
 
-    masked_embeddings = mm.ReplaceMaskedEmbeddings()
+    masked_embeddings = mm.SequentialBlock(ExtractMaskFromTargets(), mm.ReplaceMaskedEmbeddings())
     output = masked_embeddings(item_id_emb_seq, targets=targets, training=True)
     # Checks that no input embedding was replaced, as there was no masking defined
     tf.Assert(tf.reduce_all(output == item_id_emb_seq), [])
 
 
 def test_replace_masked_input_2d_embeddings_incompatible_2d_mask():
     item_id_emb_seq = tf.random.uniform((8, 10), dtype=tf.float32)
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/transforms/test_tensor.py` & `merlin-models-23.4.0/tests/unit/tf/transforms/test_tensor.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import tensorflow as tf
 
 import merlin.models.tf as mm
+from merlin.schema import ColumnSchema, Schema
 
 
 def test_expand_dims_same_axis():
     NUM_ROWS = 100
 
     # Creating some input sequences with padding in the end
     # (to emulate sessions with different lengths)
@@ -69,18 +70,27 @@
         "multi_hot_categ_feat": tf.RaggedTensor.from_tensor(
             tf.random.uniform((NUM_ROWS, 4), minval=1, maxval=100, dtype=tf.int32)
         ),
         "multi_hot_embedding_feat": tf.RaggedTensor.from_tensor(
             tf.random.uniform((NUM_ROWS, 4, 32), minval=1, maxval=100, dtype=tf.int32)
         ),
     }
-    list_to_dense_op = mm.ListToDense(max_seq_length=MAX_LEN)
+
+    schema = Schema(
+        [
+            ColumnSchema("cont_feat", dtype="float32").with_shape((NUM_ROWS,)),
+            ColumnSchema("multi_hot_categ_feat", dtype="int32").with_shape((NUM_ROWS, MAX_LEN)),
+            ColumnSchema("multi_hot_embedding_feat", dtype="int32").with_shape(
+                (NUM_ROWS, MAX_LEN, 32)
+            ),
+        ]
+    )
+
+    list_to_dense_op = mm.ToDense(schema)
     dense_inputs = list_to_dense_op(inputs)
-    dense_tensor = list_to_dense_op(inputs["multi_hot_embedding_feat"])
-    output_shape = list_to_dense_op.compute_output_shape(inputs["multi_hot_embedding_feat"].shape)
+    output_shapes = list_to_dense_op.compute_output_shape({k: v.shape for k, v in inputs.items()})
 
     assert inputs.keys() == dense_inputs.keys()
     assert list(dense_inputs["cont_feat"].shape) == [NUM_ROWS]
     assert list(dense_inputs["multi_hot_categ_feat"].shape) == [NUM_ROWS, MAX_LEN]
     assert list(dense_inputs["multi_hot_embedding_feat"].shape) == [NUM_ROWS, MAX_LEN, 32]
-    assert list(dense_tensor.shape) == [NUM_ROWS, MAX_LEN, 32]
-    assert list(output_shape) == [NUM_ROWS, MAX_LEN, 32]
+    assert list(output_shapes["multi_hot_embedding_feat"]) == [NUM_ROWS, MAX_LEN, 32]
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/utils/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/utils/test_batch.py` & `merlin-models-23.4.0/tests/unit/tf/utils/test_batch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,41 @@
 import pandas as pd
 import pytest
 
 import merlin.models.tf as ml
 from merlin.io import Dataset
+from merlin.models.tf.models.base import get_task_names_from_outputs
 
 
+@pytest.mark.parametrize(
+    "output_type", ["prediction_tasks_v1", "model_outputs_v2-single", "model_outputs_v2-multiple"]
+)
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_model_encode(ecommerce_data: Dataset, run_eagerly):
+def test_model_encode(ecommerce_data: Dataset, output_type: str, run_eagerly):
+    if output_type == "prediction_tasks_v1":
+        output_block = ml.PredictionTasks(ecommerce_data.schema)
+    elif output_type == "model_outputs_v2-single":
+        output_block = ml.BinaryOutput("click")
+    elif output_type == "model_outputs_v2-multiple":
+        output_block = ml.OutputBlock(ecommerce_data.schema)
+    output_task_names = get_task_names_from_outputs(output_block)
+
     model = ml.Model(
         ml.InputBlock(ecommerce_data.schema),
         ml.MLPBlock([2]),
-        ml.PredictionTasks(ecommerce_data.schema),
+        output_block,
     )
 
     model.compile(run_eagerly=run_eagerly, optimizer="adam")
     model.fit(ecommerce_data, batch_size=50, epochs=1, steps_per_epoch=1)
     data = model.batch_predict(ecommerce_data, batch_size=10)
     ddf = data.compute(scheduler="synchronous")
 
-    assert len(list(ddf.columns)) == 27
-    assert all([task in list(ddf.columns) for task in model.last.task_names])
+    assert len(list(ddf.columns)) == 26 if output_type == "model_outputs_v2-single" else 27
+    assert all([task in list(ddf.columns) for task in output_task_names])
 
 
 def test_two_tower_embedding_extraction(ecommerce_data: Dataset):
     model = ml.RetrievalModel(
         ml.TwoTowerBlock(ecommerce_data.schema, query_tower=ml.MLPBlock([2])),
         ml.ItemRetrievalTask(ecommerce_data.schema, target_name="click"),
     )
```

### Comparing `merlin-models-23.2.0/tests/unit/tf/utils/test_dataset.py` & `merlin-models-23.4.0/tests/unit/tf/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/tf/utils/test_tf_utils.py` & `merlin-models-23.4.0/tests/unit/tf/utils/test_tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/_conftest.py` & `merlin-models-23.4.0/tests/unit/torch/_conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/block/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/block/test_base.py` & `merlin-models-23.4.0/tests/unit/torch/block/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/block/test_mlp.py` & `merlin-models-23.4.0/tests/unit/torch/block/test_mlp.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/features/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/features/test_embedding.py` & `merlin-models-23.4.0/tests/unit/torch/features/test_embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/features/test_tabular.py` & `merlin-models-23.4.0/tests/unit/torch/features/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/model/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/model/test_head.py` & `merlin-models-23.4.0/tests/unit/torch/model/test_head.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/model/test_model.py` & `merlin-models-23.4.0/tests/unit/torch/model/test_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/tabular/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/tabular/test_aggregation.py` & `merlin-models-23.4.0/tests/unit/torch/tabular/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/tabular/test_tabular.py` & `merlin-models-23.4.0/tests/unit/torch/tabular/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/tabular/test_transformations.py` & `merlin-models-23.4.0/tests/unit/torch/tabular/test_transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     out = emb_module(torch_tabular_data)
 
     assert list(out["item_id"].shape) == [100, 100]
     assert list(out["categories"].shape) == [100, 64]
 
 
 def test_stochastic_swap_noise_raise_exception_not_2d_item_id():
-
     s = Schema(
         [
             create_categorical_column("item_id_feat", num_items=1000, tags=[Tags.ITEM_ID.value]),
         ]
     )
 
     NUM_SEQS = 100
```

### Comparing `merlin-models-23.2.0/tests/unit/torch/test_dataloader_utils.py` & `merlin-models-23.4.0/tests/unit/torch/test_dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/test_losses.py` & `merlin-models-23.4.0/tests/unit/torch/test_losses.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/test_public_api.py` & `merlin-models-23.4.0/tests/unit/torch/test_public_api.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/torch/utils/__init__.py` & `merlin-models-23.4.0/tests/unit/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/utils/test_schema_utils.py` & `merlin-models-23.4.0/tests/unit/utils/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.2.0/tests/unit/xgb/__init__.py` & `merlin-models-23.4.0/tests/unit/tf/horovod/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2022, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import pytest
 
-pytest.importorskip("xgboost")
+pytest.importorskip("horovod.tensorflow")
```

### Comparing `merlin-models-23.2.0/tests/unit/xgb/test_xgboost.py` & `merlin-models-23.4.0/tests/unit/xgb/test_xgboost.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 import sklearn.datasets
 import xgboost
 
-from merlin.core.dispatch import HAS_GPU
+from merlin.core.compat import HAS_GPU
 from merlin.datasets.synthetic import generate_data
 from merlin.io import Dataset
 from merlin.models.xgb import XGBoost, dataset_to_xy
 
 
 def test_without_dask_client(music_streaming_data: Dataset):
     with pytest.raises(ValueError) as exc_info:
```

### Comparing `merlin-models-23.2.0/tox.ini` & `merlin-models-23.4.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -11,72 +11,112 @@
 
 [testenv:py38-gpu]
 ; Runs in: Github Actions
 ; Runs GPU-based tests.
 deps =
     -rrequirements/test.txt
 setenv =
+    CUDA_VISIBLE_DEVICES=0
     TF_GPU_ALLOCATOR=cuda_malloc_async
-passenv =
-    CUDA_VISIBLE_DEVICES
+sitepackages=true
 commands =
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/systems.git@{posargs:main}
     python -m pytest --cov-report term --cov merlin -rxs tests/unit/
 
+[testenv:py38-multi-gpu]
+; Runs in: Github Actions
+; Runs GPU-based tests.
+allowlist_externals =
+    horovodrun
+    sh
+#deps =
+#    -rrequirements/test.txt
+passenv =
+    OPAL_PREFIX
+setenv =
+    TF_GPU_ALLOCATOR=cuda_malloc_async
+    CPATH={env:CPATH}{:}{envdir}/hugectr/include
+    LD_LIBRARY_PATH=${envdir}/hugectr/include/lib{:}/usr/local/lib/python3.8/dist-packages/tensorflow{:}{env:LD_LIBRARY_PATH}
+    LIBRARY_PATH=${envdir}/hugectr/lib{:}{env:LIBRARY_PATH}
+sitepackages=true
+commands =
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{posargs:main}
+    # TODO: Move SOK installation to ci-runner dockerfile
+    # Install SOK
+    sh examples/usecases/multi-gpu/install_sparse_operation_kit.sh {envdir}
+    # Run multi-gpu tests marked with `horovod` marker
+    horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh python -m pytest -m horovod -rxs tests/unit
+
 [testenv:py38-horovod-cpu]
 setenv =
     HOROVOD_WITH_MPI=1
     HOROVOD_WITH_TENSORFLOW=1
     PATH={env:PATH}{:}{envdir}/env/bin
     LD_LIBRARY_PATH={env:LD_LIBRARY_PATH}{:}{envdir}/env/lib
 commands =
     conda update --yes --name base --channel defaults conda
     conda env create --prefix {envdir}/env --file requirements/horovod-cpu-environment.yml --force
-    {envdir}/env/bin/python -m pip install horovod --no-cache-dir
+    {envdir}/env/bin/python -m pip install 'horovod==0.27.0' --no-cache-dir
     {envdir}/env/bin/horovodrun --check-build
     {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git
-    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git
-    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git
+    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git    
+    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git    
     {envdir}/env/bin/horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh pytest -m horovod -rxs tests/unit
 
 [testenv:py38-nvtabular-cpu]
 passenv=GIT_COMMIT
 allowlist_externals = git
 deps =
     -rrequirements/base.txt
     -rrequirements/dev.txt
 commands =
     ; the GIT_COMMIT env is the current commit of the models repo
     git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/NVTabular.git nvtabular-{env:GIT_COMMIT}
     python -m pip install --upgrade "./nvtabular-{env:GIT_COMMIT}"
     python -m pip install --upgrade -r "./nvtabular-{env:GIT_COMMIT}/requirements/test.txt"
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
-    python -m pip install .
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}    
+    python -m pip install .    
     python -m pytest nvtabular-{env:GIT_COMMIT}/tests/unit
 
 [testenv:py38-systems-cpu]
 passenv=GIT_COMMIT
 allowlist_externals = git
 deps =
     -rrequirements/base.txt
     -rrequirements/dev.txt
 commands =
-    ; the GIT_COMMIT env is the current commit of the core repo
+    ; the GIT_COMMIT env is the current commit of the models repo
     git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/systems.git systems-{env:GIT_COMMIT}
     python -m pip install --upgrade "./systems-{env:GIT_COMMIT}"
     python -m pip install --upgrade -r "./systems-{env:GIT_COMMIT}/requirements/test-cpu.txt"
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{posargs:main}
     python -m pip install .
     python -m pytest -m "not notebook" systems-{env:GIT_COMMIT}/tests/unit
 
+[testenv:py38-transformers4rec-cpu]
+passenv=GIT_COMMIT
+allowlist_externals = git
+commands =
+    ; the GIT_COMMIT env is the current commit of the models repo
+    git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/Transformers4Rec.git Transformers4Rec-{env:GIT_COMMIT}
+    python -m pip install --upgrade -r "./Transformers4Rec-{env:GIT_COMMIT}/requirements/test.txt"
+    python -m pip install --upgrade "./Transformers4Rec-{env:GIT_COMMIT}"
+    python -m pip install --no-deps git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
+    python -m pip install --no-deps git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
+    python -m pip install --no-deps .
+    python -m pytest Transformers4Rec-{env:GIT_COMMIT}/tests/unit
+
 [testenv:docs]
 ; Runs in: Github Actions
 ; Generates documentation with sphinx. There are other steps in the Github Actions workflow
 ; to publish the documentation on release.
 changedir = {toxinidir}
 deps = -rrequirements/docs.txt
        {[testenv:py38-gpu]deps}
```

### Comparing `merlin-models-23.2.0/versioneer.py` & `merlin-models-23.4.0/versioneer.py`

 * *Files identical despite different names*

