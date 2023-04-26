# Comparing `tmp/bitfinex-api-py-2.0.6.tar.gz` & `tmp/bitfinex-api-py-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitfinex-api-py-2.0.6.tar", last modified: Fri Feb 17 18:19:31 2023, max compression
+gzip compressed data, was "bitfinex-api-py-3.0.0b1.tar", last modified: Wed Apr 26 14:59:19 2023, max compression
```

## Comparing `bitfinex-api-py-2.0.6.tar` & `bitfinex-api-py-3.0.0b1.tar`

### file list

```diff
@@ -1,64 +1,48 @@
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      179 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/constants.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      513 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1051 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/client.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       90 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/bfxapi/version.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/utils/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      357 2022-01-03 10:40:35.000000 bitfinex-api-py-2.0.6/bfxapi/utils/decorators.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2866 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/testing_tools.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1375 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/decimal.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       15 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1673 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/auth.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3028 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/custom_logger.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/models/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3168 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_offer.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1231 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/deposit_address.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3434 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_loan.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3856 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/order_book.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      805 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/models/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1645 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_trade.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2714 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/subscription.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1601 2023-02-17 18:13:42.000000 bitfinex-api-py-2.0.6/bfxapi/models/withdraw.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4180 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/position.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1422 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/margin_info.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1612 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/margin_info_base.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4445 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/notification.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2516 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/models/movement.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3351 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_ticker.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1781 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/transfer.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3851 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_credit.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1586 2022-10-19 15:01:18.000000 bitfinex-api-py-2.0.6/bfxapi/models/ledger.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2294 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/ticker.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     7449 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/order.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1006 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/wallet.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2540 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/trade.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     6705 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/generic_websocket.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       20 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      870 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/wallet_manager.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    31761 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/bfx_websocket.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    12433 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/order_manager.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     7604 2022-01-04 19:41:31.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/subscription_manager.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/tests/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1330 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_rest_get_public_trades.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        0 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     5582 2021-12-20 10:21:11.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_subscriptions.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     9981 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orders.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      728 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_decimal.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4960 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orderbook.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1776 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_capacity.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3468 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/helpers.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/rest/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       14 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/rest/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    56997 2022-10-04 14:32:18.000000 bitfinex-api-py-2.0.6/bfxapi/rest/bfx_rest.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2120 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/setup.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       38 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/setup.cfg
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/PKG-INFO
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/PKG-INFO
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        7 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/top_level.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        1 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/dependency_links.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       54 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/requires.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1554 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/SOURCES.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     6447 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/README.md
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      743 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/PKG-INFO
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.544849 bitfinex-api-py-3.0.0b1/bfxapi/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      135 2023-04-26 14:44:30.524468 bitfinex-api-py-3.0.0b1/bfxapi/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      987 2023-04-26 14:44:30.524468 bitfinex-api-py-3.0.0b1/bfxapi/client.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1242 2023-04-26 14:44:30.524468 bitfinex-api-py-3.0.0b1/bfxapi/enums.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      397 2023-04-26 14:44:30.524468 bitfinex-api-py-3.0.0b1/bfxapi/exceptions.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3725 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/labeler.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1338 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/notification.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/rest/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      134 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/__init__.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      233 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      639 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/bfx_rest_interface.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    21520 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/rest_authenticated_endpoints.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     7310 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/rest_merchant_endpoints.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    13779 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/endpoints/rest_public_endpoints.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1675 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/enums.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      973 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/exceptions.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/rest/middleware/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       35 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/middleware/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3784 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/middleware/middleware.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    20285 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/serializers.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    13801 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/rest/types.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      183 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/urls.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/utils/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/utils/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      815 2023-04-26 14:44:30.528468 bitfinex-api-py-3.0.0b1/bfxapi/utils/camel_and_snake_case_helpers.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1061 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/utils/json_encoder.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1611 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/utils/logger.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       24 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/version.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/websocket/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       79 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/__init__.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/websocket/client/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      159 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/client/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4072 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/client/bfx_websocket_bucket.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    11573 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/client/bfx_websocket_client.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4152 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/client/bfx_websocket_inputs.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      219 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/enums.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1835 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/exceptions.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-04-26 14:59:19.548849 bitfinex-api-py-3.0.0b1/bfxapi/websocket/handlers/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      132 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/handlers/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3145 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/handlers/authenticated_channels_handler.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     5348 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/handlers/public_channels_handler.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     7391 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/serializers.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      766 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/subscriptions.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4398 2023-04-26 14:44:30.532468 bitfinex-api-py-3.0.0b1/bfxapi/websocket/types.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1539 2023-04-26 14:58:53.088582 bitfinex-api-py-3.0.0b1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitfinex-api-py-2.0.6/PKG-INFO` & `bitfinex-api-py-3.0.0b1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: bitfinex-api-py
-Version: 2.0.6
+Version: 3.0.0b1
 Summary: Official Bitfinex Python API
 Home-page: https://github.com/bitfinexcom/bitfinex-api-py
 Author: Bitfinex
 Author-email: support@bitfinex.com
-License: UNKNOWN
-Project-URL: Source, https://github.com/bitfinexcom/bitfinex-api-py
-Project-URL: Bug Reports, https://github.com/bitfinexcom/bitfinex-api-py/issues
+License: Apache-2.0
 Description: A Python reference implementation of the Bitfinex API for both REST and websocket interaction
 Keywords: bitfinex,api,trading
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.0
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.0.0, <4
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.10
```

