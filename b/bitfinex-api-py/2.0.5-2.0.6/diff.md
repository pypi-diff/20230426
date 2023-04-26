# Comparing `tmp/bitfinex-api-py-2.0.5.tar.gz` & `tmp/bitfinex-api-py-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitfinex-api-py-2.0.5.tar", last modified: Fri Feb 17 18:14:54 2023, max compression
+gzip compressed data, was "dist/bitfinex-api-py-2.0.6.tar", last modified: Fri Feb 17 18:19:31 2023, max compression
```

## Comparing `bitfinex-api-py-2.0.5.tar` & `bitfinex-api-py-2.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      179 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.5/bfxapi/constants.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      513 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.5/bfxapi/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1051 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.5/bfxapi/client.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       90 2023-02-17 18:13:42.000000 bitfinex-api-py-2.0.5/bfxapi/version.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/utils/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      357 2022-01-03 10:40:35.000000 bitfinex-api-py-2.0.5/bfxapi/utils/decorators.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2866 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/utils/testing_tools.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1375 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/utils/decimal.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       15 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/utils/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1673 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/utils/auth.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3028 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/utils/custom_logger.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/models/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3168 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/funding_offer.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1231 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/deposit_address.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3434 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/funding_loan.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3856 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/order_book.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      805 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.5/bfxapi/models/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1645 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/funding_trade.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2714 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/subscription.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1601 2023-02-17 18:13:42.000000 bitfinex-api-py-2.0.5/bfxapi/models/withdraw.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4180 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/position.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1422 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/margin_info.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1612 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/margin_info_base.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4445 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/notification.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2516 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.5/bfxapi/models/movement.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3351 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/funding_ticker.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1781 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/transfer.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3851 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/funding_credit.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1586 2022-10-19 15:01:18.000000 bitfinex-api-py-2.0.5/bfxapi/models/ledger.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2294 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/ticker.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     7449 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/order.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1006 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/wallet.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2540 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/models/trade.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     6705 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/generic_websocket.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       20 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      870 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/wallet_manager.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    31737 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/bfx_websocket.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    12433 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/order_manager.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     7604 2022-01-04 19:41:31.000000 bitfinex-api-py-2.0.5/bfxapi/websockets/subscription_manager.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/tests/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1330 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_rest_get_public_trades.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        0 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     5582 2021-12-20 10:21:11.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_subscriptions.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     9981 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_orders.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)      728 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_decimal.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     4960 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_orderbook.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1776 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_capacity.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     3468 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/tests/helpers.py
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bfxapi/rest/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       14 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/bfxapi/rest/__init__.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)    56997 2022-10-04 14:32:18.000000 bitfinex-api-py-2.0.5/bfxapi/rest/bfx_rest.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     2120 2023-02-17 18:13:42.000000 bitfinex-api-py-2.0.5/setup.py
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       38 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/setup.cfg
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/PKG-INFO
-drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/PKG-INFO
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        7 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/top_level.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)        1 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/dependency_links.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)       54 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/requires.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     1554 2023-02-17 18:14:54.000000 bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/SOURCES.txt
--rw-rw-r--   0 vigan     (1000) vigan     (1000)     6447 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.5/README.md
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      179 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/constants.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      513 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1051 2022-08-27 18:59:36.000000 bitfinex-api-py-2.0.6/bfxapi/client.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       90 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/bfxapi/version.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/utils/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      357 2022-01-03 10:40:35.000000 bitfinex-api-py-2.0.6/bfxapi/utils/decorators.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2866 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/testing_tools.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1375 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/decimal.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       15 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1673 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/auth.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3028 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/utils/custom_logger.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/models/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3168 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_offer.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1231 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/deposit_address.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3434 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_loan.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3856 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/order_book.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      805 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/models/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1645 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_trade.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2714 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/subscription.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1601 2023-02-17 18:13:42.000000 bitfinex-api-py-2.0.6/bfxapi/models/withdraw.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4180 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/position.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1422 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/margin_info.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1612 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/margin_info_base.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4445 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/notification.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2516 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/models/movement.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3351 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_ticker.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1781 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/transfer.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3851 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/funding_credit.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1586 2022-10-19 15:01:18.000000 bitfinex-api-py-2.0.6/bfxapi/models/ledger.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2294 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/ticker.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     7449 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/order.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1006 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/wallet.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2540 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/models/trade.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     6705 2022-01-21 16:47:11.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/generic_websocket.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       20 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      870 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/wallet_manager.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    31761 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/bfx_websocket.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    12433 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/order_manager.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     7604 2022-01-04 19:41:31.000000 bitfinex-api-py-2.0.6/bfxapi/websockets/subscription_manager.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/tests/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1330 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_rest_get_public_trades.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)        0 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     5582 2021-12-20 10:21:11.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_subscriptions.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     9981 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orders.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)      728 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_decimal.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     4960 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orderbook.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1776 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_capacity.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     3468 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/tests/helpers.py
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bfxapi/rest/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       14 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/bfxapi/rest/__init__.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)    56997 2022-10-04 14:32:18.000000 bitfinex-api-py-2.0.6/bfxapi/rest/bfx_rest.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     2120 2023-02-17 18:18:25.000000 bitfinex-api-py-2.0.6/setup.py
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       38 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/setup.cfg
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/PKG-INFO
+drwxrwxr-x   0 vigan     (1000) vigan     (1000)        0 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1267 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/PKG-INFO
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)        7 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/top_level.txt
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)        1 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)       54 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/requires.txt
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     1554 2023-02-17 18:19:31.000000 bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 vigan     (1000) vigan     (1000)     6447 2021-11-05 15:22:50.000000 bitfinex-api-py-2.0.6/README.md
```

### Comparing `bitfinex-api-py-2.0.5/bfxapi/__init__.py` & `bitfinex-api-py-2.0.6/bfxapi/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/client.py` & `bitfinex-api-py-2.0.6/bfxapi/client.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/utils/testing_tools.py` & `bitfinex-api-py-2.0.6/bfxapi/utils/testing_tools.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/utils/decimal.py` & `bitfinex-api-py-2.0.6/bfxapi/utils/decimal.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/utils/auth.py` & `bitfinex-api-py-2.0.6/bfxapi/utils/auth.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/utils/custom_logger.py` & `bitfinex-api-py-2.0.6/bfxapi/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/funding_offer.py` & `bitfinex-api-py-2.0.6/bfxapi/models/funding_offer.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/deposit_address.py` & `bitfinex-api-py-2.0.6/bfxapi/models/deposit_address.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/funding_loan.py` & `bitfinex-api-py-2.0.6/bfxapi/models/funding_loan.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/order_book.py` & `bitfinex-api-py-2.0.6/bfxapi/models/order_book.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/__init__.py` & `bitfinex-api-py-2.0.6/bfxapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/funding_trade.py` & `bitfinex-api-py-2.0.6/bfxapi/models/funding_trade.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/subscription.py` & `bitfinex-api-py-2.0.6/bfxapi/models/subscription.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/withdraw.py` & `bitfinex-api-py-2.0.6/bfxapi/models/withdraw.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/position.py` & `bitfinex-api-py-2.0.6/bfxapi/models/position.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/margin_info.py` & `bitfinex-api-py-2.0.6/bfxapi/models/margin_info.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/margin_info_base.py` & `bitfinex-api-py-2.0.6/bfxapi/models/margin_info_base.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/notification.py` & `bitfinex-api-py-2.0.6/bfxapi/models/notification.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/movement.py` & `bitfinex-api-py-2.0.6/bfxapi/models/movement.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/funding_ticker.py` & `bitfinex-api-py-2.0.6/bfxapi/models/funding_ticker.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/transfer.py` & `bitfinex-api-py-2.0.6/bfxapi/models/transfer.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/funding_credit.py` & `bitfinex-api-py-2.0.6/bfxapi/models/funding_credit.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/ledger.py` & `bitfinex-api-py-2.0.6/bfxapi/models/ledger.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/ticker.py` & `bitfinex-api-py-2.0.6/bfxapi/models/ticker.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/order.py` & `bitfinex-api-py-2.0.6/bfxapi/models/order.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/wallet.py` & `bitfinex-api-py-2.0.6/bfxapi/models/wallet.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/models/trade.py` & `bitfinex-api-py-2.0.6/bfxapi/models/trade.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/websockets/generic_websocket.py` & `bitfinex-api-py-2.0.6/bfxapi/websockets/generic_websocket.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/websockets/wallet_manager.py` & `bitfinex-api-py-2.0.6/bfxapi/websockets/wallet_manager.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/websockets/bfx_websocket.py` & `bitfinex-api-py-2.0.6/bfxapi/websockets/bfx_websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         'amount': tData[5],
         'symbol': symbol
     }
 
 
 def _parse_trade(tData, symbol):
     return {
+        'id': tData[0],
         'mts': tData[1],
         'price': tData[3],
         'amount': tData[2],
         'symbol': symbol
     }
```

### Comparing `bitfinex-api-py-2.0.5/bfxapi/websockets/order_manager.py` & `bitfinex-api-py-2.0.6/bfxapi/websockets/order_manager.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/websockets/subscription_manager.py` & `bitfinex-api-py-2.0.6/bfxapi/websockets/subscription_manager.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_rest_get_public_trades.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_rest_get_public_trades.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_subscriptions.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_subscriptions.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_orders.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orders.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_decimal.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_decimal.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_orderbook.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_orderbook.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/test_ws_capacity.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/test_ws_capacity.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/tests/helpers.py` & `bitfinex-api-py-2.0.6/bfxapi/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/bfxapi/rest/bfx_rest.py` & `bitfinex-api-py-2.0.6/bfxapi/rest/bfx_rest.py`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/setup.py` & `bitfinex-api-py-2.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 setup(
     name='bitfinex-api-py',
-    version='2.0.5',
+    version='2.0.6',
     description='Official Bitfinex Python API',
     long_description='A Python reference implementation of the Bitfinex API for both REST and websocket interaction',
     long_description_content_type='text/markdown',
     url='https://github.com/bitfinexcom/bitfinex-api-py',
     author='Bitfinex',
     author_email='support@bitfinex.com',
     classifiers=[
```

### Comparing `bitfinex-api-py-2.0.5/PKG-INFO` & `bitfinex-api-py-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitfinex-api-py
-Version: 2.0.5
+Version: 2.0.6
 Summary: Official Bitfinex Python API
 Home-page: https://github.com/bitfinexcom/bitfinex-api-py
 Author: Bitfinex
 Author-email: support@bitfinex.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/bitfinexcom/bitfinex-api-py
 Project-URL: Bug Reports, https://github.com/bitfinexcom/bitfinex-api-py/issues
```

### Comparing `bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/PKG-INFO` & `bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitfinex-api-py
-Version: 2.0.5
+Version: 2.0.6
 Summary: Official Bitfinex Python API
 Home-page: https://github.com/bitfinexcom/bitfinex-api-py
 Author: Bitfinex
 Author-email: support@bitfinex.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/bitfinexcom/bitfinex-api-py
 Project-URL: Bug Reports, https://github.com/bitfinexcom/bitfinex-api-py/issues
```

### Comparing `bitfinex-api-py-2.0.5/bitfinex_api_py.egg-info/SOURCES.txt` & `bitfinex-api-py-2.0.6/bitfinex_api_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitfinex-api-py-2.0.5/README.md` & `bitfinex-api-py-2.0.6/README.md`

 * *Files identical despite different names*

