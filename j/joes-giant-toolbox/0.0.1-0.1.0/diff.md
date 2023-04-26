# Comparing `tmp/joes_giant_toolbox-0.0.1.tar.gz` & `tmp/joes_giant_toolbox-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joes_giant_toolbox-0.0.1.tar", last modified: Tue Apr 18 20:45:28 2023, max compression
+gzip compressed data, was "joes_giant_toolbox-0.1.0.tar", last modified: Wed Apr 26 19:50:33 2023, max compression
```

## Comparing `joes_giant_toolbox-0.0.1.tar` & `joes_giant_toolbox-0.1.0.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.778648 joes_giant_toolbox-0.0.1/
--rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.0.1/LICENSE
--rw-r--r--   0 josephbolton   (501) staff       (20)    57767 2023-04-18 20:45:28.778489 joes_giant_toolbox-0.0.1/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)    16509 2023-04-18 20:44:44.000000 joes_giant_toolbox-0.0.1/README.md
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.773163 joes_giant_toolbox-0.0.1/joes_giant_toolbox/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/__init__.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.776528 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/
--rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/__init__.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/ascii_density_histogram.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/create_project_scope_doc.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/list_all_python_imports.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1785 2023-03-22 13:13:52.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/print_progress_bar.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/run_python_function_in_parallel.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    11586 2023-04-17 14:57:06.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/string_cleaner.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/view_nested_dict_structure.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/convenience.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      172 2023-04-17 13:24:11.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/dataviz.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      792 2023-04-17 12:30:30.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/google_cloud.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.777588 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/
--rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/ascii_barplot.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/query_wikipedia_api.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/proj_mgmt.py
--rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/sklearn.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      104 2023-04-17 13:58:31.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/stats.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      206 2023-04-17 14:09:24.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/text.py
--rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox/web.py
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.773804 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/
--rw-r--r--   0 josephbolton   (501) staff       (20)    57767 2023-04-18 20:45:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 josephbolton   (501) staff       (20)     2407 2023-04-18 20:45:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-04-18 20:45:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-04-18 20:45:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/requires.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-04-18 20:45:28.000000 joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/top_level.txt
--rw-r--r--   0 josephbolton   (501) staff       (20)      923 2023-04-18 20:45:20.000000 joes_giant_toolbox-0.0.1/pyproject.toml
--rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-04-18 20:45:28.778686 joes_giant_toolbox-0.0.1/setup.cfg
-drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-18 20:45:28.778248 joes_giant_toolbox-0.0.1/tests/
--rw-r--r--   0 josephbolton   (501) staff       (20)      834 2023-04-13 17:59:20.000000 joes_giant_toolbox-0.0.1/tests/test_conjugate_prior_beta_binomial.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     1045 2023-04-13 18:12:57.000000 joes_giant_toolbox-0.0.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     2497 2023-03-18 11:26:58.000000 joes_giant_toolbox-0.0.1/tests/test_make_url_request.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     8284 2023-03-24 06:41:18.000000 joes_giant_toolbox-0.0.1/tests/test_rapid_binary_classifier.py
--rw-r--r--   0 josephbolton   (501) staff       (20)     4695 2023-04-13 17:56:54.000000 joes_giant_toolbox-0.0.1/tests/test_string_cleaner.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.809391 joes_giant_toolbox-0.1.0/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    35149 2023-03-02 13:11:21.000000 joes_giant_toolbox-0.1.0/LICENSE
+-rw-r--r--   0 josephbolton   (501) staff       (20)    58561 2023-04-26 19:50:33.809154 joes_giant_toolbox-0.1.0/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)    17280 2023-04-26 19:47:46.000000 joes_giant_toolbox-0.1.0/README.md
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.792653 joes_giant_toolbox-0.1.0/joes_giant_toolbox/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/__init__.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.803910 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/
+-rw-r--r--   0 josephbolton   (501) staff       (20)        0 2023-04-13 17:58:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/__init__.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10700 2023-04-12 10:02:27.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4964 2023-04-17 13:22:54.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/ascii_density_histogram.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      967 2023-03-03 07:53:04.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4317 2023-04-17 13:55:24.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/create_project_scope_doc.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1727 2023-03-21 12:21:56.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1430 2023-03-20 07:50:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    10974 2023-04-06 12:30:49.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2261 2023-04-17 14:00:23.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_all_python_imports.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      878 2023-03-20 07:49:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4736 2023-04-17 14:11:08.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4358 2023-03-03 08:08:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      376 2023-04-23 20:15:27.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/manual_keyword_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2318 2023-04-19 11:00:23.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1845 2023-04-01 21:15:07.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/print_progress_bar.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2098 2023-04-26 19:31:41.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/python_plotting_tutorials.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      501 2023-03-29 13:35:25.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    48271 2023-04-10 13:38:46.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4608 2023-03-30 09:37:03.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/run_python_function_in_parallel.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     5776 2023-04-17 12:08:12.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    13692 2023-04-25 10:48:25.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/string_cleaner.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1536 2023-04-13 10:47:28.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2360 2023-03-29 14:15:20.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2282 2023-04-17 13:33:49.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/view_nested_dict_structure.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1805 2023-03-21 10:01:14.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      264 2023-04-17 12:16:19.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/convenience.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      413 2023-04-25 07:40:31.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/dataviz.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1150 2023-04-21 18:17:10.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/google_cloud.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.806525 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2126 2023-04-03 18:18:28.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/ascii_barplot.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1108 2023-03-07 09:48:13.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     3563 2023-03-16 08:04:10.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2088 2023-03-15 19:17:57.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      446 2023-03-10 07:50:35.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/query_wikipedia_api.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1161 2023-04-10 13:40:03.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)    47227 2023-04-01 21:12:12.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       85 2023-04-17 13:38:24.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/proj_mgmt.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)       81 2023-04-17 14:03:06.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/sklearn.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      161 2023-04-26 19:46:54.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/stats.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      246 2023-04-25 10:34:50.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/text.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      515 2023-04-17 12:09:22.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox/web.py
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.793753 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/
+-rw-r--r--   0 josephbolton   (501) staff       (20)    58561 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2511 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)        1 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)      186 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/requires.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)       19 2023-04-26 19:50:33.000000 joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/top_level.txt
+-rw-r--r--   0 josephbolton   (501) staff       (20)     1084 2023-04-26 19:49:36.000000 joes_giant_toolbox-0.1.0/pyproject.toml
+-rw-r--r--   0 josephbolton   (501) staff       (20)       38 2023-04-26 19:50:33.809446 joes_giant_toolbox-0.1.0/setup.cfg
+drwxr-xr-x   0 josephbolton   (501) staff       (20)        0 2023-04-26 19:50:33.808561 joes_giant_toolbox-0.1.0/tests/
+-rw-r--r--   0 josephbolton   (501) staff       (20)      557 2023-04-26 19:48:17.000000 joes_giant_toolbox-0.1.0/tests/test_conjugate_prior_beta_binomial.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)      571 2023-04-25 09:26:34.000000 joes_giant_toolbox-0.1.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     2617 2023-04-25 09:27:22.000000 joes_giant_toolbox-0.1.0/tests/test_make_url_request.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     8681 2023-04-25 09:28:50.000000 joes_giant_toolbox-0.1.0/tests/test_rapid_binary_classifier.py
+-rw-r--r--   0 josephbolton   (501) staff       (20)     4500 2023-04-25 09:29:06.000000 joes_giant_toolbox-0.1.0/tests/test_string_cleaner.py
```

### Comparing `joes_giant_toolbox-0.0.1/LICENSE` & `joes_giant_toolbox-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/PKG-INFO` & `joes_giant_toolbox-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes_giant_toolbox
-Version: 0.0.1
+Version: 0.1.0
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,21 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: doc
+Provides-Extra: google
 License-File: LICENSE
 
 # Joe's Giant Tool Box
 
+https://github.com/J-sephB-lt-n/joes_giant_toolbox
+
 A large collection of general python functions and classes that I use in my daily work
 
 ```
                                                      .-.
                                                     /   \
                                      _____.....-----|(o) |
                                _..--'          _..--|  .''
@@ -709,14 +712,17 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
+![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox)
+
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
@@ -762,22 +768,23 @@
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
@@ -795,34 +802,44 @@
 | scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+help( joes_giant_toolbox.dataviz )
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
+help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
 
+```bash
+pip install joes-giant-toolbox[google]
+```
+
 ```python
 import joes_giant_toolbox.google_cloud
-help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
-help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
-help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
+
+help(joes_giant_toolbox.google_cloud)
+
+help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
+help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
+help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
@@ -855,14 +872,15 @@
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
 ## Statistical Inference and Hypothesis Testing 
 ```python
 import joes_giant_toolbox.stats
+help( joes_giant_toolbox.stats )
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
@@ -875,23 +893,24 @@
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
+help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
-git clone https://github.com/J-sephB-lt-n/joes_giant_toolbox.git
 pip install pytest
+cd joes_giant_toolbox/tests
 pytest -v
 ```
```

### Comparing `joes_giant_toolbox-0.0.1/README.md` & `joes_giant_toolbox-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Joe's Giant Tool Box
 
+https://github.com/J-sephB-lt-n/joes_giant_toolbox
+
 A large collection of general python functions and classes that I use in my daily work
 
 ```
                                                      .-.
                                                     /   \
                                      _____.....-----|(o) |
                                _..--'          _..--|  .''
@@ -18,14 +20,17 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
+![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox)
+
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
@@ -71,22 +76,23 @@
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
@@ -104,34 +110,44 @@
 | scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+help( joes_giant_toolbox.dataviz )
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
+help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
 
+```bash
+pip install joes-giant-toolbox[google]
+```
+
 ```python
 import joes_giant_toolbox.google_cloud
-help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
-help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
-help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
+
+help(joes_giant_toolbox.google_cloud)
+
+help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
+help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
+help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
@@ -164,14 +180,15 @@
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
 ## Statistical Inference and Hypothesis Testing 
 ```python
 import joes_giant_toolbox.stats
+help( joes_giant_toolbox.stats )
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
@@ -184,23 +201,24 @@
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
+help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
-git clone https://github.com/J-sephB-lt-n/joes_giant_toolbox.git
 pip install pytest
+cd joes_giant_toolbox/tests
 pytest -v
 ```
```

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/anonymous_view_public_linkedin_page.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/ascii_density_histogram.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/ascii_density_histogram.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/conjugate_prior_beta_binomial.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/create_project_scope_doc.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/create_project_scope_doc.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/duckduckgo_search_multipage.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/duckduckgo_search_multipage.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/list_all_python_imports.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_all_python_imports.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/list_files_in_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/make_url_request.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/make_url_request.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,26 @@
         Bucket name that file is currently in
     source_filename: str,
         Current name of the file in the source bucket
     destination_bucket_name: str
         Name of bucket that you want to move file to (can be the same as [source_bucket_name])
     destination_filename: str
         Desired name of the file in the destination bucket
+    verbose: bool (default: True)
+        Print process information to standard out during running of the function
+
+    Example Usage
+    -------------
+    >>> move_or_rename_file_in_gcloud_bucket(
+    ...     source_bucket_name="bucket1",
+    ...     source_filename="folder5/sixty9.json",
+    ...     destination_bucket_name="bucket2",
+    ...     destination_filename="folder5/sixty9.json",
+    ... )
+    File (blob) 'folder5/sixty9.json' in bucket 'bucket1' moved to file (blob) 'folder5/sixty9.json' in bucket 'bucket2'
     """
     storage_client = google.cloud.storage.Client()
     source_bucket = storage_client.bucket(source_bucket_name)
     source_blob = source_bucket.blob(source_filename)
     destination_bucket = storage_client.bucket(destination_bucket_name)
 
     destination_generation_match_precondition = 0
@@ -40,9 +52,9 @@
         if_generation_match=destination_generation_match_precondition,
     )
 
     source_bucket.delete_blob(source_filename)
 
     if verbose:
         print(
-            f"File (blob) {source_blob.name} in bucket {source_bucket.name} moved to file (blob) {blob_copy.name} in bucket {destination_bucket.name}"
+            f"File (blob) '{source_blob.name}' in bucket '{source_bucket.name}' moved to file (blob) '{blob_copy.name}' in bucket '{destination_bucket.name}'"
         )
```

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/print_progress_bar.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/print_progress_bar.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/rapid_binary_classifier.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/rapid_binary_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/run_python_function_in_parallel.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/run_python_function_in_parallel.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/string_cleaner.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/string_cleaner.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,66 +13,33 @@
     >>
 
     Attributes
     ----------
     operations: dict
         A dictionary containing each individual string cleaning function
     verbose: str, optional (default: True)
-        A global parameter dictating the verbosity of every string cleaning function
+        A global parameter dictating the verbosity of the output
 
     Methods
     -------
     apply_sequential_operations
-        Sequentially applies 1 or more string cleaning operations to a given string
+        Sequentially applies multiple string cleaning operations to the same string
 
     Notes
     -----
     You can get help on a specific string cleaning function using the built-in python help() function:
     >>> string_cleaner = StringCleaner()
-    >>> help( string_cleaner.operations["to_lowercase"] )
+    >>> help( string_cleaner.operations["extract_domain_from_url"] )
 
     A single string cleaning operation can be accessed directly:
     >>> string_cleaner.operations["remove_punctuation"]("j!o@e#i$s%t^h&e&b*e(s)t")
     joeisthebest
         ...or called via a chain consisting of only that 1 operation:
     >>> string_cleaner.apply_sequential_operations("j!o@e#i$s%t^h&e&b*e(s)t", operation_names_list=["remove_punctuation"])
     joeisthebest
-
-    Available String Cleaning Operations
-    ------------------------------------
-    extract_domain_from_url
-        Extracts the base domain from a given website URL
-    remove_words_or_phrases
-        Removes specific 'words' or 'phrases' (i.e. specific characters in a specific order) from a given string, possibly observing word boundaries
-    to_lowercase
-        Converts all upper case characters in the given string to lower case
-    punctuation_to_spaces
-        Turns any character which is not a letter or a number into a space character
-    remove_punctuation
-        Removes any character which is not a letter or a number
-    numbers_to_spaces
-        Turns all number characters in a given string into space characters
-    remove_numbers
-        Removes all number characters from a given string
-    remove_spaces
-        Removes all spaces from a given string
-    newlines_to_spaces
-        Turn newline characters ("\\n") into space characters in a given string
-    multiple_spaces_to_single_spaces
-        Turns every sequence of space characters in a given string into a single space character
-    remove_spaces_at_start_and_end
-        Remove any spaces characters
-    non_letters_to_spaces
-        Turn every character in a given string which is not a letter into a single space character
-    remove_non_letters
-        Remove every character in a given string which is not a letter
-    join_single_space_separated_letters_together
-        Removes the space characters between sequences of single letter characters separated by a single space (e.g. "a  B c D  e" becomes "a  BcD  e")
-    remove_non_printable_ascii_chars
-        Removes all characters from a given string which are not in the python constant 'string.printable'
     """
 
     def __init__(self, verbose: bool = True) -> None:
         self.operations = {}
         self.verbose = verbose
         self.printable_ascii_chars = string.printable
 
@@ -87,23 +54,23 @@
             """
             if self.verbose:
                 print(
                     f"""
 # extract domain from URL #
 " ".join(
     re.findall(
-        "(?P<url>https?://[^/]+)",
+        "(?P<url>https?://[^/?]+)",
         "{raw_str}",
     )     
 )           
 """
                 )
             return " ".join(
                 re.findall(
-                    "(?P<url>https?://[^/]+)",
+                    "(?P<url>https?://[^/?]+)",
                     raw_str,
                 )
             )
 
         def remove_words_or_phrases(
             raw_str: str,
             remove_list: typing.List[str],
@@ -177,98 +144,188 @@
             Example Usage
             -------------
             >>> string_cleaner = StringCleaner()
             >>> string_cleaner.operations["punctuation_to_spaces"]("!@Joe#$is%^the_best&*")
             ' Joe is the best '
             """
             if verbose:
-                print(f're.sub(r"[^A-Za-z0-9 ]+", " ", "{raw_str}")')
+                print(f're.sub(r"[^A-Za-z0-9]+", " ", "{raw_str}")')
             return re.sub(r"[^A-Za-z0-9 ]+", " ", raw_str)
 
         def remove_punctuation(raw_str):
             """Removes any character which is not a letter or a number
 
             Example Usage
             -------------
             >>> string_cleaner = StringCleaner()
-            >>> string_cleaner.operations["remove_punctuation"]("!@Joe#$Is%^The_Best&*")
-            'JoeIsTheBest'
+            >>> string_cleaner.operations["remove_punctuation"]("!@Joe# $is% ^the_ :best&*")
+            'Joe is the best'
             """
             if verbose:
-                print(f're.sub(r"[^A-Za-z0-9 ]+", "", "{raw_str}")')
+                print(f're.sub(r"[^A-Za-z0-9]+", "", "{raw_str}")')
             return re.sub(r"[^A-Za-z0-9 ]+", "", raw_str)
 
         def numbers_to_spaces(raw_str):
             """Turns all number characters in a given string into space characters
 
             Example Usage
             -------------
-            TODO
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["numbers_to_spaces"]("time2go2number136street")
+            'time go number   street'
             """
+            if verbose:
+                print(
+                    f'"{raw_str}".translate(str.maketrans("0123456789", " " * len("0123456789")))'
+                )
             return raw_str.translate(
                 str.maketrans("0123456789", " " * len("0123456789"))
             )
 
         def remove_numbers(raw_str):
             """Removes all number characters from a given string
 
             Example Usage
             -------------
-            TODO
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["remove_numbers"]("time2go2number136street")
+            'timegonumberstreet'
             """
+            if verbose:
+                print(f'"{raw_str}".translate(str.maketrans("", "", "0123456789"))')
             return raw_str.translate(str.maketrans("", "", "0123456789"))
 
         def remove_spaces(raw_str):
+            """Removes all spaces from a given string
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["remove_spaces"]("U  S  A")
+            'USA'
+            """
+            if verbose:
+                print(f're.sub(" ", "", "{raw_str}")')
             return re.sub(" ", "", raw_str)
 
         def newlines_to_spaces(raw_str):
+            """Turn newline characters ("\\n") into space characters in a given string
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["newlines_to_spaces"]("\\nU\\nS\\nS\\nR\\n")
+            ' U S S R '
+            """
+            if verbose:
+                print(f'"{raw_str}".replace("\\n", " ")')
             return raw_str.replace("\n", " ")
 
         def multiple_spaces_to_single_spaces(raw_str):
+            """Turns every sequence of space characters in a given string into a single space character
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["multiple_spaces_to_single_spaces"]("the quick  brown   fox     jumped        over")
+            'the quick brown fox jumped over'
+            """
+            if verbose:
+                print(f're.sub(" +", " ", "{raw_str}")')
             return re.sub(" +", " ", raw_str)
 
-        def remove_spaces_at_start_and_end(raw_str):
+        def remove_whitespace_at_start_and_end(raw_str):
+            """Remove all space and newline characters at the start and end of a string
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["remove_whitespace_at_start_and_end"]("\\n\\n text of interest   ")
+            'text of interest'
+            """
+            if verbose:
+                print(f'"{raw_str}".strip()')
             return raw_str.strip()
 
         def non_letters_to_spaces(raw_str):
+            """Turn all non-letter (i.e. not A-Z) characters into space characters in given string
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["non_letters_to_spaces"]("  joe123is-:the8==|>best  ")
+            '  joe   is  the     best  '
+            """
+            if verbose:
+                print(f're.sub("[^a-zA-Z]", " ", "{raw_str}")')
             return re.sub("[^a-zA-Z]", " ", raw_str)
 
         def remove_non_letters(raw_str):
+            """Remove all non-letter (i.e. not A-Z) characters in given string
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["remove_non_letters"]("  joe123is-:the8==|>best  ")
+            'joeisthebest'
+            """
+            if verbose:
+                print(f're.sub("[^a-zA-Z]", "", "{raw_str}")')
             return re.sub("[^a-zA-Z]", "", raw_str)
 
         def join_single_space_separated_letters_together(raw_str):
+            """Removes the space characters between sequences of single letter characters separated by a single space
+            (e.g. "a  B c D  e" becomes "a  BcD  e")
+
+            Example Usage
+            -------------
+            >>> string_cleaner = StringCleaner()
+            >>> string_cleaner.operations["join_single_space_separated_letters_together"]("a  B c D ef  g h  ")
+            'a  BcD ef  gh  '
+            """
+            if verbose:
+                print(f're.sub(r"\\b([a-zA-Z]) (?=[a-zA-Z]\\b)", r"\\1", "{raw_str}")')
             return re.sub(r"\b([a-zA-Z]) (?=[a-zA-Z]\b)", r"\1", raw_str)
 
         def remove_non_printable_ascii_chars(raw_str):
-            """Removes all characters from a given string which are not in the python constant 'string.printable'"""
+            """Removes all characters from a given string which are not in the python constant 'string.printable'
+
+            Example Usage
+            -------------
+            TODO
+            """
+            if verbose:
+                print(
+                    f'"".join(filter(lambda x: x in self.printable_ascii_chars, {raw_str}))'
+                )
             return "".join(filter(lambda x: x in self.printable_ascii_chars, raw_str))
 
         self.operations["extract_domain_from_url"] = extract_domain_from_url
-        self.operations["remove_words_or_phrases"] = remove_words_or_phrases
-        self.operations["to_lowercase"] = to_lowercase
-        self.operations["punctuation_to_spaces"] = punctuation_to_spaces
-        self.operations["remove_punctuation"] = remove_punctuation
-        self.operations["numbers_to_spaces"] = numbers_to_spaces
-        self.operations["remove_numbers"] = remove_numbers
-        self.operations["remove_spaces"] = remove_spaces
-        self.operations["newlines_to_spaces"] = newlines_to_spaces
+        self.operations[
+            "join_single_space_separated_letters_together"
+        ] = join_single_space_separated_letters_together
         self.operations[
             "multiple_spaces_to_single_spaces"
         ] = multiple_spaces_to_single_spaces
-        self.operations[
-            "remove_spaces_at_start_and_end"
-        ] = remove_spaces_at_start_and_end
+        self.operations["newlines_to_spaces"] = newlines_to_spaces
         self.operations["non_letters_to_spaces"] = non_letters_to_spaces
+        self.operations["numbers_to_spaces"] = numbers_to_spaces
+        self.operations["punctuation_to_spaces"] = punctuation_to_spaces
         self.operations["remove_non_letters"] = remove_non_letters
         self.operations[
-            "join_single_space_separated_letters_together"
-        ] = join_single_space_separated_letters_together
-        self.operations[
             "remove_non_printable_ascii_chars"
         ] = remove_non_printable_ascii_chars
+        self.operations["remove_numbers"] = remove_numbers
+        self.operations["remove_punctuation"] = remove_punctuation
+        self.operations["remove_spaces"] = remove_spaces
+        self.operations[
+            "remove_whitespace_at_start_and_end"
+        ] = remove_whitespace_at_start_and_end
+        self.operations["remove_words_or_phrases"] = remove_words_or_phrases
+        self.operations["to_lowercase"] = to_lowercase
 
         if self.verbose:
             print("-- Initiated StringCleaner() --")
             print("available string-cleaning operations:")
             for op_name in self.operations:
                 print(f"\to {op_name}")
```

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/url_to_filename_to_url_mapper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/view_nested_dict_structure.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/view_nested_dict_structure.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/all/write_pandas_df_to_google_bigquery_table.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/google_cloud.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/google_cloud.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+"""Utilities for interacting with Google Cloud
+
+Available modules: 
+    - delete_file_in_gcloud_bucket
+    - download_file_from_gcloud_bucket_to_python
+    - list_files_in_gcloud_bucket
+    - move_or_rename_file_in_gcloud_bucket
+    - query_bigquery_to_pandas_df
+    - upload_file_python_to_gcloud_bucket
+    - write_pandas_df_to_google_bigquery_table
+
+"""
+
 from joes_giant_toolbox.all.delete_file_in_gcloud_bucket import (
     delete_file_in_gcloud_bucket,
 )
 from joes_giant_toolbox.all.download_file_from_gcloud_bucket_to_python import (
     download_file_from_gcloud_bucket_to_python,
 )
 from joes_giant_toolbox.all.list_files_in_gcloud_bucket import (
```

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/ascii_barplot.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/ascii_barplot.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/conjugate_prior_normal_normal.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/imdb_item_page_scraper.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/longest_portion_of_phrase_in_search_string.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/rapid_bag_of_words_classifier.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/in_progress/recsys_data_simulator.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/in_progress/recsys_data_simulator.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox/web.py` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox/web.py`

 * *Files identical despite different names*

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/PKG-INFO` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joes-giant-toolbox
-Version: 0.0.1
+Version: 0.1.0
 Summary: A large collection of general python functions and classes that I use in my daily work
 Author-email: Joseph Bolton <joseph.jazz.bolton@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -683,18 +683,21 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: doc
+Provides-Extra: google
 License-File: LICENSE
 
 # Joe's Giant Tool Box
 
+https://github.com/J-sephB-lt-n/joes_giant_toolbox
+
 A large collection of general python functions and classes that I use in my daily work
 
 ```
                                                      .-.
                                                     /   \
                                      _____.....-----|(o) |
                                _..--'          _..--|  .''
@@ -709,14 +712,17 @@
  `-------------._______.----'                        /  `.
     .,.,.,.,.,.,.,.,.,.,.,.,.,                      /     \
    ((O) o o o o ======= o o(O))                 ._.'      /
 LGB `-.,.,.,.,.,.,.,.,.,.,.,-'                   `.......'
 ```
 source: https://ascii.co.uk
 
+![PyPI](https://img.shields.io/pypi/v/joes-giant-toolbox?label=pypi%20package)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/joes-giant-toolbox)
+
 # Installation
 
 ```bash
 pip install joes-giant-toolbox
 ```
 
 # Usage
@@ -762,22 +768,23 @@
 | duckduckgo_search_multipage                       | Fetches search results from the DuckDuckGo Lite search engine                                                |         2        |
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | make_url_request                                  | A convenience function for making API requests using the urllib library                                      |         3        |
 | move_or_rename_file_in_gcloud_bucket              | Move or rename a file which is in a google cloud bucket (which includes moving it to a different bucket)     |         4        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
 | query_bigquery_to_pandas_df                       | Runs a query on Google BigQuery and writes the result into a local pandas.DataFrame                          |         4        |
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 | scrape_webpage_and_all_linked_webpages            | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 | upload_file_python_to_gcloud_bucket               | Writes an object in python memory to a file (blob) on a google cloud bucket                                  |         4        |
 | url_to_filename_to_url_mapper                     | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 | write_pandas_df_to_google_bigquery_table          | Writes a pandas dataframe to a table on Google BigQuery                                                      |         4        |
 
 ## API and Web
 
 ```python
 import joes_giant_toolbox.web
 help( joes_giant_toolbox.web.anonymous_view_public_linkedin_page )
@@ -795,34 +802,44 @@
 | scrape_webpage_and_all_linked_webpages                   | Extracts HTML from given web page, and also follows all of the hyperlinks on that page and scrapes those too |         1        | 
 | url_to_filename_to_url_mapper                            | Converts a webpage URL into a useable filename, where the URL can be recovered directly from the filename    |         2        |
 
 ## Data Visualisation
 
 ```python
 import joes_giant_toolbox.dataviz
+help( joes_giant_toolbox.dataviz )
 help( joes_giant_toolbox.dataviz.ascii_density_histogram )
+help( joes_giant_toolbox.dataviz.PythonPlottingTutorials )
 help( joes_giant_toolbox.dataviz.view_nested_dict_structure )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | ascii_density_histogram                           | Draws a histogram using only raw text symbols                                                                |         2        |
-| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         2        |
+| PythonPlottingTutorials                           | Example code snippets for creating common data visualisations in python                                      |         4        |
+| view_nested_dict_structure                        | Generates a simple printout for understanding the structure of a complex nested python dictionary            |         4        |
 
 ## Google Cloud
 
+```bash
+pip install joes-giant-toolbox[google]
+```
+
 ```python
 import joes_giant_toolbox.google_cloud
-help( joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python )
-help( joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df )
-help( joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket )
-help( joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table )
+
+help(joes_giant_toolbox.google_cloud)
+
+help(joes_giant_toolbox.google_cloud.delete_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.download_file_from_gcloud_bucket_to_python)
+help(joes_giant_toolbox.google_cloud.list_files_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.move_or_rename_file_in_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.query_bigquery_to_pandas_df)
+help(joes_giant_toolbox.google_cloud.upload_file_python_to_gcloud_bucket)
+help(joes_giant_toolbox.google_cloud.write_pandas_df_to_google_bigquery_table)
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | delete_file_in_gcloud_bucket                      | Deletes a file which is in a google cloud bucket                                                             |         4        |
 | download_file_from_gcloud_bucket_to_python        | Reads a file from a google cloud bucket into python memory                                                   |         4        |
 | list_files_in_gcloud_bucket                       | Returns a list of the files present in a specified google cloud bucket                                       |         4        |
@@ -855,14 +872,15 @@
 | list_all_python_imports                           | Searches every python script in a given folder and lists all python modules imported within those scripts    |         2        |
 | print_progress_bar                                | Prints a progress bar (to standard out) while code is running                                                |         3        |
 | run_python_function_in_parallel                   | Runs a python function in parallel on multiple cores or threads                                              |         4        |
 
 ## Statistical Inference and Hypothesis Testing 
 ```python
 import joes_giant_toolbox.stats
+help( joes_giant_toolbox.stats )
 help( joes_giant_toolbox.stats.conjugate_prior_beta_binomial )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | conjugate_prior_beta_binomial                     | Calculates the posterior distribution of the success probability parameter [p] of a binomial distribution, from observed data and a user-specified beta prior | 4                |
 
@@ -875,23 +893,24 @@
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | RapidBinaryClassifier                             | Ultra rapid generation of binary classifier models in scikit-learn by abstracting away a lot of the decisions and model code| 3 |
 
 ## Text and Natural Language Processing
 ```python 
 import joes_giant_toolbox.text
+help( joes_giant_toolbox.text )
 help( joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector )
 help( joes_giant_toolbox.text.StringCleaner )
 ```
 
 | Name                                              | Description                                                                                                  | Confidence Score |
 |---------------------------------------------------|--------------------------------------------------------------------------------------------------------------|------------------|
 | longest_sentence_subsequence_plagiarism_detector  | Finds phrases (sequences of consecutive words) common to 2 documents (e.g. to act as a naive plagiarism detector) |    3        |
 | StringCleaner                                     | Performs common string-cleaning operations to a text string, also allowing them to be chained in sequence    |         1        |
 
 # Run Unit Tests
 
 ```bash
-git clone https://github.com/J-sephB-lt-n/joes_giant_toolbox.git
 pip install pytest
+cd joes_giant_toolbox/tests
 pytest -v
 ```
```

### Comparing `joes_giant_toolbox-0.0.1/joes_giant_toolbox.egg-info/SOURCES.txt` & `joes_giant_toolbox-0.1.0/joes_giant_toolbox.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 joes_giant_toolbox/all/delete_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/download_file_from_gcloud_bucket_to_python.py
 joes_giant_toolbox/all/duckduckgo_search_multipage.py
 joes_giant_toolbox/all/list_all_python_imports.py
 joes_giant_toolbox/all/list_files_in_gcloud_bucket.py
 joes_giant_toolbox/all/longest_sentence_subsequence_plagiarism_detector.py
 joes_giant_toolbox/all/make_url_request.py
+joes_giant_toolbox/all/manual_keyword_classifier.py
 joes_giant_toolbox/all/move_or_rename_file_in_gcloud_bucket.py
 joes_giant_toolbox/all/print_progress_bar.py
+joes_giant_toolbox/all/python_plotting_tutorials.py
 joes_giant_toolbox/all/query_bigquery_to_pandas_df.py
 joes_giant_toolbox/all/rapid_binary_classifier.py
 joes_giant_toolbox/all/run_python_function_in_parallel.py
 joes_giant_toolbox/all/scrape_webpage_and_all_linked_webpages.py
 joes_giant_toolbox/all/string_cleaner.py
 joes_giant_toolbox/all/upload_file_python_to_gcloud_bucket.py
 joes_giant_toolbox/all/url_to_filename_to_url_mapper.py
```

### Comparing `joes_giant_toolbox-0.0.1/pyproject.toml` & `joes_giant_toolbox-0.1.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "joes_giant_toolbox"
-version = "0.0.1"
+version = "0.1.0"
 description = "A large collection of general python functions and classes that I use in my daily work"
 readme = "README.md"
 authors = [{ name = "Joseph Bolton", email = "joseph.jazz.bolton@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -17,10 +17,11 @@
 keywords = ["api", "web", "dataviz", "google cloud", "project management", "convenience", "statistics", "hypothesis testing", "machine learning", "NLP"]
 dependencies = []
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 all = ["black", "pytest"]
 doc = ["m2r","sphinx"]
+google = ["db-dtypes==1.0.5", "google-cloud-bigquery-storage==2.18", "google-cloud-compute==1.10.0","google-cloud-logging==3.5.0","google-cloud-storage==2.7.0"]
 
 [project.urls]
 Homepage = "https://github.com/J-sephB-lt-n/joes_giant_toolbox"
```

### Comparing `joes_giant_toolbox-0.0.1/tests/test_longest_sentence_subsequence_plagiarism_detector.py` & `joes_giant_toolbox-0.1.0/tests/test_longest_sentence_subsequence_plagiarism_detector.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,12 @@
-"""
-If this suite of tests is not run as a module, need to run the following additional code: 
-# add the root project directory to the system path:
->>> import sys
->>> import pathlib
->>> parent_dir_path = pathlib.Path(__file__).parent.parent
->>> sys.path.append(str(parent_dir_path))
->>> sys.path.append(f"{str(parent_dir_path)}/joes_giant_toolbox/")
-"""
-
-# import the function to be tested:
-from joes_giant_toolbox.longest_sentence_subsequence_plagiarism_detector import (
-    longest_sentence_subsequence_plagiarism_detector,
-)
+import joes_giant_toolbox.text
 
 # run the tests:
 def test_known_output_example():
-    result = longest_sentence_subsequence_plagiarism_detector(
+    result = joes_giant_toolbox.text.longest_sentence_subsequence_plagiarism_detector(
         doc1_str="cd efg opq rs ab cd efg az by opq rs tu vw xy af gq errty h ijk l mn a b c d e",
         doc2_str="ab cd efg h ijk l mn opq rs tu vw xy z",
         min_seq_len=3,
     )
     assert result == [
         "opq rs tu vw xy",
         "h ijk l mn",
```

### Comparing `joes_giant_toolbox-0.0.1/tests/test_make_url_request.py` & `joes_giant_toolbox-0.1.0/tests/test_make_url_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-# add the root project directory to the system path:
-import sys
-import pathlib
-import json
-import time
-
-parent_dir_path = pathlib.Path(__file__).parent.parent
-sys.path.append(str(parent_dir_path))
-
-# import the function to be tested:
-from joes_giant_toolbox.make_url_request import make_url_request
-
-# run the tests:
-def test_successful_request_with_known_output():
-    """test if expected content can be successfully pulled from a known response URL"""
-    url_response = make_url_request(url="https://jsonplaceholder.typicode.com/todos/1")
-    output = json.loads(url_response["returned_content"])
-    expected_output = {
-        "userId": 1,
-        "id": 1,
-        "title": "delectus aut autem",
-        "completed": False,
-    }
-    assert (
-        output == expected_output
-    ), f"request to known URL produced unexpected result \nReturned: {output}. \nExpected: {expected_output}"
-
-
-def test_url_does_not_exist():
-    """request to a non-existent URL must return no content and no status code"""
-    url_response = make_url_request(url="https://non.existent.website.name/")
-    assert (
-        url_response["returned_content"] is None
-    ), "non-existent website must return no content"
-    assert (
-        url_response["response_status_code"] is None
-    ), "non-existent website must return no status code"
-
-
-def test_request_timeout():
-    """timeout parameter must quickly force the request to stop"""
-    start_time = time.perf_counter()
-    url_response = make_url_request(
-        url="https://hastie.su.domains/Papers/ESLII.pdf", timeout=0.1
-    )
-    end_time = time.perf_counter()
-    assert (
-        end_time - start_time
-    ) < 1.0, "timeout parameter must quickly force the request to stop"
-
-
-def test_efficient_stream_content_from_large_request():
-    """max_bytes parameter must allow quick download of a small amount of information from a large request
-    ..and must stream exactly the right amount
-    """
-    start_time = time.perf_counter()
-    url_response = make_url_request(
-        url="https://hastie.su.domains/Papers/ESLII.pdf", max_bytes=100
-    )
-    end_time = time.perf_counter()
-    assert (
-        url_response["response_status_code"] == 200
-    ), "straightforward request must not be rejected by server"
-    assert (
-        end_time - start_time
-    ) < 5, "small number of requested bytes from large request must complete quickly"
-    assert (
-        len(url_response["returned_content"]) == 100
-    ), "exactly [max_bytes] must be returned"
+# # add the root project directory to the system path:
+# import sys
+# import pathlib
+# import json
+# import time
+
+# parent_dir_path = pathlib.Path(__file__).parent.parent
+# sys.path.append(str(parent_dir_path))
+
+# # import the function to be tested:
+# from joes_giant_toolbox.make_url_request import make_url_request
+
+# # run the tests:
+# def test_successful_request_with_known_output():
+#     """test if expected content can be successfully pulled from a known response URL"""
+#     url_response = make_url_request(url="https://jsonplaceholder.typicode.com/todos/1")
+#     output = json.loads(url_response["returned_content"])
+#     expected_output = {
+#         "userId": 1,
+#         "id": 1,
+#         "title": "delectus aut autem",
+#         "completed": False,
+#     }
+#     assert (
+#         output == expected_output
+#     ), f"request to known URL produced unexpected result \nReturned: {output}. \nExpected: {expected_output}"
+
+
+# def test_url_does_not_exist():
+#     """request to a non-existent URL must return no content and no status code"""
+#     url_response = make_url_request(url="https://non.existent.website.name/")
+#     assert (
+#         url_response["returned_content"] is None
+#     ), "non-existent website must return no content"
+#     assert (
+#         url_response["response_status_code"] is None
+#     ), "non-existent website must return no status code"
+
+
+# def test_request_timeout():
+#     """timeout parameter must quickly force the request to stop"""
+#     start_time = time.perf_counter()
+#     url_response = make_url_request(
+#         url="https://hastie.su.domains/Papers/ESLII.pdf", timeout=0.1
+#     )
+#     end_time = time.perf_counter()
+#     assert (
+#         end_time - start_time
+#     ) < 1.0, "timeout parameter must quickly force the request to stop"
+
+
+# def test_efficient_stream_content_from_large_request():
+#     """max_bytes parameter must allow quick download of a small amount of information from a large request
+#     ..and must stream exactly the right amount
+#     """
+#     start_time = time.perf_counter()
+#     url_response = make_url_request(
+#         url="https://hastie.su.domains/Papers/ESLII.pdf", max_bytes=100
+#     )
+#     end_time = time.perf_counter()
+#     assert (
+#         url_response["response_status_code"] == 200
+#     ), "straightforward request must not be rejected by server"
+#     assert (
+#         end_time - start_time
+#     ) < 5, "small number of requested bytes from large request must complete quickly"
+#     assert (
+#         len(url_response["returned_content"]) == 100
+#     ), "exactly [max_bytes] must be returned"
```

### Comparing `joes_giant_toolbox-0.0.1/tests/test_rapid_binary_classifier.py` & `joes_giant_toolbox-0.1.0/tests/test_rapid_binary_classifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-import sys
-import pathlib
-import pathlib
-import subprocess
-import pandas as pd
-import sklearn
-import sklearn.preprocessing
-import sklearn.model_selection
-import sklearn.naive_bayes
-import sklearn.tree
-import sklearn.linear_model
-import sklearn.neural_network
-import sklearn.discriminant_analysis
-import sklearn.ensemble
-import sklearn.gaussian_process
-import sklearn.metrics
-import sklearn.calibration
-from matplotlib import pyplot as plt
-
-# add the root project directory to the system path #
-parent_dir_path = pathlib.Path(__file__).parent.parent
-sys.path.append(str(parent_dir_path))
-
-# import the function to be tested:
-from joes_giant_toolbox.rapid_binary_classifier import RapidBinaryClassifier
-
-# run the tests #
-def test_good_performance_cleveland_heart_disease_dataset():
-    """This test checks that the process can produce a model which achieves an ROC/AUC score of at least 0.85 on the Cleveland Heart Dataset:
-
-    1. Using the methods in the class directly
-    2. Exporting the full auto-generated script and running it
-    """
-    data_df = pd.read_csv(
-        "https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data",
-        sep=",",
-        header=None,
-        names=[
-            "age",
-            "sex",
-            "chest_pain_type",
-            "resting_blood_pressure",
-            "serum_cholesterol_mg_dl",
-            "fasting_blood_sugar",
-            "resting_electrocardiographic_results",
-            "maximum_heart_rate_achieved",
-            "exercise_induced_angina",
-            "st_depression_induced_by_exercise_relative_to_rest",
-            "slope_of_peak_exercise_st_segment",
-            "num_major_vessels_colored_by_flourosopy",
-            "thal",
-            "angiographic_disease_status",
-        ],
-        dtype=float,
-        skiprows=[87, 166, 192, 266, 287, 302],  # rows with missing values
-    )
-    data_df["heart_disease_yes_no"] = (
-        data_df["angiographic_disease_status"] > 0
-    ).astype(int)
-    # data_df.nunique()
-    sk_classifier = RapidBinaryClassifier(
-        data_df=data_df, verbose=False, eval_code=True
-    )
-    sk_classifier.set_variable_roles_in_model(
-        y_varname="heart_disease_yes_no",
-        x_numeric_varnames=[
-            "age",
-            "resting_blood_pressure",
-            "serum_cholesterol_mg_dl",
-            "maximum_heart_rate_achieved",
-            "st_depression_induced_by_exercise_relative_to_rest",
-        ],
-        x_categorical_varnames=[
-            "sex",
-            "chest_pain_type",
-            "fasting_blood_sugar",
-            "resting_electrocardiographic_results",
-            "exercise_induced_angina",
-            "slope_of_peak_exercise_st_segment",
-            "num_major_vessels_colored_by_flourosopy",
-            "thal",
-        ],
-    )
-    sk_classifier.generate_train_test_split(test_percent=0.2)
-    sk_classifier.transform_x_features(rare_category_min_freq=20)
-    sk_classifier.define_models(
-        {
-            "adaboost": sklearn.ensemble.AdaBoostClassifier(),
-            "decision_tree": sklearn.tree.DecisionTreeClassifier(),
-            "extremely_random_trees": sklearn.ensemble.ExtraTreesClassifier(),
-            "gaussian_naive_bayes": sklearn.naive_bayes.GaussianNB(),
-            "gaussian_process": sklearn.gaussian_process.GaussianProcessClassifier(),
-            "hist_gbm": sklearn.ensemble.HistGradientBoostingClassifier(),
-            "logistic_regression": sklearn.linear_model.LogisticRegression(
-                penalty=None,
-                max_iter=1_000,
-            ),
-            "neural_net": sklearn.neural_network.MLPClassifier(
-                hidden_layer_sizes=(50, 30, 10, 5), activation="relu", max_iter=1_000
-            ),
-            "quadratic_discriminant_analysis": sklearn.discriminant_analysis.QuadraticDiscriminantAnalysis(),
-            "random_forest": sklearn.ensemble.RandomForestClassifier(),
-        }
-    )
-    all_model_names = list(sk_classifier.sklearn_components["models"].keys())
-    sk_classifier.fit_cross_valid_models(
-        k_folds=4,
-        model_names_list=all_model_names,
-    )
-    # sk_classifier.compare_models_cross_valid_roc_auc()
-    sk_classifier.add_ensemble_model(
-        ensemble_name="weighted_avg_ensemble_all_models",
-        model_names_list=all_model_names,
-        combine_strategy="weighted_average",
-    )
-    sk_classifier.add_ensemble_model(
-        ensemble_name="stacked_classifier_ensemble_all_models",
-        model_names_list=all_model_names,
-        combine_strategy="stacked_classifier",
-        meta_model=sklearn.ensemble.HistGradientBoostingClassifier(),
-    )
-    sk_classifier.fit_cross_valid_models(
-        k_folds=4,
-        model_names_list=[
-            "weighted_avg_ensemble_all_models",
-            "stacked_classifier_ensemble_all_models",
-        ],
-    )
-    per_model_mean_cross_valid_test_score = {
-        model_name: sk_classifier.sklearn_components["k_fold_cv_results"][model_name][
-            "test_score"
-        ].mean()
-        for model_name in sk_classifier.sklearn_components["k_fold_cv_results"]
-    }
-    best_model_name_cross_valid_test = max(
-        per_model_mean_cross_valid_test_score,
-        key=per_model_mean_cross_valid_test_score.get,
-    )
-    # sk_classifier.compare_models_cross_valid_roc_auc()
-    sk_classifier.fit_models(model_names_list=[best_model_name_cross_valid_test])
-    sk_classifier.generate_test_set_predictions(
-        model_names_list=[best_model_name_cross_valid_test]
-    )
-    test_data_roc_auc = sklearn.metrics.roc_auc_score(
-        y_true=sk_classifier.data["y_test_for_model"],
-        y_score=sk_classifier.sklearn_components["test_set_predictions"][
-            best_model_name_cross_valid_test
-        ],
-    )
-
-    assert (
-        test_data_roc_auc >= 0.85
-    ), f"Best model ({best_model_name_cross_valid_test}) achieved roc_auc={test_data_roc_auc:.3f} on Cleveland Heart Dataset (test partition) - should achieve at least 0.85"
-
-    edit_full_model_script = (
-        sk_classifier.full_model_script.replace(
-            r"data_df = pd.read_csv(...)",
-            r"""data_df = pd.read_csv(
-        "https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data",
-        sep=",",
-        header=None,
-        names=[
-            "age",
-            "sex",
-            "chest_pain_type",
-            "resting_blood_pressure",
-            "serum_cholesterol_mg_dl",
-            "fasting_blood_sugar",
-            "resting_electrocardiographic_results",
-            "maximum_heart_rate_achieved",
-            "exercise_induced_angina",
-            "st_depression_induced_by_exercise_relative_to_rest",
-            "slope_of_peak_exercise_st_segment",
-            "num_major_vessels_colored_by_flourosopy",
-            "thal",
-            "angiographic_disease_status",
-        ],
-        dtype=float,
-        skiprows=[87, 166, 192, 266, 287, 302],  # rows with missing values
-)
-data_df["heart_disease_yes_no"] = (data_df["angiographic_disease_status"] > 0).astype(int)""",
-        )
-        + f"""
-test_data_roc_auc = sklearn.metrics.roc_auc_score(
-    y_true=y_test_for_model,
-    y_score=test_data_predictions[models_to_predict_list[0]],
-)    
-with open("temp_external_script_output.txt", "w") as f:   
-        f.write(f"{{models_to_predict_list[0]}}{{chr(10)}}")
-        f.write(f"{{test_data_roc_auc:.3f}}")
-    """
-    )
-    try:
-        with open("temp_model_script.py", "w") as f:
-            f.write(edit_full_model_script)
-        subprocess.run(["python", "temp_model_script.py"])
-        with open("temp_external_script_output.txt", "r") as f:
-            external_script_output_list = [x.strip() for x in f.readlines()]
-        best_external_model_name = external_script_output_list[0]
-        external_best_roc_auc = float(external_script_output_list[1])
-        assert (
-            external_best_roc_auc >= 0.85
-        ), f"External script best model ({best_external_model_name}) achieved roc_auc={external_best_roc_auc} on Cleveland Heart Dataset (test partition) - should achieve at least 0.85"
-    except:
-        pass
-    finally:
-        for filename in ["temp_external_script_output.txt", "temp_model_script.py"]:
-            pathlib.Path(filename).unlink(missing_ok=True)
+# import sys
+# import pathlib
+# import pathlib
+# import subprocess
+# import pandas as pd
+# import sklearn
+# import sklearn.preprocessing
+# import sklearn.model_selection
+# import sklearn.naive_bayes
+# import sklearn.tree
+# import sklearn.linear_model
+# import sklearn.neural_network
+# import sklearn.discriminant_analysis
+# import sklearn.ensemble
+# import sklearn.gaussian_process
+# import sklearn.metrics
+# import sklearn.calibration
+# from matplotlib import pyplot as plt
+
+# # add the root project directory to the system path #
+# parent_dir_path = pathlib.Path(__file__).parent.parent
+# sys.path.append(str(parent_dir_path))
+
+# # import the function to be tested:
+# from joes_giant_toolbox.rapid_binary_classifier import RapidBinaryClassifier
+
+# # run the tests #
+# def test_good_performance_cleveland_heart_disease_dataset():
+#     """This test checks that the process can produce a model which achieves an ROC/AUC score of at least 0.85 on the Cleveland Heart Dataset:
+
+#     1. Using the methods in the class directly
+#     2. Exporting the full auto-generated script and running it
+#     """
+#     data_df = pd.read_csv(
+#         "https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data",
+#         sep=",",
+#         header=None,
+#         names=[
+#             "age",
+#             "sex",
+#             "chest_pain_type",
+#             "resting_blood_pressure",
+#             "serum_cholesterol_mg_dl",
+#             "fasting_blood_sugar",
+#             "resting_electrocardiographic_results",
+#             "maximum_heart_rate_achieved",
+#             "exercise_induced_angina",
+#             "st_depression_induced_by_exercise_relative_to_rest",
+#             "slope_of_peak_exercise_st_segment",
+#             "num_major_vessels_colored_by_flourosopy",
+#             "thal",
+#             "angiographic_disease_status",
+#         ],
+#         dtype=float,
+#         skiprows=[87, 166, 192, 266, 287, 302],  # rows with missing values
+#     )
+#     data_df["heart_disease_yes_no"] = (
+#         data_df["angiographic_disease_status"] > 0
+#     ).astype(int)
+#     # data_df.nunique()
+#     sk_classifier = RapidBinaryClassifier(
+#         data_df=data_df, verbose=False, eval_code=True
+#     )
+#     sk_classifier.set_variable_roles_in_model(
+#         y_varname="heart_disease_yes_no",
+#         x_numeric_varnames=[
+#             "age",
+#             "resting_blood_pressure",
+#             "serum_cholesterol_mg_dl",
+#             "maximum_heart_rate_achieved",
+#             "st_depression_induced_by_exercise_relative_to_rest",
+#         ],
+#         x_categorical_varnames=[
+#             "sex",
+#             "chest_pain_type",
+#             "fasting_blood_sugar",
+#             "resting_electrocardiographic_results",
+#             "exercise_induced_angina",
+#             "slope_of_peak_exercise_st_segment",
+#             "num_major_vessels_colored_by_flourosopy",
+#             "thal",
+#         ],
+#     )
+#     sk_classifier.generate_train_test_split(test_percent=0.2)
+#     sk_classifier.transform_x_features(rare_category_min_freq=20)
+#     sk_classifier.define_models(
+#         {
+#             "adaboost": sklearn.ensemble.AdaBoostClassifier(),
+#             "decision_tree": sklearn.tree.DecisionTreeClassifier(),
+#             "extremely_random_trees": sklearn.ensemble.ExtraTreesClassifier(),
+#             "gaussian_naive_bayes": sklearn.naive_bayes.GaussianNB(),
+#             "gaussian_process": sklearn.gaussian_process.GaussianProcessClassifier(),
+#             "hist_gbm": sklearn.ensemble.HistGradientBoostingClassifier(),
+#             "logistic_regression": sklearn.linear_model.LogisticRegression(
+#                 penalty=None,
+#                 max_iter=1_000,
+#             ),
+#             "neural_net": sklearn.neural_network.MLPClassifier(
+#                 hidden_layer_sizes=(50, 30, 10, 5), activation="relu", max_iter=1_000
+#             ),
+#             "quadratic_discriminant_analysis": sklearn.discriminant_analysis.QuadraticDiscriminantAnalysis(),
+#             "random_forest": sklearn.ensemble.RandomForestClassifier(),
+#         }
+#     )
+#     all_model_names = list(sk_classifier.sklearn_components["models"].keys())
+#     sk_classifier.fit_cross_valid_models(
+#         k_folds=4,
+#         model_names_list=all_model_names,
+#     )
+#     # sk_classifier.compare_models_cross_valid_roc_auc()
+#     sk_classifier.add_ensemble_model(
+#         ensemble_name="weighted_avg_ensemble_all_models",
+#         model_names_list=all_model_names,
+#         combine_strategy="weighted_average",
+#     )
+#     sk_classifier.add_ensemble_model(
+#         ensemble_name="stacked_classifier_ensemble_all_models",
+#         model_names_list=all_model_names,
+#         combine_strategy="stacked_classifier",
+#         meta_model=sklearn.ensemble.HistGradientBoostingClassifier(),
+#     )
+#     sk_classifier.fit_cross_valid_models(
+#         k_folds=4,
+#         model_names_list=[
+#             "weighted_avg_ensemble_all_models",
+#             "stacked_classifier_ensemble_all_models",
+#         ],
+#     )
+#     per_model_mean_cross_valid_test_score = {
+#         model_name: sk_classifier.sklearn_components["k_fold_cv_results"][model_name][
+#             "test_score"
+#         ].mean()
+#         for model_name in sk_classifier.sklearn_components["k_fold_cv_results"]
+#     }
+#     best_model_name_cross_valid_test = max(
+#         per_model_mean_cross_valid_test_score,
+#         key=per_model_mean_cross_valid_test_score.get,
+#     )
+#     # sk_classifier.compare_models_cross_valid_roc_auc()
+#     sk_classifier.fit_models(model_names_list=[best_model_name_cross_valid_test])
+#     sk_classifier.generate_test_set_predictions(
+#         model_names_list=[best_model_name_cross_valid_test]
+#     )
+#     test_data_roc_auc = sklearn.metrics.roc_auc_score(
+#         y_true=sk_classifier.data["y_test_for_model"],
+#         y_score=sk_classifier.sklearn_components["test_set_predictions"][
+#             best_model_name_cross_valid_test
+#         ],
+#     )
+
+#     assert (
+#         test_data_roc_auc >= 0.85
+#     ), f"Best model ({best_model_name_cross_valid_test}) achieved roc_auc={test_data_roc_auc:.3f} on Cleveland Heart Dataset (test partition) - should achieve at least 0.85"
+
+#     edit_full_model_script = (
+#         sk_classifier.full_model_script.replace(
+#             r"data_df = pd.read_csv(...)",
+#             r"""data_df = pd.read_csv(
+#         "https://archive.ics.uci.edu/ml/machine-learning-databases/heart-disease/processed.cleveland.data",
+#         sep=",",
+#         header=None,
+#         names=[
+#             "age",
+#             "sex",
+#             "chest_pain_type",
+#             "resting_blood_pressure",
+#             "serum_cholesterol_mg_dl",
+#             "fasting_blood_sugar",
+#             "resting_electrocardiographic_results",
+#             "maximum_heart_rate_achieved",
+#             "exercise_induced_angina",
+#             "st_depression_induced_by_exercise_relative_to_rest",
+#             "slope_of_peak_exercise_st_segment",
+#             "num_major_vessels_colored_by_flourosopy",
+#             "thal",
+#             "angiographic_disease_status",
+#         ],
+#         dtype=float,
+#         skiprows=[87, 166, 192, 266, 287, 302],  # rows with missing values
+# )
+# data_df["heart_disease_yes_no"] = (data_df["angiographic_disease_status"] > 0).astype(int)""",
+#         )
+#         + f"""
+# test_data_roc_auc = sklearn.metrics.roc_auc_score(
+#     y_true=y_test_for_model,
+#     y_score=test_data_predictions[models_to_predict_list[0]],
+# )
+# with open("temp_external_script_output.txt", "w") as f:
+#         f.write(f"{{models_to_predict_list[0]}}{{chr(10)}}")
+#         f.write(f"{{test_data_roc_auc:.3f}}")
+#     """
+#     )
+#     try:
+#         with open("temp_model_script.py", "w") as f:
+#             f.write(edit_full_model_script)
+#         subprocess.run(["python", "temp_model_script.py"])
+#         with open("temp_external_script_output.txt", "r") as f:
+#             external_script_output_list = [x.strip() for x in f.readlines()]
+#         best_external_model_name = external_script_output_list[0]
+#         external_best_roc_auc = float(external_script_output_list[1])
+#         assert (
+#             external_best_roc_auc >= 0.85
+#         ), f"External script best model ({best_external_model_name}) achieved roc_auc={external_best_roc_auc} on Cleveland Heart Dataset (test partition) - should achieve at least 0.85"
+#     except:
+#         pass
+#     finally:
+#         for filename in ["temp_external_script_output.txt", "temp_model_script.py"]:
+#             pathlib.Path(filename).unlink(missing_ok=True)
```

### Comparing `joes_giant_toolbox-0.0.1/tests/test_string_cleaner.py` & `joes_giant_toolbox-0.1.0/tests/test_string_cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-# # add the root project directory to the system path:
-# import sys
-# import pathlib
+import joes_giant_toolbox.text
 
-# parent_dir_path = pathlib.Path(__file__).parent.parent
-# sys.path.append(str(parent_dir_path))
-
-# # import the function to be tested:
-# from joes_giant_toolbox.string_cleaner import StringCleaner
+string_cleaner = joes_giant_toolbox.text.StringCleaner()
 
 # # run the tests:
 # def test_remove_words_or_phrases():
 #     """Confirms that the remove_words_or_phrases() function works as expected, both in isolation and within a chained sequence of cleaning operations"""
 #     string_cleaner = StringCleaner()
 
 #     # test 1 #
```

