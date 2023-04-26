# Comparing `tmp/frontrunner-sdk-0.1.0.tar.gz` & `tmp/frontrunner-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontrunner-sdk-0.1.0.tar", last modified: Tue Apr 25 18:53:45 2023, max compression
+gzip compressed data, was "frontrunner-sdk-0.1.1.tar", last modified: Tue Apr 25 21:21:50 2023, max compression
```

## Comparing `frontrunner-sdk-0.1.0.tar` & `frontrunner-sdk-0.1.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.911345 frontrunner-sdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-25 18:53:45.911345 frontrunner-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/backend_shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.899345 frontrunner-sdk-0.1.0/frontrunner_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.899345 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_light_client_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/clients/openapi_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.899345 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.903345 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/find_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_leagues.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.903345 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/cancel_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/create_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/create_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_account_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_order_books.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_trades.py
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_markets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_orders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_positions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_trades.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.903345 frontrunner-sdk-0.1.0/frontrunner_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/chained.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/conditional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/config/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.903345 frontrunner-sdk-0.1.0/frontrunner_sdk/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.903345 frontrunner-sdk-0.1.0/frontrunner_sdk/facades/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/facades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/facades/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/facades/frontrunner.py
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/facades/injective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.907345 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/paginators.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/streams.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/ioc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.907345 frontrunner-sdk-0.1.0/frontrunner_sdk/logging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/logging/log_external_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/logging/log_operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.907345 frontrunner-sdk-0.1.0/frontrunner_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/models/cancel_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/models/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/models/wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.895345 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.907345 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.907345 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.911345 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 18:53:45.899345 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 18:53:45.911345 frontrunner-sdk-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-04-25 18:53:45.000000 frontrunner-sdk-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/backend_shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.159138 frontrunner-sdk-0.1.1/frontrunner_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_light_client_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/clients/openapi_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/find_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_leagues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/cancel_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_account_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_order_books.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_trades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_markets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_orders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_positions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_trades.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/chained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/config/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/frontrunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/facades/injective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/streams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/ioc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_external_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/cancel_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/models/wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.159138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19663 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25184 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18121 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/frontrunner_sdk/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:21:50.163138 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-25 21:21:50.000000 frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 21:21:50.167138 frontrunner-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-25 21:21:49.000000 frontrunner-sdk-0.1.1/setup.py
```

### Comparing `frontrunner-sdk-0.1.0/backend_shim.py` & `frontrunner-sdk-0.1.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_chain.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_chain.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_faucet.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/clients/injective_light_client_daemon.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/injective_light_client_daemon.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/clients/openapi_client.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/clients/openapi_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/base.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/find_markets.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/find_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_leagues.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_leagues.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_markets.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_props.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_props.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sport_entities.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_entities.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sport_events.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sport_events.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/frontrunner/get_sports.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/frontrunner/get_sports.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/cancel_orders.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/cancel_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/create_orders.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/create_wallet.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/create_wallet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/fund_wallet_from_faucet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_account_portfolio.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_account_portfolio.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_order_books.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_order_books.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_orders.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_positions.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_positions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/get_trades.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/get_trades.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_markets.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_markets.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_orders.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_orders.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_positions.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_positions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/commands/injective/stream_trades.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/commands/injective/stream_trades.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/__init__.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/base.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/chained.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/chained.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/conditional.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/conditional.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/environment_variable.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/environment_variable.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/config/static.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/config/static.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/exceptions/__init__.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/facades/base.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/base.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/facades/frontrunner.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/frontrunner.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/facades/injective.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/facades/injective.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/paginators.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/paginators.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/streams.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/streams.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/helpers/validation.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/helpers/validation.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/ioc.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/ioc.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/logging/log_external_exceptions.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_external_exceptions.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/logging/log_operation.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/logging/log_operation.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/models/order.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/models/order.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/models/wallet.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/models/wallet.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/__init__.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api/frontrunner_api.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/api_client.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/api_client.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/configuration.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/configuration.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/error.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/error.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/league_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/market.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/market_status.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/prop_type.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_entity.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_id.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_name.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/models/sport_event_type.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/openapi/frontrunner_api/rest.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/openapi/frontrunner_api/rest.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk/sdk.py` & `frontrunner-sdk-0.1.1/frontrunner_sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `frontrunner-sdk-0.1.0/frontrunner_sdk.egg-info/SOURCES.txt` & `frontrunner-sdk-0.1.1/frontrunner_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

