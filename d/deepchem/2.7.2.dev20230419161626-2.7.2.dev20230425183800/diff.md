# Comparing `tmp/deepchem-2.7.2.dev20230419161626.tar.gz` & `tmp/deepchem-2.7.2.dev20230425183800.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230419161626.tar", last modified: Wed Apr 19 16:16:26 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230425183800.tar", last modified: Tue Apr 25 18:38:00 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230419161626.tar` & `deepchem-2.7.2.dev20230425183800.tar`

### file list

```diff
@@ -1,287 +1,287 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.878829 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.882829 deepchem-2.7.2.dev20230419161626/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.886830 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    45861 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.890830 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    32724 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18074 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.894830 deepchem-2.7.2.dev20230419161626/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.898831 deepchem-2.7.2.dev20230419161626/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.902831 deepchem-2.7.2.dev20230419161626/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-19 16:16:14.000000 deepchem-2.7.2.dev20230419161626/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:16:26.874829 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 16:16:26.000000 deepchem-2.7.2.dev20230419161626/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-19 16:16:26.906831 deepchem-2.7.2.dev20230419161626/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-19 16:16:15.000000 deepchem-2.7.2.dev20230419161626/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.771360 deepchem-2.7.2.dev20230425183800/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 18:38:00.771360 deepchem-2.7.2.dev20230425183800/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.735360 deepchem-2.7.2.dev20230425183800/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.739359 deepchem-2.7.2.dev20230425183800/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67617 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.739359 deepchem-2.7.2.dev20230425183800/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.743360 deepchem-2.7.2.dev20230425183800/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.747360 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17552 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.747360 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17291 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.751360 deepchem-2.7.2.dev20230425183800/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9576 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48770 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.755360 deepchem-2.7.2.dev20230425183800/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.759360 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37609 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37602 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109518 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52629 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.759360 deepchem-2.7.2.dev20230425183800/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.763360 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.763360 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.763360 deepchem-2.7.2.dev20230425183800/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.767360 deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.767360 deepchem-2.7.2.dev20230425183800/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.767360 deepchem-2.7.2.dev20230425183800/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.767360 deepchem-2.7.2.dev20230425183800/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65677 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.771360 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:38:00.735360 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-25 18:38:00.000000 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-04-25 18:38:00.000000 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:38:00.000000 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-25 18:38:00.000000 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 18:38:00.000000 deepchem-2.7.2.dev20230425183800/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-25 18:38:00.771360 deepchem-2.7.2.dev20230425183800/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-25 18:37:49.000000 deepchem-2.7.2.dev20230425183800/setup.py
```

### Comparing `deepchem-2.7.2.dev20230419161626/LICENSE` & `deepchem-2.7.2.dev20230425183800/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/PKG-INFO` & `deepchem-2.7.2.dev20230425183800/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230419161626
+Version: 2.7.2.dev20230425183800
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230419161626/README.md` & `deepchem-2.7.2.dev20230425183800/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230425183800/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230425183800/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230425183800/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230425183800/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230425183800/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230425183800/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230425183800/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230425183800/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230425183800/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230425183800/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230425183800/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230425183800/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230425183800/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230425183800/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230425183800/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 except ModuleNotFoundError as e:
     logger.warning(
         f'Skipped loading some PyTorch models, missing a dependency. {e}')
 
 # Pytorch models with torch-geometric dependency
 try:
     # TODO We should clean up DMPNN and remove torch_geometric dependency during import
-    from deepchem.models.torch_models import DMPNN, DMPNNModel
+    from deepchem.models.torch_models import DMPNN, DMPNNModel, GNNModular
 except ImportError as e:
     logger.warning(
         f'Skipped loading modules with pytorch-geometric dependency, missing a dependency. {e}'
     )
 
 # Pytorch-lightning modules import
 try:
```

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1108,14 +1108,70 @@
             labels = torch.argmax(inputs.mask_edge_label, dim=1)
             loss = self.criterion(pred_edge, labels)
             return loss
 
         return loss
 
 
+class DeepGraphInfomaxLoss(Loss):
+    """
+    Loss that maximizes mutual information between local node representations and a pooled global graph representation. This is to encourage nearby nodes to have similar embeddings.
+
+    Parameters
+    ----------
+    positive_score: torch.Tensor
+        Positive score. This score measures the similarity between the local node embeddings (`node_emb`) and the global graph representation (`positive_expanded_summary_emb`) derived from the same graph.
+        The goal is to maximize this score, as it indicates that the local node embeddings and the global graph representation are highly correlated, capturing the mutual information between them.
+    negative_score: torch.Tensor
+        Negative score. This score measures the similarity between the local node embeddings (`node_emb`) and the global graph representation (`negative_expanded_summary_emb`) derived from a different graph (shifted by one position in this case).
+        The goal is to minimize this score, as it indicates that the local node embeddings and the global graph representation from different graphs are not correlated, ensuring that the model learns meaningful representations that are specific to each graph.
+
+    Examples
+    --------
+    >>> import torch
+    >>> import numpy as np
+    >>> from deepchem.feat.graph_data import GraphData
+    >>> from torch_geometric.nn import global_mean_pool
+    >>> from deepchem.models.losses import DeepGraphInfomaxLoss
+    >>> x = np.array([[1, 0], [0, 1], [1, 1], [0, 0]])
+    >>> edge_index = np.array([[0, 1, 2, 0, 3], [1, 0, 1, 3, 2]])
+    >>> graph_index = np.array([0, 0, 1, 1])
+    >>> data = GraphData(node_features=x, edge_index=edge_index, graph_index=graph_index).numpy_to_torch()
+    >>> graph_infomax_loss = DeepGraphInfomaxLoss()._create_pytorch_loss()
+    >>> # Initialize node_emb randomly
+    >>> num_nodes = data.num_nodes
+    >>> embedding_dim = 8
+    >>> node_emb = torch.randn(num_nodes, embedding_dim)
+    >>> # Compute the global graph representation
+    >>> summary_emb = global_mean_pool(node_emb, data.graph_index)
+    >>> # Compute positive and negative scores
+    >>> positive_score = torch.matmul(node_emb, summary_emb.t())
+    >>> negative_score = torch.matmul(node_emb, summary_emb.roll(1, dims=0).t())
+    >>> loss = graph_infomax_loss(positive_score, negative_score)
+
+    References
+    ----------
+    .. [1] Veličković, P. et al. Deep Graph Infomax. Preprint at https://doi.org/10.48550/arXiv.1809.10341 (2018).
+
+    """
+
+    def _create_pytorch_loss(self):
+        import torch
+        self.criterion = torch.nn.BCEWithLogitsLoss()
+
+        def loss(positive_score, negative_score):
+
+            return self.criterion(
+                positive_score,
+                torch.ones_like(positive_score)) + self.criterion(
+                    negative_score, torch.zeros_like(negative_score))
+
+        return loss
+
+
 def _make_tf_shapes_consistent(output, labels):
     """Try to make inputs have the same shape by adding dimensions of size 1."""
     import tensorflow as tf
     shape1 = output.shape
     shape2 = labels.shape
     len1 = len(shape1)
     len2 = len(shape2)
```

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/models.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/gnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import random
 import copy
 import torch
 import numpy as np
 from torch_geometric.nn import GINEConv, global_add_pool, global_mean_pool, global_max_pool
 from torch_geometric.nn.aggr import AttentionalAggregation, Set2Set
+from torch_geometric.nn.inits import uniform
+import torch.nn as nn
 from torch.functional import F
 from deepchem.data import Dataset
-from deepchem.models.losses import SoftmaxCrossEntropy, EdgePredictionLoss, GraphNodeMaskingLoss, GraphEdgeMaskingLoss
+from deepchem.models.losses import SoftmaxCrossEntropy, EdgePredictionLoss, GraphNodeMaskingLoss, GraphEdgeMaskingLoss, DeepGraphInfomaxLoss
 from deepchem.models.torch_models import ModularTorchModel
 from deepchem.feat.graph_data import BatchGraphData
 from typing import Iterable, List, Tuple
 from deepchem.metrics import to_one_hot
 
 num_node_type = 120  # including the extra mask tokens
 num_chirality_tag = 3
@@ -174,14 +176,73 @@
         pooled = self.pool(node_representation, input_batch.graph_index)
         out = self.head(pooled)
         if self.task == "classification":
             out = torch.reshape(out, (-1, self.num_tasks, self.num_classes))
         return out
 
 
+class LocalGlobalDiscriminator(nn.Module):
+    """
+    This discriminator module is a linear layer without bias, used to measure the similarity between local node representations (`x`) and global graph representations (`summary`).
+
+    The goal of the discriminator is to distinguish between positive and negative pairs of local and global representations.
+
+    Examples
+    --------
+    >>> import torch
+    >>> from deepchem.models.torch_models.gnn import LocalGlobalDiscriminator
+    >>> discriminator = LocalGlobalDiscriminator(hidden_dim=64)
+    >>> x = torch.randn(32, 64)  # Local node representations
+    >>> summary = torch.randn(32, 64)  # Global graph representations
+    >>> similarity_scores = discriminator(x, summary)
+    >>> print(similarity_scores.shape)
+    torch.Size([32])
+    """
+
+    def __init__(self, hidden_dim):
+        """
+        `self.weight` is a learnable weight matrix of shape `(hidden_dim, hidden_dim)`.
+
+        nn.Parameters are tensors that require gradients and are optimized during the training process.
+
+        Parameters
+        ----------
+        hidden_dim : int
+            The size of the hidden dimension for the weight matrix.
+
+        """
+        super().__init__()
+        self.weight = nn.Parameter(torch.Tensor(hidden_dim, hidden_dim))
+        self.reset_parameters()
+
+    def reset_parameters(self):
+        size = self.weight.size(0)
+        uniform(size, self.weight)
+
+    def forward(self, x, summary):
+        """
+        Computes the product of `summary` and `self.weight`, and then calculates the element-wise product of `x` and the resulting matrix `h`.
+        It then sums over the `hidden_dim` dimension, resulting in a tensor of shape `(batch_size,)`, which represents the similarity scores between the local and global representations.
+
+        Parameters
+        ----------
+        x : torch.Tensor
+            Local node representations of shape `(batch_size, hidden_dim)`.
+        summary : torch.Tensor
+            Global graph representations of shape `(batch_size, hidden_dim)`.
+
+        Returns
+        -------
+        torch.Tensor
+            A tensor of shape `(batch_size,)`, representing the similarity scores between the local and global representations.
+        """
+        h = torch.matmul(summary, self.weight)
+        return torch.sum(x * h, dim=1)
+
+
 class GNNModular(ModularTorchModel):
     """
     Modular GNN which allows for easy swapping of GNN layers.
 
     Parameters
     ----------
     gnn_type: str
@@ -262,14 +323,17 @@
             self.mask_rate = mask_rate
             self.mask_edge = mask_edge
             self.node_mask_loss = GraphNodeMaskingLoss()._create_pytorch_loss(
                 self.mask_edge)
         elif task == "mask_edges":
             self.mask_rate = mask_rate
             self.edge_mask_loss = GraphEdgeMaskingLoss()._create_pytorch_loss()
+        elif task == "infomax":
+            self.graph_infomax_loss = DeepGraphInfomaxLoss(
+            )._create_pytorch_loss()
 
         self.graph_pooling = graph_pooling
         self.dropout = dropout
         self.jump_knowledge = jump_knowledge
         self.task = task
 
         self.components = self.build_components()
@@ -340,15 +404,15 @@
                                                 1)  # -1 to remove mask token
             components.update({
                 'linear_pred_nodes': linear_pred_nodes,
                 'linear_pred_edges': linear_pred_edges
             })
 
         # for supervised tasks, add prediction head
-        if self.task in ("regression", "classification"):
+        elif self.task in ("regression", "classification"):
             if self.graph_pooling == "sum":
                 pool = global_add_pool
             elif self.graph_pooling == "mean":
                 pool = global_mean_pool
             elif self.graph_pooling == "max":
                 pool = global_max_pool
             elif self.graph_pooling == "attention":
@@ -379,26 +443,35 @@
             else:
                 head = torch.nn.Linear(mult * self.emb_dim, self.output_dim)
 
             components.update({'pool': pool, 'head': head})
 
             self.gnn_head = GNNHead(components['pool'], components['head'],
                                     self.task, self.num_tasks, self.num_classes)
+
+        elif self.task == 'infomax':
+            self.emb_dim = (self.num_layer + 1) * self.emb_dim
+            descrim = LocalGlobalDiscriminator(self.emb_dim)
+            components.update({
+                'discriminator': descrim,
+                'pool': global_mean_pool
+            })
+
         return components
 
     def build_model(self):
         """
         Builds the appropriate model based on the specified task.
 
         For the edge prediction task, the model is simply the GNN module because it is an unsupervised task and does not require a prediction head.
 
         Supervised tasks such as node classification and graph regression require a prediction head, so the model is a sequential module consisting of the GNN module followed by the GNN_head module.
         """
         # unsupervised tasks do not need a pred head
-        if self.task in ("edge_pred", "mask_nodes", "mask_edges"):
+        if self.task in ("edge_pred", "mask_nodes", "mask_edges", "infomax"):
             return self.gnn
         elif self.task in ("regression", "classification"):
             return torch.nn.Sequential(self.gnn, self.gnn_head)
         else:
             raise ValueError(f"Task {self.task} is not supported.")
 
     def loss_func(self, inputs, labels, weights):
@@ -408,14 +481,16 @@
         if self.task == "edge_pred":
             node_emb, inputs = self.model(inputs)
             loss = self.edge_pred_loss(node_emb, inputs)
         elif self.task == "mask_nodes":
             loss = self.masked_node_loss(inputs)
         elif self.task == "mask_edges":
             loss = self.masked_edge_loss(inputs)
+        elif self.task == "infomax":
+            loss = self.infomax_loss(inputs)
         elif self.task == "regression":
             loss = self.regression_loss(inputs, labels)
         elif self.task == "classification":
             loss = self.classification_loss(inputs, labels)
         return (loss * weights).mean()
 
     def regression_loss(self, inputs, labels):
@@ -458,14 +533,38 @@
         masked_edge_index = inputs.edge_index[:, inputs.masked_edge_idx]
         edge_emb = node_emb[masked_edge_index[0]] + node_emb[
             masked_edge_index[1]]
         pred_edge = self.components['linear_pred_edges'](edge_emb)
 
         return self.edge_mask_loss(pred_edge, inputs)
 
+    def infomax_loss(self, inputs):
+        """
+        Loss that maximizes mutual information between local node representations and a pooled global graph representation. The positive and negative scores represent the similarity between local node representations and global graph representations of simlar and dissimilar graphs, respectively.
+
+        Parameters
+        ----------
+        inputs: BatchedGraphData
+            BatchedGraphData object containing the node features, edge indices, and graph indices for the batch of graphs.
+        """
+        node_emb, inputs = self.model(inputs)
+        summary_emb = torch.sigmoid(self.components['pool'](node_emb,
+                                                            inputs.graph_index))
+        positive_expanded_summary_emb = summary_emb[inputs.graph_index]
+
+        shifted_summary_emb = summary_emb[cycle_index(len(summary_emb), 1)]
+        negative_expanded_summary_emb = shifted_summary_emb[inputs.graph_index]
+
+        positive_score = self.components['discriminator'](
+            node_emb, positive_expanded_summary_emb)
+        negative_score = self.components['discriminator'](
+            node_emb, negative_expanded_summary_emb)
+
+        return self.graph_infomax_loss(positive_score, negative_score)
+
     def _prepare_batch(self, batch):
         """
         Prepares the batch for the model by converting the GraphData numpy arrays to BatchedGraphData torch tensors and moving them to the device, then transforming the input to the appropriate format for the task.
 
         Parameters
         ----------
         batch: tuple
@@ -755,7 +854,31 @@
             (1, num_edge_feat))
     # zeros are meant to represent the masked features. This is distinct from the
     # original implementation, where the masked features are represented by 0s and
     # an additional mask feature
     # link to source: https://github.com/snap-stanford/pretrain-gnns/blob/08f126ac13623e551a396dd5e511d766f9d4f8ff/bio/util.py#L101
 
     return data
+
+
+def cycle_index(num, shift):
+    """
+    Creates a 1-dimensional tensor of integers with a specified length (`num`) and a cyclic shift (`shift`). The tensor starts with integers from `shift` to `num - 1`, and then wraps around to include integers from `0` to `shift - 1` at the end.
+
+    Parameters
+    ----------
+    num: int
+        Length of the tensor.
+    shift: int
+        Amount to shift the tensor by.
+
+    Example
+    -------
+    >>> num = 10
+    >>> shift = 3
+    >>> arr = cycle_index(num, shift)
+    >>> print(arr)
+    tensor([3, 4, 5, 6, 7, 8, 9, 0, 1, 2])
+    """
+    arr = torch.arange(num) + shift
+    arr[-shift:] = torch.arange(shift)
+    return arr
```

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/modular.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,16 @@
         self.model = model
         self.components = components
         # FIXME self.loss_func is an incorrect argument for TorchModel.loss because
         # it performs more than computing loss
         super().__init__(self.model, self.loss_func, **kwargs)
         self.model.to(self.device)
         self.components = {
-            k: v.to(self.device)
+            k: v.to(self.device) if isinstance(v, nn.Module) else v
             for k, v in self.components.items()
-            if isinstance(v, nn.Module)
         }
 
     def build_model(self) -> nn.Module:
         """Builds the final model from the components."""
         raise NotImplementedError("Subclass must define the components")
 
     def build_components(self) -> dict:
@@ -344,15 +343,16 @@
         data = {
             'model': self.model.state_dict(),
             'optimizer_state_dict': self._pytorch_optimizer.state_dict(),
             'global_step': self._global_step
         }
 
         for name, component in self.components.items():
-            data[name] = component.state_dict()
+            if hasattr(component, 'state_dict'):
+                data[name] = component.state_dict()
 
         temp_file = os.path.join(model_dir, 'temp_checkpoint.pt')
         torch.save(data, temp_file)
 
         # Rename and delete older files.
 
         paths = [
```

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230425183800/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230425183800/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230425183800/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230425183800/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230425183800/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230425183800/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230425183800/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230425183800/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230425183800/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230425183800/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230419161626
+Version: 2.7.2.dev20230425183800
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230419161626/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230425183800/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/setup.cfg` & `deepchem-2.7.2.dev20230425183800/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230419161626/setup.py` & `deepchem-2.7.2.dev20230425183800/setup.py`

 * *Files identical despite different names*

