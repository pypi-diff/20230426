# Comparing `tmp/transpose_data-4.0.0.tar.gz` & `tmp/transpose_data-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transpose_data-4.0.0.tar", last modified: Thu Apr  6 22:05:38 2023, max compression
+gzip compressed data, was "transpose_data-4.0.1.tar", last modified: Wed Apr 26 16:14:53 2023, max compression
```

## Comparing `transpose_data-4.0.0.tar` & `transpose_data-4.0.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.085889 transpose_data-4.0.0/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     1066 2022-05-27 16:10:33.000000 transpose_data-4.0.0/LICENSE
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        9 2022-06-01 23:37:24.000000 transpose_data-4.0.0/MANIFEST.in
--rw-r--r--   0 jonathanbecker   (501) staff       (20)    15881 2023-04-06 22:05:38.085349 transpose_data-4.0.0/PKG-INFO
--rw-r--r--   0 jonathanbecker   (501) staff       (20)    15011 2023-04-06 21:38:19.000000 transpose_data-4.0.0/README.md
--rw-r--r--   0 jonathanbecker   (501) staff       (20)       38 2023-04-06 22:05:38.086033 transpose_data-4.0.0/setup.cfg
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     1562 2023-04-06 22:04:16.000000 transpose_data-4.0.0/setup.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.039327 transpose_data-4.0.0/transpose/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      201 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-06-01 22:54:03.000000 transpose_data-4.0.0/transpose/__main__.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.040121 transpose_data-4.0.0/transpose/extras/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      220 2022-06-28 17:30:52.000000 transpose_data-4.0.0/transpose/extras/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     6916 2022-06-16 15:05:28.000000 transpose_data-4.0.0/transpose/extras/plot.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.040696 transpose_data-4.0.0/transpose/models/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      103 2022-06-28 17:30:34.000000 transpose_data-4.0.0/transpose/models/__init__.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.041702 transpose_data-4.0.0/transpose/src/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:48.000000 transpose_data-4.0.0/transpose/src/__init__.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.042691 transpose_data-4.0.0/transpose/src/api/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 17:29:51.000000 transpose_data-4.0.0/transpose/src/api/__init__.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.051250 transpose_data-4.0.0/transpose/src/api/block/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:56.000000 transpose_data-4.0.0/transpose/src/api/block/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      405 2022-06-02 15:28:23.000000 transpose_data-4.0.0/transpose/src/api/block/_accounts_by_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      599 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/block/_accounts_by_date_created.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      451 2022-10-31 15:56:44.000000 transpose_data-4.0.0/transpose/src/api/block/_blocks_by_date.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      458 2022-10-31 02:07:41.000000 transpose_data-4.0.0/transpose/src/api/block/_blocks_by_number.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      589 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/block/_contracts_by_creator.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      744 2022-05-31 20:16:32.000000 transpose_data-4.0.0/transpose/src/api/block/_logs_by_block.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      431 2022-05-31 21:53:19.000000 transpose_data-4.0.0/transpose/src/api/block/_logs_by_transaction.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      480 2023-01-04 14:43:27.000000 transpose_data-4.0.0/transpose/src/api/block/_transactions_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      483 2022-05-31 18:41:18.000000 transpose_data-4.0.0/transpose/src/api/block/_transactions_by_block.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      495 2022-05-31 18:41:08.000000 transpose_data-4.0.0/transpose/src/api/block/_transactions_by_date.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      405 2022-05-31 21:53:33.000000 transpose_data-4.0.0/transpose/src/api/block/_transactions_by_hash.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     6752 2023-01-04 14:43:27.000000 transpose_data-4.0.0/transpose/src/api/block/base.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     6114 2022-10-31 15:56:30.000000 transpose_data-4.0.0/transpose/src/api/constants.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.052245 transpose_data-4.0.0/transpose/src/api/endpoint/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 17:42:25.000000 transpose_data-4.0.0/transpose/src/api/endpoint/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     1247 2023-04-06 18:06:39.000000 transpose_data-4.0.0/transpose/src/api/endpoint/base.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.056745 transpose_data-4.0.0/transpose/src/api/ens/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:55.000000 transpose_data-4.0.0/transpose/src/api/ens/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      228 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/ens/_records_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      533 2022-05-27 21:18:51.000000 transpose_data-4.0.0/transpose/src/api/ens/_records_by_date.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      355 2022-05-31 21:50:53.000000 transpose_data-4.0.0/transpose/src/api/ens/_records_by_name.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      284 2022-05-27 20:41:28.000000 transpose_data-4.0.0/transpose/src/api/ens/_records_by_owner.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      388 2022-05-27 22:44:42.000000 transpose_data-4.0.0/transpose/src/api/ens/_records_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      583 2022-12-21 18:57:18.000000 transpose_data-4.0.0/transpose/src/api/ens/_transfers_by_name.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      591 2022-12-21 18:57:29.000000 transpose_data-4.0.0/transpose/src/api/ens/_transfers_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     3988 2022-12-21 18:57:46.000000 transpose_data-4.0.0/transpose/src/api/ens/base.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.068014 transpose_data-4.0.0/transpose/src/api/nft/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:54.000000 transpose_data-4.0.0/transpose/src/api/nft/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      436 2022-05-31 22:08:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_collections_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      718 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_collections_by_date_created.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      325 2022-07-26 20:53:53.000000 transpose_data-4.0.0/transpose/src/api/nft/_collections_by_name.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      337 2022-07-26 20:54:17.000000 transpose_data-4.0.0/transpose/src/api/nft/_collections_by_symbol.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      319 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      646 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_date_minted.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      297 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_name.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      422 2022-05-31 22:52:06.000000 transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_owner.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      632 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      325 2022-05-31 23:09:34.000000 transpose_data-4.0.0/transpose/src/api/nft/_owners_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      385 2022-05-31 23:11:35.000000 transpose_data-4.0.0/transpose/src/api/nft/_owners_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      396 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_sales.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      541 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_sales_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      520 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_sales_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      552 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_sales_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      457 2022-12-21 18:58:22.000000 transpose_data-4.0.0/transpose/src/api/nft/_transfers.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      603 2022-12-21 18:57:56.000000 transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      660 2022-12-21 18:58:03.000000 transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      683 2022-12-21 18:58:12.000000 transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_token_id.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)    10684 2022-12-21 18:58:37.000000 transpose_data-4.0.0/transpose/src/api/nft/base.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.068960 transpose_data-4.0.0/transpose/src/api/sql/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 17:19:08.000000 transpose_data-4.0.0/transpose/src/api/sql/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     1220 2023-04-06 17:36:35.000000 transpose_data-4.0.0/transpose/src/api/sql/base.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.079662 transpose_data-4.0.0/transpose/src/api/token/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:53.000000 transpose_data-4.0.0/transpose/src/api/token/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      434 2022-06-01 20:16:47.000000 transpose_data-4.0.0/transpose/src/api/token/_native_token_balances_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      526 2022-06-01 20:11:31.000000 transpose_data-4.0.0/transpose/src/api/token/_native_token_transfers.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      805 2022-06-01 20:12:47.000000 transpose_data-4.0.0/transpose/src/api/token/_native_token_transfers_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      331 2022-06-02 17:25:00.000000 transpose_data-4.0.0/transpose/src/api/token/_owners_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      423 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/token/_swaps.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      558 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/token/_swaps_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      649 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/token/_swaps_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      581 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/token/_swaps_by_pair.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      430 2022-06-01 19:06:51.000000 transpose_data-4.0.0/transpose/src/api/token/_tokens_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      712 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/api/token/_tokens_by_date_created.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      300 2022-07-26 20:55:18.000000 transpose_data-4.0.0/transpose/src/api/token/_tokens_by_name.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      434 2022-06-01 19:44:57.000000 transpose_data-4.0.0/transpose/src/api/token/_tokens_by_owner.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      312 2022-07-26 20:55:27.000000 transpose_data-4.0.0/transpose/src/api/token/_tokens_by_symbol.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      461 2022-12-21 18:58:59.000000 transpose_data-4.0.0/transpose/src/api/token/_transfers.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      607 2022-12-21 18:58:45.000000 transpose_data-4.0.0/transpose/src/api/token/_transfers_by_account.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      664 2022-12-21 18:58:53.000000 transpose_data-4.0.0/transpose/src/api/token/_transfers_by_contract_address.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     9696 2022-12-21 18:59:10.000000 transpose_data-4.0.0/transpose/src/api/token/base.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     6097 2023-04-06 18:02:55.000000 transpose_data-4.0.0/transpose/src/base.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.081750 transpose_data-4.0.0/transpose/src/util/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:52.000000 transpose_data-4.0.0/transpose/src/util/__init__.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     2315 2022-10-31 01:46:12.000000 transpose_data-4.0.0/transpose/src/util/errors.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)      410 2022-05-27 19:56:33.000000 transpose_data-4.0.0/transpose/src/util/io.py
--rw-r--r--   0 jonathanbecker   (501) staff       (20)    18327 2023-04-06 16:49:24.000000 transpose_data-4.0.0/transpose/src/util/models.py
-drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 22:05:38.084633 transpose_data-4.0.0/transpose_data.egg-info/
--rw-r--r--   0 jonathanbecker   (501) staff       (20)    15881 2023-04-06 22:05:38.000000 transpose_data-4.0.0/transpose_data.egg-info/PKG-INFO
--rw-r--r--   0 jonathanbecker   (501) staff       (20)     3485 2023-04-06 22:05:38.000000 transpose_data-4.0.0/transpose_data.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanbecker   (501) staff       (20)        1 2023-04-06 22:05:38.000000 transpose_data-4.0.0/transpose_data.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanbecker   (501) staff       (20)       23 2023-04-06 22:05:38.000000 transpose_data-4.0.0/transpose_data.egg-info/requires.txt
--rw-r--r--   0 jonathanbecker   (501) staff       (20)       10 2023-04-06 22:05:38.000000 transpose_data-4.0.0/transpose_data.egg-info/top_level.txt
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.591105 transpose_data-4.0.1/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     1066 2022-05-27 16:10:33.000000 transpose_data-4.0.1/LICENSE
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        9 2022-06-01 23:37:24.000000 transpose_data-4.0.1/MANIFEST.in
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)    15880 2023-04-26 16:14:53.590243 transpose_data-4.0.1/PKG-INFO
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)    15010 2023-04-26 16:13:47.000000 transpose_data-4.0.1/README.md
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)       38 2023-04-26 16:14:53.591222 transpose_data-4.0.1/setup.cfg
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     1562 2023-04-26 16:14:33.000000 transpose_data-4.0.1/setup.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.514064 transpose_data-4.0.1/transpose/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      201 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-06-01 22:54:03.000000 transpose_data-4.0.1/transpose/__main__.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.515254 transpose_data-4.0.1/transpose/extras/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      220 2022-06-28 17:30:52.000000 transpose_data-4.0.1/transpose/extras/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     6916 2022-06-16 15:05:28.000000 transpose_data-4.0.1/transpose/extras/plot.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.515900 transpose_data-4.0.1/transpose/models/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      103 2022-06-28 17:30:34.000000 transpose_data-4.0.1/transpose/models/__init__.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.516992 transpose_data-4.0.1/transpose/src/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:48.000000 transpose_data-4.0.1/transpose/src/__init__.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.518007 transpose_data-4.0.1/transpose/src/api/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 17:29:51.000000 transpose_data-4.0.1/transpose/src/api/__init__.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.533998 transpose_data-4.0.1/transpose/src/api/block/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:56.000000 transpose_data-4.0.1/transpose/src/api/block/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      405 2022-06-02 15:28:23.000000 transpose_data-4.0.1/transpose/src/api/block/_accounts_by_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      599 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/block/_accounts_by_date_created.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      451 2022-10-31 15:56:44.000000 transpose_data-4.0.1/transpose/src/api/block/_blocks_by_date.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      458 2022-10-31 02:07:41.000000 transpose_data-4.0.1/transpose/src/api/block/_blocks_by_number.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      589 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/block/_contracts_by_creator.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      744 2022-05-31 20:16:32.000000 transpose_data-4.0.1/transpose/src/api/block/_logs_by_block.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      431 2022-05-31 21:53:19.000000 transpose_data-4.0.1/transpose/src/api/block/_logs_by_transaction.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      480 2023-01-04 14:43:27.000000 transpose_data-4.0.1/transpose/src/api/block/_transactions_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      483 2022-05-31 18:41:18.000000 transpose_data-4.0.1/transpose/src/api/block/_transactions_by_block.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      495 2022-05-31 18:41:08.000000 transpose_data-4.0.1/transpose/src/api/block/_transactions_by_date.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      405 2022-05-31 21:53:33.000000 transpose_data-4.0.1/transpose/src/api/block/_transactions_by_hash.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     6752 2023-01-04 14:43:27.000000 transpose_data-4.0.1/transpose/src/api/block/base.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     6114 2022-10-31 15:56:30.000000 transpose_data-4.0.1/transpose/src/api/constants.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.537158 transpose_data-4.0.1/transpose/src/api/endpoint/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 17:42:25.000000 transpose_data-4.0.1/transpose/src/api/endpoint/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     1247 2023-04-06 18:06:39.000000 transpose_data-4.0.1/transpose/src/api/endpoint/base.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.545788 transpose_data-4.0.1/transpose/src/api/ens/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:55.000000 transpose_data-4.0.1/transpose/src/api/ens/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      228 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/ens/_records_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      533 2022-05-27 21:18:51.000000 transpose_data-4.0.1/transpose/src/api/ens/_records_by_date.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      355 2022-05-31 21:50:53.000000 transpose_data-4.0.1/transpose/src/api/ens/_records_by_name.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      284 2022-05-27 20:41:28.000000 transpose_data-4.0.1/transpose/src/api/ens/_records_by_owner.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      388 2022-05-27 22:44:42.000000 transpose_data-4.0.1/transpose/src/api/ens/_records_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      583 2022-12-21 18:57:18.000000 transpose_data-4.0.1/transpose/src/api/ens/_transfers_by_name.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      591 2022-12-21 18:57:29.000000 transpose_data-4.0.1/transpose/src/api/ens/_transfers_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     3988 2022-12-21 18:57:46.000000 transpose_data-4.0.1/transpose/src/api/ens/base.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.558835 transpose_data-4.0.1/transpose/src/api/nft/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:54.000000 transpose_data-4.0.1/transpose/src/api/nft/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      436 2022-05-31 22:08:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_collections_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      718 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_collections_by_date_created.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      325 2022-07-26 20:53:53.000000 transpose_data-4.0.1/transpose/src/api/nft/_collections_by_name.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      337 2022-07-26 20:54:17.000000 transpose_data-4.0.1/transpose/src/api/nft/_collections_by_symbol.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      319 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      646 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_date_minted.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      297 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_name.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      422 2022-05-31 22:52:06.000000 transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_owner.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      632 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      325 2022-05-31 23:09:34.000000 transpose_data-4.0.1/transpose/src/api/nft/_owners_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      385 2022-05-31 23:11:35.000000 transpose_data-4.0.1/transpose/src/api/nft/_owners_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      396 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_sales.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      541 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_sales_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      520 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_sales_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      552 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_sales_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      457 2022-12-21 18:58:22.000000 transpose_data-4.0.1/transpose/src/api/nft/_transfers.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      603 2022-12-21 18:57:56.000000 transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      660 2022-12-21 18:58:03.000000 transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      683 2022-12-21 18:58:12.000000 transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_token_id.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)    10684 2022-12-21 18:58:37.000000 transpose_data-4.0.1/transpose/src/api/nft/base.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.559660 transpose_data-4.0.1/transpose/src/api/sql/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2023-04-06 17:19:08.000000 transpose_data-4.0.1/transpose/src/api/sql/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     2954 2023-04-26 16:14:33.000000 transpose_data-4.0.1/transpose/src/api/sql/base.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.580136 transpose_data-4.0.1/transpose/src/api/token/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:53.000000 transpose_data-4.0.1/transpose/src/api/token/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      434 2022-06-01 20:16:47.000000 transpose_data-4.0.1/transpose/src/api/token/_native_token_balances_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      526 2022-06-01 20:11:31.000000 transpose_data-4.0.1/transpose/src/api/token/_native_token_transfers.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      805 2022-06-01 20:12:47.000000 transpose_data-4.0.1/transpose/src/api/token/_native_token_transfers_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      331 2022-06-02 17:25:00.000000 transpose_data-4.0.1/transpose/src/api/token/_owners_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      423 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/token/_swaps.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      558 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/token/_swaps_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      649 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/token/_swaps_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      581 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/token/_swaps_by_pair.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      430 2022-06-01 19:06:51.000000 transpose_data-4.0.1/transpose/src/api/token/_tokens_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      712 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/api/token/_tokens_by_date_created.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      300 2022-07-26 20:55:18.000000 transpose_data-4.0.1/transpose/src/api/token/_tokens_by_name.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      434 2022-06-01 19:44:57.000000 transpose_data-4.0.1/transpose/src/api/token/_tokens_by_owner.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      312 2022-07-26 20:55:27.000000 transpose_data-4.0.1/transpose/src/api/token/_tokens_by_symbol.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      461 2022-12-21 18:58:59.000000 transpose_data-4.0.1/transpose/src/api/token/_transfers.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      607 2022-12-21 18:58:45.000000 transpose_data-4.0.1/transpose/src/api/token/_transfers_by_account.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      664 2022-12-21 18:58:53.000000 transpose_data-4.0.1/transpose/src/api/token/_transfers_by_contract_address.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     9696 2022-12-21 18:59:10.000000 transpose_data-4.0.1/transpose/src/api/token/base.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     6097 2023-04-13 13:30:46.000000 transpose_data-4.0.1/transpose/src/base.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.583420 transpose_data-4.0.1/transpose/src/util/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        0 2022-05-27 16:33:52.000000 transpose_data-4.0.1/transpose/src/util/__init__.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     2315 2022-10-31 01:46:12.000000 transpose_data-4.0.1/transpose/src/util/errors.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)      410 2022-05-27 19:56:33.000000 transpose_data-4.0.1/transpose/src/util/io.py
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)    18327 2023-04-06 16:49:24.000000 transpose_data-4.0.1/transpose/src/util/models.py
+drwxr-xr-x   0 jonathanbecker   (501) staff       (20)        0 2023-04-26 16:14:53.589397 transpose_data-4.0.1/transpose_data.egg-info/
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)    15880 2023-04-26 16:14:53.000000 transpose_data-4.0.1/transpose_data.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)     3485 2023-04-26 16:14:53.000000 transpose_data-4.0.1/transpose_data.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)        1 2023-04-26 16:14:53.000000 transpose_data-4.0.1/transpose_data.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)       23 2023-04-26 16:14:53.000000 transpose_data-4.0.1/transpose_data.egg-info/requires.txt
+-rw-r--r--   0 jonathanbecker   (501) staff       (20)       10 2023-04-26 16:14:53.000000 transpose_data-4.0.1/transpose_data.egg-info/top_level.txt
```

### Comparing `transpose_data-4.0.0/LICENSE` & `transpose_data-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/PKG-INFO` & `transpose_data-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpose_data
-Version: 4.0.0
+Version: 4.0.1
 Summary: Web3 Data Made Simple. Powerful APIs for accessing human-readable blockchain data at scale: from blocks and transactions to NFTs and tokens.
 Home-page: https://github.com/TransposeData/transpose-python-sdk
 Author: Michael Calvey (michaeljohncalvey), Alex Langshur (alangshur), Jonathan Becker (jon-becker)
 Author-email: michael@transpose.io, alex@transpose.io, jon@transpose.io
 License: MIT
 Keywords: web3,data,ethereum,web3 data,ethereum data
 Classifier: Development Status :: 3 - Alpha
@@ -47,15 +47,15 @@
 |  Product  | Description                                                                                                                                                                                                                  | Documentation                                                                                   |
 | :-------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
 | Block API | The Block API provides endpoints for accessing low-level blockchain data at scale, including accounts, blocks, transactions, internal transactions, and logs.                                                                | [Block API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/block.md) |
 |  ENS API  | The ENS API provides endpoints for looking up ENS names (both historical and primary), resolving ENS names and records, and monitoring ENS transfers and sales.                                                              | [ENS API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/ens.md)     |
 |  NFT API  | The NFT API provides endpoints for retrieving any collection and NFT in existence, as well as NFT images, operators, owners, transfers, approvals, and much more (fully supports both ERC-721 and ERC-1155 NFTs).            | [NFT API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/nft.md)     |
 | Token API | The Token API provides endpoints for retrieving any token, token balance, transfer, and symbol in existence, including full support for native token transfers and balances (fully supports both ERC-20 and ERC-777 tokens). | [Token API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/token.md) |
 | SQL API | The SQL API provides direct SQL access to our entire ecosystem of indexed blockchain data. Paired with our robust indexing pipeline, SQL access gives unlimited flexibility in how you mix, aggregate, and query activity across the blockchain.  | [SQL API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/sql.md) |
-| Endpoint API | The Endpoint API provides customized REST endpoints that you ca n create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
+| Endpoint API | The Endpoint API provides customized REST endpoints that you can create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
 
 ## SDK Documentation
 You can learn more about the Transpose SDK and how it works below.
 
 
 ### SDK Classes
 The Transpose SDK uses custom classes to represent API responses:
@@ -138,15 +138,15 @@
 </details>
 
 ### Raw JSON Responses
 <details>
 <summary>
 Opt-in to raw JSON Responses
 </summary>
-If you wish to recieve responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
+If you wish to receive responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
 
 **Response classes are considered deprecated as of v3.1.0 and will be removed in v4.0.0. JSON responses will become standard in v4.0.0**
 
 ```python
 from transpose_sdk import Transpose
 api = Transpose(api_key="YOUR_API_KEY", json=True)
 ```
```

### Comparing `transpose_data-4.0.0/README.md` & `transpose_data-4.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 |  Product  | Description                                                                                                                                                                                                                  | Documentation                                                                                   |
 | :-------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
 | Block API | The Block API provides endpoints for accessing low-level blockchain data at scale, including accounts, blocks, transactions, internal transactions, and logs.                                                                | [Block API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/block.md) |
 |  ENS API  | The ENS API provides endpoints for looking up ENS names (both historical and primary), resolving ENS names and records, and monitoring ENS transfers and sales.                                                              | [ENS API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/ens.md)     |
 |  NFT API  | The NFT API provides endpoints for retrieving any collection and NFT in existence, as well as NFT images, operators, owners, transfers, approvals, and much more (fully supports both ERC-721 and ERC-1155 NFTs).            | [NFT API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/nft.md)     |
 | Token API | The Token API provides endpoints for retrieving any token, token balance, transfer, and symbol in existence, including full support for native token transfers and balances (fully supports both ERC-20 and ERC-777 tokens). | [Token API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/token.md) |
 | SQL API | The SQL API provides direct SQL access to our entire ecosystem of indexed blockchain data. Paired with our robust indexing pipeline, SQL access gives unlimited flexibility in how you mix, aggregate, and query activity across the blockchain.  | [SQL API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/sql.md) |
-| Endpoint API | The Endpoint API provides customized REST endpoints that you ca n create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
+| Endpoint API | The Endpoint API provides customized REST endpoints that you can create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
 
 ## SDK Documentation
 You can learn more about the Transpose SDK and how it works below.
 
 
 ### SDK Classes
 The Transpose SDK uses custom classes to represent API responses:
@@ -119,15 +119,15 @@
 </details>
 
 ### Raw JSON Responses
 <details>
 <summary>
 Opt-in to raw JSON Responses
 </summary>
-If you wish to recieve responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
+If you wish to receive responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
 
 **Response classes are considered deprecated as of v3.1.0 and will be removed in v4.0.0. JSON responses will become standard in v4.0.0**
 
 ```python
 from transpose_sdk import Transpose
 api = Transpose(api_key="YOUR_API_KEY", json=True)
 ```
```

### Comparing `transpose_data-4.0.0/setup.py` & `transpose_data-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = f.read()
     
 setup(
     name='transpose_data',
     
     # version compliant with PEP440
     # https://peps.python.org/pep-0440/
-    version='4.0.0',
+    version='4.0.1',
     
     # project meta
     long_description = long_description,
     long_description_content_type="text/markdown",
     include_package_data = True,
     description='Web3 Data Made Simple. Powerful APIs for accessing human-readable blockchain data at scale: from blocks and transactions to NFTs and tokens.',
     keywords=['web3', 'data', 'ethereum', 'web3 data', 'ethereum data'],
```

### Comparing `transpose_data-4.0.0/transpose/extras/plot.py` & `transpose_data-4.0.1/transpose/extras/plot.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/block/_accounts_by_date_created.py` & `transpose_data-4.0.1/transpose/src/api/block/_accounts_by_date_created.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/block/_contracts_by_creator.py` & `transpose_data-4.0.1/transpose/src/api/block/_contracts_by_creator.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/block/_logs_by_block.py` & `transpose_data-4.0.1/transpose/src/api/block/_logs_by_block.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/block/base.py` & `transpose_data-4.0.1/transpose/src/api/block/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/constants.py` & `transpose_data-4.0.1/transpose/src/api/constants.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/endpoint/base.py` & `transpose_data-4.0.1/transpose/src/api/endpoint/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/ens/_records_by_date.py` & `transpose_data-4.0.1/transpose/src/api/ens/_records_by_date.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/ens/_transfers_by_name.py` & `transpose_data-4.0.1/transpose/src/api/ens/_transfers_by_name.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/ens/_transfers_by_token_id.py` & `transpose_data-4.0.1/transpose/src/api/ens/_transfers_by_token_id.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/ens/base.py` & `transpose_data-4.0.1/transpose/src/api/ens/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_collections_by_date_created.py` & `transpose_data-4.0.1/transpose/src/api/nft/_collections_by_date_created.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_date_minted.py` & `transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_date_minted.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_nfts_by_token_id.py` & `transpose_data-4.0.1/transpose/src/api/nft/_nfts_by_token_id.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_sales_by_account.py` & `transpose_data-4.0.1/transpose/src/api/nft/_sales_by_account.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_sales_by_contract_address.py` & `transpose_data-4.0.1/transpose/src/api/nft/_sales_by_contract_address.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_sales_by_token_id.py` & `transpose_data-4.0.1/transpose/src/api/nft/_sales_by_token_id.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_account.py` & `transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_account.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_contract_address.py` & `transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_contract_address.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/_transfers_by_token_id.py` & `transpose_data-4.0.1/transpose/src/api/nft/_transfers_by_token_id.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/nft/base.py` & `transpose_data-4.0.1/transpose/src/api/nft/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_native_token_transfers.py` & `transpose_data-4.0.1/transpose/src/api/token/_native_token_transfers.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_native_token_transfers_by_account.py` & `transpose_data-4.0.1/transpose/src/api/token/_native_token_transfers_by_account.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_swaps_by_account.py` & `transpose_data-4.0.1/transpose/src/api/token/_swaps_by_account.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_swaps_by_contract_address.py` & `transpose_data-4.0.1/transpose/src/api/token/_swaps_by_contract_address.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_swaps_by_pair.py` & `transpose_data-4.0.1/transpose/src/api/token/_swaps_by_pair.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_tokens_by_date_created.py` & `transpose_data-4.0.1/transpose/src/api/token/_tokens_by_date_created.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_transfers_by_account.py` & `transpose_data-4.0.1/transpose/src/api/token/_transfers_by_account.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/_transfers_by_contract_address.py` & `transpose_data-4.0.1/transpose/src/api/token/_transfers_by_contract_address.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/api/token/base.py` & `transpose_data-4.0.1/transpose/src/api/token/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/base.py` & `transpose_data-4.0.1/transpose/src/base.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/util/errors.py` & `transpose_data-4.0.1/transpose/src/util/errors.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose/src/util/models.py` & `transpose_data-4.0.1/transpose/src/util/models.py`

 * *Files identical despite different names*

### Comparing `transpose_data-4.0.0/transpose_data.egg-info/PKG-INFO` & `transpose_data-4.0.1/transpose_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transpose-data
-Version: 4.0.0
+Version: 4.0.1
 Summary: Web3 Data Made Simple. Powerful APIs for accessing human-readable blockchain data at scale: from blocks and transactions to NFTs and tokens.
 Home-page: https://github.com/TransposeData/transpose-python-sdk
 Author: Michael Calvey (michaeljohncalvey), Alex Langshur (alangshur), Jonathan Becker (jon-becker)
 Author-email: michael@transpose.io, alex@transpose.io, jon@transpose.io
 License: MIT
 Keywords: web3,data,ethereum,web3 data,ethereum data
 Classifier: Development Status :: 3 - Alpha
@@ -47,15 +47,15 @@
 |  Product  | Description                                                                                                                                                                                                                  | Documentation                                                                                   |
 | :-------: | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- |
 | Block API | The Block API provides endpoints for accessing low-level blockchain data at scale, including accounts, blocks, transactions, internal transactions, and logs.                                                                | [Block API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/block.md) |
 |  ENS API  | The ENS API provides endpoints for looking up ENS names (both historical and primary), resolving ENS names and records, and monitoring ENS transfers and sales.                                                              | [ENS API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/ens.md)     |
 |  NFT API  | The NFT API provides endpoints for retrieving any collection and NFT in existence, as well as NFT images, operators, owners, transfers, approvals, and much more (fully supports both ERC-721 and ERC-1155 NFTs).            | [NFT API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/nft.md)     |
 | Token API | The Token API provides endpoints for retrieving any token, token balance, transfer, and symbol in existence, including full support for native token transfers and balances (fully supports both ERC-20 and ERC-777 tokens). | [Token API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/token.md) |
 | SQL API | The SQL API provides direct SQL access to our entire ecosystem of indexed blockchain data. Paired with our robust indexing pipeline, SQL access gives unlimited flexibility in how you mix, aggregate, and query activity across the blockchain.  | [SQL API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/sql.md) |
-| Endpoint API | The Endpoint API provides customized REST endpoints that you ca n create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
+| Endpoint API | The Endpoint API provides customized REST endpoints that you can create, version, and use directly in your production applications. | [Endpoint API Docs](https://github.com/TransposeData/transpose-python-sdk/blob/main/docs/endpoint.md) |
 
 ## SDK Documentation
 You can learn more about the Transpose SDK and how it works below.
 
 
 ### SDK Classes
 The Transpose SDK uses custom classes to represent API responses:
@@ -138,15 +138,15 @@
 </details>
 
 ### Raw JSON Responses
 <details>
 <summary>
 Opt-in to raw JSON Responses
 </summary>
-If you wish to recieve responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
+If you wish to receive responses in JSON format, you can set the `json` parameter to `True` when initializing the SDK. This will return all responses as JSON objects.
 
 **Response classes are considered deprecated as of v3.1.0 and will be removed in v4.0.0. JSON responses will become standard in v4.0.0**
 
 ```python
 from transpose_sdk import Transpose
 api = Transpose(api_key="YOUR_API_KEY", json=True)
 ```
```

### Comparing `transpose_data-4.0.0/transpose_data.egg-info/SOURCES.txt` & `transpose_data-4.0.1/transpose_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

