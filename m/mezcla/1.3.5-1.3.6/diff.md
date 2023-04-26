# Comparing `tmp/mezcla-1.3.5.tar.gz` & `tmp/mezcla-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.5.tar", last modified: Wed Dec 14 06:01:12 2022, max compression
+gzip compressed data, was "mezcla-1.3.6.tar", last modified: Tue Apr 25 21:57:50 2023, max compression
```

## Comparing `mezcla-1.3.5.tar` & `mezcla-1.3.6.tar`

### file list

```diff
@@ -1,152 +1,152 @@
--rw-r--r--   0        0        0      542 2022-12-14 05:41:54.725724 mezcla-1.3.5/.coveragerc
--rw-r--r--   0        0        0     1325 2022-12-14 05:41:54.725724 mezcla-1.3.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0     1262 2022-12-14 05:41:54.725724 mezcla-1.3.5/.gitignore
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.175684 mezcla-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0      777 2022-06-03 04:33:57.175684 mezcla-1.3.5/README.txt
--rw-r--r--   0        0        0       84 2022-10-25 19:04:34.956398 mezcla-1.3.5/TODO.txt
--rwxr-xr-x   0        0        0     1927 2022-12-14 05:56:07.093355 mezcla-1.3.5/mezcla/__init__.py
--rwxr-xr-x   0        0        0    10860 2022-06-02 23:46:45.000000 mezcla-1.3.5/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    13029 2022-12-14 05:41:54.725724 mezcla-1.3.5/mezcla/audio.py
--rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.588655 mezcla-1.3.5/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25702 2022-06-03 05:22:44.104859 mezcla-1.3.5/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     7625 2022-12-14 05:41:54.725724 mezcla-1.3.5/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     8925 2022-02-01 06:41:33.000000 mezcla-1.3.5/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14338 2022-07-16 02:12:42.988675 mezcla-1.3.5/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0    22190 2022-12-14 05:41:54.729723 mezcla-1.3.5/mezcla/cut.py
--rwxr-xr-x   0        0        0     4279 2022-11-25 22:51:38.472697 mezcla-1.3.5/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    44616 2022-12-14 05:41:54.729723 mezcla-1.3.5/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2022-12-14 05:41:54.729723 mezcla-1.3.5/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2022-11-11 01:58:12.573316 mezcla-1.3.5/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12834 2021-10-26 07:06:23.000000 mezcla-1.3.5/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3608 2022-06-16 07:59:25.588655 mezcla-1.3.5/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2022-11-01 22:06:48.768053 mezcla-1.3.5/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2022-11-11 01:52:38.317145 mezcla-1.3.5/mezcla/examples/download_user_gist.py
--rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.119975 mezcla-1.3.5/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.229030 mezcla-1.3.5/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8779 2022-02-21 09:16:29.886156 mezcla-1.3.5/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2021-05-07 02:08:15.000000 mezcla-1.3.5/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0     3200 2022-11-11 01:59:16.744612 mezcla-1.3.5/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     3361 2022-11-26 07:40:43.379384 mezcla-1.3.5/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2022-09-25 01:54:34.121735 mezcla-1.3.5/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.5/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.5/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.076477 mezcla-1.3.5/mezcla/examples/plot_forest_importances.py
--rwxr-xr-x   0        0        0    12989 2021-10-16 04:41:00.000000 mezcla-1.3.5/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     1410 2022-11-01 21:46:53.985464 mezcla-1.3.5/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2022-11-01 21:38:37.296840 mezcla-1.3.5/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0     3607 2022-10-26 21:42:12.776794 mezcla-1.3.5/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     3802 2022-12-14 05:01:09.014808 mezcla-1.3.5/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     5879 2022-06-30 00:48:39.136921 mezcla-1.3.5/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.5/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.5/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32894 2022-06-02 07:16:58.000000 mezcla-1.3.5/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    31147 2022-12-14 05:41:54.729723 mezcla-1.3.5/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    32492 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.5/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17916 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    40964 2022-11-25 22:51:38.472697 mezcla-1.3.5/mezcla/main.py
--rwxr-xr-x   0        0        0     9131 2022-12-14 05:03:22.477527 mezcla-1.3.5/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2022-09-05 00:03:22.272746 mezcla-1.3.5/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0    11640 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0     9489 2022-11-27 23:19:31.521604 mezcla-1.3.5/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    13640 2022-07-11 18:13:47.564445 mezcla-1.3.5/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0      183 2022-04-08 02:22:06.000000 mezcla-1.3.5/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31436 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      828 2022-12-14 05:01:09.014808 mezcla-1.3.5/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     7053 2022-11-01 23:07:50.308605 mezcla-1.3.5/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     7012 2022-11-25 22:51:38.476697 mezcla-1.3.5/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.5/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.592656 mezcla-1.3.5/mezcla/run_bert_classifier.py
--rwxr-xr-x   0        0        0    17400 2022-10-25 19:16:24.448196 mezcla-1.3.5/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.5/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    19596 2022-10-18 15:15:14.045264 mezcla-1.3.5/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     2103 2022-09-05 00:03:22.272746 mezcla-1.3.5/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.5/mezcla/sys_version_info_hack.py
--rw-r--r--   0        0        0    49663 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/system.py
--rwxr-xr-x   0        0        0    45776 2022-07-11 18:17:58.306115 mezcla-1.3.5/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     5368 2022-11-26 07:43:32.007681 mezcla-1.3.5/mezcla/template.py
--rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.199684 mezcla-1.3.5/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      722 2022-07-11 03:52:31.719683 mezcla-1.3.5/mezcla/tests/adhoc-tests.batspp
--rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.199684 mezcla-1.3.5/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0      113 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      810 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/tests/resources/cars-len-3.txt
--rw-r--r--   0        0        0      659 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      755 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2022-12-14 05:41:54.733723 mezcla-1.3.5/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0     1152 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0       65 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      159 2022-07-27 17:44:45.918359 mezcla-1.3.5/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     4296 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     4295 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_audio.py
--rw-r--r--   0        0        0      969 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_bert_multi_classification.py
--rw-r--r--   0        0        0      834 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_bing_search.py
--rw-r--r--   0        0        0     1974 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_compute_tfidf.py
--rw-r--r--   0        0        0     2932 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_cut.py
--rw-r--r--   0        0        0     2068 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    13297 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_debug.py
--rw-r--r--   0        0        0     1030 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4290 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2868 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0     2562 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    15122 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13008 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_html_utils.py
--rw-r--r--   0        0        0      892 2022-12-14 05:41:54.737723 mezcla-1.3.5/mezcla/tests/test_kenlm_example.py
--rw-r--r--   0        0        0     1683 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     8809 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_main.py
--rw-r--r--   0        0        0     2313 2022-12-14 05:51:48.766898 mezcla-1.3.5/mezcla/tests/test_merge_files.py
--rw-r--r--   0        0        0     1291 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6565 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     2882 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_my_regex.py
--rw-r--r--   0        0        0      916 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_ngram_tfidf.py
--rw-r--r--   0        0        0      819 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_os_utils.py
--rw-r--r--   0        0        0     8095 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_pandas_sklearn.py
--rw-r--r--   0        0        0      829 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_plot_utils.py
--rw-r--r--   0        0        0      854 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2657 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_rgb_color_name.py
--rw-r--r--   0        0        0      895 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_run_albert_classifier.py
--rw-r--r--   0        0        0      930 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_run_bert_classifier.py
--rw-r--r--   0        0        0     1602 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_show_bert_representation.py
--rw-r--r--   0        0        0      878 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_simple_main_example.py
--rw-r--r--   0        0        0     2060 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_spacy_nlp.py
--rw-r--r--   0        0        0      882 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    33090 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     1769 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     3651 2022-12-14 05:41:54.741723 mezcla-1.3.5/mezcla/tests/test_text_categorizer.py
--rw-r--r--   0        0        0     7027 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7362 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    21785 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_tpo_common.py
--rw-r--r--   0        0        0      715 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_train_language_model.py
--rw-r--r--   0        0        0      725 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_train_text_categorizer.py
--rw-r--r--   0        0        0      686 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_transpose_data.py
--rwxr-xr-x   0        0        0     2859 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/test_xml_utils.py
--rw-r--r--   0        0        0      676 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/tfidf/test_corpus.py
--rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/tfidf/test_dockeyword.py
--rw-r--r--   0        0        0      688 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/tfidf/test_document.py
--rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    33271 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    22985 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    16223 2022-12-14 05:41:54.745723 mezcla-1.3.5/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.387124 mezcla-1.3.5/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0    18423 2022-07-16 02:20:12.481890 mezcla-1.3.5/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     2282 2022-07-16 02:21:08.306400 mezcla-1.3.5/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7983 2022-07-16 02:23:27.003581 mezcla-1.3.5/mezcla/tfidf/document.py
-lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.207684 mezcla-1.3.5/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
--rwxr-xr-x   0        0        0    16072 2022-07-16 02:26:31.785008 mezcla-1.3.5/mezcla/tfidf/preprocess.py
--rwxr-xr-x   0        0        0    59862 2022-12-14 05:41:54.749723 mezcla-1.3.5/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.5/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.5/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.5/mezcla/transpose_data.py
--rw-r--r--   0        0        0    12934 2022-12-14 05:52:55.717367 mezcla-1.3.5/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.5/mezcla/xml_utils.py
--rw-r--r--   0        0        0      958 2022-06-03 04:33:57.211684 mezcla-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     1659 2022-12-14 05:41:54.749723 mezcla-1.3.5/requirements.txt
--rw-r--r--   0        0        0     1162 2022-12-14 05:56:07.093355 mezcla-1.3.5/setup.py
--rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.791484 mezcla-1.3.5/temp/simple_batspp.py
--rwxr-xr-x   0        0        0      458 2022-12-14 05:41:54.749723 mezcla-1.3.5/tools/run_tests.bash
--rw-r--r--   0        0        0      567 2022-06-12 21:53:35.675247 mezcla-1.3.5/tox.ini
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0      542 2022-12-14 05:41:54.725724 mezcla-1.3.6/.coveragerc
+-rw-r--r--   0        0        0     1660 2023-04-03 16:37:03.715727 mezcla-1.3.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     1639 2023-04-03 16:37:03.715727 mezcla-1.3.6/.gitignore
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.175684 mezcla-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0      777 2022-06-03 04:33:57.175684 mezcla-1.3.6/README.txt
+-rw-r--r--   0        0        0       84 2022-10-25 19:04:34.956398 mezcla-1.3.6/TODO.txt
+-rwxr-xr-x   0        0        0     1927 2023-04-25 21:52:34.589331 mezcla-1.3.6/mezcla/__init__.py
+-rwxr-xr-x   0        0        0    10860 2022-06-02 23:46:45.000000 mezcla-1.3.6/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    13029 2022-12-14 05:41:54.725724 mezcla-1.3.6/mezcla/audio.py
+-rwxr-xr-x   0        0        0    16055 2022-06-16 07:59:25.588655 mezcla-1.3.6/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25702 2022-06-03 05:22:44.104859 mezcla-1.3.6/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     7625 2022-12-14 05:41:54.725724 mezcla-1.3.6/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     8925 2022-02-01 06:41:33.000000 mezcla-1.3.6/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14338 2022-07-16 02:12:42.988675 mezcla-1.3.6/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0    22279 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4279 2022-11-25 22:51:38.472697 mezcla-1.3.6/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    45580 2023-04-25 17:58:45.655571 mezcla-1.3.6/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2022-12-14 05:41:54.729723 mezcla-1.3.6/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0        0 2022-11-11 01:58:12.573316 mezcla-1.3.6/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12834 2021-10-26 07:06:23.000000 mezcla-1.3.6/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3608 2022-06-16 07:59:25.588655 mezcla-1.3.6/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2022-11-01 22:06:48.768053 mezcla-1.3.6/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2022-11-11 01:52:38.317145 mezcla-1.3.6/mezcla/examples/download_user_gist.py
+-rwxr-xr-x   0        0        0     6477 2022-06-09 02:23:07.119975 mezcla-1.3.6/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2022-02-20 02:05:16.229030 mezcla-1.3.6/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8779 2022-02-21 09:16:29.886156 mezcla-1.3.6/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2021-05-07 02:08:15.000000 mezcla-1.3.6/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0     3338 2023-01-27 00:16:57.067013 mezcla-1.3.6/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     3922 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2022-09-25 01:54:34.121735 mezcla-1.3.6/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2020-04-12 09:44:23.000000 mezcla-1.3.6/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2020-05-01 07:18:00.000000 mezcla-1.3.6/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2022-06-09 02:26:58.076477 mezcla-1.3.6/mezcla/examples/plot_forest_importances.py
+-rwxr-xr-x   0        0        0    12989 2021-10-16 04:41:00.000000 mezcla-1.3.6/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     1467 2023-04-03 16:37:03.715727 mezcla-1.3.6/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2022-11-01 21:38:37.296840 mezcla-1.3.6/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0     3607 2022-10-26 21:42:12.776794 mezcla-1.3.6/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     4031 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     5879 2022-06-30 00:48:39.136921 mezcla-1.3.6/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2022-03-01 08:46:55.000000 mezcla-1.3.6/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2998 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32894 2022-06-02 07:16:58.000000 mezcla-1.3.6/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    32128 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    32492 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     4708 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17916 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    41468 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/main.py
+-rwxr-xr-x   0        0        0     9131 2022-12-14 05:03:22.477527 mezcla-1.3.6/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11717 2022-09-05 00:03:22.272746 mezcla-1.3.6/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0    11640 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0     9507 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    13776 2023-04-25 18:02:39.556316 mezcla-1.3.6/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0      183 2022-04-08 02:22:06.000000 mezcla-1.3.6/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31436 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      828 2022-12-14 05:01:09.014808 mezcla-1.3.6/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     7053 2022-11-01 23:07:50.308605 mezcla-1.3.6/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     7012 2022-11-25 22:51:38.476697 mezcla-1.3.6/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40529 2022-03-01 08:46:55.000000 mezcla-1.3.6/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39613 2022-06-16 07:59:25.592656 mezcla-1.3.6/mezcla/run_bert_classifier.py
+-rwxr-xr-x   0        0        0    17400 2022-10-25 19:16:24.448196 mezcla-1.3.6/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     1508 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    19931 2023-04-03 16:37:03.719727 mezcla-1.3.6/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3011 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2021-09-30 11:10:06.000000 mezcla-1.3.6/mezcla/sys_version_info_hack.py
+-rw-r--r--   0        0        0    49992 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/system.py
+-rwxr-xr-x   0        0        0    45776 2022-07-11 18:17:58.306115 mezcla-1.3.6/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     5763 2023-04-25 17:58:45.659572 mezcla-1.3.6/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2022-06-03 04:33:57.199684 mezcla-1.3.6/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      722 2022-07-11 03:52:31.719683 mezcla-1.3.6/mezcla/tests/adhoc-tests.batspp
+-rwxr-xr-x   0        0        0     3905 2022-06-03 04:33:57.199684 mezcla-1.3.6/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0      113 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      810 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars-len-3.txt
+-rw-r--r--   0        0        0      659 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      755 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2022-12-14 05:41:54.733723 mezcla-1.3.6/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0     1152 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0       65 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/resources/word-POS.freq
+-rw-r--r--   0        0        0      254 2023-04-25 17:58:45.675574 mezcla-1.3.6/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     4296 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     4295 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0      834 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     1974 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     2932 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2068 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    13297 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     1030 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4290 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2868 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0     2562 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    15122 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13008 2022-12-14 05:41:54.737723 mezcla-1.3.6/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0      892 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     1683 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0     8809 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2313 2022-12-14 07:11:50.877858 mezcla-1.3.6/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     6565 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     2882 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0      916 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0      819 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8095 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0      829 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0      854 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2657 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0      878 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     2060 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0      882 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    33090 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     1769 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     3651 2022-12-14 05:41:54.741723 mezcla-1.3.6/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     7027 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7362 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    21785 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0      725 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0      686 2022-12-14 07:11:50.881858 mezcla-1.3.6/mezcla/tests/test_transpose_data.py
+-rwxr-xr-x   0        0        0     2859 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/test_xml_utils.py
+-rw-r--r--   0        0        0      676 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_corpus.py
+-rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_dockeyword.py
+-rw-r--r--   0        0        0      688 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_document.py
+-rw-r--r--   0        0        0      697 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    33807 2023-04-03 16:37:03.723726 mezcla-1.3.6/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    23132 2022-12-14 07:12:36.328736 mezcla-1.3.6/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    16223 2022-12-14 05:41:54.745723 mezcla-1.3.6/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2022-07-10 04:39:58.387124 mezcla-1.3.6/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0    18423 2022-07-16 02:20:12.481890 mezcla-1.3.6/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     2282 2022-07-16 02:21:08.306400 mezcla-1.3.6/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7983 2022-07-16 02:23:27.003581 mezcla-1.3.6/mezcla/tfidf/document.py
+lrwxr-xr-x   0        0        0        0 2022-06-03 04:33:57.207684 mezcla-1.3.6/mezcla/tfidf/old-version -> /home/tomohara/python/tfidf
+-rwxr-xr-x   0        0        0    16163 2023-04-25 18:35:58.058712 mezcla-1.3.6/mezcla/tfidf/preprocess.py
+-rwxr-xr-x   0        0        0    59862 2022-12-14 05:41:54.749723 mezcla-1.3.6/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5267 2022-04-12 04:31:30.000000 mezcla-1.3.6/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5098 2021-10-22 05:45:54.000000 mezcla-1.3.6/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6778 2021-09-30 12:02:57.000000 mezcla-1.3.6/mezcla/transpose_data.py
+-rw-r--r--   0        0        0    12934 2022-12-14 05:52:55.717367 mezcla-1.3.6/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2022-04-12 04:50:46.000000 mezcla-1.3.6/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      958 2022-06-03 04:33:57.211684 mezcla-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1709 2023-04-03 16:37:03.723726 mezcla-1.3.6/requirements.txt
+-rw-r--r--   0        0        0     1162 2023-04-25 21:52:34.589331 mezcla-1.3.6/setup.py
+-rwxr-xr-x   0        0        0    45023 2022-07-16 02:44:46.791484 mezcla-1.3.6/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0      458 2022-12-14 05:41:54.749723 mezcla-1.3.6/tools/run_tests.bash
+-rw-r--r--   0        0        0      567 2022-06-12 21:53:35.675247 mezcla-1.3.6/tox.ini
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 mezcla-1.3.6/PKG-INFO
```

### Comparing `mezcla-1.3.5/.coveragerc` & `mezcla-1.3.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/.gitignore` & `mezcla-1.3.6/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,58 @@
 # Rules for telling git which untracked files to ignore, mainly based on
 # file extension but also accounting for some idiosyncratic usages.
 #
 # Note:
+# - *** Please add examples when adding exclusions.
+# - ** Also Explain used for if not standard Python (e.g., tox.ini)
 # - This is shared across projects, so there might seem to be
 #   some apparently extraneous patterns included.
 # - Used to pruned 'git status' output, which gets
 #   shown during check-in's (as a sanity check).
 # - The patterns are glob-like with the extension that **/GLOB
 #   matches the glob pattern in any subdirectory.
 # - See 'man gitignore' for details.
 #
+# TODO:
+# - Address the TODO's below.
+#
 
 # Log files and listings
 # TODO: figure out how to apply to subdirs
 **/*.log
 **/*.list
 
 # Any files with leading _, except specified cases
 ## OLD: __pycache__/
 **/_*
 !**/*__init__.py
 # Likewise for trailing _'s (e.g., requirements.link_)
 **/*_
 
+# Special case
+# TODO: see why excluded by the rules
+# Workflow files (e.g., .github/workflows/tests.yml).
+!.github/**
+
 # Backup file
 **/*.bak
 **/backup/
 
 # Old or archived files
 **/old
 **/archive
 
 # Output or log-file directories
 **/log-files
 **/output-files
 **/downloads
 
 # Top level distribution dir and related
+# Note: tox support PyPi packaging
+# TODO: dist created by tox utiility???
 dist
 .tox
 
 # Idiosyncratic stuff for Tom
 #
 # ex: reempl-notes.txt
 **/*notes*txt
@@ -49,11 +61,12 @@
 # ex: usage.list.08Jan22.2
 **/*.[0-9][0-9][A-Za-z]*[0-9][0-9].*
 
 # Emacs
 TAGS
 
 # Unit test / coverage reports
+# TODO: show examples
 .pytest_cache
 **/tests/htmlcov
 .coverage
 .coverage.*
```

### Comparing `mezcla-1.3.5/LICENSE.txt` & `mezcla-1.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/README.txt` & `mezcla-1.3.6/README.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/__init__.py` & `mezcla-1.3.6/mezcla/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-__VERSION__ = '1.3.5'
+__VERSION__ = '1.3.6'
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
 PYTHON3_PLUS = (sys.version_info[0] >= 3)
```

### Comparing `mezcla-1.3.5/mezcla/analyze_tfidf.py` & `mezcla-1.3.6/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/audio.py` & `mezcla-1.3.6/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/bert_multi_classification.py` & `mezcla-1.3.6/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/bert_text_classification.py` & `mezcla-1.3.6/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/bing_search.py` & `mezcla-1.3.6/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/check_html_javascript.py` & `mezcla-1.3.6/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/compute_tfidf.py` & `mezcla-1.3.6/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/cut.py` & `mezcla-1.3.6/mezcla/cut.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,20 +410,22 @@
         # Do sanity checks
         # Note: this compares row extraction against Pandas dataframe
         ## OLD: if (self.input_stream != sys.stdin):
         if (debug.debugging() and (self.input_stream != sys.stdin)):
             debug.trace(4, "note: csv vs. pandas row count sanity check")
             ## BAD: debug.assertion(num_rows == len(du.read_csv(self.filename, delimiter=self.delimiter))
             dataframe = du.read_csv(self.filename, delimiter=self.delimiter, dialect=self.dialect)
-            df_num_rows = 1 + len(dataframe)
-            df_num_cols = len(dataframe.columns)
-            debug.trace_fmt(3, "csv dimensions: {nr}x{nc}", nr=num_rows, nc=num_cols)
-            debug.trace_fmt(3, "pandas dimensions: {nr}x{nc}", nr=df_num_rows, nc=df_num_cols)
-            debug.assertion(num_rows == df_num_rows)
-            debug.assertion(num_cols == df_num_cols)
+            debug.assertion(dataframe)
+            if dataframe:
+                df_num_rows = 1 + len(dataframe)
+                df_num_cols = len(dataframe.columns)
+                debug.trace_fmt(3, "csv dimensions: {nr}x{nc}", nr=num_rows, nc=num_cols)
+                debug.trace_fmt(3, "pandas dimensions: {nr}x{nc}", nr=df_num_rows, nc=df_num_cols)
+                debug.assertion(num_rows == df_num_rows)
+                debug.assertion(num_cols == df_num_cols)
 
         return
 
 if __name__ == '__main__':
     debug.trace_current_context()
     debug.trace_fmt(4, "Environment options: {eo}",
                     eo=system.formatted_environment_option_descriptions())
```

### Comparing `mezcla-1.3.5/mezcla/data_utils.py` & `mezcla-1.3.6/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/debug.py` & `mezcla-1.3.6/mezcla/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 import enum
 import inspect
 from itertools import zip_longest
 import logging
 import os
 from pprint import pprint
 import re
-from xml.dom.minidom import Element
+## OLD: from xml.dom.minidom import Element
 import six
 import sys
 import time
 
 # Local packages
 # note: The following redefines sys.version_info to be python3 compatible;
 # this is used in _to_utf8, which should be reworked via six-based wrappers.
@@ -265,20 +265,22 @@
                                  format(exc=sys.exc_info()))
         return
 
 
     STANDARD_TYPES = (int, float, dict, list)
     SIMPLE_TYPES = (bool, int, float, type(None), str)
     #
-    def trace_object(level, obj, label=None, show_all=None, show_private=None, show_methods_etc=None, indentation=None, pretty_print=None, max_value_len=max_trace_value_len, max_depth=0):
+    def trace_object(level, obj, label=None, show_all=None, show_private=None, show_methods_etc=None, indentation=None, pretty_print=None, max_value_len=max_trace_value_len, max_depth=0, regular_standard=False):
         """Trace out OBJ's members to stderr if at trace LEVEL or higher.
         Note: Optionally uses output LABEL, with INDENTATION, SHOWing_ALL members, and PRETTY_PRINTing.
         TODO: Use SHOW_PRIVATE to display private members and SHOW_METHODS_ETC for methods.
-        If max_depth > 0, this uses recursion to show values for instance members."""
+        Unless REGULAR_STANDARD, object like lists and dicts treated specially.
+        If MAX_DEPTH > 0, this uses recursion to show values for instance members."""
         # HACK: Members for STANDARD_TYPES omitted unless show_all.
+        # TODO: Make REGULAR_STANDARD True by default
         # Notes:
         # - This is intended for arbitrary objects, use trace_values for objects known to be lists or hashes.
         # - Support for show_private and show_methods_etc is not yet implemented (added for sake of tpo_common.py).
         # - See https://stackoverflow.com/questions/383944/what-is-a-python-equivalent-of-phps-var-dump.
         # TODO: support recursive trace; specialize show_all into show_private and show_methods
         ## OLD: print("{stmt} < {current}: {r}".format(stmt=level, current=trace_level,
         # TODO: handle tuples
@@ -313,15 +315,15 @@
         member_info = []
         try:
             member_info = inspect.getmembers(obj)
         except:
             trace_fmtd(QUITE_VERBOSE, "Warning: Problem getting member list in trace_object: {exc}",
                        exc=sys.exc_info())
         ## HACK: show standard type value as special member
-        if isinstance(obj, STANDARD_TYPES):
+        if (isinstance(obj, STANDARD_TYPES) and (not regular_standard)):
             member_info = [("(value)", obj)] + [(("__(" + m + ")__"), v) for (m, v) in member_info]
             trace_fmtd(QUITE_VERBOSE, "{ind}Special casing standard type as member {m}",
                        ind=indentation, m=member_info[0][0])
         for (member, value) in member_info:
             # If high trace level, output the value as is
             # TODO: value = clip_text(value)
             trace_fmtd(MOST_DETAILED, "{i}{m}={v}; type={t}", i=indentation, m=member, v=value, t=type(value))
@@ -342,15 +344,16 @@
                                                 re.search(r"^<.*(method|module|function).*>$", value_spec))))
             # Optionally, process recursively (TODO: make INDENT an env. option)
             if ((max_depth > 0) and include_member and (not isinstance(value, SIMPLE_TYPES))):
                 # TODO: add helper for formatting type & address (for use here and above)
                 member_type_id_label = (member + " [" + str(type(value)) + " " + hex(id(value)) + "]")
                 trace_object(level, value, label=member_type_id_label, show_all=show_all,
                              indentation=(indentation + INDENT), pretty_print=None,
-                             max_depth=(max_depth - 1), max_value_len=max_value_len)
+                             max_depth=(max_depth - 1), max_value_len=max_value_len,
+                             regular_standard=regular_standard)
                 continue
             # Otherwise, derive value spec. (trapping for various exceptions)
             ## TODO: pprint.pprint(member, stream=sys.stderr, indent=4, width=512)
             try:
                 try:
                     value_spec = format_value("%s" % ((value),), max_len=max_value_len)
                 except(TypeError, ValueError):
@@ -374,15 +377,15 @@
                     logging.debug(_to_utf8((indentation + member + ":" + value_spec)))
         trace(ALWAYS, indentation + "}")
         if para_mode_tracing:
             trace(ALWAYS, "")
         return
 
 
-    def trace_values(level, collection, label=None, indentation=None, use_repr=None):
+    def trace_values(level, collection, label=None, indentation=None, use_repr=None, max_len=None):
         """Trace out elements of array or hash COLLECTION if at trace LEVEL or higher"""
         trace_fmt(MOST_VERBOSE, "trace_values(dl, {coll}, label={lbl}, indent={ind})",
                   dl=level, lbl=label, coll=collection, ind=indentation)
         if (trace_level < level):
             return
         if para_mode_tracing:
             trace(ALWAYS, "")
@@ -405,30 +408,29 @@
         keys_iter = list(collection.keys()) if isinstance(collection, dict) else range(len(collection))
         for k in keys_iter:
             try:
                 value = format_value(_to_utf8(collection[k]))
                 if use_repr:
                     value = repr(value)
                 trace_fmtd(ALWAYS, "{ind}{k}: {v}", ind=indentation, k=k,
-                           v=value)
+                           v=format_value(value, max_len=max_len))
             except:
                 trace_fmtd(QUITE_VERBOSE, "Warning: Problem tracing item {k}",
                            k=_to_utf8(k), exc=sys.exc_info())
         trace(ALWAYS, indentation + "}")
         if para_mode_tracing:
             trace(ALWAYS, "")
         return
 
 
     def trace_expr(level, *values, **kwargs):
         """Trace each of the arguments (if at trace LEVEL or higher), using introspection
         to derive label for each expression. By default, the following format is used:
            expr1=value1; ... exprN=valueN
         Notes:
-        - Currently, the labels are not resolved properly under ipython (or Jupyter).
         - For simplicity, the values are assumed to separated by ', ' (or expression _SEP)--barebones parsing applied.
         - Use DELIM to specify delimiter; otherwise '; ' used;
           if so, NO_EOL applies to intermediate values (EOL always used at end).
         - Use USE_REPR=False to use tracing via str instead of repr.
         - Use _KW_ARG for KW_ARG in case of conflict, as in following:
           trace_expr(DETAILED, term, _term="; ")
         - Use MAX_LEN to specify maximum value length.
@@ -438,54 +440,61 @@
                   l=level, args=values, kw=kwargs, dl=trace_level)
         ## DEBUG:
         ## trace_fmt(1, "(global_trace_level:{g} < level:{l})={v}",
         ##           g=trace_level, l=level, v=(trace_level < level))
         if (trace_level < level):
             # note: Short-circuits processing to avoid errors about known problem (e.g., under ipython)
             return
-        sep = kwargs.get('sep') or kwargs.get('_sep')
-        delim = kwargs.get('delim') or kwargs.get('_delim')
-        no_eol = kwargs.get('no_eol') or kwargs.get('_no_eol')
-        use_repr = kwargs.get('use_repr') or kwargs.get('_use_repr')
-        max_len = kwargs.get('max_len') or kwargs.get('_max_len')
-        prefix = kwargs.get('prefix') or kwargs.get('_prefix')
+        # Note: checks alternative keyword first, so False ones not misintepretted
+        sep = kwargs.get('_sep') or kwargs.get('sep')
+        delim = kwargs.get('_delim') or kwargs.get('delim')
+        no_eol = kwargs.get('_no_eol') or kwargs.get('no_eol')
+        in_no_eol = no_eol
+        use_repr = kwargs.get('_use_repr') or kwargs.get('use_repr')
+        max_len = kwargs.get('_max_len') or kwargs.get('max_len')
+        prefix = kwargs.get('_prefix') or kwargs.get('prefix')
         if sep is None:
             sep = ", "
         if no_eol is None:
-            no_eol = False
+            ## OLD: no_eol = False
+            ## DEBUG: trace(7, "1")
+            no_eol = (delim == "\n")
         if delim is None:
             delim = "; "
-            no_eol = True
+            if in_no_eol is None:
+                ## DEBUG: trace(7, "2")
+                no_eol = True
         if use_repr is None:
             use_repr = True
         if prefix is None:
             prefix = ""
+        trace(8, f"sep={sep!r}, del={delim!r}, noe={no_eol}, rep={use_repr}, len={max_len}, pre={prefix}")
         # Get symbolic expressions for the values
         # TODO: handle cases split across lines
         try:
             # TODO: rework introspection following icecream (e.g., using abstract syntax tree)
             caller = inspect.stack()[1]
             ## OLD: (_frame, filename, line_number, _function, _context, _index) = caller
             (_frame, filename, line_number, _function, context, _index) = caller
-            trace(6, f"filename={filename!r}, context={context!r}")
+            trace(8, f"filename={filename!r}, context={context!r}")
             statement = read_line(filename, line_number).strip()
             if statement == MISSING_LINE:
                 ## OLD: statement = str(context).replace(")\\n']", "")
                 statement = str(context).replace("\\n']", "")
             # Extract list of argument expressions (removing optional comment)
             statement = re.sub(r"#.*$", "", statement)
             statement = re.sub(r"^\s*\S*trace_expr\s*\(", "", statement)
             # Remove trailing paren with optional semicolon
             statement = re.sub(r"\)\s*;?\s*$", "", statement)
             # Remove trailing comma (e.g., if split across lines)
             statement = re.sub(r",?\s*$", "", statement)
             # Skip first argument (level)
             ## BAD: expressions = statement.split(sep)[1:]
             expressions = re.split(", +", statement)[1:]
-            trace(7, f"expressions={expressions!r}\nvalues={values!r}")
+            trace(8, f"expressions={expressions!r}\nvalues={values!r}")
         except:
             trace_fmtd(ALWAYS, "Exception isolating expression in trace_vals: {exc}",
                        exc=sys.exc_info())
             expressions = []
         trace(level, prefix, no_eol=no_eol)
         for expression, value in zip_longest(expressions, values):
             try:
@@ -497,15 +506,16 @@
                           "Warning: Likely problem resolving expression text (try reworking trace_expr call)")
                 value_spec = format_value(repr(value) if use_repr else value,
                                           max_len=max_len)
                 trace(level, f"{expression}={value_spec}{delim}", no_eol=no_eol)
             except:
                 trace_fmtd(ALWAYS, "Exception tracing values in trace_vals: {exc}",
                        exc=sys.exc_info())            
-        if no_eol:
+        ## OLD: if no_eol:
+        if (no_eol and (delim != "\n")):
             trace(level, "", no_eol=False)
         return
 
     
     def trace_current_context(level=QUITE_DETAILED, label=None, 
                               show_methods_etc=False):
         """Traces out current context (local and global variables), with output
@@ -569,15 +579,17 @@
 
 
     def assertion(expression, message=None, assert_level=None):
         """Issue warning if EXPRESSION doesn't hold, along with optional MESSAGE
         Note:
         - This is a "soft assertion" that doesn't raise an exception (n.b., provided the test doesn't do so).
         - Currently, the expression text is not resolved properly under ipython (or Jupyter).
-        - The optional ASSERT_LEVEL overrides use of ALWAYS."""
+        - The optional ASSERT_LEVEL overrides use of ALWAYS.
+        - Uses introspection to derive text for assertion expression.
+        """
         # EX: assertion((2 + 2) != 5)
         # TODO: have streamlined version using sys.write that can be used for trace and trace_fmtd sanity checks about {}'s
         # TODO: trace out local and globals to aid in diagnosing assertion failures; ex: add automatic tarcing of variables used in the assertion expression)
         if (assert_level is None):
             assert_level = ALWAYS
         if (trace_level < assert_level):
             # note: Short-circuits processing to avoid extraneous warnings (e.g., trace_expr under ipython)
@@ -585,21 +597,23 @@
         if (not expression):
             try:
                 # Get source information for failed assertion
                 trace_fmtd(MOST_VERBOSE, "Call stack: {st}", st=inspect.stack())
                 caller = inspect.stack()[1]
                 ## OLD: (_frame, filename, line_number, _function, _context, _index) = caller
                 (_frame, filename, line_number, _function, context, _index) = caller
-                trace(6, f"filename={filename!r}, context={context!r}")
+                trace(7, f"filename={filename!r}, context={context!r}")
                 # Read statement in file and extract assertion expression
                 # TODO: handle #'s in statement proper (e.g., assertion("#" in text))
                 statement = read_line(filename, line_number).strip()
                 if statement == MISSING_LINE:
                     ## OLD: statement = str(context).replace(")\\n']", "")
                     statement = str(context).replace("\\n']", "")
+                # Format expression and message
+                # note: removes comments, along with the assertion call prefix and suffix
                 statement = re.sub("#.*$", "", statement)
                 statement = re.sub(r"^(\S*)assertion\(", "", statement)
                 expression = re.sub(r"\);?\s*$", "", statement)
                 qualification_spec = (": " + message) if message else ""
                 # Output information
                 # TODO: omit subsequent warnings
                 trace_fmtd(ALWAYS, "Assertion failed: {expr} (at {file}:{line}){qual}",
@@ -773,15 +787,15 @@
     return result
 
 
 def xor3(value1, value2, value3):
     """Whether one and only one of VALUE1, VALUE2, and VALUE3 are true"""
     ## result = (xor(value1, xor(value2m value3))
     ##           and not (bool(value1) and bool(value2) and bool(value3)))
-    num_true = sum([int(bool(v)) for v in [value1, value2, value3]])
+    num_true = sum(int(bool(v)) for v in [value1, value2, value3])
     result = (num_true == 1)
     trace_fmt(QUITE_VERBOSE, "xor3({v1}, {v2}, {v3}) => {r}",
               v1=value1, v2=value2, v3=value3, r=result)
     return result
 
 
 def init_logging():
@@ -918,16 +932,17 @@
 # Note: wrapped in function to keep things clean
 
 if __debug__:
 
     def debug_init():
         """Debug-only initialization"""
         time_start = time.time()
-        trace(DETAILED, "in debug_init()")
-        trace_expr(VERBOSE, sys.argv)
+        trace(DETAILED, f"in debug_init(); {timestamp()}")
+        trace(USUAL, " ".join(sys.argv))
+        trace_expr(DETAILED, sys.argv)
 
         # Open external file for copy of trace output
         global debug_file
         debug_filename = os.getenv("DEBUG_FILE")
         if debug_filename is not None:
             ## OLD: debug_file = open(debug_filename, mode="w", encoding="UTF-8")
             ## TEST: open unbuffered which requires binary output mode
@@ -960,23 +975,24 @@
         use_logging = _getenv_bool("USE_LOGGING", use_logging)
         enable_logging = _getenv_bool("ENABLE_LOGGING", use_logging)
         if enable_logging:
             init_logging()
         monitor_functions = _getenv_bool("MONITOR_FUNCTIONS", False)
         if monitor_functions:
             sys.setprofile(profile_function)
-        trace_expr(DETAILED, para_mode_tracing, max_trace_value_len, use_logging, enable_logging, monitor_functions)
+        trace_expr(VERBOSE, para_mode_tracing, max_trace_value_len, use_logging, enable_logging, monitor_functions)
 
         # Show additional information when detailed debugging
         # TODO: sort keys to facilate comparisons of log files
         pre = post = ""
         if para_mode_tracing:
             pre = post = "\n"
         trace_fmt(DETAILED, "{pre}environment: {{\n\t{env}\n}}{post}",
-                  env="\n\t".join([(k + ': ' + os.environ[k]) for k in sorted(dict(os.environ))]),
+                  env="\n\t".join([(k + ': ' + format_value(os.environ[k]))
+                                   for k in sorted(dict(os.environ))]),
                   pre=pre, post=post)
 
         # Likewise show additional information during verbose debug tracing
         # Note: use debug.trace_current_context() in client module to show module-specific globals like __name__
         trace_expr(VERBOSE, globals())
 
         # Register to show shuttdown time and elapsed seconds
```

### Comparing `mezcla-1.3.5/mezcla/docs/audio_uml.svg` & `mezcla-1.3.6/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.6/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.6/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.6/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/download_user_gist.py` & `mezcla-1.3.6/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.6/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.6/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/feature_importance.py` & `mezcla-1.3.6/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.6/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.6/mezcla/examples/hugging_face_speechrec.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 """Speech recognition via Hugging Face"""
 
 # Standard modules
 # TODO: import re
 
 # Intalled module
-import gradio as gr
+## OLD: import gradio as gr
 ## TODO:
 ## from transformers import pipeline
 
 # Local modules
 from mezcla import debug
 from mezcla.main import Main
 from mezcla import system
@@ -49,14 +49,20 @@
 #-------------------------------------------------------------------------------
 
 SOUND_FILE = system.getenv_text("SOUND_FILE", "fuzzy-testing-1-2-3.wav",
                                 "Audio file with speech to recognize")
 USE_INTERFACE = system.getenv_bool("USE_INTERFACE", False,
                                    "Use web-based interface via gradio")
 
+# Optionally load UI support
+gr = None
+if USE_INTERFACE:
+    import gradio as gr                 # pylint: disable=import-error
+
+
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Show simple usage if --help given
     dummy_app = Main(description=__doc__, skip_input=False, manual_input=False)
```

### Comparing `mezcla-1.3.5/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.6/mezcla/examples/hugging_face_translation.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,22 +9,23 @@
 
 """Machine translation via Hugging Face"""
 
 # Standard modules
 # TODO: import re
 
 # Intalled module
-import gradio as gr
+## OLD: import gradio as gr
 ## TODO: import transformers
 ## OLD: from transformers import pipeline
 
 # Local modules
 from mezcla import debug
 from mezcla.main import Main
 from mezcla import system
+from mezcla import glue_helpers as gh
 
 # Constants
 TL = debug.TL
 
 ## TODO:
 ## # Environment options
 ## # Notes:
@@ -42,48 +43,64 @@
                                  "Source language")
 TARGET_LANG = system.getenv_text("TARGET_LANG", TO,
                                  "Target language")
 MT_TASK = f"translation_{SOURCE_LANG}_to_{TARGET_LANG}"
 DEFAULT_MODEL = f"Helsinki-NLP/opus-mt-{SOURCE_LANG}-{TARGET_LANG}"
 MT_MODEL = system.getenv_text("MT_MODEL", DEFAULT_MODEL,
                               "Hugging Face model for MT")
+TEXT_ARG = "text"
 
 #-------------------------------------------------------------------------------
 
 TEXT_FILE = system.getenv_text("TEXT_FILE", "-",
                                "Text file to translate")
 USE_INTERFACE = system.getenv_bool("USE_INTERFACE", False,
                                    "Use web-based interface via gradio")
 
+# Optionally load UI support
+gr = None
+if USE_INTERFACE:
+    import gradio as gr                 # pylint: disable=import-error
+
+
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Show simple usage if --help given
-    dummy_app = Main(description=__doc__, skip_input=False, manual_input=False)
+    ## OLD: dummy_app = Main(description=__doc__, skip_input=False, manual_input=False)
+    dummy_app = Main(description=__doc__, skip_input=False, manual_input=True,
+                     text_options=[(TEXT_ARG, "Text to translate")])
+    debug.trace_object(5, dummy_app)
+    debug.assertion(dummy_app.parsed_args)
+    text = dummy_app.get_parsed_option(TEXT_ARG)
 
     # Get input file
     text_file = TEXT_FILE
-    if (text_file == "-"):
+    if (text is not None):
+        pass
+    elif (text_file == "-"):
         text_file = dummy_app.temp_file
         text = dummy_app.read_entire_input()
     else:
         text = system.read_file(text_file)
 
     ## TEMP:
     ## pylint: disable=import-outside-toplevel
     from transformers import pipeline
     model = pipeline(task=MT_TASK, model=MT_MODEL)
 
     if USE_INTERFACE:
         pipeline_if = gr.Interface.from_pipeline(
             model,
             title="Machine translation (MT)",
-            description="Using pipeline with default",
-            examples=[text_file])
+            ## OLD:
+            ## description="Using pipeline with default",
+            ## examples=[text_file])
+            )
         pipeline_if.launch()
     else:
         TRANSLATION_TEXT = "translation_text"
         try:
             translation = model(text)
             debug.assertion(isinstance(translation, list)
                             and (TRANSLATION_TEXT in translation[0]))
```

### Comparing `mezcla-1.3.5/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.6/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/iris.csv` & `mezcla-1.3.6/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.6/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.6/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.6/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/template.py` & `mezcla-1.3.6/mezcla/examples/template.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,8 +46,9 @@
     ## TODO:
     system.print_error("Error: Implement me!")
     return
 
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
+    debug.trace_current_context(level=TL.QUITE_DETAILED)
     main()
```

### Comparing `mezcla-1.3.5/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.6/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.6/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/extract_document_text.py` & `mezcla-1.3.6/mezcla/extract_document_text.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 TODAY_DDMMMYY = datetime.date.today().strftime("%d%b%y").lower()
 ADD_DATE = system.getenv_boolean("ADD_DATE", False)
 DEFAULT_SUFFIX = "" if (STDOUT or not ADD_DATE) else TODAY_DDMMMYY
 EXT = system.getenv_text("EXT", ".txt")
 SUFFIX = system.getenv_text("SUFFIX", DEFAULT_SUFFIX)
 USE_AFFIX = system.getenv_boolean("USE_AFFIX", False)
 FORCE = system.getenv_boolean("FORCE", False)
+EXTENSION = system.getenv_value("EXTENSION", None,
+                                "Extension of file for conversion")
 
 
 def show_usage_and_quit():
     """Show command-line usage for script and then exit"""
     ## OLD:
     ## usage = """
 ## Usage: {prog} [options] [input-dir] [output-file]
@@ -65,15 +67,17 @@
 
 
 def document_to_text(doc_filename):
     """Returns text version of document FILENAME of unspecified type"""
     text = ""
     try:
         ## OLD: text = system.from_utf8(textract.process(doc_filename))
-        text = textract.process(doc_filename).decode("UTF-8")
+        text = textract.process(doc_filename,
+                                extension=EXTENSION
+                                ).decode("UTF-8")
     except:
         debug.trace_fmtd(3, "Warning: problem converting document file {f}: {e}",
                          f=doc_filename, e=sys.exc_info())
     return text
 
 
 def main():
@@ -107,15 +111,15 @@
         text = document_to_text(filename)
         ## TODO: file_date = datetime.datetime.fromtimestamp(os.path.getmtime(filename))
         if STDOUT:
             sys.stdout.write(system.to_utf8(text) + "\n")
         else:
             new_filename = system.remove_extension(filename) + affix + EXT + suffix
             if system.non_empty_file(new_filename) and not FORCE:
-                system.print_stderr("Error: file {nf} exists".
+                system.print_stderr("Error: file {nf} exists. Use FORCE to overwrite".
                                     format(nf=new_filename))
             else:
                 system.write_file(new_filename, text)
                 print(new_filename)
 
     return
```

### Comparing `mezcla-1.3.5/mezcla/file_utils.py` & `mezcla-1.3.6/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/filter_random.py` & `mezcla-1.3.6/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/format_profile.py` & `mezcla-1.3.6/mezcla/format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/gensim_test.py` & `mezcla-1.3.6/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/glue_helpers.py` & `mezcla-1.3.6/mezcla/glue_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,23 +50,36 @@
 ## OLD: default_subtrace_level = min(tpo.USUAL, debug.get_level())
 if ALLOW_SUBCOMMAND_TRACING:
     # TODO: work out intuitive default if both SUB_DEBUG_LEVEL and ALLOW_SUBCOMMAND_TRACING specified
     default_subtrace_level = max(debug.get_level(), SUB_DEBUG_LEVEL)
 
 INDENT = "    "                          # default indentation
 
+# 
+# note: See main.py for similar support as part of Main scipt class
+FILE_BASE = system.getenv_text("FILE_BASE", "_temp",
+                               "Basename for output files including dir")
+TEMP_PREFIX = (FILE_BASE + "-")
+NTF_ARGS = {'prefix': TEMP_PREFIX,
+            'delete': not debug.detailed_debugging(),
+            ## TODO: 'suffix': "-"
+            }
+TEMP_FILE = system.getenv_text("TEMP_FILE", tempfile.NamedTemporaryFile(**NTF_ARGS).name,
+                               description="Basename for temporary files")
+
+
 #------------------------------------------------------------------------
 
 def get_temp_file(delete=None):
     """Return name of unique temporary file, optionally with DELETE"""
     # Note: delete defaults to False if detailed debugging
     # TODO: allow for overriding other options to NamedTemporaryFile
     if ((delete is None) and tpo.detailed_debugging()):
         delete = False
-    temp_file_name = tempfile.NamedTemporaryFile(delete=delete).name
+    temp_file_name = TEMP_FILE
     # HACK: get rid of double backslashes in Win32 filenames
     # ex: r'c:\\temp\\fubar' => r'c:\temp\fubar' 
     ## if os.pathsep == r'\\':
     ##     double_pathspec = os.pathsep + os.pathsep
     ##     temp_file_name = temp_file_name.replace(double_pathspec, os.pathsep)
     debug_format("get_temp_file() => {r}", 5, r=temp_file_name)
     return temp_file_name
@@ -76,14 +89,21 @@
 ##     # "Log file for stderr (e.g., for issue function)"
 ##     "TEMP_LOG_FILE", get_temp_file())
 TEMP_LOG_FILE = tpo.getenv_text("TEMP_LOG_FILE", get_temp_file() + "-log",
                                 "Log file for stderr such as for issue function")
 TEMP_SCRIPT_FILE = tpo.getenv_text("TEMP_SCRIPT_FILE", get_temp_file() + "-script",
                                    "File for command invocation")
 
+def create_temp_file(contents):
+    """Create temporary file with CONTENTS and return full path"""
+    temp_filename = get_temp_file()
+    system.write_file(temp_filename, contents)
+    debug.trace(6, "create_temp_file({contents!r}) => {temp_filename}")
+    return temp_filename
+
 
 def basename(filename, extension=None):
     """Remove directory from FILENAME along with optional EXTENSION, as with Unix basename command. Note: the period in the extension must be explicitly supplied (e.g., '.data' not 'data')"""
     # EX: basename("fubar.py", ".py") => "fubar"
     # EX: basename("fubar.py", "py") => "fubar."
     # EX: basename("/tmp/solr-4888.log", ".log") => "solr-4888"
     base = os.path.basename(filename)
@@ -170,15 +190,18 @@
                     del frame
         path = os.path.join(base_dir, path)
     debug_format("resolve_path({f}) => {p}", 4, f=filename, p=path)
     return path
 
 
 def form_path(*filenames):
-    """Wrapper around os.path.join over FILENAMEs (with tracing)"""
+    """Wrapper around os.path.join over FILENAMEs (with tracing)
+    Note: includes sanity check about absolute filenames except for first
+    """
+    debug.assertion(not any(f.startswith(os.path.sep) for f in filenames[1:]))
     path = os.path.join(*filenames)
     debug_format("form_path{f} => {p}", 6, f=tuple(filenames), p=path)
     return path
 
 
 def is_directory(path):
     """Determins wther PATH represents a directory"""
@@ -245,23 +268,25 @@
 #
 def elide(text: str, max_len=None):
     """Returns TEXT elided to at most MAX_LEN characters (with '...' used to indicate remainder). Note: intended for tracing long string."""
     # EX: elide("=" * 80, max_len=8) => "========..."
     # TODO: add support for eliding at word-boundaries
     tpo.debug_print("elide(_, _)", 8)
     debug.assertion(isinstance(text, str))
+    if text is None:
+        text = ""
     if max_len is None:
         max_len = MAX_ELIDED_TEXT_LEN
     result = text
     if (result and (len(result) > max_len)):
         result = result[:max_len] + "..."
     tpo.debug_print("elide({%s}, [{%s}]) => {%s}" % (text, max_len, result), 9)
     return result
 #
-# EX: gh.elide(None, 10) => None
+# EX: elide(None, 10) => ''
 
 def elide_values(values: list, **kwargs):
     """List version of elide [q.v.]"""
     # EX: elide_values(["1", "22", "333"], max_len=2) => ["1", "22", "33..."]
     tpo.debug_print("elide_values(_, _)", 7)
     return list(map(lambda v: elide(str(v), **kwargs),
                     values))
@@ -275,15 +300,15 @@
     global default_subtrace_level
     default_subtrace_level = 0
 
 
 def run(command, trace_level=4, subtrace_level=None, just_issue=False, **namespace):
     """Invokes COMMAND via system shell, using TRACE_LEVEL for debugging output, returning result. The command can use format-style templates, resolved from caller's namespace. The optional SUBTRACE_LEVEL sets tracing for invoked commands (default is same as TRACE_LEVEL); this works around problem with stderr not being separated, which can be a problem when tracing unit tests.
    Notes:
-   - The result includes stderr, so direct if not desired:
+   - The result includes stderr, so direct if not desired (see issue):
          gh.run("ls /tmp/fubar 2> /dev/null")
    - This is only intended for running simple commands. It would be better to create a subprocess for any complex interactions.
    - This function doesn't work fully under Win32. Tabs are not preserved, so redirect stdout to a file if needed.
    """
     # TODO: add automatic log file support as in run_script from unittest_wrapper.py
     # TODO: make sure no template markers left in command text (e.g., "tar cvfz {tar_file}")
     # EX: "root" in run("ls /")
```

### Comparing `mezcla-1.3.5/mezcla/html_utils.py` & `mezcla-1.3.6/mezcla/html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/kenlm_example.py` & `mezcla-1.3.6/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/keras_param_search.py` & `mezcla-1.3.6/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/main.py` & `mezcla-1.3.6/mezcla/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,15 @@
         if file_input_mode is None:
             file_input_mode = FILE_INPUT_MODE
         self.file_input_mode = file_input_mode
         self.newlines = newlines
         if track_pages is None:
             track_pages = TRACK_PAGES
         self.track_pages = track_pages
+        self.binary_input = kwargs.get("binary_input", False)
 
         # Setup temporary file and/or base directory
         # Note: Uses NamedTemporaryFile (hence ntf_args)
         # TODO: allow temp_base handling to be overridable by constructor options
         # TODO: reconcile with unittest_wrapper.py.get_temp_dir
         prefix = (FILE_BASE + "-")
         ntf_args = {'prefix': prefix,
@@ -243,15 +244,15 @@
         # to avoid inadvertent script processing.
         #
         if ((runtime_args is None) and (not skip_args)):
             runtime_args = sys.argv[1:]
             debug.trace(4, f"Using sys.argv[1:] for runtime args: {runtime_args}")
             if self.auto_help and not runtime_args:
                 help_arg = (USAGE_ARG if self.brief_usage else HELP_ARG)
-                debug.trace(4, f"Adding {help_arg} to command line (as per auto_help)")
+                debug.trace(4, f"FYI: Adding {help_arg} to command line (as per auto_help)")
                 runtime_args = [help_arg]
         #
         # Process special hook for converting Perl-style switches like -fu=123 to --fu=123
         # See -s option under perlrun man page for enabling this rudimentary switch parsing.
         # Note: mainly just intended for when porting Perl scripts.
         self.perl_switch_parsing = kwargs.get("perl_switch_parsing", PERL_SWITCH_PARSING)
         if self.perl_switch_parsing and runtime_args:
@@ -272,15 +273,19 @@
                     
         # Get other options
         self.program = program
         if description:
             self.description = description
         if boolean_options:
             self.boolean_options += boolean_options
-        if (VERBOSE_ARG not in [list(t)[0].lower() for t in self.boolean_options]):
+        # note: adds --verbose unless already specified (TODO: add way to disable)
+        boolean_options_proper = [t for t in self.boolean_options if isinstance(t, str)]
+        boolean_options_proper += [t[0] for t in self.boolean_options if isinstance(t, list)]
+        if (VERBOSE_ARG not in boolean_options_proper):
+            debug.trace(6, f"Adding {VERBOSE_ARG} to {self.boolean_options}")
             self.boolean_options += [(VERBOSE_ARG, "Verbose output mode")]
         if text_options:
             self.text_options = text_options
         if int_options:
             self.int_options = int_options
         if float_options:
             self.float_options = float_options
@@ -419,15 +424,15 @@
         usage_notes = self.notes
         ## OLD: if (not usage_notes and SHOW_ENV_OPTIONS):
         if (not usage_notes):
             env_opt_spec = ""
             if (SHOW_ENV_OPTIONS or (f"--{VERBOSE_ARG}" in sys.argv)):
                 env_opts = system.formatted_environment_option_descriptions(sort=True, indent=INDENT)
                 env_opt_spec = f"- Available env. options:\n{INDENT}{env_opts}"
-            elided_path = re.sub(f"^.*/", ".../", sys.argv[0])
+            elided_path = re.sub(r"^.*/", ".../", sys.argv[0])
             # note: A dash ("-") is used to indicate stdin with filename arg or to bypass usage w/o one
             # TODO1: get dash put in usage to make more explicit, such as in following:
             #     usage: main.py [-h] [--verbose] [filename] [-]
             usage_notes = ("Notes: \n"
                            + ("- Use - for filename to skip usage (i.e., a la stdin).\n" if (not self.skip_input) else "")
                            + (f"- Use \"ENV1='v1' ENV2='v2' python {elided_path} ...\" for environment options.\n")
                            + env_opt_spec)
@@ -559,15 +564,16 @@
                 if not self.multiple_files:
                     # note: check_arguments sets self.other_filenames
                     debug.trace(3, "Warning: Not opening multiple-valued filename arg")
                     debug.trace_expr(3, self.filename, self.other_filenames)
             else:
                 debug.assertion(isinstance(self.filename, str))
                 debug.assertion(os.path.exists(self.filename))
-                self.input_stream = system.open_file(self.filename)
+                mode = ("r" if (not self.binary_input) else "rb")
+                self.input_stream = system.open_file(self.filename, mode=mode)
                 debug.assertion(self.input_stream)
         if self.newlines:
             debug.trace(4, f"Changing input stream newlines from {self.input_stream.newlines!r} to {self.newlines!r}")
             ## BAD: self.input_stream.newlines = self.newlines
             ## BAD2: sys.stdin.reconfigure(newline=self.newlines)
             self.input_stream = io.TextIOWrapper(self.input_stream.buffer, encoding=self.input_stream.encoding, errors=self.input_stream.errors, newline=self.newlines, line_buffering=self.input_stream.line_buffering, write_through=self.input_stream.write_through)
             debug.trace_object(4, self.input_stream)
@@ -671,15 +677,15 @@
             self.line_num += 1
             self.raw_line = line
             if line.endswith("\n"):
                 line = line[:-1]
             debug.trace_fmt(6, "L{n}: {l}", n=self.line_num, l=line)
             if self.force_unicode:
                 line = tpo.ensure_unicode(line)
-            debug.trace(7, f"\ttype(line): {type(line)}")
+            ## TEST: debug.trace(7, f"\ttype(line): {type(line)}; offset={self.input_stream.tell()}")
             if self.track_pages:
                 for i, line_segment in enumerate(line.split(FORM_FEED)):
                     debug.trace(7, f"LS{i}: {line_segment}")
                     self.end_of_page = False
                     if i == 0:
                         self.end_of_page = (line != line_segment)
                     else:
```

### Comparing `mezcla-1.3.5/mezcla/merge_files.py` & `mezcla-1.3.6/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/merge_notes.py` & `mezcla-1.3.6/mezcla/merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/misc_utils.py` & `mezcla-1.3.6/mezcla/misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/my_regex.py` & `mezcla-1.3.6/mezcla/my_regex.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             base_trace_level = self.TRACE_LEVEL
         debug.trace_fmtd((1 + base_trace_level), "my_regex.search({r!r}, {t!r}, {f}): self={s}",
                          r=regex, t=text, f=flags, s=self)
         debug.assertion(isinstance(text, six.string_types))
         self.check_pattern(regex)
         self.match_result = re.search(regex, text, flags)
         if self.match_result:
-            debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r}", m=self.grouping(), r=regex)
+            debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r!r}", m=self.grouping(), r=regex)
         return self.match_result
 
     def match(self, regex, text, flags=0, base_trace_level=None):
         """Match REGEX to TEXT with optional FLAGS and BASE_TRACE_LEVEL (e.g., 6)"""
         ## TODO: rename as match_start for clarity; add match_all method (wrapper around fullmatch)
         if base_trace_level is None:
             base_trace_level = self.TRACE_LEVEL
@@ -150,51 +150,51 @@
         if self.match_result:
             debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r!r}", m=self.grouping(), r=regex)
         return self.match_result
 
     def get_match(self):
         """Return match result object for last search or match"""
         result = self.match_result
-        debug.trace_fmtd(self.TRACE_LEVEL, "my_regex.get_match() => {r}: self={s}",
+        debug.trace_fmtd(self.TRACE_LEVEL, "my_regex.get_match() => {r!r}: self={s}",
                          r=result, s=self)
         return result
 
     def group(self, num):
         """Return group NUM from match result from last search"""
         debug.assertion(self.match_result)
         result = self.match_result and self.match_result.group(num)
-        debug.trace_fmtd(self.TRACE_LEVEL, "my_regex.group({n}) => {r}: self={s}",
+        debug.trace_fmtd(self.TRACE_LEVEL, "my_regex.group({n}) => {r!r}: self={s}",
                          n=num, r=result, s=self)
         return result
 
     def groups(self):
         """Return all groups in match result from last search"""
         debug.assertion(self.match_result)
         result = self.match_result and self.match_result.groups()
-        debug.trace_fmt(self.TRACE_LEVEL, "my_regex.groups() => {r}: self={s}",
+        debug.trace_fmt(self.TRACE_LEVEL, "my_regex.groups() => {r!r}: self={s}",
                         r=result, s=self)
         return result
 
     def grouping(self):
         """Return groups for match result or entire matching string if no groups defined"""
         # Note: this is intended to facilitate debug tracing; see example in search method above
         result = self.match_result and (self.match_result.groups() or self.match_result.group(0))
-        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.grouping() => {r}: self={s}", r=result, s=self)
+        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.grouping() => {r!r}: self={s}", r=result, s=self)
         return result
 
     def start(self, group=0):
         """Start index for GROUP"""
         result = self.match_result and self.match_result.start(group)
-        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.start({g}) => {r}: self={s}", r=result, s=self, g=group)
+        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.start({g}) => {r!r}: self={s}", r=result, s=self, g=group)
         return result
 
     def end(self, group=0):
         """End index for GROUP"""
         result = self.match_result and self.match_result.end(group)
-        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.end({g}) => {r}: self={s}", r=result, s=self, g=group)
+        debug.trace_fmt(self.TRACE_LEVEL + 1, "my_regex.end({g}) => {r!r}: self={s}", r=result, s=self, g=group)
         return result
 
     def sub(self, pattern, replacement, string, *, count=0, flags=0):
         """Version of re.sub requiring explicit keyword parameters"""
         # Note: Explicit keywords enforced to avoid confusion
         result = re.sub(pattern, replacement, string, count, flags)
         debug.reference_var(self)
@@ -205,22 +205,22 @@
     def span(self, group=0):
         """Tuple with GROUP start and end"""
         return (self.match_result and self.match_result.span(group))
 
     def split(self, pattern, string, maxsplit=0, flags=0):
         """Use PATTERN to split STRING, optionally up to MAXSPLIT with FLAGS"""
         result = re.split(pattern, string, maxsplit, flags)
-        debug.trace_fmt(self.TRACE_LEVEL, "split{args} => {r}",
+        debug.trace_fmt(self.TRACE_LEVEL, "split{args} => {r!r}",
                         args=tuple([pattern, string, maxsplit, flags]), r=result)
         return result
     
     def findall(self, pattern, string, flags=0):
         """Use PATTERN to split STRING, optionally with specified FLAGS"""
         result = re.findall(pattern, string, flags)
-        debug.trace_fmt(self.TRACE_LEVEL, "findall{args} => {r}",
+        debug.trace_fmt(self.TRACE_LEVEL, "findall{args} => {r!r}",
                         args=tuple([pattern, string, flags]), r=result)
         return result
     
 #...............................................................................
 # Initialization
 #
 # note: creates global instance for convenience (and backward compatibility)
```

### Comparing `mezcla-1.3.5/mezcla/ngram_tfidf.py` & `mezcla-1.3.6/mezcla/ngram_tfidf.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 from mezcla import debug
 from mezcla import system
 from mezcla import tpo_common as tpo
 from mezcla import tfidf
 from mezcla.compute_tfidf import terms_overlap
 from mezcla.tfidf.corpus import Corpus as tfidf_corpus
 from mezcla.tfidf.preprocess import Preprocessor as tfidf_preprocessor
+from mezcla.tfidf import preprocess as tfidf_preprocess
 
 PREPROCESSOR_LANG = system.getenv_text("PREPROCESSOR_LANG", "english",
                                        "Language for ngram preprocessor")
 # NOTE: MIN_NGRAM_SIZE (e.g., 2) is alternative to deprecated ALL_NGRAMS (implies 1)
 MAX_NGRAM_SIZE = system.getenv_int("MAX_NGRAM_SIZE", 4)
 # TODO: add descriptions to all getenv options
 MIN_NGRAM_SIZE = system.getenv_int("MIN_NGRAM_SIZE", 2)
@@ -54,15 +55,16 @@
 IDF_WEIGHTING = system.getenv_text("IDF_WEIGHTING", DEFAULT_IDF_WEIGHTING)
 MAX_TERMS = system.getenv_int("MAX_TERMS", 100)
 ALLOW_NGRAM_SUBSUMPTION = system.getenv_boolean("ALLOW_NGRAM_SUBSUMPTION", False,
                                                 "Allow ngram subsumed by another--substring")
 ALLOW_NGRAM_OVERLAP = system.getenv_boolean("ALLOW_NGRAM_OVERLAP", False,
                                             "Allows ngrams to overlap--token boundariese")
 ALLOW_NUMERIC_NGRAMS = system.getenv_boolean("ALLOW_NUMERIC_NGRAMS", False)
-DEFAULT_USE_CORPUS_COUNTER = (not tfidf_preprocessor.USE_SKLEARN_COUNTER)
+## OLD: DEFAULT_USE_CORPUS_COUNTER = (not tfidf_preprocessor.USE_SKLEARN_COUNTER)
+DEFAULT_USE_CORPUS_COUNTER = (not tfidf_preprocess.USE_SKLEARN_COUNTER)
 USE_CORPUS_COUNTER = system.getenv_boolean("USE_CORPUS_COUNTER", DEFAULT_USE_CORPUS_COUNTER,
                                            "Use slow tfidf package ngram tabulation")
 
 try:
     # Note major and minor revision values are assumed to be integral
     major_minor = re.sub(r"^(\d+\.\d+).*", r"\1", tfidf.__version__)
     TFIDF_VERSION = float(major_minor)
```

### Comparing `mezcla-1.3.5/mezcla/pandas_sklearn.py` & `mezcla-1.3.6/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/plot_utils.py` & `mezcla-1.3.6/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/randomize_lines.py` & `mezcla-1.3.6/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/rgb_color_name.py` & `mezcla-1.3.6/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/run_albert_classifier.py` & `mezcla-1.3.6/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/run_bert_classifier.py` & `mezcla-1.3.6/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/show_bert_representation.py` & `mezcla-1.3.6/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/simple_main_example.py` & `mezcla-1.3.6/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/spacy_nlp.py` & `mezcla-1.3.6/mezcla/spacy_nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,36 +277,40 @@
                     debug.trace_fmt(4, "dir(scispacy): {d}", d=dir(scispacy))
                 exec("import " + self.spacy_model)  # pylint: disable=exec-used
                 debug.trace_fmt(4, "dir({m}): {d}", m=self.spacy_model, d=eval("dir(" + self.spacy_model + ")"))
                 self.nlp = eval(self.spacy_model + ".load()")
             except:
                 system.print_stderr("Problem with alternative load of model {m}: {exc}",
                                     m=self.spacy_model, exc=system.get_exception())
+        debug.assertion(self.nlp)
 
         # Disable pipeline components not needed
         unused = ["parser", "tok2vec"]
         if not self.run_ner:
             unused.append("ner")
         for component in unused:
-            self.nlp.disable_pipe(component)
+            try:
+                self.nlp.disable_pipe(component)
+            except:
+                system.print_exception_info(f"disable Spacy pipe component {component}")
         debug.trace(4, f"Pipeline components: {[x[0] for x in self.nlp.pipeline]}")
 
         # Load in optional SpaCy components
         if USE_PYSBD:
             ## TODO: self.nlp.add_pipe(PySBDFactory(self.nlp))
             self.nlp.add_pipe("pysbd_sentence_boundaries", before="parser")
         elif USE_NLTK:
             self.nlp.add_pipe("nltk_sentence_boundaries", before="parser")
         else:
             debug.assertion(SENT_TOKENIZER.lower() == "spacy")
             # Note: senticize is implicitly used when parser enabled
             self.nlp.add_pipe("sentencizer")
                 
         # Sanity checks
-        debug.assertion(self.nlp)
+        ## OLD: debug.assertion(self.nlp)
         debug.assertion(self.type_prefix != self.entity_delim)
                 
         debug.trace_object(5, self, label="Script instance")
 
 
     def get_entity_spec(self):
         """Return the named entities tagged in the input as string list of typed entities"""
@@ -350,15 +354,15 @@
         ## self.doc = self.nlp(re.sub(r"\S", " ", line))
         line = (re.sub(r"\s", " ", line))
         self.doc = self.nlp(line)
         debug.trace_object(7, self.doc, "doc")
         if self.verbose:
             line_text = re.sub(r"\r?\n", " <newline> ", line)
             print(f"input: {line_text}")
-        if TRACK_PAGES:
+        if TRACK_PAGES and self.verbose:
             print("location info (page/sentence):")
         self.sent_num = 0
         for s in self.doc.sents:
             if (str(s) != "\n"):
                 self.sent_num += 1
                 self.process_sentence(s)
             else:
@@ -373,15 +377,18 @@
             debug.trace_fmtd(5, "Ignoring empty sentence")
             return
         sent_info = self.doc[sentence.start: sentence.end]
         if TRACK_PAGES:
             # Notes: Paragraph numbers are relative to each page; and, likewise
             # sentence numbers are relative to each paragraph.
             # See process_line and Main.read_input.
-            print(f"Pg#{self.page_num}/Sent#{self.sent_num}: {sentence_text}")
+            ## OLD: print(f"Pg#{self.page_num}/Sent#{self.sent_num}: {sentence_text}")
+            if self.verbose:
+                print(f"Pg#{self.page_num}/Sent#{self.sent_num}: ", end="")
+            print(sentence_text)
             debug.trace(4, f"Offset: {self.char_offset}")
 
         # Show synopsis of word token representations
         # TODO: have options for specifying attributes to show
         if self.show_representation:
             # Gather the word (lexeme) information
             # Note: Based on vocab/lexemes section of https://spacy.io/usage/spacy-101
```

### Comparing `mezcla-1.3.5/mezcla/spell.py` & `mezcla-1.3.6/mezcla/spell.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,75 +1,98 @@
 #! /usr/bin/env python
 #
 # spell.py: simple spell checker (e.g., via Enchant module)
 #
+# Note:
+# - New languages can be added as follows:
+#       sudo apt-get install myspell-ID
+#   See https://stackoverflow.com/questions/32712557/pyenchant-italian-and-spanish-languages.
+#
 # TODO:
 # - integrate code for suggestions based on spelling distance
 #
 
 """Basic spell checking"""
 
 # Standard modules
 # TODO: sys => system
 import sys
 import fileinput
 
 # Installed modules
-import enchant			# spell checking
+import enchant                  # spell checking
 
 # Local modules
 from mezcla import debug
 ## TODO: from mezcla.main import Main
-## TODO: from mezcla import system
+from mezcla import system
 ## OLD: from mezcla.my_regex import my_re
 from mezcla.text_processing import split_word_tokens
 
+
+# Environment options
+SPELL_LANG = system.getenv_text("SPELL_LANG", "en_US",
+                                "Language for spelling")
+
+# Constants
+TL = debug.TL
+
 ## TEMP:
 # pylint: disable=consider-using-f-string
 
-# Process command line
-# TODO: upgrade to using Main script (see template.py)
-i = 1
-show_usage = (i == len(sys.argv))
-while (i < len(sys.argv)) and (sys.argv[i][0] == "-"):
-    if (sys.argv[i] == "--help"):
-        show_usage = True
-    elif (sys.argv[i] == "-"):
-        pass
-    else:
-        print("Error: unexpected argument '%s'" % sys.argv[i])
-        show_usage = True
-    i += 1
-if (show_usage):
-    print("Usage: %s [options] input-file" % sys.argv[0])
-    print("")
-    print("Options: [--help]")
-    print("")
-    print("Examples:")
-    print("")
-    print("  %s query-keywords.list" % sys.argv[0])
-    print("")
-    print("  echo 'how now browne cow?' | {prog} -".format(prog=sys.argv[0]))
-    print("")
-    sys.exit()
-# Discard any used arguments (for sake of fileinput)
-if (i > 1):
-    debug.trace(5, f"discarding used args: {sys.argv[1: i]}")
-    sys.argv = [sys.argv[0]] + sys.argv[i:]
-
-# Initialize spell checking
-speller = enchant.Dict("en_US")
-
-# Check input
-for line in fileinput.input():
-    line = line.strip()
-    debug.trace_fmt(5, "L{line_num}: {line_text}", line_num=fileinput.filelineno(), line_text=line)
-
-    # Extract word tokens and print those not recognized
-    ## BAD:
-    ## word_tokens = [t.strip() for t in my_re.split(r"\W+", line.lower(), my_re.LOCALE|my_re.UNICODE)
-    ##                if (len(t.strip()) > 0)]
-    word_tokens = split_word_tokens(line.lower())
-    debug.trace(4, f"tokens: {word_tokens}")
-    for w in word_tokens:
-        if not speller.check(w):
-            print(w)
+def main():
+    """Entry point for script"""
+    # Process command line
+    # TODO: upgrade to using Main script (see template.py)
+    i = 1
+    show_usage = (i == len(sys.argv))
+    while (i < len(sys.argv)) and (sys.argv[i][0] == "-"):
+        if (sys.argv[i] == "--help"):
+            show_usage = True
+        elif (sys.argv[i] == "-"):
+            pass
+        else:
+            print("Error: unexpected argument '%s'" % sys.argv[i])
+            show_usage = True
+        i += 1
+    if (show_usage):
+        print("Usage: %s [options] input-file" % sys.argv[0])
+        print("")
+        print("Options: [--help]")
+        print("")
+        print("Examples:")
+        print("")
+        print("  %s query-keywords.list" % sys.argv[0])
+        print("")
+        print("  echo 'how now browne cow?' | {prog} -".format(prog=sys.argv[0]))
+        print("")
+        sys.exit()
+    # Discard any used arguments (for sake of fileinput)
+    if (i > 1):
+        debug.trace(5, f"discarding used args: {sys.argv[1: i]}")
+        sys.argv = [sys.argv[0]] + sys.argv[i:]
+    
+    # Initialize spell checking
+    speller = enchant.Dict(SPELL_LANG)
+    
+    # Check input
+    for line in fileinput.input():
+        line = line.strip()
+        debug.trace_fmt(5, "L{line_num}: {line_text}", line_num=fileinput.filelineno(), line_text=line)
+    
+        # Extract word tokens and print those not recognized
+        ## BAD:
+        ## word_tokens = [t.strip() for t in my_re.split(r"\W+", line.lower(), my_re.LOCALE|my_re.UNICODE)
+        ##                if (len(t.strip()) > 0)]
+        word_tokens = split_word_tokens(line.lower())
+        debug.trace(4, f"tokens: {word_tokens}")
+        for w in word_tokens:
+            if not speller.check(w):
+                print(w)
+
+#-------------------------------------------------------------------------------
+    
+if __name__ == '__main__':
+    debug.trace_current_context(level=TL.QUITE_DETAILED)
+    debug.trace_fmt(TL.USUAL, "Environment options: {eo}",
+                    eo=system.formatted_environment_option_descriptions())
+    main()
```

### Comparing `mezcla-1.3.5/mezcla/sys_version_info_hack.py` & `mezcla-1.3.6/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/system.py` & `mezcla-1.3.6/mezcla/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,17 +143,19 @@
     # Note: Use getenv_* for type-specific versions with env. option description
     result = os.getenv(var, default_value)
     debug.trace_fmt(5, "getenv({v}, {dv}) => {r}", v=var, dv=default_value, r=result)
     return result
 
 
 def getenv_text(var, default=None, description=None, helper=False):
-    """Returns textual value for environment variable VAR (or DEFAULT value).
-    Notes: HELPER indicates that this call is in support of another getenv-type function (e.g., getenv_bool), so that tracing is only shown at higher verbosity level (e.g., 6 not 5).
-    DESCRIPTION used for get_environment_option_descriptions."""
+    """Returns textual value for environment variable VAR (or DEFAULT value, excluding None).
+    Notes:
+    - Use getenv_value if default can be None, as result is always a string.
+    - HELPER indicates that this call is in support of another getenv-type function (e.g., getenv_bool), so that tracing is only shown at higher verbosity level (e.g., 6 not 5).
+    - DESCRIPTION used for get_environment_option_descriptions."""
     # Note: default is empty string to ensure result is string (not NoneType)
     ## TODO: add way to block registration
     register_env_option(var, description, default)
     if default is None:
         debug.trace(4, f"Warning: getenv_text treats default None as ''; consider using getenv_value for '{var}' instead")
         default = ""
     text_value = os.getenv(var)
@@ -196,14 +198,15 @@
     return (bool_value)
 #
 getenv_boolean = getenv_bool
 
 
 def getenv_number(var, default=-1.0, description=None, helper=False):
     """Returns number based on environment VAR (or DEFAULT value), with optional description"""
+    # TODO: def getenv_number(...) -> Optional(float):
     # Note: use getenv_int or getenv_float for typed variants
     num_value = default
     value = getenv_value(var, description=description, default=default)
     if (isinstance(value, str) and value.strip()):
          num_value = to_float(value)
     trace_level = 6 if helper else 5
     debug.trace_fmtd(trace_level, "getenv_number({v}, {d}) => {r}",
@@ -344,17 +347,18 @@
     return function_name
 
 
 def open_file(filename, encoding=None, errors=None, **kwargs):
     """Wrapper around around open() with FILENAME using UTF-8 encoding and ignoring ERRORS (both by default)
     Note: mode is left at default (i.e., 'r')"""
     # TODO: implement as with-style context
-    if encoding is None:
+    ## OLD: if encoding is None:
+    if (encoding is None) and (kwargs.get("mode") != "rb"):
         encoding = "UTF-8"
-    if errors is None:
+    if (encoding and (errors is None)):
         errors = 'ignore'
     result = None
     try:
         # pylint: disable=consider-using-with; note: bogus 'Bad option value' warning
         result = open(filename, encoding=encoding, errors=errors, **kwargs)
     except IOError:
         debug.trace_fmtd(3, "Unable to open {f}: {exc}", f=filename, exc=get_exception())
@@ -365,29 +369,29 @@
 
 def save_object(file_name, obj):
     """Saves OBJ to FILE_NAME in pickle format"""
     # Note: The data file is created in binary mode to avoid quirk under Windows.
     # See https://stackoverflow.com/questions/556269/importerror-no-module-named-copy-reg-pickle.
     debug.trace_fmtd(6, "save_object({f}, _)", f=file_name)
     try:
-        with open(file_name, 'wb') as f:
+        with open(file_name, mode='wb') as f:
             pickle.dump(obj, f)
     except (AttributeError, IOError, TypeError, ValueError):
         debug.trace_fmtd(1, "Error: Unable to save object to {f}: {exc}",
                          f=file_name, exc=get_exception())
     return
 
     
 def load_object(file_name, ignore_error=False):
     """Loads object from FILE_NAME in pickle format"""
     # Note: Reads in binary mode to avoid unicode decode error. See
     #    https://stackoverflow.com/questions/32957708/python-pickle-error-unicodedecodeerror
     obj = None
     try:
-        with open(file_name, 'rb') as f:
+        with open(file_name, mode='rb') as f:
             ## OLD: obj = pickle.load(f)
             try:
                 obj = pickle.load(f)
             except (UnicodeDecodeError):
                 if (sys.version_info.major > 2):
                     # note: treats strings in python2-pickled files as bytes (not Ascii)
                     obj = pickle.load(f, encoding='bytes') 
@@ -566,15 +570,15 @@
 
 
 def read_binary_file(filename):
     """Read FILENAME as byte stream"""
     debug.trace_fmt(7, "read_binary_file({f}, _)", f=filename)
     data = []
     try:
-        with open(filename, "rb") as f:
+        with open(filename, mode="rb") as f:
             data = f.read()
     except (IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem reading file '{f}': {exc}",
                          f=filename, exc=get_exception())
     ## TODO: output hexdump excerpt (e.g., via https://pypi.org/project/hexdump)
     return data
 
@@ -612,15 +616,15 @@
     if delim is None:
         delim = "\t"
     ## OLD: hash_table = {}
     hash_table = defaultdict(str)
     line_num = 0
     try:
         # TODO: use csv.reader
-        with open(filename) as f:
+        with open(filename, encoding="UTF-8") as f:
             for line in f:
                 line_num += 1
                 if (skip_header and (line_num == 1)):
                     continue
                 ## OLD: line = from_utf8(line)
                 ## OLD: line = from_utf8(line.rstrip())
                 line = from_utf8(line.rstrip("\n"))
@@ -688,15 +692,15 @@
     # EX: f = "/tmp/_it.list"; write_file(f, "it"); read_file(f) => "it\n"
     # EX: write_file(f, "it", skip_newline=True); read_file(f) => "it"
     debug.assertion(isinstance(text, str))
     try:
         if not isinstance(text, STRING_TYPES):
             text = to_string(text)
         mode = 'a' if append else 'w'
-        with open(filename, mode) as f:
+        with open(filename, encoding="UTF-8", mode=mode) as f:
             f.write(to_utf8(text))
             if not text.endswith("\n"):
                 if not skip_newline:
                     f.write("\n")
     except (IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem writing file '{f}': {exc}",
                          f=filename, exc=get_exception())
@@ -704,17 +708,17 @@
 #
 # EX: write_file(f, "new", append=True); read_file(f) => "itnew\n"
 
 
 def write_binary_file(filename, data):
     """Create FILENAME with binary DATA"""
     debug.trace_fmt(7, "write_binary_file({f}, _)", f=filename)
-    debug.assertion(isinstance(text, bytes))
+    debug.assertion(isinstance(data, bytes))
     try:
-        with open(filename, "wb") as f:
+        with open(filename, mode="wb") as f:
             f.write(data)
     except (IOError, ValueError):
         debug.trace_fmtd(1, "Error: Problem writing file '{f}': {exc}",
                          f=filename, exc=get_exception())
     return
 
 
@@ -723,15 +727,15 @@
     debug.trace_fmt(5, "write_lines({f}, _, {a})", f=filename, a=append)
     debug.trace_fmt(6, "    text_lines={tl}", tl=text_lines)
     debug.assertion(isinstance(text_lines, list))
     f = None
     try:
         mode = 'a' if append else 'w'
         ## OLD f = open(filename, mode)
-        with open(filename, mode) as f:
+        with open(filename, encoding="UTF-8", mode=mode) as f:
             for line in text_lines:
                 line = to_utf8(line)
                 f.write(line + "\n")
     except IOError:
         debug.trace_fmt(2, "Warning: Exception writing file {f}: {e}",
                         f=filename, e=get_exception())
     finally:
@@ -815,15 +819,15 @@
     return path
 
 
 def is_directory(path):
     """Determines whether PATH represents a directory"""
     # EX: is_directory("/etc")
     is_dir = os.path.isdir(path)
-    debug.trace_fmt(6, "is_dir({p} => {r}", p=path, r=is_dir)
+    debug.trace_fmt(6, "is_dir({p}) => {r}", p=path, r=is_dir)
     return is_dir
 
 
 def is_regular_file(path):
     """Determines whether PATH represents a plain file"""
     # EX: (not is_regular_file("/etc"))
     ok = os.path.isfile(path)
@@ -1179,18 +1183,20 @@
     """Return current time in seconds since 1970, optionally INTEGRAL"""
     secs = time.time()
     if integral:
         secs = int(round_num(secs, precision=0))
     debug.trace(5, f"current_time([integral={integral}]) => {secs}")
     return secs
 
+
 def time_in_secs():
     """Wrapper around current_time"""
     return current_time(integral=True)
 
+
 def python_maj_min_version():
     """Return Python version as a float of form Major.Minor"""
     # EX: debug.assertion(python_maj_min_version() >= 3.6, "F-Strings are used")
     version = sys.version_info
     py_maj_min = to_float("{M}.{m}".format(M=version.major, m=version.minor))
     debug.trace_fmt(5, "Python version (maj.min): {v}", v=py_maj_min)
     debug.assertion(py_maj_min > 0)
@@ -1199,14 +1205,15 @@
 
 def get_args():
     """Return command-line arguments (as a list of strings)"""
     result = sys.argv
     debug.trace_fmtd(6, "get_args() => {r}", r=result)
     return result
 
+
 def init():
     """Performs module initilization"""
     # TODO: rework global initialization to avoid the need for this
     global TEMP_DIR
     TEMP_DIR = getenv_text("TMPDIR", "/tmp")
 
     ## TODO: # Register DEBUG_LEVEL for sake of new users
```

### Comparing `mezcla-1.3.5/mezcla/temp/simple_batspp.py` & `mezcla-1.3.6/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/template.py` & `mezcla-1.3.6/mezcla/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 ## #! env python
 # 
 # TODO what the script does (detailed)
 #
 ## TODO: see example/template.py for simpler version suitable for cut-n-paste from online examples
 #
 
-"""TODO: what module does (brief)"""
+"""
+TODO: what module does (brief)
+
+Sample usage:
+   echo $'TODO:task1\\nDONE:task2' | {script} --TODO-arg --
+"""
 
 # Standard modules
 ## TODO: from collections import defaultdict
 
 # Installed modules
 ## TODO: import numpy
 
@@ -24,35 +29,36 @@
 ## TODO:
 ## from mezcla import glue_helpers as gh
 ## from mezcla import data_utils as du
 ##
 ## Optional:
 ## # Increase trace level for regex searching, etc. (e.g., from 6 to 7)
 ## my_re.TRACE_LEVEL = debug.QUITE_VERBOSE
+debug.trace(5, f"global __doc__: {__doc__}")
+debug.assertion(__doc__)
 
 ## TODO: Constants for switches omitting leading dashes (e.g., DEBUG_MODE = "debug-mode")
 ## Note: Run following in Emacs to interactively replace TODO_ARG with option label
 ##    M-: (query-replace-regexp "todo\\([-_]\\)arg" "arg\\1name")
 ## where M-: is the emacs keystroke short-cut for eval-expression.
 TODO_ARG = "TODO-arg"
 ## TEXT_ARG = "text-arg"
 ## ALT_FILENAME = "alt_filename"
 
 # Constants
 TL = debug.TL
 
-## TODO:
-## # Environment options
-## # Note: These are just intended for internal options, not for end users.
-## # It also allows for enabling options in one place rather than four
-## # (e.g., [Main member] initialization, run-time value, and argument spec., along
-## # with string constant definition).
-## #
-## FUBAR = system.getenv_bool("FUBAR", False,
-##                            description="Fouled Up Beyond All Recognition processing")
+# Environment options
+# Note: These are just intended for internal options, not for end users.
+# It also allows for enabling options in one place rather than four
+# (e.g., [Main member] initialization, run-time value, and argument spec., along
+# with string constant definition).
+#
+TODO_FUBAR = system.getenv_bool("TODO_FUBAR", False,
+                                description="TODO:Fouled Up Beyond All Recognition processing")
 
 
 class Script(Main):
     """Input processing class"""
     # TODO: -or-: """Adhoc script class (e.g., no I/O loop, just run calls)"""
     ## TODO: class-level member variables for arguments (avoids need for class constructor)
     todo_arg = False
@@ -72,22 +78,24 @@
         """Check results of command line processing"""
         debug.trace_fmtd(TL.VERBOSE, "Script.setup(): self={s}", s=self)
         ## TODO: extract argument values
         self.todo_arg = self.get_parsed_option(TODO_ARG, self.todo_arg)
         ## TODO:
         ## self.text_arg = self.get_parsed_option(TEXT_ARG, self.text_arg)
         ## self.alt_filename = self.get_parsed_argument(ALT_FILENAME)
-        debug.trace_object(5, self, label="Script instance")
+        debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
 
     def process_line(self, line):
         """Processes current line from input"""
         debug.trace_fmtd(TL.QUITE_DETAILED, "Script.process_line({l})", l=line)
         # TODO: flesh out
         if self.todo_arg and "TODO" in line:
             print(f"arg1 line ({self.line_num}): {line}")
+        else:
+            debug.trace(3, f"Ignoring line ({self.line_num}): {line}")
         ## TODO: regex pattern matching
         ## elif my_re.search(self.text_arg, line):
         ##     print("arg2 line: %s" % line)
 
     ## TODO: if no input proocessed, customize run_main_step instead
     ## and specify skip_input below
     ##
@@ -100,15 +108,15 @@
     ##           """Do final processing"""
     ##           debug.trace(6, f"Script.wrap_up(); self={self}")
     ##           # ...
 
 def main():
     """Entry point"""
     app = Script(
-        description=__doc__,
+        description=__doc__.format(script=__file__),
         # Note: skip_input controls the line-by-line processing, which is inefficient but simple to
         # understand; in contrast, manual_input controls iterator-based input (the opposite of both).
         skip_input=False,
         manual_input=False,
         ## TODO (specify auto_help such as when manual_input set):
         ## # Note: shows brief usage if no arguments given
         ## auto_help=True,
@@ -127,10 +135,14 @@
     debug.assertion(not any(my_re.search(r"^TODO_", m, my_re.IGNORECASE)
                             for m in dir(app)))    
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_DETAILED)
-    debug.trace_fmt(TL.USUAL, "Environment options: {eo}",
-                    eo=system.formatted_environment_option_descriptions())
+    ## OLD:
+    ## debug.trace_fmt(TL.USUAL, "Environment options: {eo}",
+    ##                 eo=system.formatted_environment_option_descriptions())
+    ## TODO: main => global
+    debug.trace(5, f"main __doc__: {main.__doc__}")
+    debug.assertion(main.__doc__)
     main()
```

### Comparing `mezcla-1.3.5/mezcla/tests/LICENSE.txt` & `mezcla-1.3.6/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.6/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/misc_doctests.py` & `mezcla-1.3.6/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/cars-len-3.txt` & `mezcla-1.3.6/mezcla/tests/resources/cars-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/cars.csv` & `mezcla-1.3.6/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.6/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.6/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.6/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.6/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.6/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.6/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.6/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/template.py` & `mezcla-1.3.6/mezcla/tests/template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_audio.py` & `mezcla-1.3.6/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.6/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_bing_search.py` & `mezcla-1.3.6/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.6/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_cut.py` & `mezcla-1.3.6/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_data_utils.py` & `mezcla-1.3.6/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_debug.py` & `mezcla-1.3.6/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.6/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_file_utils.py` & `mezcla-1.3.6/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_filter_random.py` & `mezcla-1.3.6/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.6/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.6/mezcla/tests/test_glue_helpers.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_html_utils.py` & `mezcla-1.3.6/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.6/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.6/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_main.py` & `mezcla-1.3.6/mezcla/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_merge_files.py` & `mezcla-1.3.6/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.6/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.6/mezcla/tests/test_misc_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_my_regex.py` & `mezcla-1.3.6/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.6/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_os_utils.py` & `mezcla-1.3.6/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.6/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.6/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.6/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.6/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.6/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.6/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.6/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.6/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.6/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.6/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_system.py` & `mezcla-1.3.6/mezcla/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_template.py` & `mezcla-1.3.6/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.6/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_text_processing.py` & `mezcla-1.3.6/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_text_utils.py` & `mezcla-1.3.6/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.6/mezcla/tests/test_tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.6/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.6/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.6/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.6/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.6/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.6/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.6/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.6/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/text_categorizer.py` & `mezcla-1.3.6/mezcla/text_categorizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -597,15 +597,32 @@
     # TODO: define text area dimensions based on browser window size
     html_template += """
             <!-- Form for entering text for categorization -->
             <hr>
             <form action="{base_url}/categorize" method="get">
                 <label for="textarea1">Categorize</label>
                 <br>
-                <textarea id="textarea1" rows="5" cols="100" name="text"></textarea>
+                <textarea id="textarea1" rows="10" cols="100" name="text"></textarea>
+                <br>
+                <input type="submit">
+            </form>
+            
+        </body>
+    </html>
+    """
+
+    #
+    # TODO: define text area dimensions based on browser window size
+    html_template += """
+            <!-- Form for entering text for categorization -->
+            <hr>
+            <form action="{base_url}/probs" method="get">
+                <label for="textarea1">Probabilities</label>
+                <br>
+                <textarea id="textarea1" rows="10" cols="100" name="text"></textarea>
                 <br>
                 <input type="submit">
             </form>
             
         </body>
     </html>
     """
```

### Comparing `mezcla-1.3.5/mezcla/text_processing.py` & `mezcla-1.3.6/mezcla/text_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,25 +104,28 @@
 TERSE_OUTPUT = tpo.getenv_boolean("TERSE_OUTPUT", JUST_TAGS, "Terse output mode")
 VERBOSE = not TERSE_OUTPUT
 
 # Skip use of NLTK and/or ENCHANT packages (using simple versions of functions)
 # TODO: make misspellings optional (add --classic mode???)
 SKIP_NLTK = tpo.getenv_boolean("SKIP_NLTK", False, "Omit usage of Natural Language Toolkit (NLTK)")
 SKIP_ENCHANT = tpo.getenv_boolean("SKIP_ENCHANT", SKIP_MISSPELLINGS, "Omit usage of Enchant package for spell checking")
+DOWNLOAD_DATA = system.getenv_bool("DOWNLOAD_DATA", False,
+                                   "Download data from NLTK")
 
 # List of stopwords (e.g., high-freqency function words)
 stopwords = None
 
 #------------------------------------------------------------------------
 # Optional libraries
 
 # NLP toolkit
 if not SKIP_NLTK:
     import nltk            # pylint: disable=ungrouped-imports
-    nltk.download('all')
+    if DOWNLOAD_DATA:
+        nltk.download('all')
 # spell checking
 if not SKIP_ENCHANT:
     import enchant         # pylint: disable=ungrouped-imports
 
 #------------------------------------------------------------------------
 # Functions
```

### Comparing `mezcla-1.3.5/mezcla/text_utils.py` & `mezcla-1.3.6/mezcla/text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tfidf/corpus.py` & `mezcla-1.3.6/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.6/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tfidf/document.py` & `mezcla-1.3.6/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/tfidf/preprocess.py` & `mezcla-1.3.6/mezcla/tfidf/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # coding: utf-8
 # TODO:
 # - Fix env-spec above and put coding on same line.
 # - Verify the fixup for PEP-0479 didn't break anything in Python 2 (e.g., for regression testing).
+# - *** Remove Python2-specific code!
 #
 
 """Pre-processing step for text.
 
 Example:
     >>> from mezcla.tfidf.preprocess import Preprocessor
     >>> p = Preprocessor(gramsize=2)
@@ -20,29 +21,32 @@
 from __future__ import absolute_import, with_statement
 
 # Standard modules
 from collections import namedtuple
 import re
 import sys  # python2 support
 from threading import RLock
+import html
 
 # Installed modules
 ## TODO: find better documented memoization package
 from cachetools import LRUCache, cached  # python2 support
 from nltk.stem import SnowballStemmer
-from six.moves.html_parser import HTMLParser  # python2 support
+## OLD: from six.moves.html_parser import HTMLParser  # python2 support
 from sklearn.feature_extraction.text import CountVectorizer
 from stop_words import get_stop_words
 
 # Local modules
 from mezcla import debug
 from mezcla import system
 from mezcla.tfidf.dockeyword import DocKeyword
 
-unescape = HTMLParser().unescape
+## OLD: unescape = HTMLParser().unescape
+unescape = html.unescape
+
 
 # TPO: Allow word splitting pattern to be overwritten.
 # TODO: Get WORD_REGEX from environment.
 # TODO: Have option to ignore words with specific punctuation (or to include).
 # TODO: strip period to allow for ngrams with abbreviations (e.g., "Dr. Jones").
 SPLIT_WORDS = system.getenv_bool("SPLIT_WORDS", False,
                                  "Split by word token instead of whitespace")
@@ -398,9 +402,9 @@
     debug.assertion("my man" in ngrams)
     debug.assertion("my man fran" not in ngrams)
     debug.assertion("fran man" not in ngrams)
     
 #-------------------------------------------------------------------------------
     
 if __name__ == '__main__':
-    system.print_stderr(f"Warning: {__file__} is not intended to be run standalone. A simple test willl be run.")
+    system.print_stderr(f"Warning: {__file__} is not intended to be run standalone. A simple test will be run.")
     main()
```

### Comparing `mezcla-1.3.5/mezcla/tpo_common.py` & `mezcla-1.3.6/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/train_language_model.py` & `mezcla-1.3.6/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/train_text_categorizer.py` & `mezcla-1.3.6/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/transpose_data.py` & `mezcla-1.3.6/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/unittest_wrapper.py` & `mezcla-1.3.6/mezcla/unittest_wrapper.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/mezcla/xml_utils.py` & `mezcla-1.3.6/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/pyproject.toml` & `mezcla-1.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/requirements.txt` & `mezcla-1.3.6/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -80,7 +80,10 @@
 ## TODO: python -m bash_kernel.install
 #opt# webcolors
 #opt# flit
 #opt# pytest
 #opt# coverage
 #opt# ipython
 #opt# pylint
+#opt# gradio
+#opt# sentencepiece
+#opt# sacremoses
```

### Comparing `mezcla-1.3.5/setup.py` & `mezcla-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """Simple installer"""
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla'],
       module="mezcla",
-      version='1.3.5',
+      version='1.3.6',
       description-file="README.txt",
       dist-name="Mezcla",
       ## OLD: py_modules=PYTHON_MODULE_NAMES,
       author="Tom O'Hara",
       # TODO: find out which email key is preferred
       email="tomasohara@gmail.com",
       author-email="tomasohara@gmail.com"
```

### Comparing `mezcla-1.3.5/temp/simple_batspp.py` & `mezcla-1.3.6/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/tox.ini` & `mezcla-1.3.6/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.5/PKG-INFO` & `mezcla-1.3.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.5
+Version: 1.3.6
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
```

