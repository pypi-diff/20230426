# Comparing `tmp/adata-0.0.4b0.tar.gz` & `tmp/adata-0.0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adata-0.0.4b0.tar", last modified: Thu Apr 20 16:20:11 2023, max compression
+gzip compressed data, was "adata-0.0.5b0.tar", last modified: Tue Apr 25 16:03:22 2023, max compression
```

## Comparing `adata-0.0.4b0.tar` & `adata-0.0.5b0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.120330 adata-0.0.4b0/
--rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.4b0/HISTORY.md
--rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.4b0/LICENSE
--rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.4b0/MANIFEST.in
--rw-rw-rw-   0        0        0     6780 2023-04-20 16:20:11.120330 adata-0.0.4b0/PKG-INFO
--rw-rw-rw-   0        0        0     6141 2023-04-18 15:14:02.000000 adata-0.0.4b0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.070330 adata-0.0.4b0/adata/
--rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.4b0/adata/__init__.py
--rw-rw-rw-   0        0        0      756 2023-04-20 16:19:38.000000 adata-0.0.4b0/adata/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata/bond/
--rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/bond/__init__.py
--rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.4b0/adata/bond/bond_market.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata/common/
--rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.4b0/adata/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.090330 adata-0.0.4b0/adata/common/headers/
--rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/common/headers/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.4b0/adata/common/headers/baidu_headers.py
--rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.4b0/adata/common/headers/sina_headers.py
--rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/common/headers/ths_headers.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.090330 adata-0.0.4b0/adata/common/utils/
--rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.4b0/adata/common/utils/__init__.py
--rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.4b0/adata/common/utils/snowflake.py
--rw-rw-rw-   0        0        0      972 2023-04-19 14:58:23.000000 adata-0.0.4b0/adata/common/utils/sunrequests.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/etf/
--rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/etf/__init__.py
--rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.4b0/adata/etf/etf_market.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/message/
--rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.4b0/adata/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/stock/
--rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.100330 adata-0.0.4b0/adata/stock/index/
--rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.110330 adata-0.0.4b0/adata/stock/info/
--rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.4b0/adata/stock/info/__init__.py
--rw-rw-rw-   0        0        0     2524 2023-04-19 14:07:29.000000 adata-0.0.4b0/adata/stock/info/stock_code.py
--rw-rw-rw-   0        0        0     4193 2023-04-19 14:07:29.000000 adata-0.0.4b0/adata/stock/info/stock_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.110330 adata-0.0.4b0/adata/stock/market/
--rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.4b0/adata/stock/market/__init__.py
--rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.4b0/adata/stock/market/stock_dividend.py
--rw-rw-rw-   0        0        0    10288 2023-04-20 13:12:32.000000 adata-0.0.4b0/adata/stock/market/stock_market.py
--rw-rw-rw-   0        0        0     5740 2023-04-19 15:24:26.000000 adata-0.0.4b0/adata/stock/market/stock_market_concept.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.120330 adata-0.0.4b0/adata/stock/sentiment/
--rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.4b0/adata/stock/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 16:20:11.080331 adata-0.0.4b0/adata.egg-info/
--rw-rw-rw-   0        0        0     6780 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      964 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 16:20:10.000000 adata-0.0.4b0/adata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.4b0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 16:20:11.120330 adata-0.0.4b0/setup.cfg
--rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.4b0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.391923 adata-0.0.5b0/
+-rw-rw-rw-   0        0        0      186 2023-04-06 11:14:06.000000 adata-0.0.5b0/HISTORY.md
+-rw-rw-rw-   0        0        0    11558 2023-04-05 02:53:34.000000 adata-0.0.5b0/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-04-06 11:14:06.000000 adata-0.0.5b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7151 2023-04-25 16:03:22.391923 adata-0.0.5b0/PKG-INFO
+-rw-rw-rw-   0        0        0     6512 2023-04-25 16:01:44.000000 adata-0.0.5b0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.272569 adata-0.0.5b0/adata/
+-rw-rw-rw-   0        0        0      545 2023-04-05 04:59:22.000000 adata-0.0.5b0/adata/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-04-25 16:02:04.000000 adata-0.0.5b0/adata/__version__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.285255 adata-0.0.5b0/adata/bond/
+-rw-rw-rw-   0        0        0      122 2023-04-06 11:14:06.000000 adata-0.0.5b0/adata/bond/__init__.py
+-rw-rw-rw-   0        0        0      203 2023-04-05 09:48:31.000000 adata-0.0.5b0/adata/bond/bond_market.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.286265 adata-0.0.5b0/adata/common/
+-rw-rw-rw-   0        0        0      150 2023-04-05 09:48:31.000000 adata-0.0.5b0/adata/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.346919 adata-0.0.5b0/adata/common/headers/
+-rw-rw-rw-   0        0        0      104 2023-04-05 09:48:30.000000 adata-0.0.5b0/adata/common/headers/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-05 09:48:28.000000 adata-0.0.5b0/adata/common/headers/baidu_headers.py
+-rw-rw-rw-   0        0        0      602 2023-04-18 15:14:02.000000 adata-0.0.5b0/adata/common/headers/sina_headers.py
+-rw-rw-rw-   0        0        0     2999 2023-04-05 09:48:30.000000 adata-0.0.5b0/adata/common/headers/ths_headers.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.355955 adata-0.0.5b0/adata/common/utils/
+-rw-rw-rw-   0        0        0      205 2023-04-05 09:53:12.000000 adata-0.0.5b0/adata/common/utils/__init__.py
+-rw-rw-rw-   0        0        0     3046 2023-04-05 09:48:27.000000 adata-0.0.5b0/adata/common/utils/snowflake.py
+-rw-rw-rw-   0        0        0      979 2023-04-24 16:42:55.000000 adata-0.0.5b0/adata/common/utils/sunrequests.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.359972 adata-0.0.5b0/adata/etf/
+-rw-rw-rw-   0        0        0      118 2023-04-06 11:14:06.000000 adata-0.0.5b0/adata/etf/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-04-05 09:48:28.000000 adata-0.0.5b0/adata/etf/etf_market.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.361947 adata-0.0.5b0/adata/message/
+-rw-rw-rw-   0        0        0      103 2023-04-05 09:48:30.000000 adata-0.0.5b0/adata/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.363948 adata-0.0.5b0/adata/stock/
+-rw-rw-rw-   0        0        0      333 2023-04-06 11:14:06.000000 adata-0.0.5b0/adata/stock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.364947 adata-0.0.5b0/adata/stock/index/
+-rw-rw-rw-   0        0        0      105 2023-04-06 11:14:06.000000 adata-0.0.5b0/adata/stock/index/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.369953 adata-0.0.5b0/adata/stock/info/
+-rw-rw-rw-   0        0        0      322 2023-04-13 14:47:15.000000 adata-0.0.5b0/adata/stock/info/__init__.py
+-rw-rw-rw-   0        0        0     2550 2023-04-25 15:29:33.000000 adata-0.0.5b0/adata/stock/info/stock_code.py
+-rw-rw-rw-   0        0        0     4049 2023-04-25 15:38:23.000000 adata-0.0.5b0/adata/stock/info/stock_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.386957 adata-0.0.5b0/adata/stock/market/
+-rw-rw-rw-   0        0        0      408 2023-04-13 14:47:15.000000 adata-0.0.5b0/adata/stock/market/__init__.py
+-rw-rw-rw-   0        0        0     2941 2023-04-20 13:03:47.000000 adata-0.0.5b0/adata/stock/market/stock_dividend.py
+-rw-rw-rw-   0        0        0    10485 2023-04-25 15:43:53.000000 adata-0.0.5b0/adata/stock/market/stock_market.py
+-rw-rw-rw-   0        0        0     8363 2023-04-25 15:49:26.000000 adata-0.0.5b0/adata/stock/market/stock_market_concept.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.388954 adata-0.0.5b0/adata/stock/sentiment/
+-rw-rw-rw-   0        0        0      115 2023-04-06 11:14:06.000000 adata-0.0.5b0/adata/stock/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 16:03:22.281559 adata-0.0.5b0/adata.egg-info/
+-rw-rw-rw-   0        0        0     7151 2023-04-25 16:03:21.000000 adata-0.0.5b0/adata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-04-25 16:03:21.000000 adata-0.0.5b0/adata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 16:03:21.000000 adata-0.0.5b0/adata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-25 16:03:21.000000 adata-0.0.5b0/adata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-25 16:03:21.000000 adata-0.0.5b0/adata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-04-06 11:14:06.000000 adata-0.0.5b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 16:03:22.392948 adata-0.0.5b0/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2023-04-18 15:37:51.000000 adata-0.0.5b0/setup.py
```

### Comparing `adata-0.0.4b0/LICENSE` & `adata-0.0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/PKG-INFO` & `adata-0.0.5b0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -82,29 +82,31 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据     | API                               | 说明                                | 备注                 |
-| -------- | --------------------------------- | ----------------------------------- | -------------------- |
-| A股代码  | stock.info.all_code()             | 所有A股代码信息                     |                      |
-| 概念代码 | stock.info.all_concept_code_ths() | 所有A股概念代码信息（同花顺）pc+app | 来源：同花顺公开数据 |
-|          | stock.info.concept_code_ths_pc()  | A股概念代码信息（同花顺）pc         | 来源：同花顺数据中心 |
-|          | stock.info.concept_code_ths_app() | A股概念代码信息（同花顺）app        | 来源：问财           |
+| 数据         | API                                  | 说明                             | 备注                 |
+| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
 
 #### 	2. 行情信息
 
-| 数据     | API                                  | 说明                                  | 备注                   |
-| -------- | ------------------------------------ | ------------------------------------- | ---------------------- |
-| 分红信息 | stock.maket.get_dividend()           | 获取单只股票的分红信息                |                        |
-| 股票行情 | stock.market.get_market()            | 获取单只股票的行情信息-日、周、月 k线 |                        |
-| 概念行情 | stock.maket.get_market_concept_ths() | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
-|          |                                      |                                       |                        |
+| 数据     | API                                         | 说明                                  | 备注                   |
+| -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
+| 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
+| 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
+|          | stock.market.get_market_min()               | 获取单个股票的今日分时行情            | 只能获取当天           |
+|          | stock.market.list_market_current()          | 获取多个股票最新行情信息              | 实时行情               |
+| 概念行情 | stock.maket.get_market_concept_ths()        | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
+|          | stock.market.get_market_concept_min_ths()   | 获取同花顺概念行情当日分时            | 只能获取当天           |
+|          | stock.market.get_market_concept_today_ths() | 获取同花顺当前的概念行情              | 实时行情               |
 
 ### （2）ETF
 
 | 项目          | 进度         | 说明                           |
 | ------------- | ------------ | ------------------------------ |
 | 场内可交易etf | 排期中...... | 若您有相关资源可以一起参与贡献 |
```

### Comparing `adata-0.0.4b0/README.md` & `adata-0.0.5b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -64,29 +64,31 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据     | API                               | 说明                                | 备注                 |
-| -------- | --------------------------------- | ----------------------------------- | -------------------- |
-| A股代码  | stock.info.all_code()             | 所有A股代码信息                     |                      |
-| 概念代码 | stock.info.all_concept_code_ths() | 所有A股概念代码信息（同花顺）pc+app | 来源：同花顺公开数据 |
-|          | stock.info.concept_code_ths_pc()  | A股概念代码信息（同花顺）pc         | 来源：同花顺数据中心 |
-|          | stock.info.concept_code_ths_app() | A股概念代码信息（同花顺）app        | 来源：问财           |
+| 数据         | API                                  | 说明                             | 备注                 |
+| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
 
 #### 	2. 行情信息
 
-| 数据     | API                                  | 说明                                  | 备注                   |
-| -------- | ------------------------------------ | ------------------------------------- | ---------------------- |
-| 分红信息 | stock.maket.get_dividend()           | 获取单只股票的分红信息                |                        |
-| 股票行情 | stock.market.get_market()            | 获取单只股票的行情信息-日、周、月 k线 |                        |
-| 概念行情 | stock.maket.get_market_concept_ths() | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
-|          |                                      |                                       |                        |
+| 数据     | API                                         | 说明                                  | 备注                   |
+| -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
+| 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
+| 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
+|          | stock.market.get_market_min()               | 获取单个股票的今日分时行情            | 只能获取当天           |
+|          | stock.market.list_market_current()          | 获取多个股票最新行情信息              | 实时行情               |
+| 概念行情 | stock.maket.get_market_concept_ths()        | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
+|          | stock.market.get_market_concept_min_ths()   | 获取同花顺概念行情当日分时            | 只能获取当天           |
+|          | stock.market.get_market_concept_today_ths() | 获取同花顺当前的概念行情              | 实时行情               |
 
 ### （2）ETF
 
 | 项目          | 进度         | 说明                           |
 | ------------- | ------------ | ------------------------------ |
 | 场内可交易etf | 排期中...... | 若您有相关资源可以一起参与贡献 |
```

### Comparing `adata-0.0.4b0/adata/__init__.py` & `adata-0.0.5b0/adata/__init__.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/__version__.py` & `adata-0.0.5b0/adata/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-VERSION = (0, 0, 4)
+VERSION = (0, 0, 5)
 # PRERELEASE = None  # alpha, beta or rc
 PRERELEASE = 'beta'  # alpha, beta or rc
 REVISION = None
 
 
 def generate_version(version, prerelease=None, revision=None):
     version_parts = [".".join(map(str, version))]
```

### Comparing `adata-0.0.4b0/adata/common/headers/baidu_headers.py` & `adata-0.0.5b0/adata/common/headers/baidu_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/common/headers/sina_headers.py` & `adata-0.0.5b0/adata/common/headers/sina_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/common/headers/ths_headers.py` & `adata-0.0.5b0/adata/common/headers/ths_headers.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/common/utils/snowflake.py` & `adata-0.0.5b0/adata/common/utils/snowflake.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/common/utils/sunrequests.py` & `adata-0.0.5b0/adata/common/utils/sunrequests.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 import requests
 
 
 class SunRequests(object):
     def __init__(self) -> None:
         super().__init__()
 
-    def request(self, method='get', url=None, times=3, sleep_time=2222, **kwargs):
+    def request(self, method='get', url=None, times=3, sleep_time=1588, **kwargs):
         """
         简单封装的请求，参考requests，增加循环次数和次数之间的等待时间
         :param method: 请求方法： get；post
         :param url: url
         :param times: 次数，int
         :param sleep_time: 循环的等待时间，毫秒
         :param kwargs: 其它 requests 参数，用法相同
         :return: res
         """
         res = None
         for i in range(times):
             res = requests.request(method=method, url=url, **kwargs)
-            if res.status_code == 200:
+            if res.status_code in (200, 404):
                 return res
             time.sleep(sleep_time / 1000)
         return res
```

### Comparing `adata-0.0.4b0/adata/stock/info/stock_code.py` & `adata-0.0.5b0/adata/stock/info/stock_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """
 
     def __init__(self) -> None:
         super().__init__()
 
     def all_code(self):
         """
-        获取所有股票的代码
+        获取所有股票的代码 ,后续补充多数据源
         :return: 所有股票的代码信息： ['stock_code','short_name','exchange']
         """
         return self.__market_rank_baidu()
 
     def __market_rank_baidu(self):
         """
         获取百度当前涨幅排名的代码
```

### Comparing `adata-0.0.4b0/adata/stock/info/stock_concept.py` & `adata-0.0.5b0/adata/stock/info/stock_concept.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
         super().__init__()
 
     def all_concept_code_ths(self):
         """
         获取同花顺概念列表：代码和名称
         :return: 概念[[concept_code,name]]
         """
-        return pd.concat([self.concept_code_ths_pc(), self.concept_code_ths_app()]).reset_index(drop=True)
+        return self.__concept_code_ths_app()
 
-    def concept_code_ths_pc(self):
+    def __concept_code_ths_pc(self):
         """
-        获取同花顺的所有概念和概念代码
+        获取同花顺的所有概念和概念代码,暂时废弃
         web: http://q.10jqka.com.cn/gn/
         """
         # 1. 请求接口 url
         api_url = f"http://q.10jqka.com.cn/gn/"
         for i in range(3):
             res = requests.request('get', api_url, headers=ths_headers.text_headers, proxies={})
             # 2. 判断请求是否正确
@@ -49,15 +49,15 @@
                     data.append([href[-7: -1], a.string, href])
 
             # 4. 封装数据
             data_df = pd.DataFrame(data=data, columns=['concept_code', 'name', 'href'])[['concept_code', 'name']]
             data_df['source'] = '同花顺PC'
             return data_df
 
-    def concept_code_ths_app(self):
+    def __concept_code_ths_app(self):
         """
         获取app的概率列表，通过问财询问得到结果
         :return: app的概念列表： concept_code，name
         """
         data = []
         for i in range(1, 10):
             api_url = f"http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?perpage=100&page={i}&query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119"
@@ -73,9 +73,7 @@
                                                                                             ignore_index=False)
         data_df['source'] = '同花顺APP'
         return data_df
 
 
 if __name__ == '__main__':
     print(StockConcept().all_concept_code_ths())
-    print(StockConcept().concept_code_ths_pc())
-    print(StockConcept().concept_code_ths_app())
```

### Comparing `adata-0.0.4b0/adata/stock/market/stock_dividend.py` & `adata-0.0.5b0/adata/stock/market/stock_dividend.py`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/adata/stock/market/stock_market.py` & `adata-0.0.5b0/adata/stock/market/stock_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from adata.common.headers import baidu_headers, sina_headers
 from adata.common.utils import requests
 
 
 class StockMarket(object):
     """
-    股票行情
+    股票行情 TODO 数据返回类型转换
     """
     MARKET_COLUMNS = ['trade_time', 'open', 'close', 'volume', 'high', 'low', 'amount', 'change', 'change_pct',
                       'turnover_ratio', 'pre_close']
     MARKET_MIN_COLUMNS = ['stock_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount']
     MARKET_CURRENT_COLUMNS = ['stock_code', 'short_name', 'price', 'change', 'change_pct', 'volume', 'amount']
 
     def __init__(self) -> None:
@@ -105,14 +105,17 @@
         result_df['stock_code'] = stock_code
         result_df['trade_date'] = result_df['trade_time']
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time']).dt.strftime('%Y-%m-%d %H:%M:%S')
         result_df.replace('--', None, inplace=True)
         result_df.replace('', None, inplace=True)
         result_df['change'] = result_df['change'].str.replace('+', '', regex=True)
         result_df['change_pct'] = result_df['change_pct'].str.replace('+', '', regex=True)
+        # 剔除成交量为0的异常数据
+        result_df['amount'] = result_df['amount'].astype(float)
+        result_df = result_df[result_df['amount'] > 0]
         return result_df
 
     def __market_baidu_today_min(self, stock_code):
         """
         获取百度的股票行情数据
         web： https://gushitong.baidu.com/stock/ab-002926
         url: https://finance.pae.baidu.com/selfselect/getstockquotation?all=1&code=601318&isIndex=false&isBk=false&isBlock=false&isFutures=false&isStock=true&newFormat=1&group=quotation_minute_ab&finClientType=pc
```

### Comparing `adata-0.0.4b0/adata/stock/market/stock_market_concept.py` & `adata-0.0.5b0/adata/stock/market/stock_market_concept.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,55 +6,56 @@
 http://search.10jqka.com.cn/gateway/urp/v7/landing/getDataList?query=%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5&condition=%5B%7B%22indexName%22%3A%22%E6%8C%87%E6%95%B0%40%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22indexProperties%22%3A%5B%5D%2C%22source%22%3A%22new_parser%22%2C%22type%22%3A%22index%22%2C%22indexPropertiesMap%22%3A%7B%7D%2C%22reportType%22%3A%22null%22%2C%22chunkedResult%22%3A%22%E6%89%80%E6%9C%89%E6%A6%82%E5%BF%B5%22%2C%22valueType%22%3A%22_%E6%8C%87%E6%95%B0%E7%B1%BB%E5%9E%8B%22%2C%22domain%22%3A%22abs_a%E6%8C%87%E9%A2%86%E5%9F%9F%22%2C%22uiText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22sonSize%22%3A0%2C%22queryText%22%3A%22%E5%90%8C%E8%8A%B1%E9%A1%BA%E6%A6%82%E5%BF%B5%E6%8C%87%E6%95%B0%22%2C%22relatedSize%22%3A0%7D%5D&urp_sort_index=%E6%8C%87%E6%95%B0%E4%BB%A3%E7%A0%81&source=Ths_iwencai_Xuangu&perpage=500&page=1&urp_sort_way=desc&codelist=&page_id=&logid=35df00ee5ae706d0dfcd0dbfdb846e0c&ret=json_all&sessionid=35df00ee5ae706d0dfcd0dbfdb846e0c&iwc_token=0ac9667016801698001765831&user_id=Ths_iwencai_Xuangu_7fahywzhbkrh4lwwkwfw936njqbjzsly&uuids%5B0%5D=23119&query_type=zhishu&comp_id=6367801&business_cat=soniu&uuid=23119
 885772 表示手机端的概念代码
 @author: 1nchaos
 @date: 2023/3/30 16:17
 """
 import copy
 import json
+import time
 
 import pandas as pd
 
 from adata.common.headers import ths_headers
 from adata.common.utils import requests
 
 
 class StockMarketConcept(object):
     """
     股票概念 行情
     """
+    COLUMNS = ['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount']
 
     def __init__(self) -> None:
         super().__init__()
 
     def get_market_concept_ths(self, concept_code: str = '886013', k_type: int = 1, adjust_type: int = 1):
         """
         获取同花顺的概率的行情
         web: http://q.10jqka.com.cn/gn/
-        url: http://d.10jqka.com.cn/v6/line/48_886013/01/last1800.js
+        pc: http://d.10jqka.com.cn/v4/line/bk_885772/21/last.js
+        app: http://d.10jqka.com.cn/v6/line/48_886013/01/last1800.js
         00 日k不复权；01日k前复权；02日k后复权；11周k前复权；21月k前复权
         :param concept_code: 同花顺概念代码
         :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
         :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权
         :return: k线行情数据 [日期，开，高，低，收,成交量，成交额]
         ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000
         成交量：股 820953530  821万手
         成交额：元 16959251000.000 169.6亿
         """
         # 1.接口 url
-        api_url = f"http://d.10jqka.com.cn/v6/line/48_{concept_code}/{adjust_type}{k_type}/last1800.js"
-        headers = copy.deepcopy(ths_headers.text_headers)
-        headers['Host'] = 'd.10jqka.com.cn'
-        res = requests.request('get', api_url, headers=headers, proxies={})
-        text = res.text
+        api_url = f"http://d.10jqka.com.cn/v6/line/48_{concept_code}/{k_type - 1}{adjust_type}/last1800.js"
+        # 同花顺可能ip限制，降低请求次数
+        text = self.__get_text(api_url, concept_code)
         result_text = text[text.index('{'):-1]
         data_list = json.loads(result_text)['data'].split(';')
         data = []
         for d in data_list:
             data.append(str(d).split(',')[0:7])
-        result_df = pd.DataFrame(data=data, columns=['trade_date', 'open', 'high', 'low', 'close', 'volume', 'amount'])
+        result_df = pd.DataFrame(data=data, columns=self.COLUMNS)
         result_df['concept_code'] = concept_code
         result_df['trade_time'] = pd.to_datetime(result_df['trade_date']).dt.strftime('%Y-%m-%d %H:%M:%S')
         result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
         return result_df
 
     def get_market_concept_min_ths(self, concept_code):
         """
@@ -63,19 +64,16 @@
         0930,958.901,74456973,36.807,2022925;  "pre": "960.374",
         :param concept_code: 概念代码
         :return 时间，现价，成交额（元），均价，成交量（股） 涨跌额，涨跌幅
         'concept_code', 'trade_time', 'price', 'change', 'change_pct', 'volume', 'avg_price', 'amount'
         """
         # 1.接口 url
         api_url = f"http://d.10jqka.com.cn/v6/time/48_{concept_code}/last.js"
-        headers = copy.deepcopy(ths_headers.text_headers)
-        headers['Host'] = 'd.10jqka.com.cn'
-        res = requests.request('get', api_url, headers=headers, proxies={})
+        text = self.__get_text(api_url, concept_code)
         # 2. 解析数据
-        text = res.text
         result_json = json.loads(text[text.index('{'):-1])[f"48_{concept_code}"]
         pre_price = result_json['pre']
         trade_date = result_json['date']
         data_list = result_json['data'].split(';')
         data = []
         for d in data_list:
             data.append(str(d).split(','))
@@ -86,11 +84,63 @@
         result_df['trade_date'] = pd.to_datetime(trade_date, format='%Y%m%d').strftime('%Y-%m-%d')
         result_df['trade_time'] = pd.to_datetime(result_df['trade_time'], format='%Y%m%d%H%M').dt.strftime(
             '%Y-%m-%d %H:%M:%S')
         result_df['change'] = result_df['price'].astype(float) - float(pre_price)
         result_df['change_pct'] = result_df['change'].astype(float) / float(pre_price) * 100
         return result_df
 
+    def get_market_concept_today_ths(self, concept_code: str = '886013', k_type: int = 1, adjust_type: int = 1):
+        """
+        获取同花顺当前的概念行情
+        web: http://q.10jqka.com.cn/gn/
+        pc: http://d.10jqka.com.cn/v6/line/48_886042/01/today.js
+        quotebridge_v6_line_48_886042_01_today({"48_886042":{"1":"20230425","7":"891.344","8":"892.350","9":"853.800",
+        "11":"860.076","13":491708080,"19":"17647511000.000","74":"","1968584":"","66":"","open":1,"dt":"2244",
+        "name":"\u5b58\u50a8\u82af\u7247","marketType":""}})
+
+        :param concept_code: 同花顺概念代码
+        :param k_type: k线类型：1.日；2.周；3.月 默认：1 日k
+        :param adjust_type: k线复权类型：0.不复权；1.前复权；2.后复权 默认：1 前复权
+        :return: k线行情数据 [概念代码,概念名称,日期，开，高，低，收,成交量，成交额]
+        ;20230419,958.901,981.118,958.449,961.107,521143220,20442229000.000,存储芯片
+        k:   1,      7,      8,       9,      11,      13,         19,        name
+        成交量：股 820953530  821万手
+        成交额：元 16959251000.000 169.6亿
+        """
+        # 1.接口 url
+        api_url = f"http://d.10jqka.com.cn/v6/line/48_{concept_code}/{k_type - 1}{adjust_type}/today.js"
+        headers = copy.deepcopy(ths_headers.text_headers)
+        headers['Host'] = 'd.10jqka.com.cn'
+        # 同花顺可能ip限制，降低请求次数
+        text = self.__get_text(api_url, concept_code)
+        result_text = text[text.index('{'):-1]
+        data_list = [json.loads(result_text)[f"48_{concept_code}"]]
+        rename = {'1': 'trade_date', '7': 'open', '8': 'high', '9': 'low', '11': 'close', '13': 'volume',
+                  '19': 'amount'}
+        result_df = pd.DataFrame(data=data_list).rename(columns=rename)[self.COLUMNS]
+        result_df['concept_code'] = concept_code
+        result_df['trade_date'] = pd.to_datetime(result_df['trade_date'], format='%Y%m%d').dt.strftime('%Y-%m-%d')
+        return result_df
+
+    def __get_text(self, api_url, concept_code):
+        """
+        获取同花顺的请求 text
+        :param api_url: url
+        :param concept_code: 概念代码
+        :return:
+        """
+        headers = copy.deepcopy(ths_headers.text_headers)
+        headers['Host'] = 'd.10jqka.com.cn'
+        text = ''
+        for i in range(3):
+            res = requests.request('get', api_url, headers=headers, proxies={})
+            text = res.text
+            if concept_code in text:
+                break
+            time.sleep(2)
+        return text
+
 
 if __name__ == '__main__':
-    print(StockMarketConcept().get_market_concept_ths(concept_code='886013'))
-    print(StockMarketConcept().get_market_concept_min_ths(concept_code='886013'))
+    print(StockMarketConcept().get_market_concept_ths(concept_code='886042'))
+    print(StockMarketConcept().get_market_concept_min_ths(concept_code='886041'))
+    print(StockMarketConcept().get_market_concept_today_ths(concept_code='886041'))
```

### Comparing `adata-0.0.4b0/adata.egg-info/PKG-INFO` & `adata-0.0.5b0/adata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adata
-Version: 0.0.4b0
+Version: 0.0.5b0
 Summary: A Data,A Stock,ETF,Bond,Quant
 Home-page: https://gitee.com/inchaos/adata
 Author: 1nchaos
 Author-email: 9527@1nchaos.com
 License: Apache License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
@@ -82,29 +82,31 @@
 
 整理了最新版本的数据列表和相关使用Api，详细内容和相关使用参数，请参考数据字典文档。
 
 ### （1）股票-Stock
 
 #### 	1. 基本信息
 
-| 数据     | API                               | 说明                                | 备注                 |
-| -------- | --------------------------------- | ----------------------------------- | -------------------- |
-| A股代码  | stock.info.all_code()             | 所有A股代码信息                     |                      |
-| 概念代码 | stock.info.all_concept_code_ths() | 所有A股概念代码信息（同花顺）pc+app | 来源：同花顺公开数据 |
-|          | stock.info.concept_code_ths_pc()  | A股概念代码信息（同花顺）pc         | 来源：同花顺数据中心 |
-|          | stock.info.concept_code_ths_app() | A股概念代码信息（同花顺）app        | 来源：问财           |
+| 数据         | API                                  | 说明                             | 备注                 |
+| ------------ | ------------------------------------ | -------------------------------- | -------------------- |
+| A股代码      | stock.info.all_code()                | 所有A股代码信息                  |                      |
+| 概念代码     | stock.info.all_concept_code_ths()    | 所有A股概念代码信息（同花顺）app | 来源：同花顺公开数据 |
+| 概念成分列表 | stock.info.concept_constituent_ths() | 获取概念的成分股                 |                      |
 
 #### 	2. 行情信息
 
-| 数据     | API                                  | 说明                                  | 备注                   |
-| -------- | ------------------------------------ | ------------------------------------- | ---------------------- |
-| 分红信息 | stock.maket.get_dividend()           | 获取单只股票的分红信息                |                        |
-| 股票行情 | stock.market.get_market()            | 获取单只股票的行情信息-日、周、月 k线 |                        |
-| 概念行情 | stock.maket.get_market_concept_ths() | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
-|          |                                      |                                       |                        |
+| 数据     | API                                         | 说明                                  | 备注                   |
+| -------- | ------------------------------------------- | ------------------------------------- | ---------------------- |
+| 分红信息 | stock.maket.get_dividend()                  | 获取单只股票的分红信息                |                        |
+| 股票行情 | stock.market.get_market()                   | 获取单只股票的行情信息-日、周、月 k线 |                        |
+|          | stock.market.get_market_min()               | 获取单个股票的今日分时行情            | 只能获取当天           |
+|          | stock.market.list_market_current()          | 获取多个股票最新行情信息              | 实时行情               |
+| 概念行情 | stock.maket.get_market_concept_ths()        | 获取单个概念的行情信息-日、周、月 k线 | 只有同花顺相关概念行情 |
+|          | stock.market.get_market_concept_min_ths()   | 获取同花顺概念行情当日分时            | 只能获取当天           |
+|          | stock.market.get_market_concept_today_ths() | 获取同花顺当前的概念行情              | 实时行情               |
 
 ### （2）ETF
 
 | 项目          | 进度         | 说明                           |
 | ------------- | ------------ | ------------------------------ |
 | 场内可交易etf | 排期中...... | 若您有相关资源可以一起参与贡献 |
```

### Comparing `adata-0.0.4b0/adata.egg-info/SOURCES.txt` & `adata-0.0.5b0/adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adata-0.0.4b0/setup.py` & `adata-0.0.5b0/setup.py`

 * *Files identical despite different names*

