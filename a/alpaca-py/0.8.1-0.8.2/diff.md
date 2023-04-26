# Comparing `tmp/alpaca_py-0.8.1.tar.gz` & `tmp/alpaca_py-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_py-0.8.1.tar", max compression
+gzip compressed data, was "alpaca_py-0.8.2.tar", max compression
```

## Comparing `alpaca_py-0.8.1.tar` & `alpaca_py-0.8.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    10872 2023-03-20 15:12:59.606686 alpaca_py-0.8.1/LICENSE
--rw-r--r--   0        0        0     9810 2023-04-03 17:13:32.842661 alpaca_py-0.8.1/README.md
--rw-r--r--   0        0        0       22 2023-04-11 19:35:09.619996 alpaca_py-0.8.1/alpaca/__init__.py
--rw-r--r--   0        0        0      100 2023-03-20 15:12:59.607787 alpaca_py-0.8.1/alpaca/broker/__init__.py
--rw-r--r--   0        0        0    64825 2023-04-11 19:21:35.937449 alpaca_py-0.8.1/alpaca/broker/client.py
--rw-r--r--   0        0        0    11012 2023-03-20 15:12:59.608585 alpaca_py-0.8.1/alpaca/broker/enums.py
--rw-r--r--   0        0        0      138 2023-03-20 15:12:59.608839 alpaca_py-0.8.1/alpaca/broker/models/__init__.py
--rw-r--r--   0        0        0    13998 2023-04-03 17:13:32.844395 alpaca_py-0.8.1/alpaca/broker/models/accounts.py
--rw-r--r--   0        0        0    14499 2023-03-20 15:12:59.609458 alpaca_py-0.8.1/alpaca/broker/models/cip.py
--rw-r--r--   0        0        0     6266 2023-03-20 15:12:59.609667 alpaca_py-0.8.1/alpaca/broker/models/documents.py
--rw-r--r--   0        0        0     4372 2023-03-20 15:12:59.609845 alpaca_py-0.8.1/alpaca/broker/models/funding.py
--rw-r--r--   0        0        0     3216 2023-04-03 17:13:32.845068 alpaca_py-0.8.1/alpaca/broker/models/journals.py
--rw-r--r--   0        0        0      305 2023-03-20 15:12:59.610382 alpaca_py-0.8.1/alpaca/broker/models/trading.py
--rw-r--r--   0        0        0    43935 2023-04-03 17:13:32.846078 alpaca_py-0.8.1/alpaca/broker/requests.py
--rw-r--r--   0        0        0      136 2023-03-20 15:12:59.610982 alpaca_py-0.8.1/alpaca/common/__init__.py
--rw-r--r--   0        0        0      347 2023-03-20 15:12:59.611141 alpaca_py-0.8.1/alpaca/common/constants.py
--rw-r--r--   0        0        0     1705 2023-04-03 17:13:32.846674 alpaca_py-0.8.1/alpaca/common/enums.py
--rw-r--r--   0        0        0      987 2023-03-20 15:12:59.611559 alpaca_py-0.8.1/alpaca/common/exceptions.py
--rw-r--r--   0        0        0      403 2023-03-20 15:12:59.611781 alpaca_py-0.8.1/alpaca/common/models.py
--rw-r--r--   0        0        0     1991 2023-03-20 15:12:59.612115 alpaca_py-0.8.1/alpaca/common/requests.py
--rw-r--r--   0        0        0    13960 2023-04-11 19:21:35.938278 alpaca_py-0.8.1/alpaca/common/rest.py
--rw-r--r--   0        0        0      173 2023-03-20 15:12:59.612704 alpaca_py-0.8.1/alpaca/common/types.py
--rw-r--r--   0        0        0     1916 2023-03-20 15:12:59.612900 alpaca_py-0.8.1/alpaca/common/utils.py
--rw-r--r--   0        0        0    17332 2023-03-20 15:12:59.613119 alpaca_py-0.8.1/alpaca/common/websocket.py
--rw-r--r--   0        0        0      118 2023-03-20 15:12:59.613409 alpaca_py-0.8.1/alpaca/data/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-03 14:46:59.759940 alpaca_py-0.8.1/alpaca/data/enums.py
--rw-r--r--   0        0        0       92 2023-03-20 15:12:59.613798 alpaca_py-0.8.1/alpaca/data/historical/__init__.py
--rw-r--r--   0        0        0    14142 2023-04-03 14:46:59.761182 alpaca_py-0.8.1/alpaca/data/historical/crypto.py
--rw-r--r--   0        0        0    12392 2023-03-20 15:12:59.614199 alpaca_py-0.8.1/alpaca/data/historical/stock.py
--rw-r--r--   0        0        0     4474 2023-03-20 15:12:59.614356 alpaca_py-0.8.1/alpaca/data/historical/utils.py
--rw-r--r--   0        0        0       72 2023-03-20 15:12:59.614560 alpaca_py-0.8.1/alpaca/data/live/__init__.py
--rw-r--r--   0        0        0     1602 2023-04-03 17:13:34.312258 alpaca_py-0.8.1/alpaca/data/live/crypto.py
--rw-r--r--   0        0        0     1935 2023-03-20 15:12:59.614841 alpaca_py-0.8.1/alpaca/data/live/stock.py
--rw-r--r--   0        0        0     1012 2023-03-20 15:12:59.614987 alpaca_py-0.8.1/alpaca/data/mappings.py
--rw-r--r--   0        0        0      115 2023-03-20 15:12:59.615222 alpaca_py-0.8.1/alpaca/data/models/__init__.py
--rw-r--r--   0        0        0     2304 2023-03-20 15:12:59.615411 alpaca_py-0.8.1/alpaca/data/models/bars.py
--rw-r--r--   0        0        0     1752 2023-03-20 15:12:59.615552 alpaca_py-0.8.1/alpaca/data/models/base.py
--rw-r--r--   0        0        0     1643 2023-03-20 15:12:59.615704 alpaca_py-0.8.1/alpaca/data/models/orderbooks.py
--rw-r--r--   0        0        0     2581 2023-03-20 15:12:59.615907 alpaca_py-0.8.1/alpaca/data/models/quotes.py
--rw-r--r--   0        0        0     1979 2023-03-20 15:12:59.616060 alpaca_py-0.8.1/alpaca/data/models/snapshots.py
--rw-r--r--   0        0        0     2318 2023-03-20 15:12:59.616284 alpaca_py-0.8.1/alpaca/data/models/trades.py
--rw-r--r--   0        0        0    12288 2023-04-03 17:13:32.848638 alpaca_py-0.8.1/alpaca/data/requests.py
--rw-r--r--   0        0        0     4303 2023-03-20 15:12:59.616739 alpaca_py-0.8.1/alpaca/data/timeframe.py
--rw-r--r--   0        0        0        0 2023-03-20 15:12:59.616869 alpaca_py-0.8.1/alpaca/py.typed
--rw-r--r--   0        0        0       89 2023-03-20 15:12:59.617081 alpaca_py-0.8.1/alpaca/trading/__init__.py
--rw-r--r--   0        0        0    21010 2023-03-20 15:12:59.617276 alpaca_py-0.8.1/alpaca/trading/client.py
--rw-r--r--   0        0        0     7758 2023-03-20 15:12:59.617427 alpaca_py-0.8.1/alpaca/trading/enums.py
--rw-r--r--   0        0        0    25517 2023-04-11 19:30:55.555410 alpaca_py-0.8.1/alpaca/trading/models.py
--rw-r--r--   0        0        0    19232 2023-03-20 15:12:59.617974 alpaca_py-0.8.1/alpaca/trading/requests.py
--rw-r--r--   0        0        0     7505 2023-03-20 15:12:59.618140 alpaca_py-0.8.1/alpaca/trading/stream.py
--rw-r--r--   0        0        0      915 2023-04-11 19:35:09.620743 alpaca_py-0.8.1/pyproject.toml
--rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 alpaca_py-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    10872 2023-03-20 15:12:59.606686 alpaca_py-0.8.2/LICENSE
+-rw-r--r--   0        0        0     9810 2023-04-03 17:13:32.842661 alpaca_py-0.8.2/README.md
+-rw-r--r--   0        0        0       22 2023-04-26 13:55:31.165406 alpaca_py-0.8.2/alpaca/__init__.py
+-rw-r--r--   0        0        0      100 2023-03-20 15:12:59.607787 alpaca_py-0.8.2/alpaca/broker/__init__.py
+-rw-r--r--   0        0        0    64825 2023-04-11 19:21:35.937449 alpaca_py-0.8.2/alpaca/broker/client.py
+-rw-r--r--   0        0        0    11012 2023-03-20 15:12:59.608585 alpaca_py-0.8.2/alpaca/broker/enums.py
+-rw-r--r--   0        0        0      138 2023-03-20 15:12:59.608839 alpaca_py-0.8.2/alpaca/broker/models/__init__.py
+-rw-r--r--   0        0        0    13998 2023-04-03 17:13:32.844395 alpaca_py-0.8.2/alpaca/broker/models/accounts.py
+-rw-r--r--   0        0        0    14499 2023-03-20 15:12:59.609458 alpaca_py-0.8.2/alpaca/broker/models/cip.py
+-rw-r--r--   0        0        0     6266 2023-03-20 15:12:59.609667 alpaca_py-0.8.2/alpaca/broker/models/documents.py
+-rw-r--r--   0        0        0     4372 2023-03-20 15:12:59.609845 alpaca_py-0.8.2/alpaca/broker/models/funding.py
+-rw-r--r--   0        0        0     3216 2023-04-03 17:13:32.845068 alpaca_py-0.8.2/alpaca/broker/models/journals.py
+-rw-r--r--   0        0        0      305 2023-03-20 15:12:59.610382 alpaca_py-0.8.2/alpaca/broker/models/trading.py
+-rw-r--r--   0        0        0    43935 2023-04-03 17:13:32.846078 alpaca_py-0.8.2/alpaca/broker/requests.py
+-rw-r--r--   0        0        0      136 2023-03-20 15:12:59.610982 alpaca_py-0.8.2/alpaca/common/__init__.py
+-rw-r--r--   0        0        0      347 2023-03-20 15:12:59.611141 alpaca_py-0.8.2/alpaca/common/constants.py
+-rw-r--r--   0        0        0     1705 2023-04-03 17:13:32.846674 alpaca_py-0.8.2/alpaca/common/enums.py
+-rw-r--r--   0        0        0      987 2023-03-20 15:12:59.611559 alpaca_py-0.8.2/alpaca/common/exceptions.py
+-rw-r--r--   0        0        0      403 2023-03-20 15:12:59.611781 alpaca_py-0.8.2/alpaca/common/models.py
+-rw-r--r--   0        0        0     1991 2023-03-20 15:12:59.612115 alpaca_py-0.8.2/alpaca/common/requests.py
+-rw-r--r--   0        0        0    13960 2023-04-11 19:21:35.938278 alpaca_py-0.8.2/alpaca/common/rest.py
+-rw-r--r--   0        0        0      173 2023-03-20 15:12:59.612704 alpaca_py-0.8.2/alpaca/common/types.py
+-rw-r--r--   0        0        0     1916 2023-03-20 15:12:59.612900 alpaca_py-0.8.2/alpaca/common/utils.py
+-rw-r--r--   0        0        0    17332 2023-03-20 15:12:59.613119 alpaca_py-0.8.2/alpaca/common/websocket.py
+-rw-r--r--   0        0        0      118 2023-03-20 15:12:59.613409 alpaca_py-0.8.2/alpaca/data/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-03 14:46:59.759940 alpaca_py-0.8.2/alpaca/data/enums.py
+-rw-r--r--   0        0        0       92 2023-03-20 15:12:59.613798 alpaca_py-0.8.2/alpaca/data/historical/__init__.py
+-rw-r--r--   0        0        0    14142 2023-04-03 14:46:59.761182 alpaca_py-0.8.2/alpaca/data/historical/crypto.py
+-rw-r--r--   0        0        0    12392 2023-03-20 15:12:59.614199 alpaca_py-0.8.2/alpaca/data/historical/stock.py
+-rw-r--r--   0        0        0     4474 2023-03-20 15:12:59.614356 alpaca_py-0.8.2/alpaca/data/historical/utils.py
+-rw-r--r--   0        0        0       72 2023-03-20 15:12:59.614560 alpaca_py-0.8.2/alpaca/data/live/__init__.py
+-rw-r--r--   0        0        0     1602 2023-04-03 17:13:34.312258 alpaca_py-0.8.2/alpaca/data/live/crypto.py
+-rw-r--r--   0        0        0     1935 2023-03-20 15:12:59.614841 alpaca_py-0.8.2/alpaca/data/live/stock.py
+-rw-r--r--   0        0        0     1012 2023-03-20 15:12:59.614987 alpaca_py-0.8.2/alpaca/data/mappings.py
+-rw-r--r--   0        0        0      115 2023-03-20 15:12:59.615222 alpaca_py-0.8.2/alpaca/data/models/__init__.py
+-rw-r--r--   0        0        0     2304 2023-03-20 15:12:59.615411 alpaca_py-0.8.2/alpaca/data/models/bars.py
+-rw-r--r--   0        0        0     1752 2023-03-20 15:12:59.615552 alpaca_py-0.8.2/alpaca/data/models/base.py
+-rw-r--r--   0        0        0     1643 2023-03-20 15:12:59.615704 alpaca_py-0.8.2/alpaca/data/models/orderbooks.py
+-rw-r--r--   0        0        0     2581 2023-03-20 15:12:59.615907 alpaca_py-0.8.2/alpaca/data/models/quotes.py
+-rw-r--r--   0        0        0     1979 2023-03-20 15:12:59.616060 alpaca_py-0.8.2/alpaca/data/models/snapshots.py
+-rw-r--r--   0        0        0     2318 2023-03-20 15:12:59.616284 alpaca_py-0.8.2/alpaca/data/models/trades.py
+-rw-r--r--   0        0        0    12288 2023-04-03 17:13:32.848638 alpaca_py-0.8.2/alpaca/data/requests.py
+-rw-r--r--   0        0        0     4303 2023-03-20 15:12:59.616739 alpaca_py-0.8.2/alpaca/data/timeframe.py
+-rw-r--r--   0        0        0        0 2023-03-20 15:12:59.616869 alpaca_py-0.8.2/alpaca/py.typed
+-rw-r--r--   0        0        0       89 2023-03-20 15:12:59.617081 alpaca_py-0.8.2/alpaca/trading/__init__.py
+-rw-r--r--   0        0        0    21010 2023-03-20 15:12:59.617276 alpaca_py-0.8.2/alpaca/trading/client.py
+-rw-r--r--   0        0        0     7780 2023-04-26 13:54:12.682339 alpaca_py-0.8.2/alpaca/trading/enums.py
+-rw-r--r--   0        0        0    25517 2023-04-11 19:30:55.555410 alpaca_py-0.8.2/alpaca/trading/models.py
+-rw-r--r--   0        0        0    19232 2023-03-20 15:12:59.617974 alpaca_py-0.8.2/alpaca/trading/requests.py
+-rw-r--r--   0        0        0     7505 2023-03-20 15:12:59.618140 alpaca_py-0.8.2/alpaca/trading/stream.py
+-rw-r--r--   0        0        0      915 2023-04-26 13:55:28.655204 alpaca_py-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    10816 1970-01-01 00:00:00.000000 alpaca_py-0.8.2/PKG-INFO
```

### Comparing `alpaca_py-0.8.1/LICENSE` & `alpaca_py-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/README.md` & `alpaca_py-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/client.py` & `alpaca_py-0.8.2/alpaca/broker/client.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/enums.py` & `alpaca_py-0.8.2/alpaca/broker/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/models/accounts.py` & `alpaca_py-0.8.2/alpaca/broker/models/accounts.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/models/cip.py` & `alpaca_py-0.8.2/alpaca/broker/models/cip.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/models/documents.py` & `alpaca_py-0.8.2/alpaca/broker/models/documents.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/models/funding.py` & `alpaca_py-0.8.2/alpaca/broker/models/funding.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/models/journals.py` & `alpaca_py-0.8.2/alpaca/broker/models/journals.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/broker/requests.py` & `alpaca_py-0.8.2/alpaca/broker/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/enums.py` & `alpaca_py-0.8.2/alpaca/common/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/exceptions.py` & `alpaca_py-0.8.2/alpaca/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/requests.py` & `alpaca_py-0.8.2/alpaca/common/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/rest.py` & `alpaca_py-0.8.2/alpaca/common/rest.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/utils.py` & `alpaca_py-0.8.2/alpaca/common/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/common/websocket.py` & `alpaca_py-0.8.2/alpaca/common/websocket.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/enums.py` & `alpaca_py-0.8.2/alpaca/data/enums.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/historical/crypto.py` & `alpaca_py-0.8.2/alpaca/data/historical/crypto.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/historical/stock.py` & `alpaca_py-0.8.2/alpaca/data/historical/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/historical/utils.py` & `alpaca_py-0.8.2/alpaca/data/historical/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/live/crypto.py` & `alpaca_py-0.8.2/alpaca/data/live/crypto.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/live/stock.py` & `alpaca_py-0.8.2/alpaca/data/live/stock.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/mappings.py` & `alpaca_py-0.8.2/alpaca/data/mappings.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/bars.py` & `alpaca_py-0.8.2/alpaca/data/models/bars.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/base.py` & `alpaca_py-0.8.2/alpaca/data/models/base.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/orderbooks.py` & `alpaca_py-0.8.2/alpaca/data/models/orderbooks.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/quotes.py` & `alpaca_py-0.8.2/alpaca/data/models/quotes.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/snapshots.py` & `alpaca_py-0.8.2/alpaca/data/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/models/trades.py` & `alpaca_py-0.8.2/alpaca/data/models/trades.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/requests.py` & `alpaca_py-0.8.2/alpaca/data/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/data/timeframe.py` & `alpaca_py-0.8.2/alpaca/data/timeframe.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/trading/client.py` & `alpaca_py-0.8.2/alpaca/trading/client.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/trading/enums.py` & `alpaca_py-0.8.2/alpaca/trading/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,14 +173,15 @@
     NASDAQ = "NASDAQ"
     NYSEARCA = "NYSEARCA"
     FTXU = "FTXU"
     CBSE = "CBSE"
     GNSS = "GNSS"
     ERSX = "ERSX"
     OTC = "OTC"
+    CRYPTO = "CRYPTO"
 
 
 class PositionSide(str, Enum):
     """
     Represents what side this position is.
     """
```

### Comparing `alpaca_py-0.8.1/alpaca/trading/models.py` & `alpaca_py-0.8.2/alpaca/trading/models.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/trading/requests.py` & `alpaca_py-0.8.2/alpaca/trading/requests.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/alpaca/trading/stream.py` & `alpaca_py-0.8.2/alpaca/trading/stream.py`

 * *Files identical despite different names*

### Comparing `alpaca_py-0.8.1/pyproject.toml` & `alpaca_py-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpaca-py"
-version = "0.8.1"
+version = "0.8.2"
 description = "The Official Python SDK for Alpaca APIs"
 authors = [
     "Rahul Chowdhury <rahul.chowdhury@alpaca.markets>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/alpacahq/alpaca-py"
```

### Comparing `alpaca_py-0.8.1/PKG-INFO` & `alpaca_py-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-py
-Version: 0.8.1
+Version: 0.8.2
 Summary: The Official Python SDK for Alpaca APIs
 Home-page: https://github.com/alpacahq/alpaca-py
 License: Apache-2.0
 Author: Rahul Chowdhury
 Author-email: rahul.chowdhury@alpaca.markets
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

