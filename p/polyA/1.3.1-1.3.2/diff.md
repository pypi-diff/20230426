# Comparing `tmp/polyA-1.3.1.tar.gz` & `tmp/polyA-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyA-1.3.1.tar", last modified: Tue Apr 25 15:27:00 2023, max compression
+gzip compressed data, was "polyA-1.3.2.tar", last modified: Tue Apr 25 21:43:03 2023, max compression
```

## Comparing `polyA-1.3.1.tar` & `polyA-1.3.2.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      184 2023-01-05 22:25:13.102196 polyA-1.3.1/AUTHORS
--rw-r--r--   0        0        0     1452 2023-01-05 22:25:13.102506 polyA-1.3.1/LICENSE
--rw-r--r--   0        0        0      280 2023-04-25 15:06:33.414804 polyA-1.3.1/Pipfile
--rw-r--r--   0        0        0    59757 2023-04-25 15:07:09.802582 polyA-1.3.1/Pipfile.lock
--rw-r--r--   0        0        0     1048 2023-01-05 22:25:13.102937 polyA-1.3.1/README.md
--rw-r--r--   0        0        0     1617 2023-01-05 22:25:13.103018 polyA-1.3.1/benchmarks/README.md
--rw-r--r--   0        0        0       34 2023-01-05 22:25:13.103064 polyA-1.3.1/benchmarks/entrypoint.py
--rwxr-xr-x   0        0        0      625 2023-01-05 22:25:13.103112 polyA-1.3.1/benchmarks/run_benchmark.sh
--rw-r--r--   0        0        0       52 2023-01-05 22:25:13.103154 polyA-1.3.1/bld.bat
--rw-r--r--   0        0        0       26 2023-01-05 22:25:13.103196 polyA-1.3.1/build.sh
--rw-r--r--   0        0        0      634 2023-01-05 22:25:13.109405 polyA-1.3.1/docs/Makefile
--rw-r--r--   0        0        0     1060 2023-01-05 22:25:13.109474 polyA-1.3.1/docs/about.rst
--rw-r--r--   0        0        0     2098 2023-01-05 22:25:13.109533 polyA-1.3.1/docs/conf.py
--rw-r--r--   0        0        0     4225 2023-01-05 22:25:13.109604 polyA-1.3.1/docs/development.rst
--rw-r--r--   0        0        0      519 2023-01-05 22:25:13.109654 polyA-1.3.1/docs/index.rst
--rw-r--r--   0        0        0     2470 2023-01-05 22:25:13.109708 polyA-1.3.1/docs/installation.rst
--rw-r--r--   0        0        0      800 2023-01-05 22:25:13.109769 polyA-1.3.1/docs/make.bat
--rw-r--r--   0        0        0       52 2023-01-05 22:25:13.109813 polyA-1.3.1/docs/modules.rst
--rw-r--r--   0        0        0      572 2023-01-05 22:25:13.109865 polyA-1.3.1/docs/polyA.converters.rst
--rw-r--r--   0        0        0     4644 2023-01-05 22:25:13.109920 polyA-1.3.1/docs/polyA.rst
--rw-r--r--   0        0        0     9324 2023-01-05 22:25:13.110007 polyA-1.3.1/docs/running.rst
--rw-r--r--   0        0        0     1382 2023-01-05 22:25:13.110057 polyA-1.3.1/docs/tutorial.rst
--rw-r--r--   0        0        0      632 2023-01-05 22:25:13.131765 polyA-1.3.1/meta.yaml
--rw-r--r--   0        0        0      106 2023-01-05 22:25:13.131841 polyA-1.3.1/polyA/__init__.py
--rw-r--r--   0        0        0       85 2023-01-05 22:25:13.131888 polyA-1.3.1/polyA/__main__.py
--rw-r--r--   0        0        0     7010 2023-04-25 13:24:22.788641 polyA-1.3.1/polyA/_app.py
--rw-r--r--   0        0        0     8257 2023-03-03 18:42:25.156077 polyA-1.3.1/polyA/_options.py
--rw-r--r--   0        0        0    22349 2023-03-06 18:39:21.504019 polyA-1.3.1/polyA/_runners.py
--rw-r--r--   0        0        0       65 2023-04-25 14:28:16.806825 polyA-1.3.1/polyA/_version.py
--rw-r--r--   0        0        0     1510 2023-01-05 22:25:13.132253 polyA-1.3.1/polyA/alignment.py
--rw-r--r--   0        0        0     7021 2023-01-05 22:25:13.132325 polyA-1.3.1/polyA/calc_repeat_scores.py
--rw-r--r--   0        0        0     7973 2023-01-05 22:25:13.132393 polyA-1.3.1/polyA/calculate_score.py
--rw-r--r--   0        0        0    12777 2023-03-03 18:42:25.157073 polyA-1.3.1/polyA/collapse_matrices.py
--rw-r--r--   0        0        0     5366 2023-01-05 22:25:13.132555 polyA-1.3.1/polyA/confidence_cm.py
--rw-r--r--   0        0        0     1626 2023-03-03 18:42:25.157216 polyA-1.3.1/polyA/constants.py
--rw-r--r--   0        0        0        0 2023-01-05 22:25:13.132651 polyA-1.3.1/polyA/converters/__init__.py
--rw-r--r--   0        0        0     8067 2023-03-03 18:42:25.157769 polyA-1.3.1/polyA/converters/cm_to_stockholm.py
--rw-r--r--   0        0        0     7590 2023-03-03 18:42:25.157940 polyA-1.3.1/polyA/converters/rm_to_stockholm.py
--rw-r--r--   0        0        0      717 2023-01-05 22:25:13.132862 polyA-1.3.1/polyA/edges.py
--rw-r--r--   0        0        0      406 2023-01-05 22:25:13.132915 polyA-1.3.1/polyA/exceptions.py
--rw-r--r--   0        0        0     2640 2023-01-05 22:25:13.132970 polyA-1.3.1/polyA/extract_nodes.py
--rw-r--r--   0        0        0    14327 2023-03-03 18:42:25.158547 polyA-1.3.1/polyA/fill_align_matrix.py
--rw-r--r--   0        0        0     2859 2023-01-05 22:25:13.133131 polyA-1.3.1/polyA/fill_confidence_matrix.py
--rw-r--r--   0        0        0     3979 2023-01-05 22:25:13.133196 polyA-1.3.1/polyA/fill_consensus_position_matrix.py
--rw-r--r--   0        0        0     9942 2023-01-05 22:25:13.133295 polyA-1.3.1/polyA/fill_node_confidence.py
--rw-r--r--   0        0        0     5988 2023-01-05 22:25:13.133385 polyA-1.3.1/polyA/fill_path_graph.py
--rw-r--r--   0        0        0     6107 2023-03-03 18:42:25.158708 polyA-1.3.1/polyA/fill_probability_matrix.py
--rw-r--r--   0        0        0     6249 2023-01-05 22:25:13.133562 polyA-1.3.1/polyA/fill_support_matrix.py
--rw-r--r--   0        0        0     4223 2023-03-03 18:42:25.158851 polyA-1.3.1/polyA/get_path.py
--rw-r--r--   0        0        0     2393 2023-01-05 22:25:13.133704 polyA-1.3.1/polyA/lambda_provider.py
--rw-r--r--   0        0        0    10162 2023-01-05 22:25:13.133795 polyA-1.3.1/polyA/load_alignments.py
--rw-r--r--   0        0        0     3282 2023-01-05 22:25:13.133865 polyA-1.3.1/polyA/matrices.py
--rw-r--r--   0        0        0     1290 2023-04-25 13:24:32.897851 polyA-1.3.1/polyA/output.py
--rw-r--r--   0        0        0     1288 2023-01-05 22:25:13.133979 polyA-1.3.1/polyA/pad_sequences.py
--rw-r--r--   0        0        0     1945 2023-01-05 22:25:13.134036 polyA-1.3.1/polyA/performance.py
--rw-r--r--   0        0        0   346559 2023-04-25 15:16:46.419153 polyA-1.3.1/polyA/polya-soda.js
--rw-r--r--   0        0        0      627 2023-01-05 22:25:13.134087 polyA-1.3.1/polyA/print_helpers.py
--rw-r--r--   0        0        0    29413 2023-04-25 15:19:14.419694 polyA-1.3.1/polyA/printers.py
--rw-r--r--   0        0        0     1177 2023-03-03 18:42:25.159062 polyA-1.3.1/polyA/prior_counts.py
--rw-r--r--   0        0        0     6564 2023-01-05 22:25:13.134337 polyA-1.3.1/polyA/substitution_matrix.py
--rw-r--r--   0        0        0      630 2023-01-05 22:25:13.134390 polyA-1.3.1/polyA/sum_repeat_scores.py
--rw-r--r--   0        0        0     3373 2023-01-05 22:25:13.134452 polyA-1.3.1/polyA/ultra_provider.py
--rw-r--r--   0        0        0      919 2023-04-25 14:27:18.077181 polyA-1.3.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-01-05 22:25:13.218428 polyA-1.3.1/pytest.ini
--rw-r--r--   0        0        0     1368 2023-03-03 18:42:25.159194 polyA-1.3.1/requirements.txt
--rwxr-xr-x   0        0        0     1199 2023-01-05 22:25:13.218628 polyA-1.3.1/tests/RunTests.sh
--rwxr-xr-x   0        0        0     1453 2023-01-05 22:25:13.218703 polyA-1.3.1/tests/RunUltraTests.sh
--rw-r--r--   0        0        0    14909 2023-01-05 22:25:13.218805 polyA-1.3.1/tests/output_sto.txt
--rw-r--r--   0        0        0     9828 2023-01-05 22:25:13.218894 polyA-1.3.1/tests/output_to_compare_oct19.txt
--rw-r--r--   0        0        0    14764 2023-01-05 22:25:13.218997 polyA-1.3.1/tests/output_to_compare_oct29.txt
--rw-r--r--   0        0        0     7186 2023-01-05 22:25:13.219091 polyA-1.3.1/tests/test_fill_align_matrix.py
--rw-r--r--   0        0        0     3975 2023-01-05 22:25:13.219172 polyA-1.3.1/tests/test_load_alignments.py
--rwxr-xr-x   0        0        0      206 2023-04-25 14:29:30.849490 polyA-1.3.1/tool/build-runner-image.sh
--rwxr-xr-x   0        0        0      164 2023-01-05 22:25:13.219357 polyA-1.3.1/tool/push-runner-image.sh
--rwxr-xr-x   0        0        0       76 2023-01-05 22:25:13.219430 polyA-1.3.1/tool/update-docs.sh
--rw-r--r--   0        0        0     6512 2023-01-05 22:25:13.219576 polyA-1.3.1/tutorial/chr2_128348379_128354757.fa
--rw-r--r--   0        0        0   987035 2023-01-05 22:25:13.221906 polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm
--rw-r--r--   0        0        0      690 2023-01-05 22:25:13.222010 polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm.matrix
--rw-r--r--   0        0        0   491904 2023-01-05 22:25:13.222356 polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm.sto
--rw-r--r--   0        0        0     4674 2023-01-05 22:25:13.222452 polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.ultra
--rw-r--r--   0        0        0     1193 2023-01-05 22:25:13.222518 polyA-1.3.1/tutorial/polyA-tutorial.txt
--rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 polyA-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-01-05 22:25:13.102196 polyA-1.3.2/AUTHORS
+-rw-r--r--   0        0        0     1452 2023-01-05 22:25:13.102506 polyA-1.3.2/LICENSE
+-rw-r--r--   0        0        0      280 2023-04-25 15:28:50.674846 polyA-1.3.2/Pipfile
+-rw-r--r--   0        0        0    59757 2023-04-25 15:28:50.675626 polyA-1.3.2/Pipfile.lock
+-rw-r--r--   0        0        0     1048 2023-01-05 22:25:13.102937 polyA-1.3.2/README.md
+-rw-r--r--   0        0        0     1617 2023-01-05 22:25:13.103018 polyA-1.3.2/benchmarks/README.md
+-rw-r--r--   0        0        0       34 2023-01-05 22:25:13.103064 polyA-1.3.2/benchmarks/entrypoint.py
+-rwxr-xr-x   0        0        0      625 2023-01-05 22:25:13.103112 polyA-1.3.2/benchmarks/run_benchmark.sh
+-rw-r--r--   0        0        0       52 2023-01-05 22:25:13.103154 polyA-1.3.2/bld.bat
+-rw-r--r--   0        0        0       26 2023-01-05 22:25:13.103196 polyA-1.3.2/build.sh
+-rw-r--r--   0        0        0      634 2023-01-05 22:25:13.109405 polyA-1.3.2/docs/Makefile
+-rw-r--r--   0        0        0     1060 2023-01-05 22:25:13.109474 polyA-1.3.2/docs/about.rst
+-rw-r--r--   0        0        0     2098 2023-01-05 22:25:13.109533 polyA-1.3.2/docs/conf.py
+-rw-r--r--   0        0        0     4225 2023-01-05 22:25:13.109604 polyA-1.3.2/docs/development.rst
+-rw-r--r--   0        0        0      519 2023-01-05 22:25:13.109654 polyA-1.3.2/docs/index.rst
+-rw-r--r--   0        0        0     2470 2023-01-05 22:25:13.109708 polyA-1.3.2/docs/installation.rst
+-rw-r--r--   0        0        0      800 2023-01-05 22:25:13.109769 polyA-1.3.2/docs/make.bat
+-rw-r--r--   0        0        0       52 2023-01-05 22:25:13.109813 polyA-1.3.2/docs/modules.rst
+-rw-r--r--   0        0        0      572 2023-01-05 22:25:13.109865 polyA-1.3.2/docs/polyA.converters.rst
+-rw-r--r--   0        0        0     4644 2023-01-05 22:25:13.109920 polyA-1.3.2/docs/polyA.rst
+-rw-r--r--   0        0        0     9324 2023-01-05 22:25:13.110007 polyA-1.3.2/docs/running.rst
+-rw-r--r--   0        0        0     1382 2023-01-05 22:25:13.110057 polyA-1.3.2/docs/tutorial.rst
+-rw-r--r--   0        0        0      632 2023-01-05 22:25:13.131765 polyA-1.3.2/meta.yaml
+-rw-r--r--   0        0        0      106 2023-01-05 22:25:13.131841 polyA-1.3.2/polyA/__init__.py
+-rw-r--r--   0        0        0       85 2023-01-05 22:25:13.131888 polyA-1.3.2/polyA/__main__.py
+-rw-r--r--   0        0        0     7010 2023-04-25 15:28:50.675930 polyA-1.3.2/polyA/_app.py
+-rw-r--r--   0        0        0     8257 2023-03-03 18:42:25.156077 polyA-1.3.2/polyA/_options.py
+-rw-r--r--   0        0        0    22349 2023-03-06 18:39:21.504019 polyA-1.3.2/polyA/_runners.py
+-rw-r--r--   0        0        0       65 2023-04-25 20:48:11.400506 polyA-1.3.2/polyA/_version.py
+-rw-r--r--   0        0        0     1510 2023-01-05 22:25:13.132253 polyA-1.3.2/polyA/alignment.py
+-rw-r--r--   0        0        0     7021 2023-01-05 22:25:13.132325 polyA-1.3.2/polyA/calc_repeat_scores.py
+-rw-r--r--   0        0        0     7973 2023-01-05 22:25:13.132393 polyA-1.3.2/polyA/calculate_score.py
+-rw-r--r--   0        0        0    12777 2023-03-03 18:42:25.157073 polyA-1.3.2/polyA/collapse_matrices.py
+-rw-r--r--   0        0        0     5366 2023-01-05 22:25:13.132555 polyA-1.3.2/polyA/confidence_cm.py
+-rw-r--r--   0        0        0     1626 2023-03-03 18:42:25.157216 polyA-1.3.2/polyA/constants.py
+-rw-r--r--   0        0        0        0 2023-01-05 22:25:13.132651 polyA-1.3.2/polyA/converters/__init__.py
+-rw-r--r--   0        0        0     8067 2023-03-03 18:42:25.157769 polyA-1.3.2/polyA/converters/cm_to_stockholm.py
+-rw-r--r--   0        0        0     7590 2023-03-03 18:42:25.157940 polyA-1.3.2/polyA/converters/rm_to_stockholm.py
+-rw-r--r--   0        0        0      717 2023-01-05 22:25:13.132862 polyA-1.3.2/polyA/edges.py
+-rw-r--r--   0        0        0      406 2023-01-05 22:25:13.132915 polyA-1.3.2/polyA/exceptions.py
+-rw-r--r--   0        0        0     2640 2023-01-05 22:25:13.132970 polyA-1.3.2/polyA/extract_nodes.py
+-rw-r--r--   0        0        0    14327 2023-03-03 18:42:25.158547 polyA-1.3.2/polyA/fill_align_matrix.py
+-rw-r--r--   0        0        0     2859 2023-01-05 22:25:13.133131 polyA-1.3.2/polyA/fill_confidence_matrix.py
+-rw-r--r--   0        0        0     3979 2023-01-05 22:25:13.133196 polyA-1.3.2/polyA/fill_consensus_position_matrix.py
+-rw-r--r--   0        0        0     9942 2023-01-05 22:25:13.133295 polyA-1.3.2/polyA/fill_node_confidence.py
+-rw-r--r--   0        0        0     5988 2023-01-05 22:25:13.133385 polyA-1.3.2/polyA/fill_path_graph.py
+-rw-r--r--   0        0        0     6107 2023-03-03 18:42:25.158708 polyA-1.3.2/polyA/fill_probability_matrix.py
+-rw-r--r--   0        0        0     6249 2023-01-05 22:25:13.133562 polyA-1.3.2/polyA/fill_support_matrix.py
+-rw-r--r--   0        0        0     4223 2023-03-03 18:42:25.158851 polyA-1.3.2/polyA/get_path.py
+-rw-r--r--   0        0        0     2393 2023-01-05 22:25:13.133704 polyA-1.3.2/polyA/lambda_provider.py
+-rw-r--r--   0        0        0    10162 2023-01-05 22:25:13.133795 polyA-1.3.2/polyA/load_alignments.py
+-rw-r--r--   0        0        0     3282 2023-01-05 22:25:13.133865 polyA-1.3.2/polyA/matrices.py
+-rw-r--r--   0        0        0     1290 2023-04-25 15:28:50.676408 polyA-1.3.2/polyA/output.py
+-rw-r--r--   0        0        0     1288 2023-01-05 22:25:13.133979 polyA-1.3.2/polyA/pad_sequences.py
+-rw-r--r--   0        0        0     1945 2023-01-05 22:25:13.134036 polyA-1.3.2/polyA/performance.py
+-rw-r--r--   0        0        0   346559 2023-04-25 15:28:50.678796 polyA-1.3.2/polyA/polya-soda.js
+-rw-r--r--   0        0        0      627 2023-01-05 22:25:13.134087 polyA-1.3.2/polyA/print_helpers.py
+-rw-r--r--   0        0        0    29413 2023-04-25 15:28:50.679408 polyA-1.3.2/polyA/printers.py
+-rw-r--r--   0        0        0     1177 2023-03-03 18:42:25.159062 polyA-1.3.2/polyA/prior_counts.py
+-rw-r--r--   0        0        0     6564 2023-01-05 22:25:13.134337 polyA-1.3.2/polyA/substitution_matrix.py
+-rw-r--r--   0        0        0      630 2023-01-05 22:25:13.134390 polyA-1.3.2/polyA/sum_repeat_scores.py
+-rw-r--r--   0        0        0     3385 2023-04-25 20:36:58.799149 polyA-1.3.2/polyA/ultra_provider.py
+-rw-r--r--   0        0        0      919 2023-04-25 15:28:50.679633 polyA-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-01-05 22:25:13.218428 polyA-1.3.2/pytest.ini
+-rw-r--r--   0        0        0     1368 2023-03-03 18:42:25.159194 polyA-1.3.2/requirements.txt
+-rwxr-xr-x   0        0        0     1199 2023-01-05 22:25:13.218628 polyA-1.3.2/tests/RunTests.sh
+-rwxr-xr-x   0        0        0     1453 2023-01-05 22:25:13.218703 polyA-1.3.2/tests/RunUltraTests.sh
+-rw-r--r--   0        0        0    14909 2023-01-05 22:25:13.218805 polyA-1.3.2/tests/output_sto.txt
+-rw-r--r--   0        0        0     9828 2023-01-05 22:25:13.218894 polyA-1.3.2/tests/output_to_compare_oct19.txt
+-rw-r--r--   0        0        0    14764 2023-01-05 22:25:13.218997 polyA-1.3.2/tests/output_to_compare_oct29.txt
+-rw-r--r--   0        0        0     7186 2023-01-05 22:25:13.219091 polyA-1.3.2/tests/test_fill_align_matrix.py
+-rw-r--r--   0        0        0     3975 2023-01-05 22:25:13.219172 polyA-1.3.2/tests/test_load_alignments.py
+-rwxr-xr-x   0        0        0      235 2023-04-25 21:33:15.858745 polyA-1.3.2/tool/build-runner-image.sh
+-rwxr-xr-x   0        0        0      164 2023-01-05 22:25:13.219357 polyA-1.3.2/tool/push-runner-image.sh
+-rwxr-xr-x   0        0        0       76 2023-01-05 22:25:13.219430 polyA-1.3.2/tool/update-docs.sh
+-rw-r--r--   0        0        0     6512 2023-01-05 22:25:13.219576 polyA-1.3.2/tutorial/chr2_128348379_128354757.fa
+-rw-r--r--   0        0        0   987035 2023-01-05 22:25:13.221906 polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm
+-rw-r--r--   0        0        0      690 2023-01-05 22:25:13.222010 polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm.matrix
+-rw-r--r--   0        0        0   491904 2023-01-05 22:25:13.222356 polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm.sto
+-rw-r--r--   0        0        0     4674 2023-01-05 22:25:13.222452 polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.ultra
+-rw-r--r--   0        0        0     1193 2023-01-05 22:25:13.222518 polyA-1.3.2/tutorial/polyA-tutorial.txt
+-rw-r--r--   0        0        0     1667 1970-01-01 00:00:00.000000 polyA-1.3.2/PKG-INFO
```

### Comparing `polyA-1.3.1/LICENSE` & `polyA-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/Pipfile.lock` & `polyA-1.3.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/README.md` & `polyA-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/benchmarks/README.md` & `polyA-1.3.2/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/benchmarks/run_benchmark.sh` & `polyA-1.3.2/benchmarks/run_benchmark.sh`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/Makefile` & `polyA-1.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/about.rst` & `polyA-1.3.2/docs/about.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/conf.py` & `polyA-1.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/development.rst` & `polyA-1.3.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/index.rst` & `polyA-1.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/installation.rst` & `polyA-1.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/make.bat` & `polyA-1.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/polyA.converters.rst` & `polyA-1.3.2/docs/polyA.converters.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/polyA.rst` & `polyA-1.3.2/docs/polyA.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/running.rst` & `polyA-1.3.2/docs/running.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/docs/tutorial.rst` & `polyA-1.3.2/docs/tutorial.rst`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/meta.yaml` & `polyA-1.3.2/meta.yaml`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/_app.py` & `polyA-1.3.2/polyA/_app.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/_options.py` & `polyA-1.3.2/polyA/_options.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/_runners.py` & `polyA-1.3.2/polyA/_runners.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/alignment.py` & `polyA-1.3.2/polyA/alignment.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/calc_repeat_scores.py` & `polyA-1.3.2/polyA/calc_repeat_scores.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/calculate_score.py` & `polyA-1.3.2/polyA/calculate_score.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/collapse_matrices.py` & `polyA-1.3.2/polyA/collapse_matrices.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/confidence_cm.py` & `polyA-1.3.2/polyA/confidence_cm.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/constants.py` & `polyA-1.3.2/polyA/constants.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/converters/cm_to_stockholm.py` & `polyA-1.3.2/polyA/converters/cm_to_stockholm.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/converters/rm_to_stockholm.py` & `polyA-1.3.2/polyA/converters/rm_to_stockholm.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/edges.py` & `polyA-1.3.2/polyA/edges.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/extract_nodes.py` & `polyA-1.3.2/polyA/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_align_matrix.py` & `polyA-1.3.2/polyA/fill_align_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_confidence_matrix.py` & `polyA-1.3.2/polyA/fill_confidence_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_consensus_position_matrix.py` & `polyA-1.3.2/polyA/fill_consensus_position_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_node_confidence.py` & `polyA-1.3.2/polyA/fill_node_confidence.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_path_graph.py` & `polyA-1.3.2/polyA/fill_path_graph.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_probability_matrix.py` & `polyA-1.3.2/polyA/fill_probability_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/fill_support_matrix.py` & `polyA-1.3.2/polyA/fill_support_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/get_path.py` & `polyA-1.3.2/polyA/get_path.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/lambda_provider.py` & `polyA-1.3.2/polyA/lambda_provider.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/load_alignments.py` & `polyA-1.3.2/polyA/load_alignments.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/matrices.py` & `polyA-1.3.2/polyA/matrices.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/output.py` & `polyA-1.3.2/polyA/output.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/pad_sequences.py` & `polyA-1.3.2/polyA/pad_sequences.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/performance.py` & `polyA-1.3.2/polyA/performance.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/polya-soda.js` & `polyA-1.3.2/polyA/polya-soda.js`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/print_helpers.py` & `polyA-1.3.2/polyA/print_helpers.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/printers.py` & `polyA-1.3.2/polyA/printers.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/prior_counts.py` & `polyA-1.3.2/polyA/prior_counts.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/substitution_matrix.py` & `polyA-1.3.2/polyA/substitution_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/sum_repeat_scores.py` & `polyA-1.3.2/polyA/sum_repeat_scores.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/polyA/ultra_provider.py` & `polyA-1.3.2/polyA/ultra_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     start: int
     length: int
     stop: int
     position_scores: Tuple[float, ...]
 
     @staticmethod
     def from_json(json_map: Dict[str, Any]):
-        raw_scores = json_map["PositionScoreDelta"].split(":")
+        raw_scores = json_map["PositionScoreDeltas"]
         position_scores = []
         for score in raw_scores:
             if abs(float(score)) > 100:
                 position_scores.append(0.0)
                 Logger(__name__).warning(
                     """
                     Unreasonably-large score detected from ULTRA, 
@@ -90,15 +90,15 @@
         self._ultra_output_path = ultra_output_path
         self._ultra_path = ultra_path
 
     @timeit()
     def __call__(self) -> UltraOutput:
         if self._sequence_path:
             ultra_process = subprocess.run(
-                [self._ultra_path, "-ss", self._sequence_path],
+                [self._ultra_path, "--hs", "-j", "--showdelta", self._sequence_path],
                 capture_output=True,
                 text=True,
             )
 
             if ultra_process.returncode != 0:
                 raise UltraProviderException(
                     ultra_process.returncode,
```

### Comparing `polyA-1.3.1/pyproject.toml` & `polyA-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/requirements.txt` & `polyA-1.3.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/RunTests.sh` & `polyA-1.3.2/tests/RunTests.sh`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/RunUltraTests.sh` & `polyA-1.3.2/tests/RunUltraTests.sh`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/output_sto.txt` & `polyA-1.3.2/tests/output_sto.txt`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/output_to_compare_oct19.txt` & `polyA-1.3.2/tests/output_to_compare_oct19.txt`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/output_to_compare_oct29.txt` & `polyA-1.3.2/tests/output_to_compare_oct29.txt`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/test_fill_align_matrix.py` & `polyA-1.3.2/tests/test_fill_align_matrix.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tests/test_load_alignments.py` & `polyA-1.3.2/tests/test_load_alignments.py`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/chr2_128348379_128354757.fa` & `polyA-1.3.2/tutorial/chr2_128348379_128354757.fa`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm` & `polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm.matrix` & `polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm.matrix`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.cm.sto` & `polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.cm.sto`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/chr2_128348379_128354757.fa.ultra` & `polyA-1.3.2/tutorial/chr2_128348379_128354757.fa.ultra`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/tutorial/polyA-tutorial.txt` & `polyA-1.3.2/tutorial/polyA-tutorial.txt`

 * *Files identical despite different names*

### Comparing `polyA-1.3.1/PKG-INFO` & `polyA-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyA
-Version: 1.3.1
+Version: 1.3.2
 Summary: PolyA is a sequence annotation adjudicator.
 Home-page: https://github.com/TravisWheelerLab/polyA
 Author: Kaitlin Carey
 Author-email: kaitlin1.carey@umontana.edu
 Maintainer: Jack Roddy
 Maintainer-email: jroddy@arizona.edu
 Description-Content-Type: text/markdown
```

