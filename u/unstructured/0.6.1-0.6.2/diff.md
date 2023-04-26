# Comparing `tmp/unstructured-0.6.1.tar.gz` & `tmp/unstructured-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured-0.6.1.tar", last modified: Fri Apr 21 18:50:55 2023, max compression
+gzip compressed data, was "unstructured-0.6.2.tar", last modified: Wed Apr 26 20:32:28 2023, max compression
```

## Comparing `unstructured-0.6.1.tar` & `unstructured-0.6.2.tar`

### file list

```diff
@@ -1,104 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.106627 unstructured-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-21 18:50:46.000000 unstructured-0.6.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 18:50:55.106627 unstructured-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-21 18:50:46.000000 unstructured-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-21 18:50:55.106627 unstructured-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-21 18:50:47.000000 unstructured-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/test_unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/test_unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/mock_nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/test_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/nlp/test_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-21 18:50:47.000000 unstructured-0.6.1/test_unstructured/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/cleaners/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/cleaners/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/email_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/documents/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/file_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/file_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/google_filetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/file_utils/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/ingest/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/biomed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/google_drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/reddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/connector/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/ingest/doc_processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/doc_processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/doc_processor/generalized.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/ingest/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.098627 unstructured-0.6.1/unstructured/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.102627 unstructured-0.6.1/unstructured/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/english-words.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/english_words.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/nlp/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.102627 unstructured-0.6.1/unstructured/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/md.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/msg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/ppt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/rtf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/text.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/partition/text_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.106627 unstructured-0.6.1/unstructured/staging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/argilla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/datasaur.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/label_box.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/staging/prodigy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-21 18:50:47.000000 unstructured-0.6.1/unstructured/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 18:50:55.094627 unstructured-0.6.1/unstructured.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-04-21 18:50:55.000000 unstructured-0.6.1/unstructured.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-21 18:50:54.000000 unstructured-0.6.1/unstructured.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-26 20:32:16.000000 unstructured-0.6.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-26 20:32:28.080474 unstructured-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16619 2023-04-26 20:32:16.000000 unstructured-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-26 20:32:28.080474 unstructured-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-26 20:32:16.000000 unstructured-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/test_unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/test_unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/mock_nltk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/test_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/nlp/test_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-26 20:32:16.000000 unstructured-0.6.2/test_unstructured/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/cleaners/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/cleaners/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/email_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/documents/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/file_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/file_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/google_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/file_utils/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/biomed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11172 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/google_drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3891 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7517 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5411 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/connector/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/ingest/doc_processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/doc_processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/doc_processor/generalized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27999 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/ingest/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.072474 unstructured-0.6.2/unstructured/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.076474 unstructured-0.6.2/unstructured/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4472047 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/english-words.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/english_words.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/nlp/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/unstructured/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12640 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/ppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/rtf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/partition/text_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.080474 unstructured-0.6.2/unstructured/staging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/argilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/datasaur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/label_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/staging/prodigy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-26 20:32:16.000000 unstructured-0.6.2/unstructured/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 20:32:28.068474 unstructured-0.6.2/unstructured.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20852 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-26 20:32:28.000000 unstructured-0.6.2/unstructured.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-26 20:32:27.000000 unstructured-0.6.2/unstructured.egg-info/top_level.txt
```

### Comparing `unstructured-0.6.1/LICENSE.md` & `unstructured-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/PKG-INFO` & `unstructured-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.1 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.2 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.1/README.md` & `unstructured-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/setup.py` & `unstructured-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/test_unstructured/nlp/mock_nltk.py` & `unstructured-0.6.2/test_unstructured/nlp/mock_nltk.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/test_unstructured/nlp/test_tokenize.py` & `unstructured-0.6.2/test_unstructured/nlp/test_tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/test_unstructured/test_utils.py` & `unstructured-0.6.2/test_unstructured/test_utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/cleaners/core.py` & `unstructured-0.6.2/unstructured/cleaners/core.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/cleaners/extract.py` & `unstructured-0.6.2/unstructured/cleaners/extract.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/cleaners/translate.py` & `unstructured-0.6.2/unstructured/cleaners/translate.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/documents/base.py` & `unstructured-0.6.2/unstructured/documents/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/documents/elements.py` & `unstructured-0.6.2/unstructured/documents/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/documents/email_elements.py` & `unstructured-0.6.2/unstructured/documents/email_elements.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/documents/html.py` & `unstructured-0.6.2/unstructured/documents/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/documents/xml.py` & `unstructured-0.6.2/unstructured/documents/xml.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/file_utils/exploration.py` & `unstructured-0.6.2/unstructured/file_utils/exploration.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/file_utils/file_conversion.py` & `unstructured-0.6.2/unstructured/file_utils/file_conversion.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/file_utils/filetype.py` & `unstructured-0.6.2/unstructured/file_utils/filetype.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
+import re
 import zipfile
 from enum import Enum
 from typing import IO, Optional
 
+from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import exactly_one
 
 try:
     import magic
 
     LIBMAGIC_AVAILABLE = True
 except ImportError:  # pragma: nocover
@@ -165,15 +167,16 @@
 def detect_filetype(
     filename: Optional[str] = None,
     content_type: Optional[str] = None,
     file: Optional[IO] = None,
     file_filename: Optional[str] = None,
 ) -> Optional[FileType]:
     """Use libmagic to determine a file's type. Helps determine which partition brick
-    to use for a given file. A return value of None indicates a non-supported file type."""
+    to use for a given file. A return value of None indicates a non-supported file type.
+    """
     exactly_one(filename=filename, file=file)
 
     if content_type:
         filetype = STR_TO_FILETYPE.get(content_type)
         if filetype:
             return filetype
 
@@ -235,36 +238,36 @@
         return FileType.EPUB
 
     # NOTE(robinson) - examples are application/rtf or text/rtf.
     # magic often returns text/plain for RTF files
     elif mime_type.endswith("rtf"):
         return FileType.RTF
 
-    elif mime_type in TXT_MIME_TYPES:
-        if extension and extension == ".eml":
-            return FileType.EML
-        elif extension and extension == ".md":
-            return FileType.MD
-        elif extension and extension == ".rtf":
-            return FileType.RTF
-
-        if file and not extension and _check_eml_from_buffer(file=file) is True:
-            return FileType.EML
-        return FileType.TXT
-
     elif mime_type.endswith("xml"):
         if extension and extension == ".html":
             return FileType.HTML
         else:
             return FileType.XML
 
     elif mime_type == "text/html":
         return FileType.HTML
 
-    elif mime_type.startswith("text"):
+    elif mime_type in TXT_MIME_TYPES or mime_type.startswith("text"):
+        if extension and extension == ".eml":
+            return FileType.EML
+        elif extension and extension == ".md":
+            return FileType.MD
+        elif extension and extension == ".rtf":
+            return FileType.RTF
+
+        if _is_text_file_a_json(file=file, filename=filename):
+            return FileType.JSON
+
+        if file and not extension and _check_eml_from_buffer(file=file) is True:
+            return FileType.EML
         return FileType.TXT
 
     elif mime_type in XLSX_MIME_TYPES:
         return FileType.XLSX
 
     elif mime_type in XLS_MIME_TYPES:
         return FileType.XLS
@@ -313,18 +316,43 @@
         if all(f in archive_filenames for f in EXPECTED_DOCX_FILES):
             return FileType.DOCX
         elif all(f in archive_filenames for f in EXPECTED_XLSX_FILES):
             return FileType.XLSX
         elif all(f in archive_filenames for f in EXPECTED_PPTX_FILES):
             return FileType.PPTX
 
-    logger.warning("Could not detect the filetype from application/octet-stream MIME type.")
+    logger.warning(
+        "Could not detect the filetype from application/octet-stream MIME type.",
+    )
     return FileType.UNK
 
 
+def _is_text_file_a_json(
+    filename: Optional[str] = None,
+    content_type: Optional[str] = None,
+    file: Optional[IO] = None,
+):
+    """Detects if a file that has a text/plain MIME type is a JSON file."""
+    exactly_one(filename=filename, file=file)
+
+    if file is not None:
+        file.seek(0)
+        file_content = file.read(4096)
+        if isinstance(file_content, str):
+            file_text = file_content
+        else:
+            file_text = file_content.decode()
+        file.seek(0)
+    elif filename is not None:
+        with open(filename) as f:
+            file_text = f.read()
+
+    return re.match(LIST_OF_DICTS_PATTERN, file_text) is not None
+
+
 def _check_eml_from_buffer(file: IO) -> bool:
     """Checks if a text/plain file is actually a .eml file. Uses a regex pattern to see if the
     start of the file matches the typical pattern for a .eml file."""
     file.seek(0)
     file_content = file.read(4096)
     if isinstance(file_content, bytes):
         file_head = file_content.decode("utf-8")
```

### Comparing `unstructured-0.6.1/unstructured/file_utils/metadata.py` & `unstructured-0.6.2/unstructured/file_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/azure.py` & `unstructured-0.6.2/unstructured/ingest/connector/azure.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/biomed.py` & `unstructured-0.6.2/unstructured/ingest/connector/biomed.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/fsspec.py` & `unstructured-0.6.2/unstructured/ingest/connector/fsspec.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/git.py` & `unstructured-0.6.2/unstructured/ingest/connector/git.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/github.py` & `unstructured-0.6.2/unstructured/ingest/connector/github.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/gitlab.py` & `unstructured-0.6.2/unstructured/ingest/connector/gitlab.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/google_drive.py` & `unstructured-0.6.2/unstructured/ingest/connector/google_drive.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/local.py` & `unstructured-0.6.2/unstructured/ingest/connector/local.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/reddit.py` & `unstructured-0.6.2/unstructured/ingest/connector/reddit.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/s3.py` & `unstructured-0.6.2/unstructured/ingest/connector/s3.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/slack.py` & `unstructured-0.6.2/unstructured/ingest/connector/slack.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/connector/wikipedia.py` & `unstructured-0.6.2/unstructured/ingest/connector/wikipedia.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/doc_processor/generalized.py` & `unstructured-0.6.2/unstructured/ingest/doc_processor/generalized.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/interfaces.py` & `unstructured-0.6.2/unstructured/ingest/interfaces.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/ingest/main.py` & `unstructured-0.6.2/unstructured/ingest/main.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/nlp/english-words.txt` & `unstructured-0.6.2/unstructured/nlp/english-words.txt`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/nlp/english_words.py` & `unstructured-0.6.2/unstructured/nlp/english_words.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/nlp/patterns.py` & `unstructured-0.6.2/unstructured/nlp/patterns.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,7 +90,15 @@
 
 # Date, time, timezone example: Fri, 26 Mar 2021 11:04:09 +1200
 EMAIL_DATETIMETZ_PATTERN = "[a-zA-z]{3},\s[0-9]{2}\s[a-zA-Z]{3}\s[0-9]{4}\s[0-9]{2}:[0-9]{2}:[0-9]{2}\s[+0-9]{5}"  # noqa: W605,E501
 # NOTE(harrell) - skipping qa because we need the escape for the regex
 
 EMAIL_ADDRESS_PATTERN = "[a-z0-9\.\-+_]+@[a-z0-9\.\-+_]+\.[a-z]+"  # noqa: W605 NOTE(harrell)
 # - skipping qa because we need the escape for the regex
+
+
+ENDS_IN_PUNCT_PATTERN = r"[^\w\s]\Z"
+ENDS_IN_PUNCT_RE = re.compile(ENDS_IN_PUNCT_PATTERN)
+
+# NOTE(robinson) - Used to detect if text is in the expected "list of dicts"
+# format for document elements
+LIST_OF_DICTS_PATTERN = r"\A\s*\[\s*{?"
```

### Comparing `unstructured-0.6.1/unstructured/nlp/tokenize.py` & `unstructured-0.6.2/unstructured/nlp/tokenize.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/__init__.py` & `unstructured-0.6.2/unstructured/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/auto.py` & `unstructured-0.6.2/unstructured/partition/auto.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/common.py` & `unstructured-0.6.2/unstructured/partition/common.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/doc.py` & `unstructured-0.6.2/unstructured/partition/doc.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/docx.py` & `unstructured-0.6.2/unstructured/partition/docx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/email.py` & `unstructured-0.6.2/unstructured/partition/email.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/epub.py` & `unstructured-0.6.2/unstructured/partition/epub.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/html.py` & `unstructured-0.6.2/unstructured/partition/html.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/image.py` & `unstructured-0.6.2/unstructured/partition/image.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/json.py` & `unstructured-0.6.2/unstructured/partition/json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import json
 import re
 from typing import IO, List, Optional
 
 from unstructured.documents.elements import Element
+from unstructured.nlp.patterns import LIST_OF_DICTS_PATTERN
 from unstructured.partition.common import exactly_one
 from unstructured.staging.base import dict_to_elements
 
-LIST_OF_DICTS_PATTERN = r"\A\s*\[\s*{?"
-
 
 def partition_json(
     filename: Optional[str] = None,
     file: Optional[IO] = None,
     text: Optional[str] = None,
 ) -> List[Element]:
     """Partitions an .json document into its constituent elements."""
@@ -20,15 +19,20 @@
 
     exactly_one(filename=filename, file=file, text=text)
 
     if filename is not None:
         with open(filename, encoding="utf8") as f:
             file_text = f.read()
     elif file is not None:
-        file_text = file.read()
+        file_content = file.read()
+        if isinstance(file_content, str):
+            file_text = file_content
+        else:
+            file_text = file_content.decode()
+        file.seek(0)
     elif text is not None:
         file_text = str(text)
 
     # NOTE(Nathan): we expect file_text to be a list of dicts (optimization)
     if not re.match(LIST_OF_DICTS_PATTERN, file_text):
         raise ValueError("Json schema does not match the Unstructured schema")
```

### Comparing `unstructured-0.6.1/unstructured/partition/md.py` & `unstructured-0.6.2/unstructured/partition/md.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/msg.py` & `unstructured-0.6.2/unstructured/partition/msg.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/pdf.py` & `unstructured-0.6.2/unstructured/partition/pdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import warnings
 from io import StringIO
 from typing import BinaryIO, List, Optional, cast
 
+from pdfminer.pdfpage import PDFPage, PDFTextExtractionNotAllowed
+from pdfminer.utils import open_filename
+
 from unstructured.documents.elements import Element, ElementMetadata, PageBreak
 from unstructured.logger import logger
 from unstructured.partition import _partition_via_api
 from unstructured.partition.common import (
     add_element_metadata,
     document_to_element_list,
     exactly_one,
@@ -95,39 +98,57 @@
         route_args = template.strip("/").split("/")
         is_image = route_args[-1] == "image"
         out_template: Optional[str] = template
         if route_args[0] == "layout":
             out_template = None
 
         fallback_to_fast = False
+        fallback_to_hi_res = False
+
         detectron2_installed = dependency_exists("detectron2")
+        if is_image:
+            pdf_text_extractable = False
+        else:
+            pdf_text_extractable = is_pdf_text_extractable(filename=filename, file=file)
+            if file is not None:
+                file.seek(0)  # type: ignore
+
+        if not detectron2_installed and not pdf_text_extractable:
+            raise ValueError(
+                "detectron2 is not installed and the text of the PDF is not extractable. "
+                "To process this file, install detectron2 or remove copy protection from the PDF.",
+            )
+
+        if not pdf_text_extractable:
+            fallback_to_hi_res = strategy == "fast"
 
         if not detectron2_installed:
-            if is_image:
-                raise ValueError(
-                    "detectron2 is not installed. detectron2 is required for partioning images.",
+            fallback_to_fast = strategy == "hi_res"
+
+        if (strategy == "hi_res" or fallback_to_hi_res) and not fallback_to_fast:
+            if strategy == "fast":
+                logger.warning(
+                    "PDF text is not extractable. Cannot use the fast partitioning "
+                    "strategy. Falling back to partitioning with the hi_res strategy.",
                 )
-            else:
-                fallback_to_fast = True
 
-        if strategy == "hi_res" and not fallback_to_fast:
             # NOTE(robinson): Catches a UserWarning that occurs when detectron is called
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 layout_elements = _partition_pdf_or_image_local(
                     filename=filename,
                     file=file,
                     template=out_template,
                     is_image=is_image,
                     infer_table_structure=infer_table_structure,
                     include_page_breaks=True,
                     ocr_languages=ocr_languages,
                 )
 
-        elif strategy == "fast" or fallback_to_fast:
+        elif (strategy == "fast" or fallback_to_fast) and not fallback_to_hi_res:
             if strategy == "hi_res":
                 logger.warning(
                     "detectron2 is not installed. Cannot use the hi_res partitioning "
                     "strategy. Falling back to partitioning with the fast strategy.",
                 )
             if infer_table_structure:
                 logger.warning(
@@ -230,17 +251,14 @@
     processing or detectron2 is not available.
 
     Implementation is based on the `extract_text` implemenation in pdfminer.six, but
     modified to support tracking page numbers and working with file-like objects.
 
     ref: https://github.com/pdfminer/pdfminer.six/blob/master/pdfminer/high_level.py
     """
-
-    from pdfminer.utils import open_filename
-
     exactly_one(filename=filename, file=file)
     if filename:
         with open_filename(filename, "rb") as fp:
             fp = cast(BinaryIO, fp)
             elements = _process_pdfminer_pages(
                 fp=fp,
                 filename=filename,
@@ -266,22 +284,21 @@
     encoding: str = "utf-8",
     include_page_breaks: bool = False,
 ):
     """Uses PDF miner to split a document into pages and process them."""
     from pdfminer.converter import TextConverter
     from pdfminer.layout import LAParams
     from pdfminer.pdfinterp import PDFPageInterpreter, PDFResourceManager
-    from pdfminer.pdfpage import PDFPage
 
     rsrcmgr = PDFResourceManager(caching=False)
     laparams = LAParams()
 
     elements: List[Element] = []
 
-    for i, page in enumerate(PDFPage.get_pages(fp)):
+    for i, page in enumerate(PDFPage.get_pages(fp, check_extractable=True)):
         metadata = ElementMetadata(filename=filename, page_number=i + 1)
         with StringIO() as output_string:
             device = TextConverter(
                 rsrcmgr,
                 output_string,
                 codec=encoding,
                 laparams=laparams,
@@ -294,7 +311,29 @@
                 element.metadata = metadata
                 elements.append(element)
 
         if include_page_breaks:
             elements.append(PageBreak())
 
     return elements
+
+
+def is_pdf_text_extractable(filename: str = "", file: Optional[bytes] = None):
+    """Checks to see if the text from a PDF document is extractable. Sometimes the
+    text is not extractable due to PDF security settings."""
+    exactly_one(filename=filename, file=file)
+
+    def _fp_is_extractable(fp):
+        try:
+            next(PDFPage.get_pages(fp, check_extractable=True))
+            extractable = True
+        except PDFTextExtractionNotAllowed:
+            extractable = False
+        return extractable
+
+    if filename:
+        with open_filename(filename, "rb") as fp:
+            fp = cast(BinaryIO, fp)
+            return _fp_is_extractable(fp)
+    elif file:
+        fp = cast(BinaryIO, file)
+        return _fp_is_extractable(fp)
```

### Comparing `unstructured-0.6.1/unstructured/partition/ppt.py` & `unstructured-0.6.2/unstructured/partition/ppt.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/pptx.py` & `unstructured-0.6.2/unstructured/partition/pptx.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/rtf.py` & `unstructured-0.6.2/unstructured/partition/rtf.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/text.py` & `unstructured-0.6.2/unstructured/partition/text.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/partition/text_type.py` & `unstructured-0.6.2/unstructured/partition/text_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 else:
     from typing import Final
 
 from unstructured.cleaners.core import remove_punctuation
 from unstructured.logger import logger
 from unstructured.nlp.english_words import ENGLISH_WORDS
 from unstructured.nlp.patterns import (
+    ENDS_IN_PUNCT_RE,
     UNICODE_BULLETS_RE,
     US_CITY_STATE_ZIP_RE,
     US_PHONE_NUMBERS_RE,
 )
 from unstructured.nlp.tokenize import pos_tag, sent_tokenize, word_tokenize
 
 POS_VERB_TAGS: Final[List[str]] = ["VB", "VBG", "VBD", "VBN", "VBP", "VBZ"]
@@ -119,14 +120,17 @@
     if _language_checks is not None:
         language_checks = _language_checks.lower() == "true"
 
     if len(text) == 0:
         logger.debug("Not a title. Text is empty.")
         return False
 
+    if text.isupper() and ENDS_IN_PUNCT_RE.search(text) is not None:
+        return False
+
     title_max_word_length = int(
         os.environ.get("UNSTRUCTURED_TITLE_MAX_WORD_LENGTH", title_max_word_length),
     )
     # NOTE(robinson) - splitting on spaces here instead of word tokenizing because it
     # is less expensive and actual tokenization doesn't add much value for the length check
     if len(text.split(" ")) > title_max_word_length:
         return False
@@ -264,15 +268,15 @@
     """
     # NOTE(robinson) - Currently limiting this to only sections of text with one sentence.
     # The assumption is that sections with multiple sentences are not titles.
     if sentence_count(text, 3) > 1:
         return False
 
     if text.isupper():
-        return False
+        return True
 
     # NOTE(jay-ylee) - The word_tokenize function also recognizes and separates special characters
     # into one word, causing problems with ratio measurement.
     # Therefore, only words consisting of alphabets are used to measure the ratio.
     # ex. world_tokenize("ITEM 1. Financial Statements (Unaudited)")
     #     = ['ITEM', '1', '.', 'Financial', 'Statements', '(', 'Unaudited', ')'],
     # however, "ITEM 1. Financial Statements (Unaudited)" is Title, not NarrativeText
```

### Comparing `unstructured-0.6.1/unstructured/staging/argilla.py` & `unstructured-0.6.2/unstructured/staging/argilla.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/base.py` & `unstructured-0.6.2/unstructured/staging/base.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/datasaur.py` & `unstructured-0.6.2/unstructured/staging/datasaur.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/huggingface.py` & `unstructured-0.6.2/unstructured/staging/huggingface.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/label_box.py` & `unstructured-0.6.2/unstructured/staging/label_box.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/label_studio.py` & `unstructured-0.6.2/unstructured/staging/label_studio.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/staging/prodigy.py` & `unstructured-0.6.2/unstructured/staging/prodigy.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured/utils.py` & `unstructured-0.6.2/unstructured/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured-0.6.1/unstructured.egg-info/PKG-INFO` & `unstructured-0.6.2/unstructured.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured
-Version: 0.6.1
+Version: 0.6.2
 Summary: A library that prepares raw documents for downstream ML tasks.
 Home-page: https://github.com/Unstructured-IO/unstructured
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: unstructured Version: 0.6.1 Summary: A library that
+Metadata-Version: 2.1 Name: unstructured Version: 0.6.2 Summary: A library that
 prepares raw documents for downstream ML tasks. Home-page: https://github.com/
 Unstructured-IO/unstructured Author: Unstructured Technologies Author-email:
 devops@unstructuredai.io License: Apache-2.0 Description:
 **** [https://raw.githubusercontent.com/Unstructured-IO/unstructured/main/img/
                           unstructured_logo.png] ****
  ![https://pypi.python.org/pypi/unstructured/](https://img.shields.io/pypi/l/
    unstructured.svg) ![https://pypi.python.org/pypi/unstructured/](https://
```

### Comparing `unstructured-0.6.1/unstructured.egg-info/SOURCES.txt` & `unstructured-0.6.2/unstructured.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 unstructured/nlp/__init__.py
 unstructured/nlp/english-words.txt
 unstructured/nlp/english_words.py
 unstructured/nlp/partition.py
 unstructured/nlp/patterns.py
 unstructured/nlp/tokenize.py
 unstructured/partition/__init__.py
+unstructured/partition/api.py
 unstructured/partition/auto.py
 unstructured/partition/common.py
 unstructured/partition/doc.py
 unstructured/partition/docx.py
 unstructured/partition/email.py
 unstructured/partition/epub.py
 unstructured/partition/html.py
```

