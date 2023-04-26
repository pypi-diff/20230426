# Comparing `tmp/tgmount-1.0.4.tar.gz` & `tmp/tgmount-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgmount-1.0.4.tar", last modified: Tue Feb  7 09:34:43 2023, max compression
+gzip compressed data, was "tgmount-1.0.5.tar", last modified: Wed Apr 26 07:30:00 2023, max compression
```

## Comparing `tgmount-1.0.4.tar` & `tgmount-1.0.5.tar`

### file list

```diff
@@ -1,199 +1,204 @@
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.495230 tgmount-1.0.4/
--rw-r--r--   0 horn      (1000) horn      (1000)    19121 2023-02-07 09:34:43.495230 tgmount-1.0.4/PKG-INFO
--rw-r--r--   0 horn      (1000) horn      (1000)    18881 2023-02-04 09:45:15.000000 tgmount-1.0.4/README.md
--rw-r--r--   0 horn      (1000) horn      (1000)       38 2023-02-07 09:34:43.495230 tgmount-1.0.4/setup.cfg
--rw-r--r--   0 horn      (1000) horn      (1000)     1272 2023-02-07 09:33:28.000000 tgmount-1.0.4/setup.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.451896 tgmount-1.0.4/tgmount/
--rw-r--r--   0 horn      (1000) horn      (1000)      160 2023-02-01 16:39:04.000000 tgmount-1.0.4/tgmount/__init__.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.455230 tgmount-1.0.4/tgmount/cache/
--rw-r--r--   0 horn      (1000) horn      (1000)      238 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6511 2023-02-04 13:41:52.000000 tgmount-1.0.4/tgmount/cache/cache_in_blocks.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7367 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/file.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1122 2023-02-04 12:29:31.000000 tgmount-1.0.4/tgmount/cache/file_source.py
--rw-r--r--   0 horn      (1000) horn      (1000)       61 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1915 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/memory.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4200 2023-02-04 14:05:41.000000 tgmount-1.0.4/tgmount/cache/reader.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2318 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)       41 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cache/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.458563 tgmount-1.0.4/tgmount/cli/
--rw-r--r--   0 horn      (1000) horn      (1000)      405 2023-02-02 13:50:26.000000 tgmount-1.0.4/tgmount/cli/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)      162 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cli/auth.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3025 2023-02-02 15:13:02.000000 tgmount-1.0.4/tgmount/cli/download.py
--rw-r--r--   0 horn      (1000) horn      (1000)      460 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cli/list_dialogs.py
--rw-r--r--   0 horn      (1000) horn      (1000)     8586 2023-02-04 11:53:50.000000 tgmount-1.0.4/tgmount/cli/list_documents.py
--rw-r--r--   0 horn      (1000) horn      (1000)       50 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cli/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)     5902 2023-02-02 17:33:08.000000 tgmount-1.0.4/tgmount/cli/mount.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3213 2023-02-01 18:51:56.000000 tgmount-1.0.4/tgmount/cli/mount_config.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1292 2023-02-02 13:12:46.000000 tgmount-1.0.4/tgmount/cli/stats.py
--rw-r--r--   0 horn      (1000) horn      (1000)       63 2023-02-06 11:05:02.000000 tgmount-1.0.4/tgmount/cli/upload.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.458563 tgmount-1.0.4/tgmount/cli/util/
--rw-r--r--   0 horn      (1000) horn      (1000)      142 2023-01-30 14:23:33.000000 tgmount-1.0.4/tgmount/cli/util/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)      744 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/cli/util/client.py
--rw-r--r--   0 horn      (1000) horn      (1000)      308 2023-02-01 16:41:15.000000 tgmount-1.0.4/tgmount/cli/util/config.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1521 2023-02-01 16:41:15.000000 tgmount-1.0.4/tgmount/cli/util/read_env.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1517 2023-02-01 19:57:13.000000 tgmount-1.0.4/tgmount/cli/validate.py
--rwxr-xr-x   0 horn      (1000) horn      (1000)     4530 2023-02-02 16:44:21.000000 tgmount-1.0.4/tgmount/client.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.461897 tgmount-1.0.4/tgmount/common/
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/common/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)      694 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/common/filter.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.461897 tgmount-1.0.4/tgmount/config/
--rw-r--r--   0 horn      (1000) horn      (1000)       84 2023-02-01 18:46:54.000000 tgmount-1.0.4/tgmount/config/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)    11113 2023-02-01 20:26:26.000000 tgmount-1.0.4/tgmount/config/config.py
--rw-r--r--   0 horn      (1000) horn      (1000)      565 2023-02-01 18:32:02.000000 tgmount-1.0.4/tgmount/config/config_type.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2343 2023-01-31 19:42:01.000000 tgmount-1.0.4/tgmount/config/error.py
--rw-r--r--   0 horn      (1000) horn      (1000)     5169 2023-01-31 16:25:32.000000 tgmount-1.0.4/tgmount/config/helpers.py
--rw-r--r--   0 horn      (1000) horn      (1000)       76 2023-01-30 14:32:51.000000 tgmount-1.0.4/tgmount/config/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7829 2023-02-01 20:03:07.000000 tgmount-1.0.4/tgmount/config/reader.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4282 2023-02-01 18:46:05.000000 tgmount-1.0.4/tgmount/config/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)      145 2023-01-30 19:00:58.000000 tgmount-1.0.4/tgmount/config/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.461897 tgmount-1.0.4/tgmount/controlserver/
--rw-r--r--   0 horn      (1000) horn      (1000)       34 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/controlserver/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1567 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/controlserver/server.py
--rw-r--r--   0 horn      (1000) horn      (1000)      110 2023-01-31 22:28:20.000000 tgmount-1.0.4/tgmount/error.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.465230 tgmount-1.0.4/tgmount/fs/
--rw-r--r--   0 horn      (1000) horn      (1000)      408 2023-02-06 16:45:38.000000 tgmount-1.0.4/tgmount/fs/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1829 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/fs/fh.py
--rw-r--r--   0 horn      (1000) horn      (1000)     9445 2023-02-06 17:24:21.000000 tgmount-1.0.4/tgmount/fs/inode.py
--rw-r--r--   0 horn      (1000) horn      (1000)      112 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/fs/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)    17662 2023-02-06 17:21:21.000000 tgmount-1.0.4/tgmount/fs/operations.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7466 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/fs/update.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2818 2023-02-06 17:21:29.000000 tgmount-1.0.4/tgmount/fs/util.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3427 2023-02-06 17:59:56.000000 tgmount-1.0.4/tgmount/fs/writable.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.465230 tgmount-1.0.4/tgmount/main/
--rw-r--r--   0 horn      (1000) horn      (1000)       82 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/main/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3196 2023-02-06 17:54:17.000000 tgmount-1.0.4/tgmount/main/util.py
--rw-r--r--   0 horn      (1000) horn      (1000)       51 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/settings.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.468563 tgmount-1.0.4/tgmount/tgclient/
--rw-r--r--   0 horn      (1000) horn      (1000)      448 2023-01-31 22:34:32.000000 tgmount-1.0.4/tgmount/tgclient/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1293 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/auth.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4812 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/client.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2558 2023-02-04 09:28:43.000000 tgmount-1.0.4/tgmount/tgclient/client_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     5826 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/events_disptacher.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3135 2023-02-01 16:40:52.000000 tgmount-1.0.4/tgmount/tgclient/fetcher.py
--rw-r--r--   0 horn      (1000) horn      (1000)      383 2023-02-04 12:54:00.000000 tgmount-1.0.4/tgmount/tgclient/file_source_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6794 2023-02-06 15:17:23.000000 tgmount-1.0.4/tgmount/tgclient/files_source.py
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/filters.py
--rw-r--r--   0 horn      (1000) horn      (1000)    13177 2023-02-04 09:59:52.000000 tgmount-1.0.4/tgmount/tgclient/guards.py
--rw-r--r--   0 horn      (1000) horn      (1000)       64 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)      714 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/message_reaction_event.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6354 2023-01-30 11:31:20.000000 tgmount-1.0.4/tgmount/tgclient/message_source.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2524 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/message_source_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3215 2023-02-04 13:59:04.000000 tgmount-1.0.4/tgmount/tgclient/message_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3630 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/messages_collection.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.471897 tgmount-1.0.4/tgmount/tgclient/search/
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/search/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1521 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/search/search.py
--rw-r--r--   0 horn      (1000) horn      (1000)      213 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/search/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)      240 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/search/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.471897 tgmount-1.0.4/tgmount/tgclient/source/
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/source/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1096 2023-02-04 13:17:54.000000 tgmount-1.0.4/tgmount/tgclient/source/document.py
--rw-r--r--   0 horn      (1000) horn      (1000)      461 2023-02-04 13:17:37.000000 tgmount-1.0.4/tgmount/tgclient/source/item.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1809 2023-02-04 13:59:33.000000 tgmount-1.0.4/tgmount/tgclient/source/photo.py
--rw-r--r--   0 horn      (1000) horn      (1000)      132 2023-02-04 12:47:04.000000 tgmount-1.0.4/tgmount/tgclient/source/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1013 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/source/util.py
--rw-r--r--   0 horn      (1000) horn      (1000)      442 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)      295 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgclient/util.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4481 2023-02-06 15:15:15.000000 tgmount-1.0.4/tgmount/tglog.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.478563 tgmount-1.0.4/tgmount/tgmount/
--rw-r--r--   0 horn      (1000) horn      (1000)      278 2023-02-01 16:40:47.000000 tgmount-1.0.4/tgmount/tgmount/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3468 2023-02-01 20:29:24.000000 tgmount-1.0.4/tgmount/tgmount/cached_filefactory_factory.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.478563 tgmount-1.0.4/tgmount/tgmount/file_factory/
--rw-r--r--   0 horn      (1000) horn      (1000)      238 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1699 2023-02-02 10:32:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/classifier.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1517 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/classifierbase.py
--rw-r--r--   0 horn      (1000) horn      (1000)      114 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/error.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3947 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/filefactory.py
--rw-r--r--   0 horn      (1000) horn      (1000)     5735 2023-02-02 14:26:00.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/filefactorybase.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2182 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/file_factory/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)    10395 2023-02-01 19:21:42.000000 tgmount-1.0.4/tgmount/tgmount/filters.py
--rw-r--r--   0 horn      (1000) horn      (1000)      944 2023-02-01 18:46:23.000000 tgmount-1.0.4/tgmount/tgmount/filters_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)       70 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/logger.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.481897 tgmount-1.0.4/tgmount/tgmount/producers/
--rw-r--r--   0 horn      (1000) horn      (1000)      258 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7152 2023-02-02 14:26:16.000000 tgmount-1.0.4/tgmount/tgmount/producers/grouperbase.py
--rw-r--r--   0 horn      (1000) horn      (1000)       93 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2069 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_by_forward.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1904 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_by_performer.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1472 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_by_reaction.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3016 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_by_sender.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6347 2023-02-01 18:31:20.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_plain.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3409 2023-02-06 17:56:05.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_sysinfo.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6267 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/producers/producer_zip.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.481897 tgmount-1.0.4/tgmount/tgmount/providers/
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/providers/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1331 2023-02-01 17:30:17.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_caches.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1990 2023-02-01 19:12:56.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_filters.py
--rw-r--r--   0 horn      (1000) horn      (1000)      368 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_producers.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1201 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_sources.py
--rw-r--r--   0 horn      (1000) horn      (1000)      364 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_vfs_wrappers.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1376 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/providers/provider_wrappers.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.481897 tgmount-1.0.4/tgmount/tgmount/root/
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/root/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)    12576 2023-02-01 18:50:47.000000 tgmount-1.0.4/tgmount/tgmount/root_config_reader.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7687 2023-02-01 17:46:17.000000 tgmount-1.0.4/tgmount/tgmount/root_config_reader_props.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1923 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/root_config_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3883 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/tgmount_builder.py
--rw-r--r--   0 horn      (1000) horn      (1000)     6995 2023-02-01 17:46:17.000000 tgmount-1.0.4/tgmount/tgmount/tgmount_builderbase.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2519 2023-01-29 12:12:35.000000 tgmount-1.0.4/tgmount/tgmount/tgmount_providers.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1691 2023-02-01 17:46:17.000000 tgmount-1.0.4/tgmount/tgmount/tgmount_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)    10752 2023-02-01 16:42:02.000000 tgmount-1.0.4/tgmount/tgmount/tgmountbase.py
--rw-r--r--   0 horn      (1000) horn      (1000)       99 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)      138 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.485230 tgmount-1.0.4/tgmount/tgmount/validator/
--rw-r--r--   0 horn      (1000) horn      (1000)       39 2023-02-01 18:48:47.000000 tgmount-1.0.4/tgmount/tgmount/validator/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)       81 2023-02-01 18:43:55.000000 tgmount-1.0.4/tgmount/tgmount/validator/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)       83 2023-01-31 22:39:20.000000 tgmount-1.0.4/tgmount/tgmount/validator/validator.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3467 2023-02-02 15:40:58.000000 tgmount-1.0.4/tgmount/tgmount/validator/validatorbase.py
--rw-r--r--   0 horn      (1000) horn      (1000)    16101 2023-02-01 16:41:15.000000 tgmount-1.0.4/tgmount/tgmount/vfs_tree.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3601 2023-01-31 13:03:02.000000 tgmount-1.0.4/tgmount/tgmount/vfs_tree_producer.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3283 2023-01-31 12:55:51.000000 tgmount-1.0.4/tgmount/tgmount/vfs_tree_producer_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1171 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/vfs_tree_types.py
--rw-r--r--   0 horn      (1000) horn      (1000)      683 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/vfs_tree_wrapper_types.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.485230 tgmount-1.0.4/tgmount/tgmount/wrappers/
--rw-r--r--   0 horn      (1000) horn      (1000)      103 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/wrappers/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)       85 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/wrappers/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4631 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/tgmount/wrappers/wrapper_exclude_empty_dirs.py
--rw-r--r--   0 horn      (1000) horn      (1000)     7137 2023-02-01 21:33:09.000000 tgmount-1.0.4/tgmount/tgmount/wrappers/wrapper_zips_as_dirs.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.485230 tgmount-1.0.4/tgmount/util/
--rw-r--r--   0 horn      (1000) horn      (1000)     3022 2023-02-02 13:25:04.000000 tgmount-1.0.4/tgmount/util/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)      886 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/asyn.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1793 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/col.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1508 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/func.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1091 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/guards.py
--rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/path.py
--rw-r--r--   0 horn      (1000) horn      (1000)      841 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/tg.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1787 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util/timer.py
--rw-r--r--   0 horn      (1000) horn      (1000)      679 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.488563 tgmount-1.0.4/tgmount/vfs/
--rw-r--r--   0 horn      (1000) horn      (1000)     1301 2023-02-06 18:44:54.000000 tgmount-1.0.4/tgmount/vfs/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)      859 2023-02-06 18:04:30.000000 tgmount-1.0.4/tgmount/vfs/dir.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3963 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/dir_util.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3706 2023-02-06 18:45:13.000000 tgmount-1.0.4/tgmount/vfs/file.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2848 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/io.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1741 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/lookup.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1581 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/map_tree.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1157 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/root.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2730 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/tree.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.491897 tgmount-1.0.4/tgmount/vfs/types/
--rw-r--r--   0 horn      (1000) horn      (1000)      245 2023-02-06 17:34:26.000000 tgmount-1.0.4/tgmount/vfs/types/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3409 2023-02-06 18:23:55.000000 tgmount-1.0.4/tgmount/vfs/types/dir.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4442 2023-02-06 18:45:05.000000 tgmount-1.0.4/tgmount/vfs/types/file.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2902 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/vfs/util.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.495230 tgmount-1.0.4/tgmount/zip/
--rw-r--r--   0 horn      (1000) horn      (1000)      329 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/__init__.py
--rw-r--r--   0 horn      (1000) horn      (1000)       59 2023-02-01 20:19:20.000000 tgmount-1.0.4/tgmount/zip/logger.py
--rw-r--r--   0 horn      (1000) horn      (1000)      177 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/types.py
--rw-r--r--   0 horn      (1000) horn      (1000)     3023 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/util.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4380 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/zip_dir.py
--rw-r--r--   0 horn      (1000) horn      (1000)     4642 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/zip_dir_factory.py
--rw-r--r--   0 horn      (1000) horn      (1000)     2382 2023-02-01 21:05:03.000000 tgmount-1.0.4/tgmount/zip/zip_file.py
--rw-r--r--   0 horn      (1000) horn      (1000)     1347 2023-02-01 21:22:26.000000 tgmount-1.0.4/tgmount/zip/zip_file_id3v1_fix.py
--rw-r--r--   0 horn      (1000) horn      (1000)     5810 2023-01-28 18:13:13.000000 tgmount-1.0.4/tgmount/zip/zips_as_dirs.py
-drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-02-07 09:34:43.455230 tgmount-1.0.4/tgmount.egg-info/
--rw-r--r--   0 horn      (1000) horn      (1000)    19121 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/PKG-INFO
--rw-r--r--   0 horn      (1000) horn      (1000)     5201 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/SOURCES.txt
--rw-r--r--   0 horn      (1000) horn      (1000)        1 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/dependency_links.txt
--rw-r--r--   0 horn      (1000) horn      (1000)       48 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/entry_points.txt
--rw-r--r--   0 horn      (1000) horn      (1000)       66 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/requires.txt
--rw-r--r--   0 horn      (1000) horn      (1000)        8 2023-02-07 09:34:43.000000 tgmount-1.0.4/tgmount.egg-info/top_level.txt
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.578473 tgmount-1.0.5/
+-rw-r--r--   0 horn      (1000) horn      (1000)    19181 2023-04-26 07:30:00.578473 tgmount-1.0.5/PKG-INFO
+-rw-r--r--   0 horn      (1000) horn      (1000)    18941 2023-04-26 06:14:22.000000 tgmount-1.0.5/README.md
+-rw-r--r--   0 horn      (1000) horn      (1000)       38 2023-04-26 07:30:00.578473 tgmount-1.0.5/setup.cfg
+-rw-r--r--   0 horn      (1000) horn      (1000)     1272 2023-04-26 07:29:38.000000 tgmount-1.0.5/setup.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.545140 tgmount-1.0.5/tgmount/
+-rw-r--r--   0 horn      (1000) horn      (1000)      159 2023-04-24 12:27:02.000000 tgmount-1.0.5/tgmount/__init__.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.548473 tgmount-1.0.5/tgmount/cache/
+-rw-r--r--   0 horn      (1000) horn      (1000)      238 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cache/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6511 2023-02-04 13:41:52.000000 tgmount-1.0.5/tgmount/cache/cache_in_blocks.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7367 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cache/file.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1122 2023-02-04 12:29:31.000000 tgmount-1.0.5/tgmount/cache/file_source.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       61 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cache/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1915 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cache/memory.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4200 2023-02-04 14:05:41.000000 tgmount-1.0.5/tgmount/cache/reader.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2318 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cache/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       41 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cache/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.551806 tgmount-1.0.5/tgmount/cli/
+-rw-r--r--   0 horn      (1000) horn      (1000)      405 2023-02-02 13:50:26.000000 tgmount-1.0.5/tgmount/cli/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      162 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cli/auth.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3025 2023-04-24 13:44:58.000000 tgmount-1.0.5/tgmount/cli/download.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      460 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cli/list_dialogs.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     8586 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/list_documents.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       50 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/cli/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6229 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/mount.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3045 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/mount_config.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1292 2023-02-02 13:12:46.000000 tgmount-1.0.5/tgmount/cli/stats.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       63 2023-02-06 11:05:02.000000 tgmount-1.0.5/tgmount/cli/upload.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.551806 tgmount-1.0.5/tgmount/cli/util/
+-rw-r--r--   0 horn      (1000) horn      (1000)      142 2023-01-30 14:23:33.000000 tgmount-1.0.5/tgmount/cli/util/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      872 2023-04-24 13:47:29.000000 tgmount-1.0.5/tgmount/cli/util/client.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      308 2023-02-01 16:41:15.000000 tgmount-1.0.5/tgmount/cli/util/config.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       60 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/util/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2869 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/util/read_env.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1517 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/cli/validate.py
+-rwxr-xr-x   0 horn      (1000) horn      (1000)     4918 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/client.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.551806 tgmount-1.0.5/tgmount/common/
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/common/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      694 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/common/filter.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.555140 tgmount-1.0.5/tgmount/config/
+-rw-r--r--   0 horn      (1000) horn      (1000)       79 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/config/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    11201 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/config/config.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      565 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/config/config_type.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2343 2023-01-31 19:42:01.000000 tgmount-1.0.5/tgmount/config/error.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4720 2023-04-26 06:25:55.000000 tgmount-1.0.5/tgmount/config/helpers.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       76 2023-01-30 14:32:51.000000 tgmount-1.0.5/tgmount/config/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7890 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/config/reader.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4309 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/config/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      145 2023-01-30 19:00:58.000000 tgmount-1.0.5/tgmount/config/util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      223 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/constants.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.555140 tgmount-1.0.5/tgmount/controlserver/
+-rw-r--r--   0 horn      (1000) horn      (1000)       34 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/controlserver/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1567 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/controlserver/server.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      110 2023-01-31 22:28:20.000000 tgmount-1.0.5/tgmount/error.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.555140 tgmount-1.0.5/tgmount/fs/
+-rw-r--r--   0 horn      (1000) horn      (1000)      408 2023-02-06 16:45:38.000000 tgmount-1.0.5/tgmount/fs/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1829 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/fs/fh.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     9445 2023-02-06 17:24:21.000000 tgmount-1.0.5/tgmount/fs/inode.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      112 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/fs/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    17290 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/fs/operations.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7517 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/fs/update.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3296 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/fs/util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4588 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/fs/writable.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.555140 tgmount-1.0.5/tgmount/main/
+-rw-r--r--   0 horn      (1000) horn      (1000)       82 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/main/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3217 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/main/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.558473 tgmount-1.0.5/tgmount/tgclient/
+-rw-r--r--   0 horn      (1000) horn      (1000)      448 2023-01-31 22:34:32.000000 tgmount-1.0.5/tgmount/tgclient/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1293 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/auth.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4870 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/client.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2558 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/client_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     5826 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/events_disptacher.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.561807 tgmount-1.0.5/tgmount/tgclient/fetcher/
+-rw-r--r--   0 horn      (1000) horn      (1000)       45 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgclient/fetcher/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3135 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgclient/fetcher/fetcher.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      850 2023-04-26 06:33:41.000000 tgmount-1.0.5/tgmount/tgclient/fetcher/fetcher_cache.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       90 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgclient/fetcher/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      383 2023-02-04 12:54:00.000000 tgmount-1.0.5/tgmount/tgclient/file_source_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6759 2023-04-26 06:26:44.000000 tgmount-1.0.5/tgmount/tgclient/files_source.py
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/filters.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    13177 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/guards.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       64 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      714 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/message_reaction_event.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6566 2023-04-26 06:29:41.000000 tgmount-1.0.5/tgmount/tgclient/message_source.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2524 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/message_source_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3215 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/message_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3630 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/messages_collection.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.561807 tgmount-1.0.5/tgmount/tgclient/search/
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/search/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1521 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/search/search.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      213 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/search/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      240 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/search/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.561807 tgmount-1.0.5/tgmount/tgclient/source/
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/source/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1096 2023-02-04 13:17:54.000000 tgmount-1.0.5/tgmount/tgclient/source/document.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      461 2023-02-04 13:17:37.000000 tgmount-1.0.5/tgmount/tgclient/source/item.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1809 2023-02-04 13:59:33.000000 tgmount-1.0.5/tgmount/tgclient/source/photo.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      132 2023-02-04 12:47:04.000000 tgmount-1.0.5/tgmount/tgclient/source/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1013 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/source/util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      442 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgclient/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      295 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgclient/util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4436 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tglog.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.568473 tgmount-1.0.5/tgmount/tgmount/
+-rw-r--r--   0 horn      (1000) horn      (1000)      278 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3468 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/cached_filefactory_factory.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.568473 tgmount-1.0.5/tgmount/tgmount/file_factory/
+-rw-r--r--   0 horn      (1000) horn      (1000)      238 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1699 2023-02-02 10:32:13.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/classifier.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1518 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/classifierbase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      114 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/error.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4853 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/filefactory.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     5735 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/filefactorybase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2182 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/file_factory/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    10395 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/filters.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      944 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/filters_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       70 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/logger.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.568473 tgmount-1.0.5/tgmount/tgmount/producers/
+-rw-r--r--   0 horn      (1000) horn      (1000)      258 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/producers/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7152 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/producers/grouperbase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       93 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/producers/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2067 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_by_forward.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1904 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_by_performer.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1472 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_by_reaction.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3045 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_by_sender.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6344 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_plain.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3409 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_sysinfo.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     6324 2023-04-26 06:30:26.000000 tgmount-1.0.5/tgmount/tgmount/producers/producer_zip.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.571807 tgmount-1.0.5/tgmount/tgmount/providers/
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/providers/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1331 2023-02-01 17:30:17.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_caches.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1990 2023-02-01 19:12:56.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_filters.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      368 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_producers.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1201 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_sources.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      364 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_vfs_wrappers.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1376 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/providers/provider_wrappers.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.571807 tgmount-1.0.5/tgmount/tgmount/root/
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/root/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    11369 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/root_config_reader.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7687 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/root_config_reader_props.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1923 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/root_config_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3883 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/tgmount_builder.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7079 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/tgmount_builderbase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2519 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/tgmount_providers.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1691 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/tgmount_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    10749 2023-04-26 06:15:23.000000 tgmount-1.0.5/tgmount/tgmount/tgmountbase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       99 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      138 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.571807 tgmount-1.0.5/tgmount/tgmount/validator/
+-rw-r--r--   0 horn      (1000) horn      (1000)       39 2023-02-01 18:48:47.000000 tgmount-1.0.5/tgmount/tgmount/validator/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       81 2023-02-01 18:43:55.000000 tgmount-1.0.5/tgmount/tgmount/validator/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       83 2023-01-31 22:39:20.000000 tgmount-1.0.5/tgmount/tgmount/validator/validator.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3494 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/validator/validatorbase.py
+-rw-r--r--   0 horn      (1000) horn      (1000)    16106 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/vfs_tree.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3601 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/vfs_tree_producer.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3283 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/vfs_tree_producer_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1171 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/vfs_tree_types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      683 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/vfs_tree_wrapper_types.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.571807 tgmount-1.0.5/tgmount/tgmount/wrappers/
+-rw-r--r--   0 horn      (1000) horn      (1000)      103 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/wrappers/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       85 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/tgmount/wrappers/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4631 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/wrappers/wrapper_exclude_empty_dirs.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     7137 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/tgmount/wrappers/wrapper_zips_as_dirs.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.575140 tgmount-1.0.5/tgmount/util/
+-rw-r--r--   0 horn      (1000) horn      (1000)     3022 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/util/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      886 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/util/asyn.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1793 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/util/col.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1508 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/util/func.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1091 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/util/guards.py
+-rw-r--r--   0 horn      (1000) horn      (1000)        0 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/util/path.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      841 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/util/tg.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1787 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/util/timer.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      679 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.575140 tgmount-1.0.5/tgmount/vfs/
+-rw-r--r--   0 horn      (1000) horn      (1000)     1301 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      859 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/dir.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3963 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/dir_util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3736 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/file.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2848 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/io.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1741 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/lookup.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1581 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/map_tree.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1157 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/root.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2730 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/vfs/tree.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.578473 tgmount-1.0.5/tgmount/vfs/types/
+-rw-r--r--   0 horn      (1000) horn      (1000)      245 2023-02-10 15:17:00.000000 tgmount-1.0.5/tgmount/vfs/types/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3409 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/types/dir.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4688 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/types/file.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2902 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/vfs/util.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.578473 tgmount-1.0.5/tgmount/zip/
+-rw-r--r--   0 horn      (1000) horn      (1000)      329 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/zip/__init__.py
+-rw-r--r--   0 horn      (1000) horn      (1000)       59 2023-02-01 20:19:20.000000 tgmount-1.0.5/tgmount/zip/logger.py
+-rw-r--r--   0 horn      (1000) horn      (1000)      177 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/zip/types.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     3023 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/zip/util.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4380 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/zip/zip_dir.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     4642 2023-01-28 18:13:13.000000 tgmount-1.0.5/tgmount/zip/zip_dir_factory.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     2382 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/zip/zip_file.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     1347 2023-02-01 21:22:26.000000 tgmount-1.0.5/tgmount/zip/zip_file_id3v1_fix.py
+-rw-r--r--   0 horn      (1000) horn      (1000)     5810 2023-04-26 06:14:22.000000 tgmount-1.0.5/tgmount/zip/zips_as_dirs.py
+drwxr-xr-x   0 horn      (1000) horn      (1000)        0 2023-04-26 07:30:00.548473 tgmount-1.0.5/tgmount.egg-info/
+-rw-r--r--   0 horn      (1000) horn      (1000)    19181 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/PKG-INFO
+-rw-r--r--   0 horn      (1000) horn      (1000)     5351 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/SOURCES.txt
+-rw-r--r--   0 horn      (1000) horn      (1000)        1 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/dependency_links.txt
+-rw-r--r--   0 horn      (1000) horn      (1000)       48 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/entry_points.txt
+-rw-r--r--   0 horn      (1000) horn      (1000)       66 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/requires.txt
+-rw-r--r--   0 horn      (1000) horn      (1000)        8 2023-04-26 07:30:00.000000 tgmount-1.0.5/tgmount.egg-info/top_level.txt
```

### Comparing `tgmount-1.0.4/PKG-INFO` & `tgmount-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: tgmount
-Version: 1.0.4
-Summary: Mount telegram messages as files
-Home-page: https://github.com/nktknshn/tgmount-ng
-Author: Nikita Kanashin
-Author-email: nikita@kanash.in
-Description-Content-Type: text/markdown
-
 # Overview
 
 Creates virtual file system with files posted on telegram.  
 <!-- tgmount lets you to mount files uploaded to telegram as a virtual file system 
 so access them like regular files from a cloud without downloading. This allows to use
 regular desktop media players to listen to music streaming it directly from telegram servers. Pictures and videos 
 
@@ -280,26 +271,26 @@
 
 Exclude repeating documents 
 
 `--include-unsupported`
 
 Include messages that are not supported for mounting
 
-`--only-unique-docs`
+`--only-unsupported`
 
 Print only them
 
 `--json`
 
 Print in json format
 
 ### tgmount download
 
 ```
-tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request_size REQUEST_SIZE] entity ids [ids ...]
+tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request-size REQUEST_SIZE] entity ids [ids ...]
 ```
 
 `--keep-filename`
 
 Keep original filenames
 
 `--output-dir`
@@ -357,14 +348,17 @@
 
   # telegram api credentials
   api_id: int
   api_hash: str
 
   # optional field
   request_size: 128KB
+
+  # optional field. Default: False
+  use_ipv6: True
 ```
 
 ### message_sources
 A message source defines a list of messages that will be used in vfs tree construction. Every message source is a separate [TelegramClient.get_messages](https://docs.telethon.dev/en/stable/modules/client.html#telethon.client.messages.MessageMethods.get_messages) request. Message source is also subscribed to events of posting, removing and editing messages in the entity it is sourced from. 
 
 ```yaml
 message_sources:
@@ -432,26 +426,27 @@
   # optional. sets a filter for the current folder. Default is no filter
   filter: MessageWithMusic
   filter: {filter: MessageWithMusic}
 
   # sets a filter for the current folder and subfolders
   filter: {filter: MessageWithMusic, recursive: True}
 
-  # sets a filter for the current folder and subfolders overwriting another recursive filter if any 
+  # sets a filter for the current folder and subfolders overwriting another 
+  # recursive filter if any 
   filter: {filter: MessageWithMusic, overwright: True, recursive: True}
 
   # the following combines multiple filters. Only messages that match every filter
   # in the list will pass. The filter below allows all documents that
   # that are not video, photo or audio and not a zip file 
   filter: 
     - MessageWithOtherDocument
     - Not:
       - ByExtension: .zip
 
-  # on line
+  # in one line
   filter: {filter: [MessageWithOtherDocument, Not: {ByExtension: .zip}], overwright: True, recursive: True}
 
   # defines a producer that controls the content of the folder. 
   # Default is PlainDir
   producer: BySender
 
   # producer may have properties
@@ -492,15 +487,15 @@
 ```
 
 
 #### source
 
 Message source is a list of messages which is used to produce a directory content. Message source is initialized from get_messages() request and is updated by events of posting message, removing message and editing message in the corresponding entity. 
 
-Producer is subscribed to a message source and takes a care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
+Producer is subscribed to a message source and takes care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
 
 The content of a folder is defined by a combination of properties `source`, `filter`, `producer` and `treat_as`. 
 
 This will create a tree of empty folders
 ```yaml
 root:
   everything:
@@ -720,8 +715,8 @@
 In case of mounting a config set `fix_id3v1` property of `UnpackedZip` to False:
 ```yaml
 producer: {UnpackedZip: {fix_id3v1: False}}
 ```
 
 ## Known bugs
 - No updates received during reconnection
-- Combination of `--filter`, `--offset-date` and `--reverse` always returns empty result
+- Combination of `--filter`, `--offset-date` and `--reverse` always returns empty result
```

### Comparing `tgmount-1.0.4/README.md` & `tgmount-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1
+Name: tgmount
+Version: 1.0.5
+Summary: Mount telegram messages as files
+Home-page: https://github.com/nktknshn/tgmount-ng
+Author: Nikita Kanashin
+Author-email: nikita@kanash.in
+Description-Content-Type: text/markdown
+
 # Overview
 
 Creates virtual file system with files posted on telegram.  
 <!-- tgmount lets you to mount files uploaded to telegram as a virtual file system 
 so access them like regular files from a cloud without downloading. This allows to use
 regular desktop media players to listen to music streaming it directly from telegram servers. Pictures and videos 
 
@@ -271,26 +280,26 @@
 
 Exclude repeating documents 
 
 `--include-unsupported`
 
 Include messages that are not supported for mounting
 
-`--only-unique-docs`
+`--only-unsupported`
 
 Print only them
 
 `--json`
 
 Print in json format
 
 ### tgmount download
 
 ```
-tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request_size REQUEST_SIZE] entity ids [ids ...]
+tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request-size REQUEST_SIZE] entity ids [ids ...]
 ```
 
 `--keep-filename`
 
 Keep original filenames
 
 `--output-dir`
@@ -348,14 +357,17 @@
 
   # telegram api credentials
   api_id: int
   api_hash: str
 
   # optional field
   request_size: 128KB
+
+  # optional field. Default: False
+  use_ipv6: True
 ```
 
 ### message_sources
 A message source defines a list of messages that will be used in vfs tree construction. Every message source is a separate [TelegramClient.get_messages](https://docs.telethon.dev/en/stable/modules/client.html#telethon.client.messages.MessageMethods.get_messages) request. Message source is also subscribed to events of posting, removing and editing messages in the entity it is sourced from. 
 
 ```yaml
 message_sources:
@@ -423,26 +435,27 @@
   # optional. sets a filter for the current folder. Default is no filter
   filter: MessageWithMusic
   filter: {filter: MessageWithMusic}
 
   # sets a filter for the current folder and subfolders
   filter: {filter: MessageWithMusic, recursive: True}
 
-  # sets a filter for the current folder and subfolders overwriting another recursive filter if any 
+  # sets a filter for the current folder and subfolders overwriting another 
+  # recursive filter if any 
   filter: {filter: MessageWithMusic, overwright: True, recursive: True}
 
   # the following combines multiple filters. Only messages that match every filter
   # in the list will pass. The filter below allows all documents that
   # that are not video, photo or audio and not a zip file 
   filter: 
     - MessageWithOtherDocument
     - Not:
       - ByExtension: .zip
 
-  # on line
+  # in one line
   filter: {filter: [MessageWithOtherDocument, Not: {ByExtension: .zip}], overwright: True, recursive: True}
 
   # defines a producer that controls the content of the folder. 
   # Default is PlainDir
   producer: BySender
 
   # producer may have properties
@@ -483,15 +496,15 @@
 ```
 
 
 #### source
 
 Message source is a list of messages which is used to produce a directory content. Message source is initialized from get_messages() request and is updated by events of posting message, removing message and editing message in the corresponding entity. 
 
-Producer is subscribed to a message source and takes a care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
+Producer is subscribed to a message source and takes care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
 
 The content of a folder is defined by a combination of properties `source`, `filter`, `producer` and `treat_as`. 
 
 This will create a tree of empty folders
 ```yaml
 root:
   everything:
@@ -711,8 +724,8 @@
 In case of mounting a config set `fix_id3v1` property of `UnpackedZip` to False:
 ```yaml
 producer: {UnpackedZip: {fix_id3v1: False}}
 ```
 
 ## Known bugs
 - No updates received during reconnection
-- Combination of `--filter`, `--offset-date` and `--reverse` always returns empty result
+- Combination of `--filter`, `--offset-date` and `--reverse` always returns empty result
```

### Comparing `tgmount-1.0.4/setup.py` & `tgmount-1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             package_name = relpath.replace(os.sep, ".")
             packages.append(package_name)
 
     assert packages
 
     setup(
         name="tgmount",
-        version="1.0.4",
+        version="1.0.5",
         description="Mount telegram messages as files",
         author="Nikita Kanashin",
         author_email="nikita@kanash.in",
         url="https://github.com/nktknshn/tgmount-ng",
         packages=packages,
         long_description=long_description,
         long_description_content_type="text/markdown",
```

### Comparing `tgmount-1.0.4/tgmount/cache/cache_in_blocks.py` & `tgmount-1.0.5/tgmount/cache/cache_in_blocks.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cache/file.py` & `tgmount-1.0.5/tgmount/cache/file.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cache/file_source.py` & `tgmount-1.0.5/tgmount/cache/file_source.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cache/memory.py` & `tgmount-1.0.5/tgmount/cache/memory.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cache/reader.py` & `tgmount-1.0.5/tgmount/cache/reader.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cache/types.py` & `tgmount-1.0.5/tgmount/cache/types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cli/download.py` & `tgmount-1.0.5/tgmount/cli/download.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cli/list_documents.py` & `tgmount-1.0.5/tgmount/cli/list_documents.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cli/mount.py` & `tgmount-1.0.5/tgmount/cli/mount.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import sqlite3
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 import yaml
 
 from tgmount import config
 from tgmount.config.config import ConfigParser
-from tgmount.tgmount.validator import ConfigValidator
 from tgmount.config.types import parse_datetime
+from tgmount.error import TgmountError
 from tgmount.tgclient.fetcher import TelegramMessagesFetcher
 from tgmount.tgmount.tgmount_builder import TgmountBuilder
-from tgmount.error import TgmountError
 from tgmount.tgmount.tgmount_providers import ProducersProvider
+from tgmount.tgmount.validator import ConfigValidator
 from tgmount.util import int_or_string, map_none, yes
+
 from .logger import logger
 
 
 def add_get_messages_args(parser: ArgumentParser):
     parser.add_argument(
         "--filter",
         type=str,
@@ -31,15 +33,15 @@
 
     parser.add_argument("--reply-to", type=int, dest="reply_to")
     parser.add_argument("--from-user", type=int_or_string, dest="from_user")
     parser.add_argument("--reverse", default=False, action="store_true", dest="reverse")
 
 
 def add_mount_arguments(command_mount: ArgumentParser):
-    command_mount.add_argument("entity", type=str)
+    command_mount.add_argument("entity", type=int_or_string)
     command_mount.add_argument("mount_dir", type=str, metavar="mount-dir")
 
     config_arg = command_mount.add_mutually_exclusive_group()
 
     add_get_messages_args(command_mount)
 
     config_arg.add_argument(
@@ -83,44 +85,48 @@
 
 
 async def mount(
     args: Namespace,
     *,
     api_credentials: Optional[tuple[int, str]] = None,
     session: Optional[str] = None,
+    loop=None,
 ):
     builder = TgmountBuilder()
     validator = ConfigValidator(builder)
 
+    source_id = str(args.entity)
+
     producer = None
     root_content = {
-        "source": {"source": args.entity, "recursive": True},
+        "source": {"source": source_id, "recursive": True},
         "filter": "MessageDownloadable" if not args.mount_texts else "All",
-        ".sysinfo": {"producer": "SysInfo", "source": args.entity},
+        ".sysinfo": {"producer": "SysInfo", "source": source_id},
     }
 
     if yes(args.root_config, str):
         try:
             with open(args.root_config, "r+") as f:
                 cfg_dict: dict = yaml.safe_load(f)
+                # XXX validate
                 root_content.update(cfg_dict)
         except Exception as e:
             raise TgmountError(f"Error load config file:\n\n{e}")
 
     if yes(args.producer, str):
         producer = builder.producers.get_by_name(args.producer)
 
         if producer is None:
             raise TgmountError(f"Invalid producer: {args.producer}")
 
     if api_credentials is None:
-        raise TgmountError(f"Missing api_credentials")
+        raise TgmountError("Missing api_credentials")
 
     if session is None:
-        raise TgmountError(f"Missing session")
+        raise TgmountError("Missing session")
 
     if yes(producer):
         root_content["producer"] = {
             args.producer: {"fix_id3v1": not args.no_fix_id3v1},
         }
 
         if args.producer == "UnpackedZip":
@@ -128,23 +134,25 @@
                 "type": "memory",
                 "capacity": "300MB",
                 "block_size": "256KB",
             }
 
     logger.debug(f"{root_content}")
     config_parser = ConfigParser()
+
     cfg = config.Config(
         client=config.Client(
             session=session,
             api_id=api_credentials[0],
             api_hash=api_credentials[1],
+            use_ipv6=args.use_ipv6,
         ),
         message_sources=config.MessageSources(
             sources={
-                args.entity: config.MessageSource(
+                source_id: config.MessageSource(
                     entity=args.entity,
                     filter=args.filter,
                     from_user=args.from_user,
                     limit=args.limit,
                     max_id=args.max_id,
                     min_id=args.min_id,
                     offset_date=args.offset_date,
@@ -157,26 +165,33 @@
             }
         ),
         root=config_parser.parse_root(root_content),
     )
 
     await validator.verify_config(cfg)
 
-    tgm = await builder.create_tgmount(cfg)
+    logger.debug("Creating tgmount")
+
+    try:
+        tgm = await builder.create_tgmount(cfg, loop=loop)
+    except sqlite3.OperationalError as e:
+        logger.error(f"{e}")
+        # logger.error(f"Database is locked")
+        return
 
     try:
-        logger.debug(f"Connecting Telegram")
+        logger.debug("Connecting Telegram")
         await tgm.client.auth()
     except Exception as e:
         # await tgm.client.disconnect()
         raise TgmountError(f"Error while authenticating the client: {e}")
 
     if not tgm.client.is_connected():  # type: ignore
         raise TgmountError(
-            f"Error while connecting the client. Check api_id and api_hash"
+            "Error while connecting the client. Check api_id and api_hash"
         )
 
     await tgm.mount(
         mount_dir=args.mount_dir,
         debug_fuse=args.debug_fuse,
         min_tasks=args.min_tasks,
     )
```

### Comparing `tgmount-1.0.4/tgmount/cli/mount_config.py` & `tgmount-1.0.5/tgmount/cli/mount_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,35 +53,29 @@
 
     await validator.verify_config(cfg)
 
     if session is not None:
         cfg.client = replace(cfg.client, session=session)
 
     if api_credentials is not None:
-        logger.info(f"Using api credentials from os enviroment or args")
+        logger.info(f"Using api credentials from os environment or args")
         cfg.client = replace(
             cfg.client, api_id=api_credentials[0], api_hash=api_credentials[1]
         )
 
-    # if subfolder is not None:
-    #     subfolder_root = cfg.root.content.get(subfolder)
-
-    #     if subfolder_root is None:
-    #         raise TgmountError(f"Invalid subfolder")
-
     tgm = await builder.create_tgmount(cfg)
 
     try:
         logger.info(f"Connecting Telegram")
         await tgm.client.auth()
     except Exception as e:
         # await tgm.client.disconnect()
         raise TgmountError(f"Error while authenticating the client: {e}")
 
-    if not tgm.client.is_connected():
+    if not tgm.client.is_connected():  # type: ignore
         raise TgmountError(
             f"Error while connecting the client. Check api_id and api_hash"
         )
 
     # client: TgmountTelegramClient = tgm.client
 
     # async def printa(c):
```

### Comparing `tgmount-1.0.4/tgmount/cli/stats.py` & `tgmount-1.0.5/tgmount/cli/stats.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/cli/validate.py` & `tgmount-1.0.5/tgmount/cli/validate.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/client.py` & `tgmount-1.0.5/tgmount/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import argparse
 import logging
 
 from tgmount import cli
 from tgmount import main as main_settings
 from tgmount.cli.util import get_client, get_tgapp_and_session
+from tgmount.cli.util.read_env import try_get_tgapp_and_session
 
 from tgmount.main.util import run_main
 from tgmount.tglog import init_logging
 from tgmount.error import TgmountError
 
 
 def get_parser():
@@ -21,14 +22,22 @@
     parser.add_argument("--tgapp", type=str, required=False)
 
     parser.add_argument("--debug", default=False, action="store_true")
     parser.add_argument(
         "--debug-fs-ops", default=False, action="store_true", dest="debug_fs_ops"
     )
 
+    parser.add_argument(
+        "--use-ipv6",
+        action="store_true",
+        default=False,
+        help="enable IPv6",
+        dest="use_ipv6",
+    )
+
     commands_subparsers = parser.add_subparsers(dest="command")
 
     # command_auth = commands_subparsers.add_parser("auth")
     command_mount = commands_subparsers.add_parser("mount-config")
     command_mount_args = commands_subparsers.add_parser("mount")
     command_validate = commands_subparsers.add_parser("validate")
     # command_stats = commands_subparsers.add_parser("stats")
@@ -47,74 +56,80 @@
     cli.add_validate_arguments(command_validate)
     cli.add_download_arguments(command_download)
 
     return parser, command_list
 
 
 async def client_main(loop):
-
     parser, command_list = get_parser()
     args = parser.parse_args()
 
     init_logging(
         debug_level=logging.DEBUG if args.debug else logging.INFO,
         debug_fs_ops=args.debug_fs_ops,
     )
 
     if args.command == "list" and args.list_subcommand == "dialogs":
         session, api_id, api_hash = get_tgapp_and_session(args)
 
-        async with get_client(session, api_id, api_hash, loop=loop) as client:
+        async with get_client(
+            session, api_id, api_hash, loop=loop, use_ipv6=args.use_ipv6
+        ) as client:
             await cli.list_dialogs(client)
 
     elif args.command == "list" and args.list_subcommand == "documents":
         session, api_id, api_hash = get_tgapp_and_session(args)
 
-        async with get_client(session, api_id, api_hash, loop=loop) as client:
+        async with get_client(
+            session, api_id, api_hash, loop=loop, use_ipv6=args.use_ipv6
+        ) as client:
             await cli.list_documents(client, args)
     elif args.command == "list":
         command_list.print_help()
     elif args.command == "mount-config":
-        session, api_id, api_hash = get_tgapp_and_session(args)
+        session, api_id, api_hash = try_get_tgapp_and_session(args)
 
         api_credentials = (
             (api_id, api_hash) if api_id is not None and api_hash is not None else None
         )
+
         await cli.mount_config(
             args.config,
             api_credentials=api_credentials,
-            session=args.session,
+            session=session,
             mount_dir=args.mount_dir,
             debug_fuse=args.debug_fuse,
             min_tasks=args.min_tasks,
-            # run_server=args.run_server,
+            # use_ipv6=args.use_ipv6,
         )
     elif args.command == "mount":
         session, api_id, api_hash = get_tgapp_and_session(args)
 
         api_credentials = (
             (api_id, api_hash) if api_id is not None and api_hash is not None else None
         )
+
         await cli.mount(
-            args,
-            api_credentials=api_credentials,
-            session=session,
+            args, api_credentials=api_credentials, session=session, loop=loop
         )
+
     elif args.command == "stats":
         session, api_id, api_hash = get_tgapp_and_session(args)
 
-        async with get_client(session, api_id, api_hash, loop=loop) as client:
+        async with get_client(
+            session, api_id, api_hash, loop=loop, use_ipv6=args.use_ipv6
+        ) as client:
             await cli.stats(args)
     elif args.command == "validate":
         await cli.validate(args)
     elif args.command == "download":
-
         session, api_id, api_hash = get_tgapp_and_session(args)
-        async with get_client(session, api_id, api_hash, loop=loop) as client:
-
+        async with get_client(
+            session, api_id, api_hash, loop=loop, use_ipv6=args.use_ipv6
+        ) as client:
             await cli.download(client, args)
 
     else:
         parser.print_help()
 
 
 def main():
```

### Comparing `tgmount-1.0.4/tgmount/common/filter.py` & `tgmount-1.0.5/tgmount/common/filter.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/config/config.py` & `tgmount-1.0.5/tgmount/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from tgmount.util import get_bytes_count, map_none, no
 from tgmount.util.col import get_first_pair
 
 
 from .logger import logger
 from collections.abc import Mapping
 from .reader import PropertyReader, ConfigContext
+from . import types
 
 T = TypeVar("T")
 
 
 def ensure_list(value: T | list[T]) -> list[T]:
     if isinstance(value, list):
         return value
@@ -36,30 +37,30 @@
             return (value, None)
         elif t == "mapping":
             self.ctx.assert_that(
                 len(value) == 1, "Filter is a mapping with one key or a string"
             )
             return get_first_pair(value)
         else:
-            self.ctx.fail(f"Invalid filter value item: {value}")
+            return self.ctx.fail(f"Invalid filter value item: {value}")
 
     def parse_filter_value(self, value: Any) -> FilterInputType:
         t = self.typeof_value(value)
 
         if t == "string" or t == "mapping":
             return [self.parse_filter_value_item(value)]
         elif t == "list":
             result = []
             for idx, el in enumerate(value):
                 result.append(
                     self.add_path(str(idx)).parse_filter_value_item(el),
                 )
             return result
 
-        self.ctx.fail_typecheck(f"Invalid filter value {value}")
+        return self.ctx.fail_typecheck(f"Invalid filter value {value}")
 
     def read_filter_value(self):
         filter_value = self.get_key("filter")
 
         self.result["filter"] = self.add_path("filter").parse_filter_value(filter_value)
 
 
@@ -68,15 +69,14 @@
         super().__init__(ctx)
 
     @property
     def klass(self):
         return CachesReader
 
     def read_caches(self) -> config.Caches | None:
-
         result = {}
         caches = self
 
         for cache_id in caches.keys():
             result[cache_id] = caches.enter(cache_id).read_cache()
 
         return config.Caches(result)
@@ -238,15 +238,14 @@
             pass
         else:
             self.ctx.fail(f"Invalid wrapper value: {wrapper_prop_value}")
 
         return wrapper_prop
 
     def read_root(self):
-
         source_prop = self.read_source_prop()
         filter_prop = self.read_filter_prop()
         cache_prop = self.read_cache_prop()
         producer_prop = self.read_producer_prop()
         treat_as_prop = self.read_treat_as_prop()
         wrapper_prop = self.read_wrappers_prop()
 
@@ -281,15 +280,17 @@
     def __init__(self, ctx: "ConfigContext") -> None:
         super().__init__(ctx)
 
     def read_client(self) -> config.Client:
         self.string("session")
         self.integer("api_id")
         self.string("api_hash")
-        self.getter("request_size", get_bytes_count)
+        self.getter("request_size", get_bytes_count, optional=True)
+        self.boolean("use_ipv6", optional=True, default=False)
+
         return config.Client(**self.get())
 
     def read_message_sources(self):
         result = {}
         for source_id in self.keys():
             source_reader = self.enter(source_id)
             result[source_id] = source_reader.read_message_source()
@@ -298,15 +299,14 @@
 
     def read_message_source(self):
         return self.ctx.failing(
             lambda: config.MessageSource.from_mapping(self.ctx.mapping),
         )
 
     def read_config(self) -> config.Config:
-
         mount_dir = self.string("mount_dir", True)
         client = self.enter("client").read_client()
 
         message_sources = self.enter("message_sources").read_message_sources()
 
         if self.has("caches"):
             caches = self.enter("caches").read_caches()
@@ -320,17 +320,14 @@
             client=client,
             message_sources=message_sources,
             caches=caches,
             root=root,
         )
 
 
-from . import types
-
-
 class ConfigParser(ConfigParserProto, ConfigParserFilter):
     def parse_root(self, mapping: Mapping) -> types.DirConfig:
         return ConfigReader(ConfigContext(mapping)).read_root()
 
     def parse_config(self, mapping: Mapping) -> types.Config:
         return ConfigReader(ConfigContext(mapping)).read_config()
```

### Comparing `tgmount-1.0.4/tgmount/config/config_type.py` & `tgmount-1.0.5/tgmount/config/config_type.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/config/error.py` & `tgmount-1.0.5/tgmount/config/error.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/config/helpers.py` & `tgmount-1.0.5/tgmount/config/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 )
 from tgmount.config.util import get_type_name
 
 from tgmount.util import col, none_fallback
 from .logger import logger
 
 T = TypeVar("T")
+R = TypeVar("R")
 
 
 @overload
 def assert_that(condition: TypeGuard[T], error: Exception) -> TypeGuard[T]:
     ...
 
 
@@ -41,19 +42,17 @@
     return True
 
 
 def _typecheck_union(
     value,
     typ,
 ):
-
     type_args = typing.get_args(typ)
 
     if type(value) is list:
-
         for arg in type_args:
             _type_origin = typing.get_origin(arg)
 
             if _type_origin is list:
                 (_typ,) = typing.get_args(arg)
                 for v in value:
                     if type(v) is not _typ:
@@ -195,31 +194,7 @@
 
         if isinstance(cls, Type):
             return load_class_from_mapping(cls, d)
 
         return cls(d)
 
     return {k: load_class(v) for k, v in d.items()}
-
-
-T = TypeVar("T")
-R = TypeVar("R")
-
-# Tree = T | Mapping[str, "Tree[T]"]
-
-
-# def fold_tree(
-#     f: Callable[[T, R], R],
-#     tree: Tree[T],
-#     initial: R,
-# ) -> R:
-#     res = initial
-#     if isinstance(tree, Mapping):
-#         for k, v in tree.items():
-#             if isinstance(v, Mapping):
-#                 res = fold_tree(f, v, res)
-#             else:
-#                 res = f(v, res)
-#     else:
-#         return f(tree, res)
-
-#     return res
```

### Comparing `tgmount-1.0.4/tgmount/config/reader.py` & `tgmount-1.0.5/tgmount/config/reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,27 +162,26 @@
             raise e
         except Exception as e:
             self.ctx.fail(e)
 
     def typeof_value(self, value: Any) -> ValueType:
         if isinstance(value, list):
             return "list"
-
         if isinstance(value, str):
             return "string"
         if isinstance(value, (Mapping, dict)):
             return "mapping"
         if isinstance(value, int):
             return "integer"
         if isinstance(value, bool):
             return "boolean"
         if value is None:
             return "none"
 
-        self.ctx.fail(f"Unsupported type: {value}")
+        return self.ctx.fail(f"Unsupported type: {value}")
 
     def typeof(self, key: str) -> ValueType:
         return self.typeof_value(self.get_key(key))
 
     def value_with_type(self, key: str, optional=False) -> tuple[Any, ValueType]:
         value = self.get_key(key, optional=optional)
 
@@ -227,21 +226,22 @@
     def get_property(self, key: str, typ: Type[T]):
         pass
 
     def keys(self) -> list[str]:
         return list(self.mapping.keys())
 
     def failing(self, lazy_value: Callable[[], T]) -> T:
+        """Runs `lazy_value` wrapping exception into `ConfigErrorWithPath`"""
         try:
             return lazy_value()
         except Exception as e:
             self.fail(e)
 
     def enter(self, key: str) -> "ConfigContext":
-        self.logger.debug(f"enter({key}")
+        self.logger.debug(f"enter({key})")
         mapping = self.mapping.get(key)
 
         if mapping is None:
             self.fail(f"Missing key: {key}")
 
         self.assert_type(mapping, dict, f"Cannot enter key `{key}`. Expected mapping.")
 
@@ -261,15 +261,14 @@
 
     def assert_type(
         self, value: Any, typ: Type, error: InputErrorType | None = None
     ) -> Any:
         if isinstance(value, typ):
             return value
 
-        # ConfigError()
         self.fail(
             TypecheckError(typ, type(value), map_none(error, self.get_error)),
         )
 
     def assert_that(self, condition, error):
         if not condition:
             self.fail(self.get_error(error))
```

### Comparing `tgmount-1.0.4/tgmount/config/types.py` & `tgmount-1.0.5/tgmount/config/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 
 @dataclass
 class Client:
     session: str
     api_id: int
     api_hash: str
     request_size: int | None = None
+    use_ipv6: bool = False
 
     @staticmethod
     def from_mapping(mapping: Mapping) -> "Client":
         return load_class_from_mapping(
             Client,
             mapping,
             loaders={
```

### Comparing `tgmount-1.0.4/tgmount/controlserver/server.py` & `tgmount-1.0.5/tgmount/controlserver/server.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/fs/fh.py` & `tgmount-1.0.5/tgmount/fs/fh.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/fs/inode.py` & `tgmount-1.0.5/tgmount/fs/inode.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/fs/operations.py` & `tgmount-1.0.5/tgmount/fs/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from tgmount.vfs.util import MyLock
 from .fh import FileSystemHandles
 from .inode import InodesRegistry, RegistryItem, RegistryRoot
 from .util import (
     create_directory_attributes,
     create_file_attributes,
     exception_handler,
+    flags_to_str,
 )
 
 
 """ 
 TODO
 lookup coconut
 
@@ -54,15 +55,14 @@
 )
 
 
 class FileSystemOperationsMixin:
     def get_inodes_tree(
         self: "FileSystemOperations", inode=InodesRegistry.ROOT_INODE  # type: ignore
     ) -> InodesTree:
-
         item = self.inodes.get_item_by_inode(inode)
 
         if item is None:
             raise ValueError(f"item with {inode} was not found")
 
         inodes = self.inodes
 
@@ -101,15 +101,14 @@
         )
 
 
 from .logger import logger
 
 
 class FileSystemOperations(pyfuse3.Operations, FileSystemOperationsMixin):
-
     FsRegistryItem = RegistryItem[FileSystemItem] | RegistryRoot[FileSystemItem]
     logger = logger.getChild(f"FileSystemOperations")
 
     def __init__(
         self,
         root: vfs.DirLike,
     ):
@@ -192,15 +191,14 @@
                 size=item.content.size,
                 stamp=int(item.creation_time.timestamp() * 1e9),
             )
 
     def update_subitem(
         self, path: str, new_item: vfs.DirContentItem, parent_inode: int
     ):
-
         self.logger.debug(
             f"update_subitem: {new_item.name}, parent_inode={parent_inode} ({self.inodes.get_item_path(parent_inode)})"
         )
 
         # old_fs_item = self.inodes.get_child_item_by_name(new_item.name, parent_inode)
         old_fs_item = self.inodes.get_by_path(path)
 
@@ -238,15 +236,14 @@
         item.data.attrs.st_ino = item.inode
         item.data.attrs.st_ctime_ns = old_fs_item.data.attrs.st_ctime_ns
         item.data.attrs.st_mtime_ns = int(datetime.now().timestamp() * 1e9)
 
         return item
 
     def add_subitem(self, vfs_item: vfs.DirContentItem, parent_inode: int):
-
         self.logger.debug(
             f"add_subitem: {vfs_item.name}, parent_inode={parent_inode} ({self.inodes.get_item_path(parent_inode)})"
         )
 
         fs_item = self.create_FileSystemItem(
             vfs_item,
             self._create_attributes_for_item(vfs_item, inode=0),
@@ -457,47 +454,35 @@
 
         self._handles.release_fh(fh)
         self.logger.debug("= releasedir(): ok")
 
     @measure_time(logger_func=logger.debug)
     @exception_handler
     async def open(self, inode, flags, ctx):
-
         handle = None
 
         item = self._inodes.get_item_by_inode(inode)
 
         if item is None:
             self.logger.error(f"open({inode}) missing inode")
             raise pyfuse3.FUSEError(errno.ENOENT)
 
         if not vfs.FileLike.guard(item.data.structure_item):
             self.logger.error(f"open({inode}): is not file")
             raise pyfuse3.FUSEError(errno.EIO)
 
-        # if flags & os.O_RDWR or flags & os.O_WRONLY:
-
-        # parent_dir = self.inodes.get_parent(inode)
-
-        # if parent_dir is None:
-        #     self.logger.error("open(): missing parent")
-        #     raise pyfuse3.FUSEError(errno.EIO)
-
-        # if not vfs.DirLike.guard(parent_dir.data.structure_item):
-        #     self.logger.error("open(): parent is not a folder")
-        #     raise pyfuse3.FUSEError(errno.EIO)
-
         # parent_dir.data.structure_item.writable
+        self.logger.debug(
+            f"= open({inode}, flags={flags_to_str(flags)}) = {item.data.structure_item.name}"
+        )
 
         if flags & os.O_RDWR or flags & os.O_WRONLY:
             self.logger.error("open(): readonly")
             raise pyfuse3.FUSEError(errno.EPERM)
 
-        self.logger.debug(f"= open({inode}) = {item.data.structure_item.name}")
-
         handle = await item.data.structure_item.content.open_func()
 
         fh = self._handles.open_fh(item, handle)
 
         self.logger.debug(
             f"- done open({inode}): fh={fh}, name={item.data.structure_item.name}"
         )
```

### Comparing `tgmount-1.0.4/tgmount/fs/update.py` & `tgmount-1.0.5/tgmount/fs/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 class FileSystemOperationsUpdatable(FileSystemOperations):
     def __init__(self, root: vfs.DirLike):
         super().__init__(root)
 
         self._removed_items = []
 
     async def update(self, update: FileSystemOperationsUpdate):
-
         for f in update.new_files:
             self.logger.info(f"New file: {f}")
 
         for path, filelike in update.update_items.items():
             parent_path = os.path.dirname(path)
             parent_item = self.inodes.get_by_path(parent_path)
 
@@ -92,15 +91,14 @@
             # skip adding subitems into inode registries
             if not self.inodes.was_content_read(parent_item):
                 continue
 
             self.add_subitem(filelike, parent_item.inode)
 
         for path, dir_like_or_content in update.new_dirs.items():
-
             parent_path = os.path.dirname(path)
             name = os.path.basename(path)
             parent_item = self.inodes.get_by_path(parent_path)
 
             if parent_item is None:
                 self.logger.debug(f"on_update: new_files: {path} is not in inodes")
                 continue
@@ -115,15 +113,14 @@
                 if isinstance(dir_like_or_content, vfs.DirLike)
                 else vfs.DirLike(name, dir_like_or_content)
             )
 
             self.add_subitem(vfs_item, parent_item.inode)
 
         for path in update.removed_files:
-
             self.logger.info(f"Removed file: {path}")
 
             item = self.inodes.get_by_path(path)
             if item is None:
                 self.logger.debug(
                     f"on_update: update_dir_content: {path} is not in inodes"
                 )
@@ -132,14 +129,16 @@
                 pyfuse3.invalidate_entry_async(
                     item.parent_inode, item.name, ignore_enoent=True
                 )
 
             await self._remove_item(item)
 
         for path in update.removed_dirs:
+            self.logger.info(f"Removed dir: {path}")
+
             item = self.inodes.get_by_path(path)
 
             if item is None:
                 self.logger.debug(
                     f"on_update: update_dir_content: {path} is not in inodes"
                 )
                 continue
```

### Comparing `tgmount-1.0.4/tgmount/fs/util.py` & `tgmount-1.0.5/tgmount/fs/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -131,7 +131,38 @@
 
 
 def bytes_to_str(bs: bytes | list[bytes]) -> str | list[str]:
     if isinstance(bs, list):
         return list(map(lambda b: b.decode("utf-8"), bs))
 
     return bs.decode("utf-8")
+
+
+""" 
+https://man7.org/linux/man-pages/man2/open.2.html
+"""
+open_flags = [
+    "O_RDWR",
+    "O_WRONLY",
+    "O_RDONLY",
+    "O_CLOEXEC",
+    "O_CREAT",
+    "O_DIRECTORY",
+    "O_EXCL",
+    "O_NOCTTY",
+    "O_NOFOLLOW",
+    "O_TMPFILE",
+    "O_TRUNC",
+    "O_DIRECT",
+]
+
+
+def flags_to_str(flags: int) -> str:
+    flags_strs = []
+
+    for f in open_flags:
+        flag = getattr(os, f)
+
+        if flags & flag:
+            flags_strs.append(f)
+
+    return ",".join(flags_strs)
```

### Comparing `tgmount-1.0.4/tgmount/fs/writable.py` & `tgmount-1.0.5/tgmount/fs/writable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 import errno
 import os
 from dataclasses import dataclass, field
 
 import pyfuse3
+from tgmount.fs.update import FileSystemOperationsUpdatable
+from tgmount.fs.util import flags_to_str
 
 import tgmount.vfs as vfs
 from tgmount.util.col import map_keys
+from tgmount.vfs.types.file import FileContentWritableProto
 
 from .inode import InodesRegistry, RegistryItem
 from .operations import FileSystemOperations
+from .logger import logger
 
 
-class FileSystemOperationsWritable(FileSystemOperations):
+class FileSystemOperationsWritable(FileSystemOperationsUpdatable):
+    logger = logger.getChild("FileSystemOperationsWritable")
+
     def __init__(self, root: vfs.DirLike):
         super().__init__(root)
 
     """ 
     Create a file with permissions *mode* and open it with *flags*.
 
     *ctx* will be a `RequestContext` instance.
@@ -39,44 +45,51 @@
     ):
         parent_dir = self.inodes.get_item_by_inode(parent_inode)
 
         if parent_dir is None:
             self.logger.error("create(): missing parent")
             raise pyfuse3.FUSEError(errno.EIO)
 
+        self.logger.debug(
+            f"create(f{parent_dir.name}, {name}, {mode}, flags={flags_to_str(flags)})"
+        )
+
+        if not flags & os.O_WRONLY:
+            self.logger.warning("create(): write only creation is only supported")
+            raise pyfuse3.FUSEError(errno.EPERM)
+
         if not vfs.DirLike.guard(parent_dir.data.structure_item):
             self.logger.error("create(): parent is not a folder")
             raise pyfuse3.FUSEError(errno.EIO)
 
-        if not parent_dir.data.structure_item.writable:
-            self.logger.warning("create(): parent_dir is not writable")
-            raise pyfuse3.FUSEError(errno.EPERM)
+        # if not parent_dir.data.structure_item.writable:
+        #     self.logger.warning("create(): parent_dir is not writable")
+        #     raise pyfuse3.FUSEError(errno.EPERM)
 
-        if not vfs.DirContentProtoWritable.guard(
+        if not vfs.DirContentWritableProto.guard(
             parent_dir.data.structure_item.content
         ):
             self.logger.warning("create(): parent_dir content is not writable")
             raise pyfuse3.FUSEError(errno.EPERM)
 
         filelike = await parent_dir.data.structure_item.content.create(
             self._bytes_to_str(name)
         )
 
-        attrs = self._create_attributes_for_item(filelike, inode=None)
-        fs_item = self.create_FileSystemItem(filelike, attrs)
+        item = self.add_subitem(filelike, parent_inode)
 
-        item = self.inodes.add_item_to_inodes(name, fs_item, parent_inode=parent_inode)
+        # attrs = self._create_attributes_for_item(filelike, inode=None)
+        # fs_item = self.create_FileSystemItem(filelike, attrs)
 
-        fh = self._handles.open_fh(item, None)
-        attrs.st_ino = item.inode
+        # item = self.inodes.add_item_to_inodes(name, fs_item, parent_inode=parent_inode)
+        # attrs.st_ino = item.inode
 
-        if flags & os.O_RDWR or flags & os.O_WRONLY:
-            pass
+        fh = self._handles.open_fh(item, None)
 
-        return (pyfuse3.FileInfo(fh), attrs)
+        return (pyfuse3.FileInfo(fh), item.data.attrs)
 
     """ 
     Write *buf* into *fh* at *off*.
 
     *fh* will be an integer filehandle returned by a prior `open` or
     `create` call.
 
@@ -92,16 +105,34 @@
 
         item, handle = self._handles.get_by_fh(fh)
 
         if item is None:
             self.logger.error(f"write(fh={fh}): missing item in open handles")
             return
 
+        self.logger.debug(f"writing into {item.name}. inode = {item.inode}")
+
         if not vfs.FileLike.guard(
             item.data.structure_item,
         ):
             self.logger.error(f"release({fh}): is not file")
             raise pyfuse3.FUSEError(errno.EIO)
 
         if not item.data.structure_item.writable:
             self.logger.error(f"write({fh}): is not writable")
             raise pyfuse3.FUSEError(errno.EPERM)
+
+        if not FileContentWritableProto.guard(item.data.structure_item.content):
+            self.logger.error(f"write({fh}): content is not writable")
+            raise pyfuse3.FUSEError(errno.EPERM)
+
+        content = item.data.structure_item.content
+
+        try:
+            byte_written = await content.write(handle, off, buf)
+        except Exception as e:
+            self.logger.error(f"Error while writing: {e}")
+            raise e
+
+        item.data.attrs.st_size = content.size
+
+        return byte_written
```

### Comparing `tgmount-1.0.4/tgmount/main/util.py` & `tgmount-1.0.5/tgmount/main/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from tgmount.util.asyn import print_tasks_sync
 
 logger = logging.getLogger("tgvfs")
 
 
 def read_tgapp_api(tgapp_file="tgapp.txt"):
-    if "TGAPP" in os.environ:
+    if "TGAPP" in os.environ and ":" in os.environ:
         [api, hash] = os.environ["TGAPP"].split(":")
 
         api_id = int(api)
         api_hash = hash
 
         return api_id, api_hash
 
@@ -62,15 +62,14 @@
 
     main.mounted = True
 
     await pyfuse3.main(min_tasks=min_tasks)
 
 
 def run_main(main_func, forever=None, loop=None):
-
     loop = loop if loop is not None else asyncio.get_event_loop()
 
     loop.set_debug(True)
     # warnings.simplefilter('always', ResourceWarning)
     # warnings.filterwarnings("error")
 
     # loop.slow_callback_duration = 0.001
```

### Comparing `tgmount-1.0.4/tgmount/tgclient/auth.py` & `tgmount-1.0.5/tgmount/tgclient/auth.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/client.py` & `tgmount-1.0.5/tgmount/tgclient/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import logging
 
 import typing
-from abc import abstractmethod
-from typing import Optional, Protocol
+from typing import Optional
 
 import telethon
 from telethon import TelegramClient
 from tgmount import tglog
 
 from tgmount.tgclient.message_source_types import Subscribable
 from tgmount.util import map_none_else, yes
@@ -21,14 +20,15 @@
     ListenerNewMessages,
     ListenerRemovedMessages,
 )
 from telethon import events
 from .message_reaction_event import MessageReactionEvent
 
 from .logger import logger as module_logger
+from ..constants import client_info
 
 
 class TgmountTelegramClient(
     TelegramClient,
     TelegramAuthen,
     TelegramSearch,
     TgmountTelegramClientEventProto,
@@ -36,15 +36,15 @@
     logger = module_logger.getChild("TgmountTelegramClient")
 
     def __repr__(self):
         return f"TgmountTelegramClient({self.session.filename if yes(self.session) else None})"
 
     def __init__(
         self,
-        session_user_id,
+        session,
         api_id,
         api_hash,
         *,
         connection: "typing.Type[telethon.network.Connection]" = telethon.network.ConnectionTcpFull,
         use_ipv6: bool = False,
         proxy: Optional[typing.Union[tuple, dict]] = None,
         local_addr: Optional[typing.Union[str, tuple]] = None,
@@ -52,26 +52,25 @@
         request_retries: int = 5,
         connection_retries: int = 5,
         retry_delay: int = 1,
         auto_reconnect: bool = True,
         sequential_updates: bool = False,
         flood_sleep_threshold: int = 60,
         raise_last_call_error: bool = False,
-        device_model: Optional[str] = None,
-        system_version: Optional[str] = None,
-        app_version: Optional[str] = None,
-        lang_code: str = "en",
-        system_lang_code: str = "en",
+        device_model: Optional[str] = client_info['device_model'],
+        system_version: Optional[str] = client_info['system_version'],
+        app_version: Optional[str] = client_info['app_version'],
+        lang_code: str = client_info['lang_code'],
+        system_lang_code: str = client_info['system_lang_code'],
         loop: Optional[asyncio.AbstractEventLoop] = None,
         base_logger: Optional[typing.Union[str, logging.Logger]] = None,
         receive_updates: bool = True,
     ):
-
         super().__init__(
-            session_user_id,
+            session,
             api_id,
             api_hash,
             connection=connection,
             use_ipv6=use_ipv6,
             local_addr=local_addr,
             timeout=timeout,
             request_retries=request_retries,
@@ -88,22 +87,22 @@
             system_lang_code=system_lang_code,
             loop=loop,
             base_logger=base_logger,
             receive_updates=receive_updates,
             proxy=proxy,
         )  # type: ignore
 
-        # self.api_id = api_id
-        # self.api_hash = api_hash
         self.logger = TgmountTelegramClient.logger.getChild(
-            # self.session.filename if yes(self.session) else None,
-            map_none_else(self.session, lambda s: s.filename, "No session"),
+            # map_none_else(self.session, lambda s: s.filename, "No session"),
+            session,
             suffix_as_tag=True,
         )
 
+        self.logger.debug(f"TgmountTelegramClient(use_ipv6={use_ipv6})")
+
         async def aprint(d):
             print(d)
 
         self.on_disconnected = Subscribable()
 
         self._reconnections = 0
```

### Comparing `tgmount-1.0.4/tgmount/tgclient/client_types.py` & `tgmount-1.0.5/tgmount/tgclient/client_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/events_disptacher.py` & `tgmount-1.0.5/tgmount/tgclient/events_disptacher.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/fetcher.py` & `tgmount-1.0.5/tgmount/tgclient/fetcher/fetcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from tgmount import config
 from tgmount.tgclient.message_types import MessageProto
 from tgmount.tgclient.types import TotalListTyped
 from tgmount.error import TgmountError
 from tgmount.util import yes
 
-from .client_types import TgmountTelegramClientGetMessagesProto
+from ..client_types import TgmountTelegramClientGetMessagesProto
 from .logger import logger as module_logger
 
 from telethon.tl import types
 from tgmount.tgclient.guards import *
 
 
 class TelegramMessagesFetcherProto(Protocol):
@@ -59,15 +59,14 @@
 
         if filt is None:
             raise TgmountError(f"Invalid fetcher filter: {self.cfg.filter}")
 
         return filt
 
     async def fetch(self):
-
         self.logger.debug(f"fetching {self.cfg}")
 
         filt = None
 
         if yes(self.cfg.filter):
             filt = self._get_filter(self.cfg.filter)
```

### Comparing `tgmount-1.0.4/tgmount/tgclient/files_source.py` & `tgmount-1.0.5/tgmount/tgclient/files_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,26 @@
 
         if MessageWithDocument.guard(message):
             return SourceItemDocument(message.document)
 
         raise ValueError(f"Message {message} is not downloadable")
 
     def file_content(self, message: MessageDownloadable) -> vfs.FileContent:
-
         item = self.get_filesource_item(message)
 
         async def read_func(handle: Any, off: int, size: int) -> bytes:
             return await self.read(message, off, size)
 
         fc = vfs.FileContent(size=item.size, read_func=read_func)
 
         return fc
 
     async def read(
         self, message: MessageDownloadable, offset: int, limit: int
     ) -> bytes:
-
         return await self._message_read(message, offset, limit)
 
     async def _get_item_input_location(self, item: FileSourceItem) -> InputLocation:
         return item.input_location(
             self._get_item_file_reference(item),
         )
 
@@ -94,18 +92,15 @@
             # b"1" * 29
             item.file_reference,
         )
 
     def _set_item_file_reference(self, item: FileSourceItem, file_reference: bytes):
         self._items_file_references[item.id] = file_reference
 
-    async def _refetch_message_file_reference(
-        self, old_message: MessageDownloadable
-    ) -> InputLocation:
-
+    async def _refetch_message_file_reference(self, old_message: MessageDownloadable):
         item = self.get_filesource_item(old_message)
 
         refetched_msg: MessageProto
 
         [refetched_msg] = await self._client.get_messages(
             old_message.chat_id, ids=[old_message.id]
         )
@@ -131,15 +126,14 @@
         input_location: InputDocumentFileLocation | InputPhotoFileLocation,
         offset: int,
         limit: int,
         document_size: int,
         *,
         request_size=BLOCK_SIZE,
     ) -> bytes:
-
         # XXX adjust request_size
         ranges = split_range(offset, limit, request_size)
         result = bytes()
 
         # if random() > 0.9:
         #     raise FileReferenceExpiredError(None)
```

### Comparing `tgmount-1.0.4/tgmount/tgclient/guards.py` & `tgmount-1.0.5/tgmount/tgclient/guards.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/message_reaction_event.py` & `tgmount-1.0.5/tgmount/tgclient/message_reaction_event.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/message_source.py` & `tgmount-1.0.5/tgmount/tgclient/message_source.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,16 +38,21 @@
 
         self._messages: MessagesCollection[M] | None = (
             MessagesCollection.from_iterable(messages) if messages is not None else None
         )
 
         self._filters: list[MessageSourceFilter[M]] = []
 
+        """ Notifies with a list of new messages """
         self.event_new_messages: Subscribable = Subscribable()
+
+        """ Notifies with a list of removed messages  """
         self.event_removed_messages: Subscribable = Subscribable()
+
+        """ Notifies with two lists: old_messages and edited_messages """
         self.event_edited_messages: Subscribable = Subscribable()
 
     @property
     def tag(self):
         return self._tag
 
     @property
@@ -65,35 +70,33 @@
                 res = await f.filter(res)
             elif isinstance(f, Callable):
                 res = list(filter(f, res))
 
         return res
 
     async def edit_messages(self, messages: Iterable[M]):
-
         if self._messages is None:
             self._logger.error(f"edit_messages(). Messages are not initiated yet")
             return
 
-        filtered = await self._filter_messages(messages)
+        edited_messages = await self._filter_messages(messages)
 
-        old_messages = self._messages.get_by_ids([m.id for m in filtered])
+        old_messages = self._messages.get_by_ids([m.id for m in edited_messages])
 
         if old_messages is None:
             self._logger.error(
                 f"edit_messages({messages}) Some of the edited messages has not been found in the message source"
             )
             return
 
-        self._messages.add_messages(filtered, overwright=True)
+        self._messages.add_messages(edited_messages, overwright=True)
 
-        await self.event_edited_messages.notify(old_messages, filtered)
+        await self.event_edited_messages.notify(old_messages, edited_messages)
 
     async def add_messages(self, messages: Iterable[M]):
-
         if self._messages is None:
             self._messages = MessagesCollection()
 
         _filtered = await self._filter_messages(messages)
 
         self._logger.debug(f"add_messages({message_ids(_filtered)})")
 
@@ -159,15 +162,14 @@
             self._logger.debug(
                 f"set_messages({len(messages)} messages, notify={notify})"
             )
 
         filtered = await self._filter_messages(messages)
 
         if self._messages is None:
-
             self._messages = MessagesCollection.from_iterable(filtered)
 
             if not notify:
                 return
 
             await self.event_new_messages.notify(filtered)
             return
```

### Comparing `tgmount-1.0.4/tgmount/tgclient/message_source_types.py` & `tgmount-1.0.5/tgmount/tgclient/message_source_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/message_types.py` & `tgmount-1.0.5/tgmount/tgclient/message_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/messages_collection.py` & `tgmount-1.0.5/tgmount/tgclient/messages_collection.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/search/search.py` & `tgmount-1.0.5/tgmount/tgclient/search/search.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/source/document.py` & `tgmount-1.0.5/tgmount/tgclient/source/document.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/source/photo.py` & `tgmount-1.0.5/tgmount/tgclient/source/photo.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgclient/source/util.py` & `tgmount-1.0.5/tgmount/tgclient/source/util.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tglog.py` & `tgmount-1.0.5/tgmount/tglog.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 import tgmount
 
 # from tgmount.tgmount.root_config_reader import TgmountConfigReader
 from tgmount.util import yes
 
 
 def init_logging(debug_level: int = 0, debug_fs_ops=False):
-
     logging.getLogger("asyncio").setLevel(logging.CRITICAL)
     logging.getLogger("telethon").setLevel(logging.ERROR)
 
     tgmount.tgmount.module_logger.setLevel(debug_level)
     tgmount.cli.logger.setLevel(debug_level)
 
     tgmount.tgmount.filters.logger.setLevel(logging.INFO)
-    # tgmount.tgmount.root_config_reader.TgmountConfigReader.logger.setLevel(logging.INFO)
+    tgmount.config.logger.setLevel(logging.INFO)
 
     tgmount.tgmount.producers.producer_plain.VfsTreeProducerPlainDir.logger.setLevel(
         logging.INFO
     )
 
     tgmount.tgmount.producers.grouperbase.VfsTreeProducerGrouperBase.logger.setLevel(
         logging.INFO
@@ -81,15 +80,14 @@
     ) -> "TgmountLogger":
         """`suffix_as_tag` suffix will be used a a tag"""
         child = super().getChild(suffix.replace(".", "[dot]"))
         child.suffix_as_tag = suffix_as_tag
         return child
 
     def makeRecord(self, *args, **kwargs) -> logging.LogRecord:
-
         rec = super().makeRecord(*args, **kwargs)
 
         if self.suffix_as_tag and yes(self.parent):
             rec.name = self.parent.name
             rec.__dict__["tag"] = get_name_part(self.name, -1)
         else:
             rec.__dict__["tag"] = None
@@ -158,14 +156,13 @@
 
         if self.print_task_name:
             log_str = f"{rec.task_name} {log_str}"
 
         return log_str
 
     def format(self, rec: TgmountLogRecord) -> str:
-
         if rec.levelno not in self.COLORS:
             return self._format(rec)
 
         color = self.COLORS[rec.levelno]
 
         return color + self._format(rec) + self.reset
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/cached_filefactory_factory.py` & `tgmount-1.0.5/tgmount/tgmount/cached_filefactory_factory.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/file_factory/classifier.py` & `tgmount-1.0.5/tgmount/tgmount/file_factory/classifier.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/file_factory/classifierbase.py` & `tgmount-1.0.5/tgmount/tgmount/file_factory/classifierbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ...
 
 
 TG = TypeVar("TG", bound=guards.ClassWithGuard)
 
 
 class ClassifierBase(ClassifierProto[Any, TG]):
-    """Takes a message and return a list of classes this message suits"""
+    """Takes a message and returns a list of classes this message suits"""
 
     classes: list[Type[TG]]
 
     @classmethod
     @property
     def classes_dict(cls) -> Mapping[str, Type[TG]]:
         return {k.__name__: k for k in cls.classes}
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/file_factory/filefactorybase.py` & `tgmount-1.0.5/tgmount/tgmount/file_factory/filefactorybase.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/file_factory/types.py` & `tgmount-1.0.5/tgmount/tgmount/file_factory/types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/filters.py` & `tgmount-1.0.5/tgmount/tgmount/filters.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/filters_types.py` & `tgmount-1.0.5/tgmount/tgmount/filters_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/grouperbase.py` & `tgmount-1.0.5/tgmount/tgmount/producers/grouperbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 M = TypeVar("M", bound=MessageProto)
 GroupedMessages = tuple[Mapping[str, list[M]], list[M]]
 
 
 class VfsTreeProducerGrouperBase(abc.ABC):
     """
-    Base class for a producer that splits messages into groups creating a directory for each group. The structure of directores is
+    Base class for a producer that splits messages into groups creating a directory for each group. The structure of directories is
     defined by `dir_structure`.
     """
 
     logger = _logger.getChild("VfsTreeProducerGrouperBase")
 
     DEFAULT_ROOT_CONFIG: Mapping = {"filter": "All"}
     VfsTreeProducer = VfsTreeProducer
@@ -71,15 +71,14 @@
         return {self.sanitize(k): v for k, v in group.items()}, root
 
     @property
     def _current_dirs(self) -> frozenset[str]:
         return frozenset(self._source_by_name.keys())
 
     async def _add_dir(self, dir_name: str, dir_messages: list[MessageProto]):
-
         dir_source = self.MessageSource(
             messages=dir_messages, tag=f"{os.path.join(self._dir.path, dir_name)}"
         )
 
         tree_dir = await self._dir.create_dir(dir_name)
 
         self._source_by_name[dir_name] = dir_source
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_by_forward.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_by_forward.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 async def group_by_forward(
     forwarded_messages: Iterable[MessageForwarded],
 ) -> Mapping[str, list[MessageForwarded]]:
     fws = {}
 
     for m in forwarded_messages:
-
         # XXX
         if m.forward is None:
             continue
 
         chat = await m.forward.get_chat()
         # sender = await m.forward.get_sender()
         from_name = m.forward.from_name
@@ -59,15 +58,14 @@
     VfsTreeProducerGrouperBase,
     VfsTreeProducerProto,
 ):
     @classmethod
     async def from_config(
         cls, resources, config: VfsTreeProducerConfig, arg: Mapping, sub_dir
     ):
-
         return VfsTreeGroupByForward(
             config=config,
             dir_structure=arg.get(
                 "dir_structure",
                 VfsTreeGroupByForward.DEFAULT_ROOT_CONFIG,
             ),
             resources=resources,
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_by_performer.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_by_performer.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_by_reaction.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_by_reaction.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_by_sender.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_by_sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,39 +16,39 @@
 
 
 async def get_message_sender_display_name(
     m: MessageProto,
     include_username=False,
 ):
     sender = await m.get_sender()
+
     key = None
 
     if sender is None:
         return None
 
-    if sender.username is not None:
+    if hasattr(sender, "username") and sender.username is not None:
         key = sender.username
 
     if key is None:
         key: str | None = telethon.utils.get_display_name(sender)
     elif include_username:
         key = f"{telethon.utils.get_display_name(sender)} @{key}"
 
     if key == "":
         key = None
 
     return key
 
 
 def get_get_key(*, use_get_sender=True):
-    """Retuns a async function that gets from a message a key for grouping"""
+    """Retuns a async function that gets a key for grouping from a message"""
 
     @measure_time(logger_func=_logger.getChild("VfsTreeDirBySender").info, threshold=3)
     async def get_key(m: MessageProto) -> str | None:
-
         if m.from_id is None:
             return
 
         sender_id = telethon.utils.get_peer_id(m.from_id)
 
         if use_get_sender:
             sender = await m.get_sender()
@@ -61,15 +61,14 @@
 
     return get_key
 
 
 async def group_by_sender(
     messages: Iterable[MessageProto], minimum=1, use_get_sender=False
 ) -> tuple[Mapping[str, list[MessageProto]], list[MessageProto], list[MessageProto],]:
-
     return await func.group_by_func_async(
         get_get_key(use_get_sender=use_get_sender),
         messages,
         minimum=minimum,
     )
 
 
@@ -80,28 +79,26 @@
         super().__init__(tree_dir, config, resources, dir_structure=dir_structure)
         self.use_get_sender = use_get_sender
 
     @classmethod
     async def from_config(
         cls, resources, config: VfsTreeProducerConfig, arg: Mapping, sub_dir
     ):
-
         return VfsTreeDirBySender(
             resources=resources,
             tree_dir=sub_dir,
             config=config,
             dir_structure=arg.get(
                 "dir_structure",
                 VfsTreeDirBySender.DEFAULT_ROOT_CONFIG,
             ),
             use_get_sender=arg.get("use_get_sender", True),
         )
 
     async def group_messages(self, messages: Iterable[MessageProto]) -> GroupedMessages:
-
         by_user, less, nones = await group_by_sender(
             messages, minimum=1, use_get_sender=self.use_get_sender
         )
 
         res = {}
 
         for sname, sender_messages in by_user.items():
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_plain.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_plain.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,29 +37,27 @@
     async def from_config(
         cls,
         resources,
         vfs_config: VfsTreeProducerConfig,
         arg: Mapping,
         tree_dir: VfsTreeDir,
     ):
-
         return VfsTreeProducerPlainDir(tree_dir, vfs_config)
 
     async def add_items_to_vfs_tree(self, items: Sequence[vfs.DirContentItem]):
         await self._tree_dir.put_content(
             items,
         )
 
     async def remove_items_from_vfs_dir(self, items: Sequence[vfs.DirContentItem]):
         for f in items:
             await self._tree_dir.remove_content(f)
 
     # @measure_time(logger_func=print)
     async def produce(self):
-
         _messages = MessagesCollection.from_iterable(await self._config.get_messages())
 
         self._logger.debug(f"Producing from {len(_messages)} messages...")
 
         self._message_to_file = {
             m.id: await self._config.produce_file(m) for m in _messages
         }
@@ -158,15 +156,14 @@
         old_files: Mapping[str, tuple[MessageProto, vfs.FileLike]],
         new_files: Mapping[str, tuple[MessageProto, vfs.FileLike]],
         update_content_dict: Mapping[str, vfs.FileLike],
     ):
         await self._tree_dir.update_content(update_content_dict)
 
     async def update_new_messages(self, source, new_messages: list[MessageProto]):
-
         self._logger.debug(
             f"update_new_messages({list(map(lambda m: m.id, new_messages))})"
         )
 
         if len(new_messages) == 0:
             return
 
@@ -179,15 +176,15 @@
         self._message_to_file.update(
             {
                 **{m.id: f for m, f in zip(new_messages_set, new_files)},
             }
         )
 
         if len(new_files):
-            await self._tree_dir.put_content(new_files)
+            await self.add_items_to_vfs_tree(new_files)
             # await self._tree_dir.put_content(new_files)
 
     async def update_removed_messages(
         self, source, removed_messages: list[MessageProto]
     ):
         self._logger.debug(
             f"update_removed_messages({list(map(lambda m: m.id, removed_messages))})"
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_sysinfo.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_sysinfo.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/producers/producer_zip.py` & `tgmount-1.0.5/tgmount/tgmount/producers/producer_zip.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
     async def update_items_in_vfs_tree(
         self,
         old_files: Mapping[str, tuple[MessageProto, vfs.FileLike]],
         new_files: Mapping[str, tuple[MessageProto, vfs.FileLike]],
         update_content_dict: Mapping[str, vfs.FileLike],
     ):
+        self._logger.debug(f"update_items_in_vfs_tree()")
+
         result = {}
 
         for old_file_name, new_file in update_content_dict.items():
             (old_msg, old_file) = old_files[old_file_name]
             (new_msg, new_file) = new_files[new_file.name]
 
             is_old_zip = await self._is_zip_file(old_file)
@@ -98,15 +100,14 @@
             else:
                 result.append(item)
 
         return await super().add_items_to_vfs_tree(result)
 
     async def _add_zip_file(self, zip_file: vfs.FileLike):
         try:
-
             zip_tree = await self._dir_content_zip_factory.get_ziptree(zip_file.content)
         except BadZipFile:
             self._logger.warning(f"{zip_file} is a bad zip file")
             return
 
         zip_tree_root_items_names = list(
             set(zip_tree.keys()).difference(
@@ -174,11 +175,10 @@
     async def from_config(
         cls,
         resources,
         vfs_config: VfsTreeProducerConfig,
         config: Mapping,
         tree_dir: VfsTreeDir,
     ):
-
         return VfsProducerZip(
             tree_dir, vfs_config, props=WrapperZipsAsDirsProps.from_config(config)
         )
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/providers/provider_caches.py` & `tgmount-1.0.5/tgmount/tgmount/providers/provider_caches.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/providers/provider_filters.py` & `tgmount-1.0.5/tgmount/tgmount/providers/provider_filters.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/providers/provider_sources.py` & `tgmount-1.0.5/tgmount/tgmount/providers/provider_sources.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/providers/provider_wrappers.py` & `tgmount-1.0.5/tgmount/tgmount/providers/provider_wrappers.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/root_config_reader.py` & `tgmount-1.0.5/tgmount/tgmount/root_config_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,27 +14,14 @@
 from .vfs_tree_producer_types import VfsTreeProducerConfig, VfsDirConfig
 from dataclasses import dataclass
 from .logger import module_logger as _logger
 
 T = TypeVar("T")
 
 
-# @dataclass
-# class DirProps:
-#     path: list[str]
-#     source_prop: RootConfigReaderProps.PropSourceType | None
-#     filters_prop: RootConfigReaderProps.PropFilterType | None
-#     cache_prop: Mapping | str | None
-#     wrappers_prop: Sequence[tuple[str, Mapping | None]] | None
-#     producer_prop: tuple[str, Mapping] | None
-#     treat_as_prop: list[str] | None
-#     other_keys: set[str]
-#     raw_config: Mapping
-
-
 class TgmountConfigReader:
     logger = _logger.getChild("TgmountConfigReader")
 
     logger.setLevel(logging.ERROR)
 
     DEFAULT_PRODUCER_NAME = "PlainDir"
 
@@ -56,37 +43,14 @@
         current_path_str = vfs.path_join(*current_path)
         other_keys = set(dir_config.other_keys.keys())
 
         yield dir_config
 
         for k, v in dir_config.other_keys.items():
             yield from self.walk_dir_props(v)
-        # other_keys = set(d.keys()).difference(self.DIR_PROPS_KEYS)
-
-        # source_prop = self.read_prop_source(d)
-        # filters_prop = self.read_prop_filter(d)
-        # cache_prop = self.read_prop_cache(d)
-        # wrappers_prop = self.read_prop_wrappers(d)
-        # producer_prop = self.read_prop_producer(d)
-        # treat_as_prop = self.read_prop_treat_as(d)
-
-        # yield DirProps(
-        #     current_path,
-        #     source_prop,
-        #     filters_prop,
-        #     cache_prop,
-        #     wrappers_prop,
-        #     producer_prop,
-        #     treat_as_prop,
-        #     other_keys,
-        #     raw_config=d,
-        # )
-
-        # for k in other_keys:
-        #     yield from (self.walk_dir_props(d[k], current_path=[*current_path, k]))
 
     async def walk_config_with_ctx(
         self,
         dir_config: config.DirConfig,
         *,
         resources: TgmountResources,
         ctx: RootConfigWalkingContext,
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/root_config_reader_props.py` & `tgmount-1.0.5/tgmount/tgmount/root_config_reader_props.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/root_config_types.py` & `tgmount-1.0.5/tgmount/tgmount/root_config_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/tgmount_builder.py` & `tgmount-1.0.5/tgmount/tgmount/tgmount_builder.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/tgmount_builderbase.py` & `tgmount-1.0.5/tgmount/tgmount/tgmount_builderbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,18 +49,21 @@
     classifier: classifier.ClassifierBase
     caches: CachesTypesProviderProto
     filters: FilterProviderProto
     wrappers: ProviderVfsWrappersBase
     producers: ProducersProviderBase
 
     async def create_client(self, cfg: config.Config, **kwargs):
+        self.logger.debug("create_client")
+
         return self.TelegramClient(
             cfg.client.session,
             cfg.client.api_id,
             cfg.client.api_hash,
+            use_ipv6=cfg.client.use_ipv6,
             **kwargs,
         )
 
     async def create_vfs_tree(self):
         return self.VfsTree()
 
     async def create_file_source(self, cfg: config.Config, client):
@@ -98,15 +101,14 @@
         client,
         msc: config.MessageSource,
         message_source,
     ):
         return self.TelegramMessagesFetcher(client, msc)
 
     async def create_tgmount_resources(self, client, cfg: config.Config, **kwargs):
-
         sources_used_in_root = await TgmountConfigReader().get_used_sources(cfg.root)
 
         files_source = await self.create_file_source(cfg, client)
         file_factory = await self.create_file_factory(cfg, client, files_source)
 
         source_provider = SourcesProvider()
 
@@ -174,15 +176,14 @@
         )
 
         tgm.producer = self.VfsTreeProducer(resources=self.resources)
         tgm.vfs_tree = await self.create_vfs_tree()
         tgm.events_dispatcher = self.TelegramEventsDispatcher()
 
         for k, msc in cfg.message_sources.sources.items():
-
             ms = self.resources.message_sources.get(k)
 
             if ms is None:
                 continue
 
             updates = none_fallback(msc.updates, True)
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/tgmount_providers.py` & `tgmount-1.0.5/tgmount/tgmount/tgmount_providers.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/tgmount_types.py` & `tgmount-1.0.5/tgmount/tgmount/tgmount_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/tgmountbase.py` & `tgmount-1.0.5/tgmount/tgmount/tgmountbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 
         self.logger.info(
             f"Fetching initial messages from ({list(self._resources.fetchers_dict.keys())})..."
         )
 
         for k, fetcher in self._resources.fetchers_dict.items():
             self.logger.info(f"Fetching from '{k}'...")
+
             source = self._resources.message_sources.get(k)
 
             assert source
 
             initial_messages = await fetcher.fetch()
 
             self.logger.info(f"Fetched {len(initial_messages)} messages.")
@@ -135,15 +136,14 @@
     async def on_new_message(self, entity_id: EntityId, event: events.NewMessage.Event):
         self.logger.info(
             f"on_new_message({entity_id}, {MessageProto.repr_short(event.message)})"
         )
         self.logger.trace(f"on_new_message({event})")
         listener = TreeListener(self._vfs_tree)
         async with self._update_lock:
-
             async with listener:
                 await self.events_dispatcher.process_new_message_event(entity_id, event)
 
             if len(listener.events) > 0:
                 self.logger.debug(f"Tree generated {len(listener.events)} events")
                 await self._on_vfs_tree_update(listener.events)
 
@@ -198,15 +198,14 @@
 
             if len(listener.events) > 0:
                 self.logger.debug(f"Tree generated {len(listener.events)} events")
                 await self._on_vfs_tree_update(listener.events)
 
     # @measure_time(logger_func=logger.info)
     async def _update_fs(self, fs_update: FileSystemOperationsUpdate):
-
         if self._fs is None:
             self.logger.error(f"self._fs is not created yet.")
             return
 
         async with self._fs._update_lock:
             await self._fs.update(fs_update)
 
@@ -227,15 +226,14 @@
         root_contet = await self._vfs_tree.get_dir_content()
 
         root = vfs.root(root_contet)
 
         self._fs = self.FileSystemOperations(root)
 
     async def _on_vfs_tree_update(self, updates: list[TreeEventType]):
-
         if len(updates) == 0:
             return
 
         await self._dispatch_to_filesystem(updates)
 
         # self.logger.debug(
         #     f"UPDATE: new_files={list(fs_update.new_files.keys())}"
@@ -244,15 +242,14 @@
         #     + f" removed_dirs={fs_update.removed_dirs}"
         #     + f" update_items={fs_update.update_items}"
         # )
 
         # await self._update_fs(fs_update)
 
     async def _dispatch_to_filesystem(self, events: list[TreeEventType[VfsTreeDir]]):
-
         for e in events:
             update = fs.FileSystemOperationsUpdate()
 
             if isinstance(e, TreeEventRemovedItems):
                 path = e.sender.path
 
                 for item in e.removed_items:
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/validator/validatorbase.py` & `tgmount-1.0.5/tgmount/tgmount/validator/validatorbase.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 
     logger = logger.getChild(f"ConfigValidatorBase")
 
     def __init__(self, builder: TgmountBuilderBase) -> None:
         self._builder = builder
 
     async def verify_config(self, cfg: config.Config):
-        client = await self._builder.create_client(cfg)
-        resources = await self._builder.create_tgmount_resources(client, cfg)
-        await self.verify_client(cfg)
-        await self.verify_message_sources(cfg)
-        await self.verify_caches(cfg)
-        await self.verify_root(resources, cfg)
+        return
+        # client = await self._builder.create_client(cfg)
+        # resources = await self._builder.create_tgmount_resources(client, cfg)
+
+        # await self.verify_client(cfg)
+        # await self.verify_message_sources(cfg)
+        # await self.verify_caches(cfg)
+        # await self.verify_root(resources, cfg)
 
     async def verify_client(self, cfg: config.Config):
         pass
 
     async def verify_message_sources(self, cfg: config.Config):
         for src_id, src in cfg.message_sources.sources.items():
             if not yes(src.filter):
                 continue
 
             pass
 
     async def verify_caches(self, cfg: config.Config):
-
         if not yes(cfg.caches):
             return
 
         for cache_id, cache in cfg.caches.caches.items():
             pass
 
     async def verify_root(self, resources: TgmountResources, cfg: config.Config):
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/vfs_tree.py` & `tgmount-1.0.5/tgmount/tgmount/vfs_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,14 @@
 
         for w in self._wrappers:
             events = await w.wrap_events(events)
 
         await parent.child_updated(events)
 
     async def get_parent(self):
-
         if self.path == "/":
             return self._parent_tree
 
         return await self._parent_tree.get_parent(self._path)
 
     def __repr__(self) -> str:
         return f"VfsTreeDir(path={self._path})"
@@ -210,15 +209,14 @@
     async def put_content(
         self,
         content: Sequence[vfs.DirContentItem] | vfs.DirContentItem,
         subpath: str = "/",
         *,
         replace=False,
     ):
-
         if not isinstance(content, Sequence):
             content = [content]
 
         await self._parent_tree.put_content(
             content, self._globalpath(subpath), replace=replace
         )
 
@@ -295,15 +293,15 @@
 
 
 class VfsTree(Subscribable, VfsTreeProto):
     """
     The structure that holds the whole generated FS tree.
     Producers use it to read and write the structures they are responsible for.
 
-    Storing dirs in a single mappig we try to avoid recursivness.
+    Storing dirs in a single mapping we try to avoid recursiveness.
 
     Provides interface for accessing dirs and their contents by their global paths.
     """
 
     logger = _logger.getChild(f"VfsTree")
 
     VfsTreeDir = VfsTreeDir
@@ -501,15 +499,15 @@
         for s in subdirs:
             res.append(self._dir_by_path[s])
 
         return res
 
     async def get_dir_content(self, path: str = "/") -> VfsTreeDirContent:
         """Returns `VfsTreeDirContent`"""
-        return VfsTreeDirContent(self, path)
+        return self.VfsTreeDirContent(self, path)
 
     async def _get_dir_content(self, path: str) -> vfs.DirContentProto:
         """Method used by `VfsTreeDirContent` to construct `vfs.DirContentProto`"""
         d = await self.get_dir(path)
 
         vfs_items, subdirs = (
             await d.get_dir_content_items(),
```

### Comparing `tgmount-1.0.4/tgmount/tgmount/vfs_tree_producer.py` & `tgmount-1.0.5/tgmount/tgmount/vfs_tree_producer.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/vfs_tree_producer_types.py` & `tgmount-1.0.5/tgmount/tgmount/vfs_tree_producer_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/vfs_tree_types.py` & `tgmount-1.0.5/tgmount/tgmount/vfs_tree_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/vfs_tree_wrapper_types.py` & `tgmount-1.0.5/tgmount/tgmount/vfs_tree_wrapper_types.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/wrappers/wrapper_exclude_empty_dirs.py` & `tgmount-1.0.5/tgmount/tgmount/wrappers/wrapper_exclude_empty_dirs.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/tgmount/wrappers/wrapper_zips_as_dirs.py` & `tgmount-1.0.5/tgmount/tgmount/wrappers/wrapper_zips_as_dirs.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/__init__.py` & `tgmount-1.0.5/tgmount/util/__init__.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/asyn.py` & `tgmount-1.0.5/tgmount/util/asyn.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/col.py` & `tgmount-1.0.5/tgmount/util/col.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/func.py` & `tgmount-1.0.5/tgmount/util/func.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/guards.py` & `tgmount-1.0.5/tgmount/util/guards.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/tg.py` & `tgmount-1.0.5/tgmount/util/tg.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util/timer.py` & `tgmount-1.0.5/tgmount/util/timer.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/util.py` & `tgmount-1.0.5/tgmount/util.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/__init__.py` & `tgmount-1.0.5/tgmount/vfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     DirContent,
     DirContentItem,
     DirContentList,
     DirContentProto,
     DirLike,
     dir_content,
     vdir,
-    DirContentProtoWritable,
+    DirContentWritableProto,
     DirContentListWritable,
 )
 from .dir_util import (
     dir_content_from_fs,
     dir_content_to_tree,
     file_like_tree_map,
     dir_content_filter_items,
```

### Comparing `tgmount-1.0.4/tgmount/vfs/dir.py` & `tgmount-1.0.5/tgmount/vfs/dir.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .types.dir import (
     DirContent,
     DirContentItem,
     DirContentList,
     DirContentProto,
     DirLike,
-    DirContentProtoWritable,
+    DirContentWritableProto,
     DirContentListWritable,
 )
 
 
 def dir_content(*items: DirContentItem) -> DirContent[None]:
     """Takes items as arguments and returns `DirContent`"""
```

### Comparing `tgmount-1.0.4/tgmount/vfs/dir_util.py` & `tgmount-1.0.5/tgmount/vfs/dir_util.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/file.py` & `tgmount-1.0.5/tgmount/vfs/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,20 @@
 
 
 def vfile(
     fname: str,
     content: FileContentProto,
     creation_time: Optional[datetime] = None,
     extra: Optional[Any] = None,
+    writable=False,
 ):
     if creation_time is None:
         creation_time = datetime.now()
 
-    return FileLike(fname, content, creation_time, extra)
+    return FileLike(fname, content, creation_time, extra, writable)
 
 
 def file_content(
     size: int,
     read_func: Callable[[Any, int, int], Awaitable[bytes]],
 ):
     return FileContent(size=size, read_func=read_func)
```

### Comparing `tgmount-1.0.4/tgmount/vfs/io.py` & `tgmount-1.0.5/tgmount/vfs/io.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/lookup.py` & `tgmount-1.0.5/tgmount/vfs/lookup.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/map_tree.py` & `tgmount-1.0.5/tgmount/vfs/map_tree.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/root.py` & `tgmount-1.0.5/tgmount/vfs/root.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/tree.py` & `tgmount-1.0.5/tgmount/vfs/tree.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/vfs/types/dir.py` & `tgmount-1.0.5/tgmount/vfs/types/dir.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Protocol,
     Sequence,
     TypeGuard,
     TypeVar,
     Union,
 )
 
-from tgmount.vfs.types.file import FileLike, FileContentProtoWritable
+from tgmount.vfs.types.file import FileLike, FileContentWritableProto
 
 T = TypeVar("T")
 
 DirContentItem = Union["DirLike", FileLike]
 
 
 OpenDirFunc = Callable[[], Awaitable[Any]]
@@ -45,21 +45,21 @@
         pass
 
     @staticmethod
     def guard(item: Any) -> TypeGuard["DirContentProto[Any]"]:
         return hasattr(item, "readdir_func")
 
 
-class DirContentProtoWritable(DirContentProto[T], Protocol[T]):
+class DirContentWritableProto(DirContentProto[T], Protocol[T]):
     @abstractmethod
     async def create(self, filename: str) -> FileLike:
         pass
 
     @staticmethod
-    def guard(dc: DirContentProto) -> TypeGuard["DirContentProtoWritable"]:
+    def guard(dc: DirContentProto) -> TypeGuard["DirContentWritableProto"]:
         return hasattr(dc, "create")
 
 
 @dataclass
 class DirLike:
     """Represents a folder with a name and content"""
 
@@ -116,15 +116,15 @@
 
     async def readdir_func(
         self, handle: list[DirContentItem], off: int
     ) -> Iterable[DirContentItem]:
         return handle[off:]
 
 
-class DirContentListWritable(DirContentList, DirContentProtoWritable):
+class DirContentListWritable(DirContentList, DirContentWritableProto):
     @abstractmethod
     async def create_filelike(self, filename: str) -> FileLike:
         pass
 
     async def create(self, filename: str) -> FileLike:
         fl = await self.create_filelike(filename)
         self.content_list.append(fl)
```

### Comparing `tgmount-1.0.4/tgmount/vfs/types/file.py` & `tgmount-1.0.5/tgmount/vfs/types/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,47 +137,53 @@
 
     # XXX
 
     def __repr__(self):
         return f"FileContent(size={self.size})"
 
 
-class FileContentProtoWritable(FileContentProto[T], Protocol):
+class FileContentWritableProto(FileContentProto[T], Protocol):
     @abstractmethod
     async def write(self, handle: T, off: int, buf: bytes):
         pass
 
     @staticmethod
-    def guard(fc: FileContentProto) -> TypeGuard["FileContentProtoWritable"]:
+    def guard(fc: FileContentProto) -> TypeGuard["FileContentWritableProto"]:
         return hasattr(fc, "write")
 
 
-class FileContentStringWritable(FileContentProtoWritable):
+class FileContentStringWritable(FileContentWritableProto):
     size: int
     encoding = "utf-8"
 
     def __init__(self, content_string="") -> None:
         self._content_bytes = content_string.encode(self.encoding)
+        self.size = len(self._content_bytes)
 
     async def seek_func(self, handle, n: int, w: int):
         raise NotImplementedError()
 
-    tell_func: Optional[Callable[[Any], Awaitable[int]]] = None
-
     async def open_func(self) -> None:
         return
 
     async def close_func(self, handle):
         return
 
     async def read_func(self, handle, off: int, size: int) -> bytes:
         return self._content_bytes[off : off + size]
 
     async def write(self, handle: None, off: int, buf: bytes):
         content_bytes = bytearray(self._content_bytes)
+        content_bytes_len = len(content_bytes)
 
         for idx, b in enumerate(buf):
-            content_bytes[off + idx] = b
+            if off + idx >= content_bytes_len:
+                content_bytes.append(b)
+            else:
+                content_bytes[off + idx] = b
 
         self._content_bytes = bytes(content_bytes)
+        self.size = len(self._content_bytes)
 
         return len(buf)
+
+    tell_func: Optional[Callable[[Any], Awaitable[int]]] = None
```

### Comparing `tgmount-1.0.4/tgmount/vfs/util.py` & `tgmount-1.0.5/tgmount/vfs/util.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/util.py` & `tgmount-1.0.5/tgmount/zip/util.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/zip_dir.py` & `tgmount-1.0.5/tgmount/zip/zip_dir.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/zip_dir_factory.py` & `tgmount-1.0.5/tgmount/zip/zip_dir_factory.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/zip_file.py` & `tgmount-1.0.5/tgmount/zip/zip_file.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/zip_file_id3v1_fix.py` & `tgmount-1.0.5/tgmount/zip/zip_file_id3v1_fix.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount/zip/zips_as_dirs.py` & `tgmount-1.0.5/tgmount/zip/zips_as_dirs.py`

 * *Files identical despite different names*

### Comparing `tgmount-1.0.4/tgmount.egg-info/PKG-INFO` & `tgmount-1.0.5/tgmount.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgmount
-Version: 1.0.4
+Version: 1.0.5
 Summary: Mount telegram messages as files
 Home-page: https://github.com/nktknshn/tgmount-ng
 Author: Nikita Kanashin
 Author-email: nikita@kanash.in
 Description-Content-Type: text/markdown
 
 # Overview
@@ -280,26 +280,26 @@
 
 Exclude repeating documents 
 
 `--include-unsupported`
 
 Include messages that are not supported for mounting
 
-`--only-unique-docs`
+`--only-unsupported`
 
 Print only them
 
 `--json`
 
 Print in json format
 
 ### tgmount download
 
 ```
-tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request_size REQUEST_SIZE] entity ids [ids ...]
+tgmount download [--output-dir OUTPUT_DIR] [--keep-filename] [--request-size REQUEST_SIZE] entity ids [ids ...]
 ```
 
 `--keep-filename`
 
 Keep original filenames
 
 `--output-dir`
@@ -357,14 +357,17 @@
 
   # telegram api credentials
   api_id: int
   api_hash: str
 
   # optional field
   request_size: 128KB
+
+  # optional field. Default: False
+  use_ipv6: True
 ```
 
 ### message_sources
 A message source defines a list of messages that will be used in vfs tree construction. Every message source is a separate [TelegramClient.get_messages](https://docs.telethon.dev/en/stable/modules/client.html#telethon.client.messages.MessageMethods.get_messages) request. Message source is also subscribed to events of posting, removing and editing messages in the entity it is sourced from. 
 
 ```yaml
 message_sources:
@@ -432,26 +435,27 @@
   # optional. sets a filter for the current folder. Default is no filter
   filter: MessageWithMusic
   filter: {filter: MessageWithMusic}
 
   # sets a filter for the current folder and subfolders
   filter: {filter: MessageWithMusic, recursive: True}
 
-  # sets a filter for the current folder and subfolders overwriting another recursive filter if any 
+  # sets a filter for the current folder and subfolders overwriting another 
+  # recursive filter if any 
   filter: {filter: MessageWithMusic, overwright: True, recursive: True}
 
   # the following combines multiple filters. Only messages that match every filter
   # in the list will pass. The filter below allows all documents that
   # that are not video, photo or audio and not a zip file 
   filter: 
     - MessageWithOtherDocument
     - Not:
       - ByExtension: .zip
 
-  # on line
+  # in one line
   filter: {filter: [MessageWithOtherDocument, Not: {ByExtension: .zip}], overwright: True, recursive: True}
 
   # defines a producer that controls the content of the folder. 
   # Default is PlainDir
   producer: BySender
 
   # producer may have properties
@@ -492,15 +496,15 @@
 ```
 
 
 #### source
 
 Message source is a list of messages which is used to produce a directory content. Message source is initialized from get_messages() request and is updated by events of posting message, removing message and editing message in the corresponding entity. 
 
-Producer is subscribed to a message source and takes a care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
+Producer is subscribed to a message source and takes care of the directory it is responsible for. It manages it by adding and removing files and subfolders.
 
 The content of a folder is defined by a combination of properties `source`, `filter`, `producer` and `treat_as`. 
 
 This will create a tree of empty folders
 ```yaml
 root:
   everything:
```

### Comparing `tgmount-1.0.4/tgmount.egg-info/SOURCES.txt` & `tgmount-1.0.5/tgmount.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 README.md
 setup.py
 tgmount/__init__.py
 tgmount/client.py
+tgmount/constants.py
 tgmount/error.py
-tgmount/settings.py
 tgmount/tglog.py
 tgmount/util.py
 tgmount.egg-info/PKG-INFO
 tgmount.egg-info/SOURCES.txt
 tgmount.egg-info/dependency_links.txt
 tgmount.egg-info/entry_points.txt
 tgmount.egg-info/requires.txt
@@ -31,14 +31,15 @@
 tgmount/cli/mount_config.py
 tgmount/cli/stats.py
 tgmount/cli/upload.py
 tgmount/cli/validate.py
 tgmount/cli/util/__init__.py
 tgmount/cli/util/client.py
 tgmount/cli/util/config.py
+tgmount/cli/util/logger.py
 tgmount/cli/util/read_env.py
 tgmount/common/__init__.py
 tgmount/common/filter.py
 tgmount/config/__init__.py
 tgmount/config/config.py
 tgmount/config/config_type.py
 tgmount/config/error.py
@@ -60,27 +61,30 @@
 tgmount/main/__init__.py
 tgmount/main/util.py
 tgmount/tgclient/__init__.py
 tgmount/tgclient/auth.py
 tgmount/tgclient/client.py
 tgmount/tgclient/client_types.py
 tgmount/tgclient/events_disptacher.py
-tgmount/tgclient/fetcher.py
 tgmount/tgclient/file_source_types.py
 tgmount/tgclient/files_source.py
 tgmount/tgclient/filters.py
 tgmount/tgclient/guards.py
 tgmount/tgclient/logger.py
 tgmount/tgclient/message_reaction_event.py
 tgmount/tgclient/message_source.py
 tgmount/tgclient/message_source_types.py
 tgmount/tgclient/message_types.py
 tgmount/tgclient/messages_collection.py
 tgmount/tgclient/types.py
 tgmount/tgclient/util.py
+tgmount/tgclient/fetcher/__init__.py
+tgmount/tgclient/fetcher/fetcher.py
+tgmount/tgclient/fetcher/fetcher_cache.py
+tgmount/tgclient/fetcher/logger.py
 tgmount/tgclient/search/__init__.py
 tgmount/tgclient/search/search.py
 tgmount/tgclient/search/types.py
 tgmount/tgclient/search/util.py
 tgmount/tgclient/source/__init__.py
 tgmount/tgclient/source/document.py
 tgmount/tgclient/source/item.py
```

