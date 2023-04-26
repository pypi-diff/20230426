# Comparing `tmp/mosaicml-streaming-0.4.0.tar.gz` & `tmp/mosaicml-streaming-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-streaming-0.4.0.tar", last modified: Fri Mar 31 02:15:13 2023, max compression
+gzip compressed data, was "mosaicml-streaming-0.4.1.tar", last modified: Tue Apr 25 13:47:32 2023, max compression
```

## Comparing `mosaicml-streaming-0.4.0.tar` & `mosaicml-streaming-0.4.1.tar`

### file list

```diff
@@ -1,134 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.234452 mosaicml-streaming-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-03-31 02:15:13.234452 mosaicml-streaming-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.218452 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-03-31 02:15:13.000000 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-03-31 02:15:13.000000 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 02:15:13.000000 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-31 02:15:13.000000 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-31 02:15:13.000000 mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 02:15:13.234452 mosaicml-streaming-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.218452 mosaicml-streaming-0.4.0/streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.218452 mosaicml-streaming-0.4.0/streaming/base/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40757 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.218452 mosaicml-streaming-0.4.0/streaming/base/format/
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/format/base/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/base/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/format/json/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/json/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/json/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/json/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/format/mds/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/mds/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/mds/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/mds/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/format/xsv/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/xsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/xsv/encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/xsv/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/format/xsv/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/partition/
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/partition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/partition/orig.py
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/shuffle/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/shuffle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/shuffle/py1s.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/shuffle/py2s.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/base/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/storage/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/storage/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/base/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.222452 mosaicml-streaming-0.4.0/streaming/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/multimodal/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/laion400m/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/laion400m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/crawl.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/crawl_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/inside_to_outside.py
--rw-r--r--   0 runner    (1001) docker     (123)    17167 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/multimodal/webvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/text/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/text/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/c4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.226452 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.230452 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/tokenization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.230452 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/count_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/tokenization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/enwiki_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/convert/pile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/enwiki.py
--rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/text/pile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.230452 mosaicml-streaming-0.4.0/streaming/vision/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.230452 mosaicml-streaming-0.4.0/streaming/vision/convert/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/ade20k.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/fake_cifar10.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/convert/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/streaming/vision/imagenet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 02:15:13.234452 mosaicml-streaming-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_compression.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_encodings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_laziness.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_mixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_streaming_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-03-31 02:14:57.000000 mosaicml-streaming-0.4.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14602 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 13:47:32.000000 mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15307 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.281400 mosaicml-streaming-0.4.1/streaming/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40046 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/base/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/json/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/json/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/mds/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/format/xsv/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/format/xsv/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/partition/
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/partition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/partition/orig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/shuffle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py1b.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py1s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/shuffle/py2s.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/base/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18362 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/storage/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13426 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/base/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.285400 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/multimodal/webvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/c4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15176 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/tokenization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/count_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14632 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12473 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/tokenization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/enwiki_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/convert/pile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/enwiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/text/pile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.289399 mosaicml-streaming-0.4.1/streaming/vision/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/streaming/vision/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/ade20k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/fake_cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/convert/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/streaming/vision/imagenet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 13:47:32.293399 mosaicml-streaming-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_encodings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_laziness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_mixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10207 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_streaming_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-04-25 13:47:18.000000 mosaicml-streaming-0.4.1/tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.4.0/LICENSE` & `mosaicml-streaming-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/PKG-INFO` & `mosaicml-streaming-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.4.0
+Version: 0.4.1
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.1 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.4.0/README.md` & `mosaicml-streaming-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/PKG-INFO` & `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-streaming
-Version: 0.4.0
+Version: 0.4.1
 Summary: Streaming lets users create PyTorch compatible datasets that can be streamed from cloud-based object stores
 Home-page: https://github.com/mosaicml/streaming/
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.0 Summary:
+Metadata-Version: 2.1 Name: mosaicml-streaming Version: 0.4.1 Summary:
 Streaming lets users create PyTorch compatible datasets that can be streamed
 from cloud-based object stores Home-page: https://github.com/mosaicml/
 streaming/ Author: MosaicML Author-email: team@mosaicml.com Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.7 Description-
 Content-Type: text/markdown Provides-Extra: dev Provides-Extra: docs Provides-
```

### Comparing `mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/SOURCES.txt` & `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,31 @@
 streaming/base/format/xsv/__init__.py
 streaming/base/format/xsv/encodings.py
 streaming/base/format/xsv/reader.py
 streaming/base/format/xsv/writer.py
 streaming/base/partition/__init__.py
 streaming/base/partition/orig.py
 streaming/base/shuffle/__init__.py
+streaming/base/shuffle/naive.py
+streaming/base/shuffle/py1b.py
 streaming/base/shuffle/py1s.py
 streaming/base/shuffle/py2s.py
 streaming/base/storage/__init__.py
 streaming/base/storage/download.py
 streaming/base/storage/upload.py
 streaming/multimodal/__init__.py
 streaming/multimodal/webvid.py
 streaming/multimodal/convert/__init__.py
 streaming/multimodal/convert/laion/__init__.py
 streaming/multimodal/convert/laion/laion400m/__init__.py
 streaming/multimodal/convert/laion/laion400m/convert_and_upload.py
 streaming/multimodal/convert/webvid/__init__.py
-streaming/multimodal/convert/webvid/crawl.py
-streaming/multimodal/convert/webvid/crawl_subsets.py
-streaming/multimodal/convert/webvid/inside_to_outside.py
+streaming/multimodal/convert/webvid/crawl_webvid.py
+streaming/multimodal/convert/webvid/crawl_webvid_subsets.py
+streaming/multimodal/convert/webvid/extract_webvid_videos.py
 streaming/text/__init__.py
 streaming/text/c4.py
 streaming/text/enwiki.py
 streaming/text/pile.py
 streaming/text/convert/__init__.py
 streaming/text/convert/c4.py
 streaming/text/convert/enwiki_text.py
@@ -95,13 +97,14 @@
 tests/test_distributed.py
 tests/test_download.py
 tests/test_encodings.py
 tests/test_hashing.py
 tests/test_laziness.py
 tests/test_mixing.py
 tests/test_reader.py
+tests/test_shared.py
 tests/test_shuffle.py
 tests/test_streaming.py
 tests/test_streaming_remote.py
 tests/test_upload.py
 tests/test_util.py
 tests/test_writer.py
```

### Comparing `mosaicml-streaming-0.4.0/mosaicml_streaming.egg-info/requires.txt` & `mosaicml-streaming-0.4.1/mosaicml_streaming.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 boto3<2,>=1.21.45
 Brotli>=1.0.9
 matplotlib<4,>=3.5.2
 paramiko<4,>=2.11.0
 python-snappy<1,>=0.6.1
-torch<2,>=1.10
+torch<3,>=1.10
 torchtext>=0.10
 torchvision>=0.10
 tqdm<5,>=4.64.0
 transformers<5,>=4.21.3
 xxhash<4,>=3.0.0
 zstd<2,>=1.5.2.5
 oci<3,>=2.88
 
 [all]
 GitPython==3.1.31
 datasets<3,>=2.4.0
 docformatter>=1.4
 docutils==0.17.1
-fastapi==0.95.0
+fastapi==0.95.1
 furo==2022.9.29
 jupyter==1.0.0
 moto<5,>=4.0
 myst-parser==0.18.1
 nbsphinx==0.8.12
 pandoc==2.3
 pre-commit<4,>=2.18.1
 pydantic==1.10.7
 pypandoc==1.11
 pytest-cov<5,>=4
-pytest==7.2.2
+pytest==7.3.1
 pytest_codeblocks==0.16.1
 sphinx-argparse==0.4.0
-sphinx-copybutton==0.5.1
+sphinx-copybutton==0.5.2
 sphinx-tabs<4,>=3
 sphinx==4.4.0
 sphinx_panels==0.6.0
 sphinxcontrib-images==0.9.4
 sphinxcontrib.katex==0.9.4
 sphinxemoji==0.2.0
-sphinxext.opengraph==0.8.1
+sphinxext.opengraph==0.8.2
 toml==0.10.2
 uvicorn==0.21.1
-yamllint==1.30.0
+yamllint==1.31.0
 
 [dev]
 datasets<3,>=2.4.0
 docformatter>=1.4
 jupyter==1.0.0
 pre-commit<4,>=2.18.1
-pytest==7.2.2
+pytest==7.3.1
 pytest_codeblocks==0.16.1
 pytest-cov<5,>=4
 toml==0.10.2
-yamllint==1.30.0
+yamllint==1.31.0
 moto<5,>=4.0
-fastapi==0.95.0
+fastapi==0.95.1
 pydantic==1.10.7
 uvicorn==0.21.1
 
 [docs]
 GitPython==3.1.31
 docutils==0.17.1
 furo==2022.9.29
 myst-parser==0.18.1
 nbsphinx==0.8.12
 pandoc==2.3
 pypandoc==1.11
 sphinx-argparse==0.4.0
-sphinx-copybutton==0.5.1
+sphinx-copybutton==0.5.2
 sphinx==4.4.0
 sphinx_panels==0.6.0
 sphinxcontrib-images==0.9.4
 sphinxcontrib.katex==0.9.4
 sphinxemoji==0.2.0
-sphinxext.opengraph==0.8.1
+sphinxext.opengraph==0.8.2
 sphinx-tabs<4,>=3
```

### Comparing `mosaicml-streaming-0.4.0/pyproject.toml` & `mosaicml-streaming-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/setup.py` & `mosaicml-streaming-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 install_requires = [
     'boto3>=1.21.45,<2',
     'Brotli>=1.0.9',
     'matplotlib>=3.5.2,<4',
     'paramiko>=2.11.0,<4',
     'python-snappy>=0.6.1,<1',
-    'torch>=1.10,<2',
+    'torch>=1.10,<3',
     'torchtext>=0.10',
     'torchvision>=0.10',
     'tqdm>=4.64.0,<5',
     'transformers>=4.21.3,<5',
     'xxhash>=3.0.0,<4',
     'zstd>=1.5.2.5,<2',
     'oci>=2.88,<3',
@@ -60,41 +60,41 @@
 extra_deps = {}
 
 extra_deps['dev'] = [
     'datasets>=2.4.0,<3',
     'docformatter>=1.4',
     'jupyter==1.0.0',
     'pre-commit>=2.18.1,<4',
-    'pytest==7.2.2',
+    'pytest==7.3.1',
     'pytest_codeblocks==0.16.1',
     'pytest-cov>=4,<5',
     'toml==0.10.2',
-    'yamllint==1.30.0',
+    'yamllint==1.31.0',
     'moto>=4.0,<5',
-    'fastapi==0.95.0',
+    'fastapi==0.95.1',
     'pydantic==1.10.7',
     'uvicorn==0.21.1',
 ]
 
 extra_deps['docs'] = [
     'GitPython==3.1.31',
     'docutils==0.17.1',
     'furo==2022.9.29',
     'myst-parser==0.18.1',
     'nbsphinx==0.8.12',
     'pandoc==2.3',
     'pypandoc==1.11',
     'sphinx-argparse==0.4.0',
-    'sphinx-copybutton==0.5.1',
+    'sphinx-copybutton==0.5.2',
     'sphinx==4.4.0',
     'sphinx_panels==0.6.0',
     'sphinxcontrib-images==0.9.4',
     'sphinxcontrib.katex==0.9.4',
     'sphinxemoji==0.2.0',
-    'sphinxext.opengraph==0.8.1',
+    'sphinxext.opengraph==0.8.2',
     'sphinx-tabs>=3,<4',
 ]
 
 extra_deps['all'] = sorted(set(dep for deps in extra_deps.values() for dep in deps))
 
 package_name = os.environ.get('MOSAIC_PACKAGE_NAME', 'mosaicml-streaming')
```

### Comparing `mosaicml-streaming-0.4.0/streaming/__init__.py` & `mosaicml-streaming-0.4.1/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/__init__.py` & `mosaicml-streaming-0.4.1/streaming/base/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/compression.py` & `mosaicml-streaming-0.4.1/streaming/base/compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/dataloader.py` & `mosaicml-streaming-0.4.1/streaming/base/dataloader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/dataset.py` & `mosaicml-streaming-0.4.1/streaming/base/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 
 """A mid-epoch-resumable streaming/caching pytorch IterableDataset."""
 
 import json
 import os
 from enum import IntEnum
 from threading import Thread
-from time import sleep, time
+from time import sleep
 from typing import Any, Dict, Iterator, Optional, Sequence, Tuple
 
 import numpy as np
-import torch
-import torch.distributed as dist
 from filelock import FileLock
 from numpy.typing import NDArray
 from torch.utils.data import IterableDataset
 
-from streaming.base.distributed import barrier
 from streaming.base.index import Index
 from streaming.base.partition import get_partitions
-from streaming.base.shared import CreateSharedMemory, SharedBarrier
+from streaming.base.shared import CreateSharedMemory, SharedBarrier, get_shm_prefix
 from streaming.base.shuffle import get_shuffle
 from streaming.base.stream import Stream
 from streaming.base.util import TICK
 from streaming.base.world import World
 
 
 class _ShardState(IntEnum):
@@ -97,37 +94,49 @@
             "epoch" :"int",
             "sample_in_epoch": "int",
             "shuffle_seed": "int",
             "num_canonical_nodes": "int"
         }
 
     StreamingDataset init takes three kinds of arguments:
-      * One or more Streams (you must provide either ``streams`` or ``remote``/``local``):
-          * ``streams``
-          * ``remote``
-          * ``local``
-      * Knobs to control streaming behavior, which, if multiple Streams are provided, become defaults
-        applied to them:
-          * ``split``
-          * ``download_retry``
-          * ``download_timeout``
-          * ``validate_hash``
-          * ``keep_zip``
-          * ``keep_raw``
-      * How to iterate (controlling prefetching, partitioning, and shuffling):
-          * Prefetching:
-              * ``predownload``
-          * Partitioning:
-              * ``partition_algo``
-              * ``num_canonical_nodes``
-              * ``batch_size``
-          * Shuffling:
-              * ``shuffle``
-              * ``shuffle_algo``
-              * ``shuffle_seed``
+
+    * One or more Streams (you must provide either ``streams`` or ``remote``/``local``):
+
+      * ``streams``
+      * ``remote``
+      * ``local``
+
+    * Knobs to control streaming behavior, which, if multiple Streams are provided, become defaults
+      applied to them:
+
+      * ``split``
+      * ``download_retry``
+      * ``download_timeout``
+      * ``validate_hash``
+      * ``keep_zip``
+      * ``keep_raw``
+
+    * How to iterate (controlling prefetching, partitioning, and shuffling):
+
+      * Prefetching:
+
+        * ``predownload``
+
+      * Partitioning:
+
+        * ``partition_algo``
+        * ``num_canonical_nodes``
+        * ``batch_size``
+
+      * Shuffling:
+
+        * ``shuffle``
+        * ``shuffle_algo``
+        * ``shuffle_seed``
+        * ``shuffle_block_size``
 
     Args:
         streams (Sequence[Stream], optional): One or more Streams to stream/cache samples from,
             which may be upsampled or downsampled. StreamingDataset uses either ``streams`` or
             ``remote``/``local``. Defaults to ``None``.
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. StreamingDataset uses either ``streams`` or
@@ -156,16 +165,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
     def __init__(self,
                  *,
                  streams: Optional[Sequence[Stream]] = None,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
@@ -177,24 +187,26 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
-                 shuffle_seed: int = 9176) -> None:
+                 shuffle_algo: str = 'py1b',
+                 shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18) -> None:
         # Global arguments (which do not live in Streams).
         self.predownload = predownload
         self.partition_algo = partition_algo
         self.num_canonical_nodes = num_canonical_nodes
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.shuffle_algo = shuffle_algo
         self.shuffle_seed = shuffle_seed
+        self.shuffle_block_size = shuffle_block_size
 
         # Check streams vs remote/local.
         if bool(streams) == (bool(remote) or bool(local)):
             raise ValueError(
                 'You must provide either "streams" or "remote"/"local", but not both -- ' +
                 'that would be confusing')
 
@@ -302,91 +314,64 @@
         # Now that we know the true props/reps/picks, inject those back into the Streams,
         for stream, proportion, repeat, pick in zip(self.streams, self.proportion_per_stream,
                                                     self.repeat_per_stream, self.pick_per_stream):
             stream.proportion = proportion
             stream.repeat = repeat
             stream.samples = pick
 
-        # Determine and distribute shuffle seed and shm prefix.
-        seed_rng = np.random.default_rng(shuffle_seed)
-        self.shuffle_seed = int(seed_rng.integers(1 << 60))
-        prefix_int = int(seed_rng.integers(1 << 24))
-        self._prefix = f'{prefix_int:06x}'
-
-        # Should be a unique shared directory per each StreamingDataset instantiation to avoid a
-        # conflict between a different StreamingDataset instance on a same machine.
-        start_time = time()
-        while True:
-            self._shared_dir = os.path.join(os.path.sep, 'tmp', 'streaming', self._prefix)
-            if os.path.exists(self._shared_dir):
-                prefix_int = int(seed_rng.integers(1 << 24))
-                self._prefix = f'{prefix_int:06x}'
-            else:
-                break
-            elapsed = time() - start_time
-            # Raise an exception if not finding a unique shared directory in 60 secs
-            if elapsed > 60:
-                raise RuntimeError(''.join([
-                    f'Could not find the unique shared directory, bailing out.',
-                    'Please provide a different `shuffle_seed` value.'
-                ]))
-
-            sleep(TICK)
-
-        # Initialize the distributed package and synchronize all the ranks
-        is_dist_pg_initialized = False
-        if self._rank_world.num_ranks > 1:
-            if dist.is_available() and not dist.is_initialized():
-                is_dist_pg_initialized = True
-                dist.init_process_group(backend='nccl' if torch.cuda.is_available() and
-                                        dist.is_nccl_available() else 'gloo',
-                                        rank=world.rank,
-                                        world_size=world.num_ranks)
-            dist.barrier()
+        # Register/lookup our shared memory prefix and filelock root directory.
+        my_locals = [
+            os.path.abspath(os.path.join(stream.local, stream.split)) for stream in streams
+        ]
+        self._shm_prefix, self._locals_shm = get_shm_prefix(my_locals, world)
+        self._filelock_root = os.path.join(os.path.sep, 'tmp', 'streaming', self._shm_prefix)
 
         # Create the shared memory-backed worker barrier, without its lock, which is unpickleable.
-        worker_barrier_filelock_path = os.path.join(self._shared_dir, 'barrier_filelock')
-        worker_barrier_shm_path = f'{self._prefix}_barrier'
+        worker_barrier_filelock_path = os.path.join(self._filelock_root, 'barrier_filelock')
+        worker_barrier_shm_path = f'{self._shm_prefix}_barrier'
         self._worker_barrier = SharedBarrier(worker_barrier_filelock_path, worker_barrier_shm_path)
 
         # Remove the lock that makes it unpickleable
         del self._worker_barrier.lock
 
         # Set up the epoch counter.
         #
         # Note: we do not assume that the end of __iter__() will ever be reached, so we need to
         # increment the epoch counter at the start of __iter__() instead of at the end, so we need
         # to track what the next epoch is, not the current epoch.
-        next_epoch_shm = CreateSharedMemory(name=f'{self._prefix}_next_epoch',
+        next_epoch_shm = CreateSharedMemory(name=f'{self._shm_prefix}_next_epoch',
                                             size=np.int64().nbytes)
         self._next_epoch_shm = next_epoch_shm.shm
         self._next_epoch_arr = np.ndarray(1, buffer=self._next_epoch_shm.buf, dtype=np.int64)
         self._next_epoch_arr[0] = 0
 
         # Get the filelock filename that protects shard_states shared memory array.
-        self.shard_states_filename = os.path.join(self._shared_dir, '_shard_states_filelock')
+        self.shard_states_filename = os.path.join(self._filelock_root, '_shard_states_filelock')
 
         # Create or attach shard_states array (tells if each shard is unknown, downloading, or
         # downloaded).
-        shard_states_shm = CreateSharedMemory(name=f'{self._prefix}_shard_states',
+        shard_states_shm = CreateSharedMemory(name=f'{self._shm_prefix}_shard_states',
                                               size=self.num_shards * np.uint8(0).nbytes)
         self._shard_states = shard_states_shm.shm
 
-        # Destroy process group, and de-initialize the distributed package
-        barrier()
-        if is_dist_pg_initialized:
-            dist.destroy_process_group()
-
         # Placeholder for a shared memory object where load_state_dict() saves its data to be
         # picked up by __iter__().
         self._resume_shm = None
 
         # Placeholder for a _PartitionState which tracks state during __iter__().
         self._partition_state = None
 
+    def __del__(self) -> None:
+        """Destructor, which releases its local working directories."""
+        if hasattr(self, '_locals_shm'):
+            try:
+                self._locals_shm.buf[:4] = np.int32(0).tobytes()
+            except:
+                pass
+
     def _get_next_epoch(self) -> int:
         """Get the next epoch.
 
         Returns:
             int: Next epoch.
         """
         return int(self._next_epoch_arr[0])
@@ -414,15 +399,15 @@
             world (World): World state.
             epoch (int): What epoch we think it is (pre-checkpoint).
 
         Returns:
             Tuple[int, int]: What epoch this is, and sample offset in that epoch.
         """
         # Get the resume state, if it exists.
-        name = f'{self._prefix}_resume'
+        name = f'{self._shm_prefix}_resume'
         try:
             resume_shm = CreateSharedMemory(name=name, create=False)
             shm = resume_shm.shm
         except FileNotFoundError:
             # There is nothing to resume.
             if not self.num_canonical_nodes:
                 self.num_canonical_nodes = world.num_nodes
@@ -480,51 +465,63 @@
             epoch (int): What epoch this is for. Used in seeding the sampling RNG.
 
         Returns:
             Tuple[NDArray[np.int64], NDArray[np.int64]]: Sampled shard sizes and sample mapping.
         """
         # Initialize random number generator and arrays.
         rng = np.random.default_rng(self.shuffle_seed + epoch)
-        pick_per_shard = np.zeros(self.num_shards, np.int64) - 1
-        pick_per_sample = np.zeros(self.num_samples, np.int64) - 1
+        shuffle_units = []
+        sample_ids = []
 
         # Iterate over each stream.
         for stream_id in range(self.num_streams):
             stream_shard_offset = self.shard_offset_per_stream[stream_id]
             num_stream_shards = self.shards_per_stream[stream_id]
             stream_shard_ids = stream_shard_offset + np.arange(num_stream_shards)
 
-            # Calculate pick per shard.
+            # Calculate pick per stream shard.
             samples_per_stream_shard = self.samples_per_shard[stream_shard_ids]
             stream_samples = sum(samples_per_stream_shard)
             stream_picks = self.pick_per_stream[stream_id]
             if stream_picks == stream_samples:
                 pick_per_stream_shard = samples_per_stream_shard
             else:
                 pick_per_stream_shard = samples_per_stream_shard * stream_picks // stream_samples
                 short = stream_picks - pick_per_stream_shard.sum()
                 indices = rng.choice(num_stream_shards, short, False)
                 pick_per_stream_shard[indices] += 1
-            pick_per_shard[stream_shard_ids] = pick_per_stream_shard
 
             # Iterate over each shard of this stream.
-            for shard_id, shard_picks in zip(stream_shard_ids, pick_per_stream_shard):
+            for shard_id, shard_samples, shard_picks in zip(stream_shard_ids,
+                                                            samples_per_stream_shard,
+                                                            pick_per_stream_shard):
+                # Calculate shuffle units.
+                shard_shuffle_units = [shard_samples] * (shard_picks // shard_samples)
+                remainder = shard_picks % shard_samples
+                if remainder:
+                    shard_shuffle_units.append(remainder)
+                shuffle_units.append(shard_shuffle_units)
+
+                # Calculate sample IDs of any full repeats.
                 shard_sample_offset = self.index.shard_offsets[shard_id]
-                shard_samples = self.samples_per_shard[shard_id]
-                indices = np.arange(shard_sample_offset, shard_sample_offset + shard_samples)
+                num_full_repeats = shard_picks // shard_samples
+                if num_full_repeats:
+                    full_repeat = shard_sample_offset + np.arange(shard_samples)
+                    sample_ids += [full_repeat] * num_full_repeats
 
-                # Calculate pick per sample.
-                pick_per_sample[indices] = shard_picks // shard_samples
+                # Calculate sample IDs of a possible partial repeat.
                 short = shard_picks % shard_samples
-                indices = shard_sample_offset + rng.choice(shard_samples, short, False)
-                pick_per_sample[indices] += 1
-
-        # Derive sample ID mapping via repeating by pick per sample.
-        small_per_big = np.repeat(np.arange(self.num_samples), pick_per_sample)
-        return pick_per_shard, small_per_big
+                if short:
+                    partial_repeat = shard_sample_offset + rng.choice(shard_samples, short, False)
+                    partial_repeat.sort()
+                    sample_ids.append(partial_repeat)
+
+        shuffle_units = np.concatenate(shuffle_units)
+        sample_ids = np.concatenate(sample_ids)
+        return shuffle_units, sample_ids
 
     def _generate_sample_ids(self, world: World, epoch: int,
                              sample_in_epoch: int) -> NDArray[np.int64]:
         """Generate this epoch's arrangement of samples.
 
         This is only called in local rank zero.
 
@@ -540,27 +537,27 @@
         # Ensure that num_canonical_nodes has been set.
         if self.num_canonical_nodes is None:
             raise RuntimeError('Number of canonical nodes can never be None')
 
         # Sample each shard of each stream according to their proportions/repeats/samples. This
         # gives us the resampled size of each underlying shard, and a mapping from each fake "big"
         # sample ID to its underlying "small" sample ID.
-        pick_per_shard, small_per_big = self._resample_streams(epoch)
+        shuffle_units, small_per_big = self._resample_streams(epoch)
 
         # Partition the global sample space (of resampled "big" sample IDs) into a tensor of shape
         # (num physical nodes, ranks per node, workers per rank, batches per worker, samples per
         # batch) such that we have an elastically deterministic sample order.
         big_ids = get_partitions(self.partition_algo, self.samples_per_epoch,
                                  self.num_canonical_nodes, world.num_nodes, world.ranks_per_node,
                                  world.workers_per_rank, self.batch_size, sample_in_epoch)
 
         # If we need to shuffle, shuffle in a node-aware and *underlying* shard-aware way.
         if self.shuffle:
-            shuffle = get_shuffle(self.shuffle_algo, pick_per_shard, self.num_canonical_nodes,
-                                  self.shuffle_seed, epoch)
+            shuffle = get_shuffle(self.shuffle_algo, shuffle_units, self.num_canonical_nodes,
+                                  self.shuffle_seed, epoch, self.shuffle_block_size)
             big_ids = np.where(big_ids != -1, shuffle[big_ids], -1)
 
         # Now that we have partitioning and shuffled with hallucinated "big" sample IDs, we don't
         # need them anymore, and can convert back to underlying "small" sample IDs.
         return np.where(big_ids != -1, small_per_big[big_ids], -1)
 
     def _share_sample_ids(self, sample_ids: NDArray[np.int64]) -> \
@@ -574,22 +571,22 @@
 
         # Validate shape.
         if sample_ids.ndim != ndim:
             raise ValueError('Sample IDs must be of shape (num physical nodes, ranks per node, ' +
                              'workers per rank, batches per worker, batch size)')
 
         # Save the generated epoch shape to shared memory.
-        name = f'{self._prefix}_epoch_shape'
+        name = f'{self._shm_prefix}_epoch_shape'
         size = ndim * np.int64().nbytes
         shape_shm_obj = CreateSharedMemory(name=name, create=True, size=size, auto_cleanup=False)
         shape_shm = shape_shm_obj.shm
         shape_shm.buf[:size] = np.array(sample_ids.shape, np.int64).tobytes()
 
         # Save the generated epoch data to shared memory.
-        name = f'{self._prefix}_epoch_data'
+        name = f'{self._shm_prefix}_epoch_data'
         size = sample_ids.size * np.int64().nbytes
         data_shm_obj = CreateSharedMemory(name=name, create=True, size=size, auto_cleanup=False)
         data_shm = data_shm_obj.shm
         data_shm.buf[:size] = sample_ids.tobytes()
 
         return shape_shm_obj, data_shm_obj
 
@@ -599,22 +596,22 @@
 
         Returns:
             NDArray[np.int64]: Sample IDs.
         """
         ndim = 5
 
         # Load the generated epoch shape from shared memory.
-        name = f'{self._prefix}_epoch_shape'
+        name = f'{self._shm_prefix}_epoch_shape'
         size = ndim * np.int64().nbytes
         shape_shm_obj = CreateSharedMemory(name=name, create=False, size=size, auto_cleanup=False)
         shape_shm = shape_shm_obj.shm
         shape = tuple(np.ndarray(5, buffer=shape_shm.buf, dtype=np.int64))
 
         # Attach to the generated epoch data in shared memory.
-        name = f'{self._prefix}_epoch_data'
+        name = f'{self._shm_prefix}_epoch_data'
         size = int(np.prod(shape)) * np.int64().nbytes
         data_shm_obj = CreateSharedMemory(name=name, create=False, size=size, auto_cleanup=False)
         data_shm = data_shm_obj.shm
         sample_ids = np.ndarray(shape, buffer=data_shm.buf, dtype=np.int64)
 
         return sample_ids, shape_shm_obj, data_shm_obj
 
@@ -904,15 +901,15 @@
         We just save the state to shared memory for workers to pick up when __iter__ is next
         called. We use shm because changes to this copy of the dataset wouldn't be picked up by
         persistent workers.
 
         Args:
             obj (Dict[str, Any]): The state.
         """
-        name = f'{self._prefix}_resume'
+        name = f'{self._shm_prefix}_resume'
         data = json.dumps(obj, sort_keys=True).encode('utf-8')
         # some platforms choose to allocate chunks of memory based upon that platform’s memory
         # page size, hence, the exact size of the shared memory block may be larger or
         # equal to the size requested.
         resume_shm = CreateSharedMemory(name=name, size=len(data))
         self._resume_shm = resume_shm.shm
         self._resume_shm.buf[:len(data)] = data
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/distributed.py` & `mosaicml-streaming-0.4.1/streaming/base/distributed.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/__init__.py` & `mosaicml-streaming-0.4.1/streaming/base/format/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/base/reader.py` & `mosaicml-streaming-0.4.1/streaming/base/format/base/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/base/writer.py` & `mosaicml-streaming-0.4.1/streaming/base/format/base/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/json/encodings.py` & `mosaicml-streaming-0.4.1/streaming/base/format/json/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/json/reader.py` & `mosaicml-streaming-0.4.1/streaming/base/format/json/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/json/writer.py` & `mosaicml-streaming-0.4.1/streaming/base/format/json/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/mds/encodings.py` & `mosaicml-streaming-0.4.1/streaming/base/format/mds/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/mds/reader.py` & `mosaicml-streaming-0.4.1/streaming/base/format/mds/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/mds/writer.py` & `mosaicml-streaming-0.4.1/streaming/base/format/mds/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/xsv/encodings.py` & `mosaicml-streaming-0.4.1/streaming/base/format/xsv/encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/xsv/reader.py` & `mosaicml-streaming-0.4.1/streaming/base/format/xsv/reader.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/format/xsv/writer.py` & `mosaicml-streaming-0.4.1/streaming/base/format/xsv/writer.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/hashing.py` & `mosaicml-streaming-0.4.1/streaming/base/hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/index.py` & `mosaicml-streaming-0.4.1/streaming/base/index.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/local.py` & `mosaicml-streaming-0.4.1/streaming/base/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/partition/__init__.py` & `mosaicml-streaming-0.4.1/streaming/base/partition/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/partition/orig.py` & `mosaicml-streaming-0.4.1/streaming/base/partition/orig.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/shared.py` & `mosaicml-streaming-0.4.1/streaming/base/shared.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,18 +9,22 @@
 
 import atexit
 import os
 import shutil
 from multiprocessing import resource_tracker  # pyright: ignore
 from multiprocessing.shared_memory import SharedMemory
 from time import sleep
-from typing import Any, Optional
+from typing import Any, List, Optional, Set, Tuple
 
 import numpy as np
+import torch
 from filelock import FileLock
+from torch import distributed as dist
+
+from streaming.base.world import World
 
 # Time to wait, in seconds.
 TICK = 0.07
 
 # Time out to wait before raising exception
 TIMEOUT = 60
 
@@ -264,7 +268,111 @@
                 resource_tracker.unregister = self.fix_unregister
                 shm.close()
         # skip the error if a child process already cleaned up the shared memory
         except FileNotFoundError:
             pass
         finally:
             resource_tracker.unregister = original_rtracker_unreg
+
+
+def _pack_locals(dirnames: Set[str]) -> bytes:
+    """Pack local dirnames.
+
+    Args:
+        dirnames (Set[str]): Unpacked local dirnames.
+
+    Returns:
+        bytes: Packed local dirnames.
+    """
+    text = '\0'.join(sorted(dirnames))
+    data = text.encode('utf-8')
+    size = 4 + len(data)
+    return b''.join([np.int32(size).tobytes(), data])
+
+
+def _unpack_locals(data: bytes) -> Set[str]:
+    """Unpack local dirnames.
+
+    Args:
+        data (bytes): Packed local dirnames.
+
+    Returns:
+        Set[str]: Unpacked local dirnames.
+    """
+    size = np.frombuffer(data[:4], np.int32)[0]
+    text = data[4:size].decode('utf-8')
+    return set(text.split('\0'))
+
+
+def get_shm_prefix(my_locals: List[str], world: World) -> Tuple[str, SharedMemory]:
+    """Register or lookup our shared memory prefix.
+
+    Args:
+        my_locals (List[str]): Local working dir of each stream, relative to /. We need to verify
+            that there is no overlap with any other currently running StreamingDataset.
+        world (World): Information about nodes, ranks, and workers.
+
+    Returns:
+        Tuple[str, CreateSharedMemory]: Shared memory prefix and object. The name is required to be
+            very short for Mac OSX.
+    """
+    # Check my locals for overlap.
+    my_locals_set = set()
+    for dirname in my_locals:
+        if dirname in my_locals_set:
+            raise ValueError(f'Reused local directory: {dirname}. Provide a different one.')
+        my_locals_set.add(dirname)
+
+    # Local leader goes first, checking and registering.
+    if world.is_local_leader:
+        # Local leader walks the existing shm prefixes starting from zero, verifying that there is
+        # no local working directory overlap.  When attaching to an existing shm fails, we have
+        # reached the end of the existing shms.
+        for prefix_int in range(10**6):
+            prefix = f'{prefix_int:06}'
+            name = f'{prefix}_locals'
+            try:
+                shm = CreateSharedMemory(name, False).shm
+            except:
+                break
+            their_locals_set = _unpack_locals(bytes(shm.buf))
+            both = my_locals_set & their_locals_set
+            if both:
+                raise ValueError(f'Reused local directory: {sorted(my_locals_set)} vs ' +
+                                 f'{sorted(their_locals_set)}. Provide a different one.')
+
+        # Local leader registers the first available shm prefix, recording its locals.
+        prefix = f'{prefix_int:06}'  # pyright: ignore
+        name = f'{prefix}_locals'
+        data = _pack_locals(my_locals_set)
+        shm = CreateSharedMemory(name, True, len(data)).shm
+        shm.buf[:len(data)] = data
+
+    # Distributed barrier over all ranks, possibly setting up dist to do so.
+    destroy_dist = False
+    if 1 < world.num_ranks:
+        if dist.is_available() and not dist.is_initialized():
+            backend = 'nccl' if torch.cuda.is_available() and dist.is_nccl_available() else 'gloo'
+            dist.init_process_group(backend=backend, rank=world.rank, world_size=world.num_ranks)
+            destroy_dist = True
+        dist.barrier()
+
+    # Non-local leaders go next, searching for match.
+    if not world.is_local_leader:
+        for prefix_int in range(10**6):
+            prefix = f'{prefix_int:06}'
+            name = f'{prefix}_locals'
+            try:
+                shm = CreateSharedMemory(name, False).shm
+            except:
+                raise RuntimeError('Internal error: shm prefix was not registered by local leader')
+            their_locals_set = _unpack_locals(bytes(shm.buf))
+            if my_locals_set == their_locals_set:
+                break
+
+    # Distributed barrier, then tear down dist if we set it up.
+    if dist.is_available() and dist.is_initialized():
+        dist.barrier()
+    if destroy_dist:
+        dist.destroy_process_group()
+
+    return prefix, shm  # pyright: ignore
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/shuffle/__init__.py` & `mosaicml-streaming-0.4.1/streaming/base/shuffle/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,36 +2,45 @@
 # SPDX-License-Identifier: Apache-2.0
 
 """Shuffle epochs of samples from different shards across worker partitions."""
 
 import numpy as np
 from numpy.typing import NDArray
 
+from streaming.base.shuffle.naive import get_shuffle_naive
+from streaming.base.shuffle.py1b import get_shuffle_py1b
 from streaming.base.shuffle.py1s import get_shuffle_py1s
 from streaming.base.shuffle.py2s import get_shuffle_py2s
 
 algos = {
+    'py1b': get_shuffle_py1b,
     'py1s': get_shuffle_py1s,
     'py2s': get_shuffle_py2s,
+    'naive': get_shuffle_naive,
 }
 
 
-def get_shuffle(algo: str, shard_sizes: NDArray[np.int64], num_canonical_nodes: int, seed: int,
-                epoch: int) -> NDArray[np.int64]:
+def get_shuffle(algo: str,
+                shard_sizes: NDArray[np.int64],
+                num_canonical_nodes: int,
+                seed: int,
+                epoch: int,
+                block_size: int = 1 << 18) -> NDArray[np.int64]:
     """Get the shuffled global ordering of samples for an epoch.
 
     The assignment of shards to nodes is fixed across epochs, but each grouping of shards is
     processed concurrently in a different order by each node's workers each epoch.
 
     Args:
         algo (str): Which shuffling algorithm to use.
         shard_sizes (NDArray[np.int64]): Number of samples contained in each shard, in order.
         num_canonical_nodes (int): Number of canonical nodes.
         seed (int): Base random seed, which is held constant over an entire training run.
         epoch (int): Current epoch, which is added to the seed to get a different deterministic
             shuffle each epoch.
+        block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
 
     Returns:
         NDArray[np.int64]: 1:1 mapping of sample ID to shuffled sample ID.
     """
     get = algos[algo]
-    return get(shard_sizes, num_canonical_nodes, seed, epoch)
+    return get(shard_sizes, num_canonical_nodes, seed, epoch, block_size)
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/shuffle/py1s.py` & `mosaicml-streaming-0.4.1/streaming/base/shuffle/py1s.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from typing import List, Tuple
 
 import numpy as np
 from numpy.typing import NDArray
 
 
-def _divide_spans(spans: List[Tuple[int, int]], num_samples: int, num_parts: int) -> \
+def divide_spans(spans: List[Tuple[int, int]], num_samples: int, num_parts: int) -> \
         Tuple[List[Tuple[int, int]], List[Tuple[int, int]]]:
     """Divide the spans into discrete, equal sized partitions.
 
     Don't use ``spans`` after this, as it is modified in-place for performance reasons.
 
     Args:
         spans (List[Tuple[int, int]]): List of spans to partition.
@@ -62,27 +62,32 @@
         super_span = begin_part, len(out_spans)
         super_spans.append(super_span)
         begin_part = len(out_spans)
 
     return out_spans, super_spans
 
 
-def get_shuffle_py1s(shard_sizes: NDArray[np.int64], num_canonical_nodes: int, seed: int,
-                     epoch: int) -> NDArray[np.int64]:
+def get_shuffle_py1s(shard_sizes: NDArray[np.int64],
+                     num_canonical_nodes: int,
+                     seed: int,
+                     epoch: int,
+                     block_size: int = 1 << 18) -> NDArray[np.int64]:
     """Get the shuffled global ordering of samples for an epoch.
 
     The assignment of shards to nodes is fixed across epochs, but each grouping of shards is
     processed concurrently in a different order by each node's workers each epoch.
 
     Args:
         shard_sizes (NDArray[np.int64]): Number of samples contained in each shard, in order.
         num_canonical_nodes (int): Number of canonical nodes.
         seed (int): Base random seed, which is held constant over an entire training run.
         epoch (int): Current epoch, which is added to the seed to get a different deterministic
             shuffle each epoch.
+        block_size (int): Unit of shuffle (ignored, because we shuffle on the basis of shards).
+            Defaults to ``1 << 18``.
 
     Returns:
         NDArray[np.int64]: 1:1 mapping of sample ID to shuffled sample ID.
     """
     # Create each shard's sample ID span (begin, end excl).
     spans = []
     num_samples = 0
@@ -92,15 +97,15 @@
         num_samples += shard_size
 
     # Generate the initial ordering of shards, which is fixed over an entire training run.
     run_rng = np.random.default_rng(seed)
     run_rng.shuffle(spans)
 
     # Break the shard spans at canonical node boundaries.
-    spans, super_spans = _divide_spans(spans, num_samples, num_canonical_nodes)
+    spans, super_spans = divide_spans(spans, num_samples, num_canonical_nodes)
 
     # Shuffle the span ordering within each canonical node uniquely to this epoch.
     epoch_rng = np.random.default_rng(seed + epoch)
     for begin, end in super_spans:
         part = spans[begin:end]
         epoch_rng.shuffle(part)  # pyright: ignore
         spans[begin:end] = part
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/shuffle/py2s.py` & `mosaicml-streaming-0.4.1/streaming/base/shuffle/py2s.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,27 +100,32 @@
             samples_so_far += samples_this_shard
 
         lists.append(new_shards)
         new_shards = []
     return lists
 
 
-def get_shuffle_py2s(shard_sizes: NDArray[np.int64], num_canonical_nodes: int, seed: int,
-                     epoch: int) -> NDArray[np.int64]:
+def get_shuffle_py2s(shard_sizes: NDArray[np.int64],
+                     num_canonical_nodes: int,
+                     seed: int,
+                     epoch: int,
+                     block_size: int = 1 << 18) -> NDArray[np.int64]:
     """Get the shuffled global ordering of samples for an epoch.
 
     The assignment of shards to nodes is fixed across epochs, but each grouping of shards is
     processed concurrently in a different order by each node's workers each epoch.
 
     Args:
         shard_sizes (NDArray[np.int64]): Number of samples contained in each shard, in order.
         num_canonical_nodes (int): Number of canonical nodes.
         seed (int): Base random seed, which is held constant over an entire training run.
         epoch (int): Current epoch, which is added to the seed to get a different deterministic
             shuffle each epoch.
+        block_size (int): Unit of shuffle (ignored, because we shuffle on the basis of shards).
+            Defaults to ``1 << 18``.
 
     Returns:
         NDArray[np.int64]: 1:1 mapping of sample ID to shuffled sample ID.
     """
     # Initiailze the sample ID range for each shard.
     shards = _create_shards(shard_sizes)
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/storage/__init__.py` & `mosaicml-streaming-0.4.1/streaming/base/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/storage/download.py` & `mosaicml-streaming-0.4.1/streaming/base/storage/download.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 """Shard downloading from various storage providers."""
 
 import os
 import shutil
 import urllib.parse
 from time import sleep, time
-from typing import Optional
+from typing import Any, Dict, Optional
 
 __all__ = ['download_or_wait']
 
 S3_NOT_FOUND_CODES = {'403', '404', 'NoSuchKey'}
 
 
 def download_from_s3(remote: str, local: str, timeout: float) -> None:
@@ -19,49 +19,68 @@
 
     Args:
         remote (str): Remote path (S3).
         local (str): Local path (local filesystem).
         timeout (float): How long to wait for shard to download before raising an exception.
     """
 
-    def _download_file(unsigned: bool = False) -> None:
+    def _download_file(unsigned: bool = False,
+                       extra_args: Optional[Dict[str, Any]] = None) -> None:
         """Download the file from AWS S3 bucket. The bucket can be either public or private.
 
         Args:
-            unsigned (bool, optional): Set to True if it is a public bucket. Defaults to False.
+            unsigned (bool, optional):  Set to True if it is a public bucket. Defaults to False.
+            extra_args (Dict[str, Any], optional): Extra arguments supported by boto3. Defaults to None.
         """
         if unsigned:
             # Client will be using unsigned mode in which public
             # resources can be accessed without credentials
             config = Config(read_timeout=timeout, signature_version=UNSIGNED)
         else:
             config = Config(read_timeout=timeout)
+
+        if extra_args is None:
+            extra_args = {}
         s3 = boto3.client('s3', config=config)
-        s3.download_file(obj.netloc, obj.path.lstrip('/'), local)
+        s3.download_file(obj.netloc, obj.path.lstrip('/'), local, ExtraArgs=extra_args)
 
     import boto3
     from botocore import UNSIGNED
     from botocore.config import Config
     from botocore.exceptions import ClientError, NoCredentialsError
 
     obj = urllib.parse.urlparse(remote)
     if obj.scheme != 's3':
         raise ValueError(f'Expected obj.scheme to be "s3", got {obj.scheme} for remote={remote}')
 
+    extra_args = {}
+    # When enabled, the requester instead of the bucket owner pays the cost of the request
+    # and the data download from the bucket.
+    if os.environ.get('MOSAICML_STREAMING_AWS_REQUESTER_PAYS') is not None:
+        requester_pays_buckets = os.environ.get(  # yapf: ignore
+            'MOSAICML_STREAMING_AWS_REQUESTER_PAYS').split(',')  # pyright: ignore
+        requester_pays_buckets = [name.strip() for name in requester_pays_buckets]
+        if obj.netloc in requester_pays_buckets:
+            extra_args['RequestPayer'] = 'requester'
+
     try:
-        _download_file()
+        _download_file(extra_args=extra_args)
     except NoCredentialsError:
         # Public S3 buckets without credentials
-        _download_file(unsigned=True)
+        _download_file(unsigned=True, extra_args=extra_args)
     except ClientError as e:
         if e.response['Error']['Code'] in S3_NOT_FOUND_CODES:
-            raise FileNotFoundError(f'Object {remote} not found.') from e
+            e.args = (f'Object {remote} not found! Either check the bucket path or the bucket ' +
+                      f'permission. If the bucket is a requester pays bucket, then provide the ' +
+                      f'bucket name to the environment variable ' +
+                      f'`MOSAICML_STREAMING_AWS_REQUESTER_PAYS`.',)
+            raise e
         elif e.response['Error']['Code'] == '400':
             # Public S3 buckets without credentials
-            _download_file(unsigned=True)
+            _download_file(unsigned=True, extra_args=extra_args)
     except Exception:
         raise
 
 
 def download_from_sftp(remote: str, local: str) -> None:
     """Download a file from remote SFTP server to local filepath.
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/storage/upload.py` & `mosaicml-streaming-0.4.1/streaming/base/storage/upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/stream.py` & `mosaicml-streaming-0.4.1/streaming/base/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,34 +23,40 @@
 class Stream:
     """A dataset, or sub-dataset if mixing, from which we stream/cache samples.
 
     We initialize a StreamingDataset with one or more Streams. Streams may be resampled to achieve
     different mixtures of samples.
 
     Stream init takes three kinds of arguments:
-      * At least one of ``remote`` and ``local`` must exist. If no ``remote``, the data must be
-        local. If no ``local``, we cache to a temp directory.
-          * ``remote``
-          * ``local``
-      * At most one of ``proportion``, ``repeat``, or ``samples`` may exist. If none are provided,
-        each sample is seen once per epoch. If provided one of these, we derive the others.
-        Note that ``proportion`` (relative) and ``repeat``/``samples`` (absolute) are mutually
-        incompatible -- you must entirely use one or the other (or neither) for all sub-datasets.
-          * ``proportion``
-          * ``repeat``
-          * ``samples``
-      * The remaining arguments are optional knobs for controlling downloading behavior and default
-        to ``None``. If ``None``, they take a default value provided to or by the StreamingDataset
-        init.
-          * ``split``
-          * ``download_retry``
-          * ``download_timeout``
-          * ``validate_hash``
-          * ``keep_zip``
-          * ``keep_raw``
+
+    * At least one of ``remote`` and ``local`` must exist. If no ``remote``, the data must be
+      local. If no ``local``, we cache to a temp directory.
+
+      * ``remote``
+      * ``local``
+
+    * At most one of ``proportion``, ``repeat``, or ``samples`` may exist. If none are provided,
+      each sample is seen once per epoch. If provided one of these, we derive the others.
+      Note that ``proportion`` (relative) and ``repeat``/``samples`` (absolute) are mutually
+      incompatible -- you must entirely use one or the other (or neither) for all sub-datasets.
+
+      * ``proportion``
+      * ``repeat``
+      * ``samples``
+
+    * The remaining arguments are optional knobs for controlling downloading behavior and default
+      to ``None``. If ``None``, they take a default value provided to or by the StreamingDataset
+      init.
+
+      * ``split``
+      * ``download_retry``
+      * ``download_timeout``
+      * ``validate_hash``
+      * ``keep_zip``
+      * ``keep_raw``
 
     Args:
         remote (str, optional): Remote path or directory to download the dataset from. If ``None``,
             its data must exist locally. Defaults to ``None``.
         local (str, optional): Local working directory to download shards to. This is where shards
             are cached while they are being used. Uses a temp directory if not set. Defaults to
             ``None``.
```

### Comparing `mosaicml-streaming-0.4.0/streaming/base/util.py` & `mosaicml-streaming-0.4.1/streaming/base/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/base/world.py` & `mosaicml-streaming-0.4.1/streaming/base/world.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py` & `mosaicml-streaming-0.4.1/streaming/multimodal/convert/laion/laion400m/convert_and_upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from time import sleep, time
 from typing import Iterator, List, Optional, Union
 
 import numpy as np
 from pyarrow import parquet as pq
 
 from streaming import MDSWriter
+from streaming.base.storage import CloudUploader
 
 
 def parse_args() -> Namespace:
     """Parse command-line arguments.
 
     Returns:
         Namespace: Command-line arguments.
@@ -177,19 +178,19 @@
 def upload(local: str, remote: str) -> None:
     """Upload a shard to remote storage.
 
     Args:
         local (str): Path on local filesystem.
         remote (str): Path on remote filesystem.
     """
-    local = local.replace(' ', '\\ ')
-    remote = remote.replace(' ', '\\ ')
-    cmd = f'aws s3 cp {local} {remote}'
-    if os.system(cmd):
-        raise RuntimeError(f'Download failed: {cmd}.')
+    local_dir = os.path.dirname(local)
+    remote_dir = os.path.dirname(remote)
+    filename = os.path.basename(local)
+    cl_uploader = CloudUploader(out=(local_dir, remote_dir))
+    cl_uploader.upload_file(filename)
 
 
 def convert_and_upload_shards(args: Namespace) -> bool:
     """Process any newly downloaded shards.
 
     Args:
         args (Namespace): Command-line arguments.
@@ -216,14 +217,19 @@
                 raise RuntimeError(f'MDS shard file is missing: {mds_shard_filename}.')
             if not os.path.exists(mds_index_filename):
                 raise RuntimeError(f'MDS index file is missing: {mds_index_filename}.')
         else:
             print(f'Shard {idx:05}: converting...')
             convert(parquet_filename, mds_dirname, hashes)
         print(f'Shard {idx:05}: uploading...')
+        # Rename the file from `shard.00000.mds` to `shard.{idx:05}.mds` since the `upload`
+        # method relies on the same filename for source and destination.
+        rename_mds_shard_filename = os.path.join(mds_dirname, f'shard.{idx:05}.mds')
+        os.rename(mds_shard_filename, rename_mds_shard_filename)
+        mds_shard_filename = rename_mds_shard_filename
         upload(mds_shard_filename, remote_shard_filename)
         with open(done_filename, 'w') as out:
             out.write('')
 
         # Clean up after ourselves to save local storage.
         if not args.keep_parquet:
             os.remove(parquet_filename)
```

### Comparing `mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/crawl.py` & `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/crawl_subsets.py` & `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/crawl_webvid_subsets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/multimodal/convert/webvid/inside_to_outside.py` & `mosaicml-streaming-0.4.1/streaming/multimodal/convert/webvid/extract_webvid_videos.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,20 +24,50 @@
 def parse_args() -> Namespace:
     """Parse command-line arguments.
 
     Returns:
         Namespace: Command-line arguments.
     """
     args = ArgumentParser()
-    args.add_argument('--in', type=str, required=True, help='Input mp4-inside MDS dataset')
-    args.add_argument('--out_mds', type=str, required=True, help='Output mp4-outside MDS dataset')
-    args.add_argument('--out_mp4', type=str, required=True, help='Output mp4 videos directory')
-    args.add_argument('--compression', type=str, default='zstd:16', help='Compression')
-    args.add_argument('--hashes', type=str, default='sha1,xxh3_64', help='Hashes')
-    args.add_argument('--size_limit', type=int, default=1 << 25, help='Shard size limit')
+    args.add_argument(
+        '--in',
+        type=str,
+        required=True,
+        help='Input mp4-inside MDS dataset directory',
+    )
+    args.add_argument(
+        '--out_mds',
+        type=str,
+        required=True,
+        help='Output mp4-outside MDS dataset directory',
+    )
+    args.add_argument(
+        '--out_mp4',
+        type=str,
+        required=True,
+        help='Output mp4 videos directory',
+    )
+    args.add_argument(
+        '--compression',
+        type=str,
+        default='zstd:16',
+        help='Compression',
+    )
+    args.add_argument(
+        '--hashes',
+        type=str,
+        default='sha1,xxh3_64',
+        help='Hashes',
+    )
+    args.add_argument(
+        '--size_limit',
+        type=int,
+        default=1 << 25,
+        help='Shard size limit',
+    )
     return args.parse_args()
 
 
 def main(args: Namespace) -> None:
     """Convert an MP4-inside MDS dataset to an MP4-outside MDS dataset.
 
     Args:
```

### Comparing `mosaicml-streaming-0.4.0/streaming/multimodal/webvid.py` & `mosaicml-streaming-0.4.1/streaming/multimodal/webvid.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
     def __getitem__(self, idx: int) -> Any:
         """Get the sample at the index.
 
         Args:
             idx (int): Sample index.
@@ -101,16 +102,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         extra_local (str, optional): Base destination of extra local sample downloads.
         extra_remote (str, optional): Base source of extra remote sample downloads.
     """
 
     def __init__(self,
                  *,
                  remote: Optional[str] = None,
@@ -123,16 +125,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  extra_local: Optional[str] = None,
                  extra_remote: Optional[str] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
@@ -142,15 +145,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
 
         # Videos are stored outside of their shards here.
         self.download_timeout = download_timeout
         self.extra_local = extra_local
         self.extra_remote = extra_remote
 
     def __getitem__(self, idx: int) -> Any:
@@ -213,16 +217,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         extra_local (str, optional): Base destination of extra local sample downloads.
         extra_remote (str, optional): Base source of extra remote sample downloads.
     """
 
     def __init__(self,
                  *,
                  remote: Optional[str] = None,
@@ -235,16 +240,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  extra_local: Optional[str] = None,
                  extra_remote: Optional[str] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
@@ -254,15 +260,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
 
         # Videos are stored outside of their shards here.
         self.download_timeout = download_timeout
         self.extra_local = extra_local
         self.extra_remote = extra_remote
 
     def __getitem__(self, idx: int) -> Any:
```

### Comparing `mosaicml-streaming-0.4.0/streaming/text/c4.py` & `mosaicml-streaming-0.4.1/streaming/text/c4.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
         group_method (str): How to group text samples into token samples. Currently only supporting
             ``'truncate'``.
     """
 
     def __init__(self,
@@ -71,16 +72,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  tokenizer_name: str,
                  max_seq_len: int,
                  group_method: str) -> None:
         if group_method not in {'truncate'}:
             raise ValueError(f"group_method='{group_method}' must be one of {'truncate'}.")
 
         super().__init__(remote=remote,
@@ -94,15 +96,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
         self.tokenizer_name = tokenizer_name
         self.max_seq_len = max_seq_len
         self.group_method = group_method
 
         # Build tokenizer
         self.tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_name)
         if self.tokenizer.pad_token is None:
```

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/c4.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/c4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/create_pretraining_data.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/make_train_parallel.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/merge_shard_groups.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/merge_shard_groups.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/pick_eval_samples.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/mds/tokenization.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/mds/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/count_samples.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/count_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/create_pretraining_data.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/make_train_parallel.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/pick_eval_samples.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki/tfrecord/tokenization.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki/tfrecord/tokenization.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/enwiki_text.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/enwiki_text.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/convert/pile.py` & `mosaicml-streaming-0.4.1/streaming/text/convert/pile.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/text/enwiki.py` & `mosaicml-streaming-0.4.1/streaming/text/enwiki.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,16 +43,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
     """
 
     def __init__(self,
                  *,
                  remote: Optional[str] = None,
                  local: Optional[str] = None,
                  split: Optional[str] = None,
@@ -63,30 +64,34 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
-                 shuffle_seed: int = 9176) -> None:
-        super().__init__(local=local,
-                         remote=remote,
+                 shuffle_algo: str = 'py1b',
+                 shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18) -> None:
+        super().__init__(remote=remote,
+                         local=local,
                          split=split,
-                         shuffle=shuffle,
-                         predownload=predownload,
-                         keep_zip=keep_zip,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
-                         shuffle_seed=shuffle_seed,
+                         keep_zip=keep_zip,
+                         keep_raw=keep_raw,
+                         samples_per_epoch=samples_per_epoch,
+                         predownload=predownload,
+                         partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
-                         partition_algo=partition_algo,
-                         shuffle_algo=shuffle_algo)
+                         shuffle=shuffle,
+                         shuffle_algo=shuffle_algo,
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
         self.field_dtypes = {
             'input_ids': np.int32,
             'input_mask': np.int32,
             'attention_mask': np.int32,
             'segment_ids': np.int32,
             'token_type_ids': np.int32,
             'masked_lm_positions': np.int32,
```

### Comparing `mosaicml-streaming-0.4.0/streaming/text/pile.py` & `mosaicml-streaming-0.4.1/streaming/text/pile.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,16 +47,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         tokenizer_name (str): The name of the HuggingFace tokenizer to use to tokenize samples.
         max_seq_len (int): The max sequence length of each token sample.
         group_method (str): How to group text samples into token samples. Currently only supporting
             ``'truncate'``.
     """
 
     def __init__(self,
@@ -71,16 +72,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  tokenizer_name: str,
                  max_seq_len: int,
                  group_method: str) -> None:
         if group_method not in ['truncate']:
             raise ValueError(f'Only group_method="truncate" is supported at this time.')
 
         super().__init__(remote=remote,
@@ -94,15 +96,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
         self.tokenizer_name = tokenizer_name
         self.max_seq_len = max_seq_len
         self.group_method = group_method
 
         # Build tokenizer
         self.tokenizer = AutoTokenizer.from_pretrained(self.tokenizer_name)
         if self.tokenizer.pad_token is None:
```

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/ade20k.py` & `mosaicml-streaming-0.4.1/streaming/vision/ade20k.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         joint_transform (callable, optional): A function/transforms that takes in an image and a
             target  and returns the transformed versions of both. Defaults to ``None``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in the target and
             transforms it. Defaults to ``None``.
     """
@@ -71,16 +72,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  joint_transform: Optional[Callable] = None,
                  transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
@@ -91,15 +93,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
         self.joint_transform = joint_transform
         self.transform = transform
         self.target_transform = target_transform
 
     def __getitem__(self, idx: int) -> Tuple[Any, Any]:
         """Get sample by global index, blocking to load its shard if missing.
```

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/base.py` & `mosaicml-streaming-0.4.1/streaming/vision/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -77,16 +77,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transforms (callable, optional): A function/transforms that takes in an image and a label
             and returns the transformed versions of both. Defaults to ``None``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in a target and
             returns a transformed version. Defaults to ``None``.
     """
@@ -103,16 +104,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  transforms: Optional[Callable] = None,
                  transform: Optional[Callable] = None,
                  target_transform: Optional[Callable] = None) -> None:
         StreamingDataset.__init__(self,
                                   remote=remote,
                                   local=local,
                                   split=split,
@@ -123,15 +125,16 @@
                                   keep_raw=keep_raw,
                                   predownload=predownload,
                                   partition_algo=partition_algo,
                                   num_canonical_nodes=num_canonical_nodes,
                                   batch_size=batch_size,
                                   shuffle=shuffle,
                                   shuffle_algo=shuffle_algo,
-                                  shuffle_seed=shuffle_seed)
+                                  shuffle_seed=shuffle_seed,
+                                  shuffle_block_size=shuffle_block_size)
 
         has_transforms = transforms is not None
         has_separate_transform = transform is not None or target_transform is not None
         if has_transforms and has_separate_transform:
             raise ValueError(
                 'Only transforms or transform/target_transform can be passed as an argument')
```

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/cifar10.py` & `mosaicml-streaming-0.4.1/streaming/vision/cifar10.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in a target and
             returns a transformed version. Defaults to ``None``.
     """
```

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/coco.py` & `mosaicml-streaming-0.4.1/streaming/vision/coco.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,16 +45,17 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transform (callable, optional): A function/transform that takes in an image and bboxes and
             returns a transformed version. Defaults to ``None``.
     """
 
     def __init__(self,
                  *,
                  remote: Optional[str] = None,
@@ -67,16 +68,17 @@
                  keep_raw: bool = True,
                  samples_per_epoch: Optional[int] = None,
                  predownload: Optional[int] = 100_000,
                  partition_algo: str = 'orig',
                  num_canonical_nodes: Optional[int] = None,
                  batch_size: Optional[int] = None,
                  shuffle: bool = False,
-                 shuffle_algo: str = 'py1s',
+                 shuffle_algo: str = 'py1b',
                  shuffle_seed: int = 9176,
+                 shuffle_block_size: int = 1 << 18,
                  transform: Optional[Callable] = None) -> None:
         super().__init__(remote=remote,
                          local=local,
                          split=split,
                          download_retry=download_retry,
                          download_timeout=download_timeout,
                          validate_hash=validate_hash,
@@ -85,15 +87,16 @@
                          samples_per_epoch=samples_per_epoch,
                          predownload=predownload,
                          partition_algo=partition_algo,
                          num_canonical_nodes=num_canonical_nodes,
                          batch_size=batch_size,
                          shuffle=shuffle,
                          shuffle_algo=shuffle_algo,
-                         shuffle_seed=shuffle_seed)
+                         shuffle_seed=shuffle_seed,
+                         shuffle_block_size=shuffle_block_size)
         self.transform = transform
 
     def __getitem__(self, idx: int) -> Any:
         """Get sample by global index, blocking to load its shard if missing.
 
         Args:
             idx (int): Sample index.
```

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/ade20k.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/ade20k.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/base.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/cifar10.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/coco.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/coco.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/fake_cifar10.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/fake_cifar10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/convert/imagenet.py` & `mosaicml-streaming-0.4.1/streaming/vision/convert/imagenet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/streaming/vision/imagenet.py` & `mosaicml-streaming-0.4.1/streaming/vision/imagenet.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         num_canonical_nodes (int, optional): Canonical number of nodes for shuffling with
             resumption. Defaults to ``None``, which is interpreted as the number of nodes of the
             initial run.
         batch_size (int, optional): Batch size of its DataLoader, which affects how the dataset is
             partitioned over the workers. Defaults to ``None``.
         shuffle (bool): Whether to iterate over the samples in randomized order. Defaults to
             ``False``.
-        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1s``.
+        shuffle_algo (str): Which shuffling algorithm to use. Defaults to ``py1b``.
         shuffle_seed (int): Seed for Deterministic data shuffling. Defaults to ``9176``.
+        shuffle_block_size (int): Unit of shuffle. Defaults to ``1 << 18``.
         transform (callable, optional): A function/transform that takes in an image and returns a
             transformed version. Defaults to ``None``.
         target_transform (callable, optional): A function/transform that takes in a target and
             returns a transformed version. Defaults to ``None``.
     """
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_barrier.py` & `mosaicml-streaming-0.4.1/tests/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_compression.py` & `mosaicml-streaming-0.4.1/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_distributed.py` & `mosaicml-streaming-0.4.1/tests/test_distributed.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,22 +33,26 @@
         assert dist.is_initialized()
         assert dist.get_world_size() == 4
         assert dist.get_rank() < 4
 
 
 class TestAllgatherObject(DistributedTest):
 
+    @pytest.mark.skip(
+        'CI non-deterministically hangs. See https://mosaicml.atlassian.net/browse/STR-61')
     @pytest.mark.world_size(2)
     @pytest.mark.parametrize(('data', 'expected_data'),
                              [(5, [5, 5]),
                               (np.array(10), [np.array(10), np.array(10)])])
     def test_all_gather_object(self, data: Any, expected_data: Any):
         output = ms_dist.all_gather_object(data)
         assert output == expected_data
 
+    @pytest.mark.skip(
+        'CI non-deterministically hangs. See https://mosaicml.atlassian.net/browse/STR-61')
     @pytest.mark.world_size(1)
     @pytest.mark.parametrize(('data', 'expected_data'), [(5, [5]), (np.array(10), [np.array(10)])])
     def test_all_gather_object_non_dist(self, data: Any, expected_data: Any):
         output = ms_dist.all_gather_object(data)
         assert output == expected_data
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_download.py` & `mosaicml-streaming-0.4.1/tests/test_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import tempfile
 from typing import Any, Tuple
 from unittest.mock import Mock, patch
 
 import boto3
 import pytest
+from botocore.exceptions import ClientError
 
 from streaming.base.storage.download import (download_file, download_from_gcs, download_from_local,
                                              download_from_s3, download_or_wait)
 from tests.conftest import GCS_URL, MY_BUCKET
 
 MY_PREFIX = 'train'
 
@@ -41,16 +42,16 @@
             mock_remote_filepath, _ = remote_local_file(cloud_prefix='s3://', filename=file_name)
             client = boto3.client('s3', region_name='us-east-1')
             client.put_object(Bucket=MY_BUCKET, Key=os.path.join(MY_PREFIX, file_name), Body='')
             download_from_s3(mock_remote_filepath, tmp.name, 60)
             assert os.path.isfile(tmp.name)
 
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
-    def test_filenotfound_exception(self, remote_local_file: Any):
-        with pytest.raises(FileNotFoundError):
+    def test_clienterror_exception(self, remote_local_file: Any):
+        with pytest.raises(ClientError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='s3://')
             download_from_s3(mock_remote_filepath, mock_local_filepath, 60)
 
     @pytest.mark.usefixtures('s3_client', 's3_test', 'remote_local_file')
     def test_invalid_cloud_prefix(self, remote_local_file: Any):
         with pytest.raises(ValueError):
             mock_remote_filepath, mock_local_filepath = remote_local_file(cloud_prefix='s9://')
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_encodings.py` & `mosaicml-streaming-0.4.1/tests/test_encodings.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_hashing.py` & `mosaicml-streaming-0.4.1/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_laziness.py` & `mosaicml-streaming-0.4.1/tests/test_laziness.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import pytest
 
 from streaming import MDSWriter, StreamingDataset
 
 
 @pytest.mark.usefixtures('local_remote_dir')
 def test_laziness(local_remote_dir: Tuple[str, str]):
-    num_samples = 100_000
+    num_samples = 10_000
     local, remote = local_remote_dir
     columns = {'value': 'int'}
     compression = None
     hashes = None
-    size_limit = 10_000
+    size_limit = 1_000
 
     with MDSWriter(out=remote,
                    columns=columns,
                    compression=compression,
                    hashes=hashes,
                    size_limit=size_limit) as out:
         for i in range(num_samples):
@@ -28,31 +28,35 @@
             out.write(sample)
 
     # Verify __getitem__ accesses.
     dataset = StreamingDataset(local=remote)
     for i in range(num_samples):
         sample = dataset[i]
         assert sample['value'] == i
+    del dataset
 
     # Verify __iter__ -> __getitem__ accesses.
     dataset = StreamingDataset(local=remote)
     for i, sample in zip(range(num_samples), dataset):
         assert sample['value'] == i
+    del dataset
 
     # Verify __getitem__ downloads/accesses.
     dataset = StreamingDataset(local=local, remote=remote)
     for i in range(num_samples):
         sample = dataset[i]
         assert sample['value'] == i
+    del dataset
 
     shutil.rmtree(local)
 
     # Verify __iter__ -> __getitem__ downloads/accesses.
     dataset = StreamingDataset(local=local, remote=remote)
     for i, sample in zip(range(num_samples), dataset):
         assert sample['value'] == i
+    del dataset
 
     # Re-verify __getitem__ downloads/accesses.
     dataset = StreamingDataset(local=local, remote=remote)
     for i in range(num_samples):
         sample = dataset[i]
         assert sample['value'] == i
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_mixing.py` & `mosaicml-streaming-0.4.1/tests/test_mixing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # Copyright 2023 MosaicML Streaming authors
 # SPDX-License-Identifier: Apache-2.0
 
 import os
-from shutil import rmtree
-from typing import List
+from typing import List, Tuple
 
+import numpy as np
 import pytest
 
 from streaming import MDSWriter, Stream, StreamingDataset
 
 
 def walk(dataset: StreamingDataset) -> List[int]:
     return [sample['value'] for sample in dataset]
 
 
 def float_eq(a: float, b: float) -> bool:
     return abs(a - b) < 1e-6
 
 
+@pytest.mark.usefixtures('local_remote_dir')
 @pytest.fixture()
-def root():
-    root = '/tmp/foo'
+def root(local_remote_dir: Tuple[str, str]):
+    root, _ = local_remote_dir
     columns = {'value': 'int'}
     for i in range(4):
         subroot = os.path.join(root, str(i))
         with MDSWriter(out=subroot, columns=columns) as out:
             begin = i * 2
             end = (i + 1) * 2
             for value in range(begin, end):
                 sample = {'value': value}
                 out.write(sample)
     yield root
-    rmtree(root)
 
 
 def test_mix_none(root: str):
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot)
@@ -68,15 +68,15 @@
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, samples=4)
         streams.append(stream)
     dataset = StreamingDataset(streams=streams)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7]
+    assert walk(dataset) == [0, 1, 0, 1, 2, 3, 2, 3, 4, 5, 4, 5, 6, 7, 6, 7]
     for stream in streams:
         assert float_eq(stream.proportion, 0.25)
         assert stream.repeat == 2
         assert stream.samples == 4
 
 
 def test_mix_samples_range(root: str):
@@ -84,15 +84,15 @@
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, samples=samples[i])
         streams.append(stream)
     dataset = StreamingDataset(streams=streams)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [2, 3, 4, 4, 5, 5, 6, 6, 6, 7, 7, 7]
+    assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.samples == i * 2
 
 
 def test_mix_repeat(root: str):
@@ -100,15 +100,15 @@
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, repeat=repeat[i])
         streams.append(stream)
     dataset = StreamingDataset(streams=streams)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [2, 3, 4, 4, 5, 5, 6, 6, 6, 7, 7, 7]
+    assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.samples == i * 2
 
 
 def test_mix_repeat_and_samples(root: str):
@@ -122,15 +122,15 @@
     for i in range(4):
         subroot = os.path.join(root, str(i))
         repeat, samples = weights[i]
         stream = Stream(local=subroot, repeat=repeat, samples=samples)
         streams.append(stream)
     dataset = StreamingDataset(streams=streams)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [2, 3, 4, 4, 5, 5, 6, 6, 6, 7, 7, 7]
+    assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.samples == i * 2
 
 
 def test_mix_repeat_samples_none(root: str):
@@ -144,15 +144,15 @@
     for i in range(4):
         subroot = os.path.join(root, str(i))
         repeat, samples = weights[i]
         stream = Stream(local=subroot, repeat=repeat, samples=samples)
         streams.append(stream)
     dataset = StreamingDataset(streams=streams)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [2, 3, 4, 4, 5, 5, 6, 6, 6, 7, 7, 7]
+    assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.samples == i * 2
 
 
 def test_mix_proportion_equal(root: str):
@@ -176,12 +176,28 @@
     streams = []
     for i in range(4):
         subroot = os.path.join(root, str(i))
         stream = Stream(local=subroot, proportion=proportion[i])
         streams.append(stream)
     dataset = StreamingDataset(streams=streams, samples_per_epoch=12)
     assert dataset.num_samples == 8
-    assert walk(dataset) == [2, 3, 4, 4, 5, 5, 6, 6, 6, 7, 7, 7]
+    assert walk(dataset) == [2, 3, 4, 5, 4, 5, 6, 7, 6, 7, 6, 7]
     for i, stream in enumerate(streams):
         assert float_eq(stream.proportion, i / 6)
         assert stream.repeat == i
         assert stream.samples == i * 2
+
+
+def test_mix_balance(root: str):
+    streams = []
+    for i in range(4):
+        subroot = os.path.join(root, str(i))
+        stream = Stream(local=subroot, samples=3)
+        streams.append(stream)
+    dataset = StreamingDataset(streams=streams)
+    counts = np.zeros(8, np.int64)
+    for _ in range(1000):
+        for value in walk(dataset):
+            counts[value] += 1
+    rates = counts / counts.sum() * len(counts)
+    for rate in rates:
+        assert 0.975 < rate < 1.025
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_reader.py` & `mosaicml-streaming-0.4.1/tests/test_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import time
 from typing import Any
 
 import pytest
 
 from streaming.base import StreamingDataset
 from tests.common.datasets import SequenceDataset, write_mds_dataset
+from tests.common.utils import copy_all_files
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope='function')
 def mds_dataset_dir():
     try:
@@ -200,7 +201,20 @@
                                shuffle=False,
                                shuffle_seed=seed)
 
     # Test retrieving random sample
     sample = dataset[index]
     assert sample['id'] == f'{index:06}'
     assert sample['sample'] == 3 * index
+
+
+@pytest.mark.usefixtures('mds_dataset_dir')
+def test_dataset_split_instantiation(mds_dataset_dir: Any):
+
+    splits = ['train', 'val']
+    remote_dir, local_dir = mds_dataset_dir
+
+    # Build StreamingDataset for each split
+    for split in splits:
+        remote_split_dir = os.path.join(remote_dir, split)
+        copy_all_files(remote_dir, remote_split_dir)
+        _ = StreamingDataset(local=local_dir, remote=remote_dir, split=split)
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_shuffle.py` & `mosaicml-streaming-0.4.1/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_streaming.py` & `mosaicml-streaming-0.4.1/tests/test_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,17 @@
     dataloader = DataLoader(dataset=dataset, batch_size=batch_size, num_workers=num_workers)
 
     # Append sample ID
     sample_order = []
     for batch in dataloader:
         sample_order.extend(batch['id'][:])
 
+    del dataloader
+    del dataset
+
     # Build StreamingDataset again to test deterministic sample ID
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
                                shuffle_seed=seed)
 
@@ -183,14 +186,17 @@
         if idx == len(dataset) // (batch_size * 2):
             sample_order.extend(batch['id'][:])
             state_dict = dataloader.state_dict()
             assert state_dict is not None
             break
         sample_order.extend(batch['id'][:])
 
+    del dataloader
+    del dataset
+
     dataset = StreamingDataset(local=local_dir,
                                remote=remote_dir,
                                shuffle=shuffle,
                                batch_size=batch_size,
                                shuffle_seed=seed)
 
     dataloader = StreamingDataLoader(dataset=dataset,
@@ -231,14 +237,16 @@
 
     # Append train sample ID
     train_sample_order = []
     for batch in train_dataloader:
         train_sample_order.extend(batch['id'][:])
 
     shutil.rmtree(local_dir)
+    del train_dataloader
+    del train_dataset
 
     # Build val StreamingDataset
     val_dataset = StreamingDataset(local=local_dir,
                                    remote=remote_dir,
                                    batch_size=batch_size,
                                    shuffle_seed=shuffle_seed_val)
```

### Comparing `mosaicml-streaming-0.4.0/tests/test_streaming_remote.py` & `mosaicml-streaming-0.4.1/tests/test_streaming_remote.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_upload.py` & `mosaicml-streaming-0.4.1/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `mosaicml-streaming-0.4.0/tests/test_writer.py` & `mosaicml-streaming-0.4.1/tests/test_writer.py`

 * *Files identical despite different names*

