# Comparing `tmp/stock_market_bytetheory-1.0.0.tar.gz` & `tmp/stock_market_bytetheory-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stock_market_bytetheory-1.0.0.tar", last modified: Tue Apr 25 21:05:05 2023, max compression
+gzip compressed data, was "stock_market_bytetheory-1.0.1.tar", last modified: Tue Apr 25 22:42:13 2023, max compression
```

## Comparing `stock_market_bytetheory-1.0.0.tar` & `stock_market_bytetheory-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 21:05:05.588930 stock_market_bytetheory-1.0.0/
--rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.0/LICENSE
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-25 21:05:05.589008 stock_market_bytetheory-1.0.0/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.0/README.md
--rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.0/pyproject.toml
--rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-04-25 21:05:05.589267 stock_market_bytetheory-1.0.0/setup.cfg
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 21:05:05.578614 stock_market_bytetheory-1.0.0/src/
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 21:05:05.580452 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/
--rw-r--r--   0 robertblom   (501) staff       (20)     3944 2023-04-25 19:22:56.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/SP500History.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/SectorIndustryTickerParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)     2279 2023-04-25 19:20:58.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/TickerLevelDataParser.py
--rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 21:05:05.588837 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/
--rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/SP500_ind.csv
--rw-r--r--   0 robertblom   (501) staff       (20)    60623 2023-04-24 21:18:29.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/SP_500.xml
--rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/__init__.py
-drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 21:05:05.581113 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/
--rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-25 21:05:05.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/PKG-INFO
--rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-04-25 21:05:05.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/SOURCES.txt
--rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-04-25 21:05:05.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/dependency_links.txt
--rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-04-25 21:05:05.000000 stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/top_level.txt
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 22:42:13.707504 stock_market_bytetheory-1.0.1/
+-rw-r--r--   0 robertblom   (501) staff       (20)     1067 2023-03-31 18:16:25.000000 stock_market_bytetheory-1.0.1/LICENSE
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-25 22:42:13.707635 stock_market_bytetheory-1.0.1/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-03-31 22:41:33.000000 stock_market_bytetheory-1.0.1/README.md
+-rw-r--r--   0 robertblom   (501) staff       (20)       84 2023-03-31 18:46:07.000000 stock_market_bytetheory-1.0.1/pyproject.toml
+-rw-r--r--   0 robertblom   (501) staff       (20)      587 2023-04-25 22:42:13.707918 stock_market_bytetheory-1.0.1/setup.cfg
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 22:42:13.698514 stock_market_bytetheory-1.0.1/src/
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 22:42:13.700211 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/
+-rw-r--r--   0 robertblom   (501) staff       (20)     4243 2023-04-25 22:39:00.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/SP500History.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2169 2023-04-25 19:21:06.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/SectorIndustryTickerParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)     2279 2023-04-25 19:20:58.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/TickerLevelDataParser.py
+-rw-r--r--   0 robertblom   (501) staff       (20)      231 2023-04-25 19:59:08.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 22:42:13.707406 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/
+-rw-r--r--   0 robertblom   (501) staff       (20)  5204000 2023-03-31 20:35:29.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/SP500_ind.csv
+-rw-r--r--   0 robertblom   (501) staff       (20)    60623 2023-04-24 21:18:29.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/SP_500.xml
+-rw-r--r--   0 robertblom   (501) staff       (20)        0 2023-04-24 20:04:28.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/__init__.py
+drwxr-xr-x   0 robertblom   (501) staff       (20)        0 2023-04-25 22:42:13.700818 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/
+-rw-r--r--   0 robertblom   (501) staff       (20)      406 2023-04-25 22:42:13.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/PKG-INFO
+-rw-r--r--   0 robertblom   (501) staff       (20)      577 2023-04-25 22:42:13.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/SOURCES.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)        1 2023-04-25 22:42:13.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/dependency_links.txt
+-rw-r--r--   0 robertblom   (501) staff       (20)       24 2023-04-25 22:42:13.000000 stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/top_level.txt
```

### Comparing `stock_market_bytetheory-1.0.0/LICENSE` & `stock_market_bytetheory-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.0/setup.cfg` & `stock_market_bytetheory-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = stock_market_bytetheory
-version = 1.0.0
+version = 1.0.1
 author = Robbie Blom
 description = Provides some sample stock data and helpers for supporting a stock samples app
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
```

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/SP500History.py` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/SP500History.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,20 @@
         self.sectorIndustryTickerHierarchy = SectorIndustryTickerParser('SP_500.xml').parse()
         self.tickerLevelData = TickerLevelDataParser('SP500_ind.csv').parse()
 
     def getTickersForIndustry(self, industry, sector):
         tickers = self.sectorIndustryTickerHierarchy[sector][industry]
         return tickers
 
+    def getAllSectorsAndIndustries(self):
+        return {sector: self.getIndustriesForSector(sector) for sector in self.sectorIndustryTickerHierarchy.keys()}
+
+    def getIndustriesForSector(self, sector):
+        return [industry for industry in self.sectorIndustryTickerHierarchy[sector].keys()]
+
     def getVolumeWeightedAveragePrice(self, ticker):
         # Return the volume weighted average price of the stock.  In order to do this,
         # first find the average price of the stock on each day.  Then, multiply that price with the
         # volume on that day.  Take the sum of these values. Finally, divide that value by the sum of all the volumes.
         # (note: average price for each day = (high + low + close)/3)
 
         sumOfWeightedDailyPrices = 0
```

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/SectorIndustryTickerParser.py` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/SectorIndustryTickerParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/TickerLevelDataParser.py` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/TickerLevelDataParser.py`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/SP500_ind.csv` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/SP500_ind.csv`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory/data/SP_500.xml` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory/data/SP_500.xml`

 * *Files identical despite different names*

### Comparing `stock_market_bytetheory-1.0.0/src/stock_market_bytetheory.egg-info/SOURCES.txt` & `stock_market_bytetheory-1.0.1/src/stock_market_bytetheory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

