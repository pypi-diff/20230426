# Comparing `tmp/splight-lib-2.3.3.tar.gz` & `tmp/splight-lib-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-lib-2.3.3.tar", last modified: Mon Apr 24 21:45:39 2023, max compression
+gzip compressed data, was "splight-lib-2.3.4.tar", last modified: Tue Apr 25 15:01:42 2023, max compression
```

## Comparing `splight-lib-2.3.3.tar` & `splight-lib-2.3.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.000000 splight-lib-2.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 21:45:39.990110 splight-lib-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-24 21:45:39.000000 splight-lib-2.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/communication/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/communication/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/database/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/database/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/datalake/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/remote_splight_lib/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/hub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-24 21:45:39.000000 splight-lib-2.3.3/remote_splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 21:45:39.990110 splight-lib-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-24 21:45:39.000000 splight-lib-2.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/splight_abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/splight_abstract/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/auth/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.982110 splight-lib-2.3.3/splight_abstract/cache/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/cache/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/client/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/client/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/client/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/communication/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/communication/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/database/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/database/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/datalake/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/deployment/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/endpoints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/hub/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/hub/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/notification/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/notification/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/remote/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_abstract/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_abstract/storage/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/auth/mac_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib/client/database/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/database/classmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/database/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/database/remote_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib/client/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/datalake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/datalake/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9219 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/datalake/remote_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/client/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/splight_lib/component/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/component/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/execution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/splight_lib/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/logging/_internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/logging/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/logging/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/splight_lib/restclient/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/restclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/restclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/restclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/restclient/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.986110 splight-lib-2.3.3/splight_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_lib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/splight_models/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 21:45:39.990110 splight-lib-2.3.3/splight_models/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/communication/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/communication/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/datalake.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/deployment.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/setpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-24 21:45:39.000000 splight-lib-2.3.3/splight_models/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:41.000000 splight-lib-2.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 15:01:42.327626 splight-lib-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-25 15:01:41.000000 splight-lib-2.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/communication/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/database/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.315625 splight-lib-2.3.4/remote_splight_lib/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9054 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/datalake/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/remote_splight_lib/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/hub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-25 15:01:41.000000 splight-lib-2.3.4/remote_splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 15:01:42.327626 splight-lib-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-25 15:01:41.000000 splight-lib-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3997 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/cache/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/client/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/communication/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/database/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/database/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/datalake/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/deployment/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/endpoints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/hub/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/notification/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/remote/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_abstract/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_abstract/storage/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.319625 splight-lib-2.3.4/splight_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/mac_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/classmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/database/remote_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/client/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9281 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/datalake/remote_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/client/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26067 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/component/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/execution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/logging/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib/restclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/restclient/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_lib/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.323626 splight-lib-2.3.4/splight_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-25 15:01:42.000000 splight-lib-2.3.4/splight_lib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/splight_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 15:01:42.327626 splight-lib-2.3.4/splight_models/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/communication/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9631 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/datalake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/setpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-25 15:01:41.000000 splight-lib-2.3.4/splight_models/webhook.py
```

### Comparing `splight-lib-2.3.3/PKG-INFO` & `splight-lib-2.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.3
+Version: 2.3.4
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.3/remote_splight_lib/communication/client.py` & `splight-lib-2.3.4/remote_splight_lib/communication/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/remote_splight_lib/database/classmap.py` & `splight-lib-2.3.4/remote_splight_lib/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/remote_splight_lib/database/client.py` & `splight-lib-2.3.4/remote_splight_lib/database/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/remote_splight_lib/datalake/client.py` & `splight-lib-2.3.4/remote_splight_lib/datalake/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from pydantic import BaseModel
 from remote_splight_lib.auth import SplightAuthToken
 from remote_splight_lib.settings import settings
 from retry import retry
 from splight_abstract import AbstractRemoteClient, QuerySet
 from splight_abstract.datalake import (
     AbstractDatalakeClient,
-    validate_instance_type,
-    validate_resource_type,
+    validate_datalake_instance_type,
+    validate_datalake_resource_type,
 )
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import (
     ConnectError,
     HTTPError,
     SplightRestClient,
     Timeout,
@@ -100,15 +100,15 @@
     def _raw_delete(self, collection: str, **kwargs) -> None:
         # DELETE /datalake/delete/
         url = self._base_url / f"{self._PREFIX}/delete/"
         params = {"source": collection}
         response = self._restclient.delete(url, params=params, json=kwargs)
         response.raise_for_status()
 
-    @validate_resource_type
+    @validate_datalake_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
         logger.debug(
@@ -140,15 +140,15 @@
             group_id=query.group_id,
             group_fields=query.group_fields,
             tzinfo=timezone(timedelta(hours=query.timezone_offset)),
             **query.filters,
         )
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
-    @validate_resource_type
+    @validate_datalake_resource_type
     def get_dataframe(
         self, resource_type: DatalakeModel, **kwargs
     ) -> pd.DataFrame:
         # GET /datalake/dumpdata/?source=collection
         url = self._base_url / f"{self._PREFIX}/dumpdata/"
         collection = resource_type.Meta.collection_name
         kwargs.update({"source": collection})
@@ -179,29 +179,29 @@
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
         return pd.DataFrame(dfs)
 
-    @validate_instance_type
+    @validate_datalake_instance_type
     def save(
         self,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
         # POST /datalake/save/
         logger.debug("Saving instances %s.", instances, tags=LogTags.DATALAKE)
         if not instances:
             return instances
         resource_type = instances[0].__class__
         collection = resource_type.Meta.collection_name
         return self._raw_save(collection=collection, instances=instances)
 
     @retry(REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
-    @validate_resource_type
+    @validate_datalake_resource_type
     def save_dataframe(
         self, resource_type: DatalakeModel, dataframe: pd.DataFrame
     ) -> None:
         # POST /datalake/loaddata/
         logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
 
         url = self._base_url / f"{self._PREFIX}/loaddata/"
@@ -213,15 +213,15 @@
         response = self._restclient.post(
             url,
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
-    @validate_resource_type
+    @validate_datalake_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
         logger.debug(
             "Deleting resources of type %s from datalake.",
             resource_type,
             tags=LogTags.DATALAKE,
         )
```

### Comparing `splight-lib-2.3.3/remote_splight_lib/hub/client.py` & `splight-lib-2.3.4/remote_splight_lib/hub/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from furl import furl
 from pydantic import BaseModel
 from remote_splight_lib.auth import SplightAuthToken
 from remote_splight_lib.settings import settings
 from splight_abstract import (
     AbstractHubClient,
     AbstractHubSubClient,
-    validate_resource_type,
+    validate_client_resource_type,
 )
 from splight_models import HubComponent, HubComponentVersion
 
 
 class _SplightHubGenericClient(AbstractHubSubClient):
     _PREFIX: str = "v2/hub"
     valid_classes = [
@@ -52,15 +52,15 @@
             if skip_ > 0:
                 kwargs["page"] = skip_ // limit_ + 1
         return kwargs
 
     def save(self, instance: BaseModel) -> BaseModel:
         raise NotImplementedError
 
-    @validate_resource_type
+    @validate_client_resource_type
     def _get(
         self,
         resource_type: Type,
         first: bool = False,
         limit_: int = -1,
         skip_: int = 0,
         **kwargs,
@@ -95,35 +95,35 @@
     def delete(self, resource_type: Type, id: str) -> None:
         url = self._get_url(resource_type, id)
         response = self._session.delete(url)
         assert (
             response.status_code == 204
         ), f"Failed to delete component {response.content}"
 
-    @validate_resource_type
+    @validate_client_resource_type
     def update(self, resource_type: Type, id: str, data: Dict) -> BaseModel:
         url = self._get_url(resource_type, id)
         response = self._session.put(url, json=data)
         assert (
             response.status_code == 200
         ), f"Failed to update component. {response.content}"
         return resource_type(**response.json())
 
-    @validate_resource_type
+    @validate_client_resource_type
     def partial_update(
         self, resource_type: Type, id: str, data: Dict
     ) -> BaseModel:
         url = self._get_url(resource_type, id)
         response = self._session.patch(url, json=data)
         assert (
             response.status_code == 200
         ), f"Failed to update component. {response.content}"
         return resource_type.parse_obj(response.json())
 
-    @validate_resource_type
+    @validate_client_resource_type
     def rebuild(self, resource_type: Type, id: str) -> None:
         url = self._get_url(resource_type, id)
         url = url / "rebuild/"
         response = self._session.post(url, headers=self.headers)
         assert (
             response.status_code == 204
         ), f"Failed to rebuild component. {response.content}"
```

### Comparing `splight-lib-2.3.3/remote_splight_lib/settings.py` & `splight-lib-2.3.4/remote_splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/setup.py` & `splight-lib-2.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 test_requires = [
     "pytest==7.1.2",
     "mock==4.0.3",
 ]
 
 setup(
     name="splight-lib",
-    version="2.3.3",
+    version="2.3.4",
     author="Splight",
     author_email="factory@splight-ae.com",
     packages=find_packages(),
     package_data={},
     include_package_data=True,
     scripts=[],
     url=None,
```

### Comparing `splight-lib-2.3.3/splight_abstract/auth/abstract.py` & `splight-lib-2.3.4/splight_abstract/auth/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/auth/exceptions.py` & `splight-lib-2.3.4/splight_abstract/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/cache/abstract.py` & `splight-lib-2.3.4/splight_abstract/cache/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/client/abstract.py` & `splight-lib-2.3.4/splight_abstract/client/abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 from .hooks import HooksMixin
 
 
 class empty:
     pass
 
 
-def validate_resource_type(func: Callable) -> Callable:
+def validate_client_resource_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, resource_type: Type, *args, **kwargs):
         if resource_type not in self.valid_classes:
             raise NotImplementedError(
                 f"Not a valid resource_type: {resource_type.__name__}"
             )
         return func(self, resource_type, *args, **kwargs)
 
     return wrapper
 
 
-def validate_instance_type(func: Callable) -> Callable:
+def validate_client_instance_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, instance: BaseModel, *args, **kwargs):
         if type(instance) not in self.valid_classes:
             raise NotImplementedError(
                 f"Not a valid instance type: {type(instance).__name__}"
             )
         return func(self, instance, *args, **kwargs)
```

### Comparing `splight-lib-2.3.3/splight_abstract/client/filter.py` & `splight-lib-2.3.4/splight_abstract/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/client/hooks.py` & `splight-lib-2.3.4/splight_abstract/client/hooks.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/communication/abstract.py` & `splight-lib-2.3.4/splight_abstract/communication/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/database/abstract.py` & `splight-lib-2.3.4/splight_abstract/database/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/datalake/abstract.py` & `splight-lib-2.3.4/splight_abstract/datalake/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 import pandas as pd
 from pydantic import BaseModel
 from splight_abstract.client import AbstractClient, QuerySet
 from splight_models import DatalakeModel, Query
 
 
-def validate_resource_type(func: Callable) -> Callable:
+def validate_datalake_resource_type(func: Callable) -> Callable:
     @wraps(func)
     def inner(self, resource_type, *args, **kwargs):
         if not issubclass(resource_type, DatalakeModel):
             raise NotImplementedError(
                 f"Not a valid resource_type: {resource_type.__name__}"
             )
         return func(self, resource_type, *args, **kwargs)
 
     return inner
 
 
-def validate_instance_type(func: Callable) -> Callable:
+def validate_datalake_instance_type(func: Callable) -> Callable:
     @wraps(func)
     def wrapper(self, instances: List[BaseModel], *args, **kwargs):
         if instances:
             resource_type = instances[0].__class__
             if not all([isinstance(i, resource_type) for i in instances]):
                 raise TypeError("All instances must be of the same type")
             if not issubclass(resource_type, DatalakeModel):
```

### Comparing `splight-lib-2.3.3/splight_abstract/deployment/abstract.py` & `splight-lib-2.3.4/splight_abstract/deployment/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/endpoints/__init__.py` & `splight-lib-2.3.4/splight_abstract/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/hub/abstract.py` & `splight-lib-2.3.4/splight_abstract/hub/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_abstract/storage/abstract.py` & `splight-lib-2.3.4/splight_abstract/storage/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/auth/mac_auth.py` & `splight-lib-2.3.4/splight_lib/auth/mac_auth.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/database/classmap.py` & `splight-lib-2.3.4/splight_lib/client/database/classmap.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/database/local_client.py` & `splight-lib-2.3.4/splight_lib/client/database/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/database/remote_client.py` & `splight-lib-2.3.4/splight_lib/client/database/remote_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/datalake/local_client.py` & `splight-lib-2.3.4/splight_lib/client/datalake/local_client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/datalake/remote_client.py` & `splight-lib-2.3.4/splight_lib/client/datalake/remote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from furl import furl
 from pydantic import BaseModel
 from remote_splight_lib.auth import SplightAuthToken
 from retry import retry
 from splight_abstract import AbstractRemoteClient, QuerySet
 from splight_abstract.datalake import (
     AbstractDatalakeClient,
-    validate_instance_type,
-    validate_resource_type,
+    validate_datalake_instance_type,
+    validate_datalake_resource_type,
 )
 from splight_lib.client.exceptions import SPLIGHT_REQUEST_EXCEPTIONS
 from splight_lib.client.settings import settings_remote as settings
 from splight_lib.logging._internal import LogTags, get_splight_logger
 from splight_lib.restclient import SplightRestClient
 from splight_models import DatalakeModel, Query
 
@@ -96,15 +96,15 @@
     def _raw_delete(self, collection: str, **kwargs) -> None:
         # DELETE /datalake/delete/
         url = self._base_url / f"{self._PREFIX}/delete/"
         params = {"source": collection}
         response = self._restclient.delete(url, params=params, json=kwargs)
         response.raise_for_status()
 
-    @validate_resource_type
+    @validate_datalake_resource_type
     def get(
         self,
         resource_type: DatalakeModel,
         *args,
         **kwargs,
     ) -> List[BaseModel]:
         logger.debug(
@@ -136,19 +136,18 @@
             group_id=query.group_id,
             group_fields=query.group_fields,
             tzinfo=timezone(timedelta(hours=query.timezone_offset)),
             **query.filters,
         )
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
-    @validate_resource_type
+    @validate_datalake_resource_type
     def get_dataframe(
         self, resource_type: DatalakeModel, **kwargs
     ) -> pd.DataFrame:
-
         # Add this parameter to the request in order to make
         # the Mongo query work faster.
         # It should be the same as the resource_type.
         if "output_format" not in kwargs:
             kwargs["output_format"] = resource_type.class_name()
 
         # GET /datalake/dumpdata/?source=collection
@@ -180,30 +179,30 @@
             self.get_dataframe(resource_type=resource_type, **query)
             for query in queries
         ]
         if dfs:
             return pd.concat(dfs, axis=1)
         return pd.DataFrame(dfs)
 
-    @validate_instance_type
+    @validate_datalake_instance_type
     def save(
         self,
         instances: List[DatalakeModel],
     ) -> List[DatalakeModel]:
         # POST /datalake/save/
         logger.debug("Saving instances %s.", instances, tags=LogTags.DATALAKE)
 
         if not instances:
             return instances
         resource_type = instances[0].__class__
         collection = resource_type.Meta.collection_name
         return self._raw_save(collection=collection, instances=instances)
 
     @retry(SPLIGHT_REQUEST_EXCEPTIONS, tries=3, delay=2, jitter=1)
-    @validate_resource_type
+    @validate_datalake_resource_type
     def save_dataframe(
         self, resource_type: DatalakeModel, dataframe: pd.DataFrame
     ) -> None:
         logger.debug("Saving dataframe.", tags=LogTags.DATALAKE)
 
         # POST /datalake/loaddata/
         url = self._base_url / f"{self._PREFIX}/loaddata/"
@@ -215,15 +214,15 @@
         response = self._restclient.post(
             url,
             data={"source": collection},
             files={"file": open(tmp_file.name, mode="rb")},
         )
         response.raise_for_status()
 
-    @validate_resource_type
+    @validate_datalake_resource_type
     def delete(self, resource_type: DatalakeModel, **kwargs) -> None:
         logger.debug(
             "Deleting resources of type %s from datalake.",
             resource_type,
             tags=LogTags.DATALAKE,
         )
```

### Comparing `splight-lib-2.3.3/splight_lib/client/exceptions.py` & `splight-lib-2.3.4/splight_lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/file_handler.py` & `splight-lib-2.3.4/splight_lib/client/file_handler.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/filter.py` & `splight-lib-2.3.4/splight_lib/client/filter.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/client/settings.py` & `splight-lib-2.3.4/splight_lib/client/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/component/abstract.py` & `splight-lib-2.3.4/splight_lib/component/abstract.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/encryption.py` & `splight-lib-2.3.4/splight_lib/encryption.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/execution.py` & `splight-lib-2.3.4/splight_lib/execution.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/logging/_internal.py` & `splight-lib-2.3.4/splight_lib/logging/_internal.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/logging/component.py` & `splight-lib-2.3.4/splight_lib/logging/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/logging/logging.py` & `splight-lib-2.3.4/splight_lib/logging/logging.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/restclient/client.py` & `splight-lib-2.3.4/splight_lib/restclient/client.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/restclient/exceptions.py` & `splight-lib-2.3.4/splight_lib/restclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/restclient/types.py` & `splight-lib-2.3.4/splight_lib/restclient/types.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/settings.py` & `splight-lib-2.3.4/splight_lib/settings.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib/webhook.py` & `splight-lib-2.3.4/splight_lib/webhook.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_lib.egg-info/PKG-INFO` & `splight-lib-2.3.4/splight_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splight-lib
-Version: 2.3.3
+Version: 2.3.4
 Summary: Library for public use. Splight
 Home-page: UNKNOWN
 Author: Splight
 Author-email: factory@splight-ae.com
 License: LICENSE.txt
 Platform: UNKNOWN
 Provides-Extra: dev
```

### Comparing `splight-lib-2.3.3/splight_lib.egg-info/SOURCES.txt` & `splight-lib-2.3.4/splight_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/__init__.py` & `splight-lib-2.3.4/splight_models/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/alert.py` & `splight-lib-2.3.4/splight_models/alert.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/asset.py` & `splight-lib-2.3.4/splight_models/asset.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/base.py` & `splight-lib-2.3.4/splight_models/base.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/blockchain.py` & `splight-lib-2.3.4/splight_models/blockchain.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/communication/context.py` & `splight-lib-2.3.4/splight_models/communication/context.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/communication/events.py` & `splight-lib-2.3.4/splight_models/communication/events.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/component.py` & `splight-lib-2.3.4/splight_models/component.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/constants.py` & `splight-lib-2.3.4/splight_models/constants.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/datalake.py` & `splight-lib-2.3.4/splight_models/datalake.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/deployment.py` & `splight-lib-2.3.4/splight_models/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/exception.py` & `splight-lib-2.3.4/splight_models/exception.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/file.py` & `splight-lib-2.3.4/splight_models/file.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/hub.py` & `splight-lib-2.3.4/splight_models/hub.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/notification.py` & `splight-lib-2.3.4/splight_models/notification.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/query.py` & `splight-lib-2.3.4/splight_models/query.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/setpoint.py` & `splight-lib-2.3.4/splight_models/setpoint.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/user.py` & `splight-lib-2.3.4/splight_models/user.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/variable.py` & `splight-lib-2.3.4/splight_models/variable.py`

 * *Files identical despite different names*

### Comparing `splight-lib-2.3.3/splight_models/webhook.py` & `splight-lib-2.3.4/splight_models/webhook.py`

 * *Files identical despite different names*

