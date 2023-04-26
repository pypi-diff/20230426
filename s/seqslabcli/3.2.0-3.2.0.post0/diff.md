# Comparing `tmp/seqslabcli-3.2.0.tar.gz` & `tmp/seqslabcli-3.2.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslabcli-3.2.0.tar", last modified: Tue Mar  7 09:47:33 2023, max compression
+gzip compressed data, was "seqslabcli-3.2.0.post0.tar", last modified: Wed Apr 26 06:15:17 2023, max compression
```

## Comparing `seqslabcli-3.2.0.tar` & `seqslabcli-3.2.0.post0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.045918 seqslabcli-3.2.0/python/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.045918 seqslabcli-3.2.0/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.045918 seqslabcli-3.2.0/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.045918 seqslabcli-3.2.0/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.045918 seqslabcli-3.2.0/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/runsheet/runsheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.049918 seqslabcli-3.2.0/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20600 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.053918 seqslabcli-3.2.0/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/template/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/wes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/python/seqslabcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-03-07 09:47:33.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 09:47:32.000000 seqslabcli-3.2.0/python/seqslabcli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-07 09:47:33.057918 seqslabcli-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-03-07 09:47:23.000000 seqslabcli-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.024158 seqslabcli-3.2.0.post0/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37716 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20396 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40704 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12838 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/runsheet/runsheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20679 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.028158 seqslabcli-3.2.0.post0/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23184 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/wes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 06:15:16.000000 seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-26 06:15:17.032158 seqslabcli-3.2.0.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-04-26 06:15:06.000000 seqslabcli-3.2.0.post0/setup.py
```

### Comparing `seqslabcli-3.2.0/LICENSE` & `seqslabcli-3.2.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/PKG-INFO` & `seqslabcli-3.2.0.post0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslabcli
-Version: 3.2.0
+Version: 3.2.0.post0
 Summary: Seqslab CLI
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Description: <!-- PROJECT SHIELDS -->
         <!--
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0 Summary: Seqslab CLI
-Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin Author-
-email: jiayou.lin@atgenomix.com License: MIT license Description:
+Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post0 Summary: Seqslab
+CLI Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin
+Author-email: jiayou.lin@atgenomix.com License: MIT license Description:
 [Contributors][contributors-url] [Stargazers][stars-url] [Issues][issues-url]
 [License][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     [Logo]
                  ***** Atgenomix SeqsLab V3 platform CLI *****
 Command Line Interface application in the Atgenomix SeqsLab platform, a cloud-
                 first and enterprise BioMed-IT infrastructure.
                              Explore_the_docs_Â»
```

### Comparing `seqslabcli-3.2.0/python/seqslab/README.md` & `seqslabcli-3.2.0.post0/python/seqslab/README.md`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/__init__.py` & `seqslabcli-3.2.0.post0/python/seqslab/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 name = "seqslab"
 
 __all__ = [
 
 ]
 
 
-__version__ = "3.2.0"
+__version__ = "3.2.0post"
 
 LOGGING = {
     "DIR_PATH": "/var/log/seqslab"
 }
```

### Comparing `seqslabcli-3.2.0/python/seqslab/auth/azuread.py` & `seqslabcli-3.2.0.post0/python/seqslab/auth/azuread.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/auth/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/auth/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/cli.py` & `seqslabcli-3.2.0.post0/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/context.py` & `seqslabcli-3.2.0.post0/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/api/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/api/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/api/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/api/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/api/template.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/internal/aiocopy.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/aiocopy.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/internal/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/internal/utils.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/storage/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/storage/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/utils/biomimetype.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/drs/utils/progressbar.py` & `seqslabcli-3.2.0.post0/python/seqslab/drs/utils/progressbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             return self.__bar_string_format(
                 self.spinner[0], self.progress_name, "█" * 1, " " * 0, 1, 0, 0)
 
     def print(self, content: str = "") -> None:
         msg = self.update(self.complete_tasks)
         if len(content):
             msg += f' {content.ljust(200)} '
-        sys.stderr.write(f'\r {msg[:200]}')
+        sys.stderr.write(f'\r {msg[:100]}')
         sys.stderr.flush()
         if self.percentage == 1:
             sys.stderr.write(f'\n')
             sys.stderr.flush()
         sys.stderr.write(f'')
         sys.stderr.flush()
         if self.logger:
```

### Comparing `seqslabcli-3.2.0/python/seqslab/exceptions.py` & `seqslabcli-3.2.0.post0/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/organization/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/organization/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/plugin.py` & `seqslabcli-3.2.0.post0/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/role/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/role/internal/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/role/resource/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/role/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/runsheet/runsheet.py` & `seqslabcli-3.2.0.post0/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/settings.py` & `seqslabcli-3.2.0.post0/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/statusbar.py` & `seqslabcli-3.2.0.post0/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,25 +5,24 @@
 from pathlib import Path
 from zipfile import ZipFile
 
 from nubia import argument
 from nubia import command
 from seqslab.exceptions import exception_handler
 from termcolor import cprint
-from typing import List
 from yarl import URL
 
 from .internal.utils import create_zip
 from .register.common import trs_register
 from .resource.common import trs_resource
 from .template.base import TrsCreateTemplate
 from .template.base import TrsImagesTemplate
 
 import logging
-from typing import List, Dict, Optional
+from typing import List, Dict, Optional, Union
 
 """
 Copyright (C) 2022, Atgenomix Incorporated.
 
 All Rights Reserved.
 
 This program is an unpublished copyrighted work which is proprietary to
@@ -61,14 +60,16 @@
                             **image,
                             "checksum_type": image.get('checksum').split(':')[0],
                             "checksum": image.get('checksum').split(':')[1]})
                     else:
                         raise ValueError(f"Wrong checksum format {image.get('checksum')} in image")
                 else:
                     raise ValueError(f"No checksum in image")
+        else:
+            raise ValueError(f"Please provide a docker image.")
 
         backend = trs_register().load_resource()
         version_id = backend.version(tool_id=tool_id, version_name=version_name,
                                      version_id=version_id, images=image_list,
                                      descriptor_type=descriptor_type, **kwargs)["version_id"]
         return version_id
 
@@ -124,15 +125,15 @@
     @argument("toolclass_description",
               type=str,
               description="Specify the type of tool that you want to register (optional).")
     @argument("description",
               type=str,
               description="Specify the description of the tool that you want to register (optional).", )
     @argument("aliases",
-              type=list,
+              type=List[str],
               description="Specify the aliases of the tool that you want to register (optional).", )
     @argument("checker_url",
               type=URL,
               description="Specify the URL of the checker tool that you want to register (optional).", )
     @argument("has_checker",
               type=bool,
               description="Specify whether or not this tool has a checker tool associated with it (optional).", )
@@ -167,27 +168,27 @@
                           "to register in this version (required).",
               choices=["WDL", "CWL", "NFL"])
     @argument("images",
               type=str,
               description="Specify a JSON string describing a list of images you want to register in this version "
                           "(required).", )
     @argument("author",
-              type=list,
+              type=List[str],
               description="Specify the name of the author of the tool that you want "
                           "to register in this version (optional).", )
     @argument("verified",
               type=bool,
               description="Specify whether or not this version of the tool that you want "
                           "to register is verified (optional, default = false).", )
     @argument("verified_source",
-              type=list,
+              type=List[str],
               description="Specify the verified source of the tool that you want "
                           "to register in this version (optional).", )
     @argument("included_apps",
-              type=list,
+              type=List[str],
               description="Specify the apps that you want to include with the tool that you want "
                           "to register in this version (optional).", )
     @argument("signed",
               type=bool,
               description="Specify whether or not this version of the tool that you want "
                           "to register is signed (optional, default = false).", )
     @argument("is_production",
@@ -198,15 +199,15 @@
                 name: str = "", **kwargs) -> int:
         """
             Register TRS version object.
         """
         if not workspace:
             cprint("Enter a valid workspace", "red")
             return errno.EIO
-        kwargs = {'workspace': workspace}
+        kwargs['workspace'] = workspace
         id = self._version(tool_id=tool_id, version_name=name, version_id=id,
                            descriptor_type=descriptor_type, images=images, **kwargs)
         if isinstance(id, int):
             return id
         cprint(f"trs version object - {tool_id}: {id} create complete", "yellow")
         return 0
```

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/internal/utils.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/register/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/register/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/register/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/register/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/register/template.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/resource/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/resource/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/template/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/trs/template/template.py` & `seqslabcli-3.2.0.post0/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/usage_logger.py` & `seqslabcli-3.2.0.post0/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/user/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/user/internal/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/user/resource/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/user/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/internal/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/resource/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/template/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/template/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/template/template.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/wes/utils.py` & `seqslabcli-3.2.0.post0/python/seqslab/wes/utils.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/workspace/commands.py` & `seqslabcli-3.2.0.post0/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/workspace/internal/common.py` & `seqslabcli-3.2.0.post0/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/workspace/resource/azure.py` & `seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslab/workspace/resource/base.py` & `seqslabcli-3.2.0.post0/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/python/seqslabcli.egg-info/PKG-INFO` & `seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslabcli
-Version: 3.2.0
+Version: 3.2.0.post0
 Summary: Seqslab CLI
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Jia-You Lin
 Author-email: jiayou.lin@atgenomix.com
 License: MIT license
 Description: <!-- PROJECT SHIELDS -->
         <!--
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0 Summary: Seqslab CLI
-Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin Author-
-email: jiayou.lin@atgenomix.com License: MIT license Description:
+Metadata-Version: 2.1 Name: seqslabcli Version: 3.2.0.post0 Summary: Seqslab
+CLI Home-page: https://github.com/AnomeGAP/seqslab-cli Author: Jia-You Lin
+Author-email: jiayou.lin@atgenomix.com License: MIT license Description:
 [Contributors][contributors-url] [Stargazers][stars-url] [Issues][issues-url]
 [License][license-url] [![LinkedIn][linkedin-shield]][linkedin-url]
                                     [Logo]
                  ***** Atgenomix SeqsLab V3 platform CLI *****
 Command Line Interface application in the Atgenomix SeqsLab platform, a cloud-
                 first and enterprise BioMed-IT infrastructure.
                              Explore_the_docs_Â»
```

### Comparing `seqslabcli-3.2.0/python/seqslabcli.egg-info/SOURCES.txt` & `seqslabcli-3.2.0.post0/python/seqslabcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqslabcli-3.2.0/setup.py` & `seqslabcli-3.2.0.post0/setup.py`

 * *Files identical despite different names*

