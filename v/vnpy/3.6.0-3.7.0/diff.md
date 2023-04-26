# Comparing `tmp/vnpy-3.6.0.tar.gz` & `tmp/vnpy-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy-3.6.0.tar", last modified: Thu Feb 16 05:51:44 2023, max compression
+gzip compressed data, was "vnpy-3.7.0.tar", last modified: Wed Apr 26 07:30:55 2023, max compression
```

## Comparing `vnpy-3.6.0.tar` & `vnpy-3.7.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:44.032478 vnpy-3.6.0/
--rw-rw-rw-   0        0        0     1107 2021-11-17 00:58:32.000000 vnpy-3.6.0/LICENSE
--rw-rw-rw-   0        0        0       85 2021-11-17 00:58:32.000000 vnpy-3.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0    18573 2023-02-16 05:51:44.033455 vnpy-3.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    17450 2023-02-16 05:42:59.000000 vnpy-3.6.0/README.md
--rw-rw-rw-   0        0        0     1362 2023-02-16 05:51:44.038995 vnpy-3.6.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2022-03-11 03:28:39.000000 vnpy-3.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.774635 vnpy-3.6.0/vnpy/
--rw-rw-rw-   0        0        0     1170 2023-02-16 05:22:03.000000 vnpy-3.6.0/vnpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.826902 vnpy-3.6.0/vnpy/chart/
--rw-rw-rw-   0        0        0       75 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/chart/__init__.py
--rw-rw-rw-   0        0        0     1161 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/chart/axis.py
--rw-rw-rw-   0        0        0      388 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/chart/base.py
--rw-rw-rw-   0        0        0     9564 2022-05-17 03:27:06.000000 vnpy-3.6.0/vnpy/chart/item.py
--rw-rw-rw-   0        0        0     5097 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/chart/manager.py
--rw-rw-rw-   0        0        0    16307 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/chart/widget.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.884780 vnpy-3.6.0/vnpy/event/
--rw-rw-rw-   0        0        0       53 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/event/__init__.py
--rw-rw-rw-   0        0        0     4370 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/event/engine.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.898846 vnpy-3.6.0/vnpy/rpc/
--rw-rw-rw-   0        0        0       62 2022-03-11 03:28:39.000000 vnpy-3.6.0/vnpy/rpc/__init__.py
--rw-rw-rw-   0        0        0     4896 2022-10-22 01:37:27.000000 vnpy-3.6.0/vnpy/rpc/client.py
--rw-rw-rw-   0        0        0      184 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/rpc/common.py
--rw-rw-rw-   0        0        0     4005 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/rpc/server.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.957709 vnpy-3.6.0/vnpy/trader/
--rw-rw-rw-   0        0        0        0 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/__init__.py
--rw-rw-rw-   0        0        0      795 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/trader/app.py
--rw-rw-rw-   0        0        0     4235 2022-06-26 07:18:12.000000 vnpy-3.6.0/vnpy/trader/constant.py
--rw-rw-rw-   0        0        0    14375 2023-02-12 11:53:25.000000 vnpy-3.6.0/vnpy/trader/converter.py
--rw-rw-rw-   0        0        0     3682 2022-10-18 14:40:45.000000 vnpy-3.6.0/vnpy/trader/database.py
--rw-rw-rw-   0        0        0     1590 2023-02-13 10:45:32.000000 vnpy-3.6.0/vnpy/trader/datafeed.py
--rw-rw-rw-   0        0        0    21837 2023-02-12 11:53:25.000000 vnpy-3.6.0/vnpy/trader/engine.py
--rw-rw-rw-   0        0        0      316 2021-12-30 02:24:59.000000 vnpy-3.6.0/vnpy/trader/event.py
--rw-rw-rw-   0        0        0    12124 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/trader/gateway.py
--rw-rw-rw-   0        0        0    10721 2023-02-15 14:50:24.000000 vnpy-3.6.0/vnpy/trader/object.py
--rw-rw-rw-   0        0        0     7384 2023-02-15 02:33:10.000000 vnpy-3.6.0/vnpy/trader/optimize.py
--rw-rw-rw-   0        0        0     1188 2022-05-17 03:10:38.000000 vnpy-3.6.0/vnpy/trader/setting.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.979686 vnpy-3.6.0/vnpy/trader/ui/
--rw-rw-rw-   0        0        0       95 2022-03-11 03:28:39.000000 vnpy-3.6.0/vnpy/trader/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:44.028942 vnpy-3.6.0/vnpy/trader/ui/ico/
--rw-rw-rw-   0        0        0        0 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/__init__.py
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/about.ico
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/connect.ico
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/contract.ico
--rw-rw-rw-   0        0        0    63038 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/database.ico
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/editor.ico
--rw-rw-rw-   0        0        0    34382 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/email.ico
--rw-rw-rw-   0        0        0    67134 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/exit.ico
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/forum.ico
--rw-rw-rw-   0        0        0    21662 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/restore.ico
--rw-rw-rw-   0        0        0    51774 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/test.ico
--rw-rw-rw-   0        0        0    67646 2021-11-17 00:58:34.000000 vnpy-3.6.0/vnpy/trader/ui/ico/vnpy.ico
--rw-rw-rw-   0        0        0    10121 2022-10-10 10:03:51.000000 vnpy-3.6.0/vnpy/trader/ui/mainwindow.py
--rw-rw-rw-   0        0        0     3919 2023-02-15 13:52:09.000000 vnpy-3.6.0/vnpy/trader/ui/qt.py
--rw-rw-rw-   0        0        0    43292 2023-02-11 08:47:36.000000 vnpy-3.6.0/vnpy/trader/ui/widget.py
--rw-rw-rw-   0        0        0    30239 2022-10-02 15:16:32.000000 vnpy-3.6.0/vnpy/trader/utility.py
-drwxrwxrwx   0        0        0        0 2023-02-16 05:51:43.799834 vnpy-3.6.0/vnpy.egg-info/
--rw-rw-rw-   0        0        0    18573 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1234 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       99 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-16 05:51:43.000000 vnpy-3.6.0/vnpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:55.380736 vnpy-3.7.0/
+-rw-rw-rw-   0        0        0     1107 2022-11-12 13:43:34.000000 vnpy-3.7.0/LICENSE
+-rw-rw-rw-   0        0        0       85 2022-11-12 13:43:34.000000 vnpy-3.7.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    18628 2023-04-26 07:30:55.380736 vnpy-3.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17528 2023-04-26 07:30:10.000000 vnpy-3.7.0/README.md
+-rw-rw-rw-   0        0        0     1362 2023-04-26 07:30:55.412801 vnpy-3.7.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2022-11-12 13:43:34.000000 vnpy-3.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:52.606220 vnpy-3.7.0/vnpy/
+-rw-rw-rw-   0        0        0     1170 2023-04-26 07:30:10.000000 vnpy-3.7.0/vnpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:52.735356 vnpy-3.7.0/vnpy/chart/
+-rw-rw-rw-   0        0        0       75 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/__init__.py
+-rw-rw-rw-   0        0        0     1161 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/axis.py
+-rw-rw-rw-   0        0        0      388 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/base.py
+-rw-rw-rw-   0        0        0     9564 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/item.py
+-rw-rw-rw-   0        0        0     5097 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/manager.py
+-rw-rw-rw-   0        0        0    16307 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/chart/widget.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:52.761051 vnpy-3.7.0/vnpy/event/
+-rw-rw-rw-   0        0        0       53 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/event/__init__.py
+-rw-rw-rw-   0        0        0     4370 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/event/engine.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:52.887783 vnpy-3.7.0/vnpy/rpc/
+-rw-rw-rw-   0        0        0       62 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/rpc/__init__.py
+-rw-rw-rw-   0        0        0     4896 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/rpc/client.py
+-rw-rw-rw-   0        0        0      184 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/rpc/common.py
+-rw-rw-rw-   0        0        0     4005 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/rpc/server.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:53.896063 vnpy-3.7.0/vnpy/trader/
+-rw-rw-rw-   0        0        0        0 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/__init__.py
+-rw-rw-rw-   0        0        0      795 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/app.py
+-rw-rw-rw-   0        0        0     4349 2023-04-23 00:06:07.000000 vnpy-3.7.0/vnpy/trader/constant.py
+-rw-rw-rw-   0        0        0    14375 2023-04-23 00:06:07.000000 vnpy-3.7.0/vnpy/trader/converter.py
+-rw-rw-rw-   0        0        0     3682 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/database.py
+-rw-rw-rw-   0        0        0     1590 2023-02-14 02:11:44.000000 vnpy-3.7.0/vnpy/trader/datafeed.py
+-rw-rw-rw-   0        0        0    21837 2023-02-14 02:11:44.000000 vnpy-3.7.0/vnpy/trader/engine.py
+-rw-rw-rw-   0        0        0      316 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/event.py
+-rw-rw-rw-   0        0        0    12124 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/gateway.py
+-rw-rw-rw-   0        0        0    10721 2023-02-14 02:11:44.000000 vnpy-3.7.0/vnpy/trader/object.py
+-rw-rw-rw-   0        0        0     7384 2023-02-16 05:30:33.000000 vnpy-3.7.0/vnpy/trader/optimize.py
+-rw-rw-rw-   0        0        0     1188 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/setting.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:54.362646 vnpy-3.7.0/vnpy/trader/ui/
+-rw-rw-rw-   0        0        0       95 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:55.378686 vnpy-3.7.0/vnpy/trader/ui/ico/
+-rw-rw-rw-   0        0        0        0 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/__init__.py
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/about.ico
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/connect.ico
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/contract.ico
+-rw-rw-rw-   0        0        0    63038 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/database.ico
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/editor.ico
+-rw-rw-rw-   0        0        0    34382 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/email.ico
+-rw-rw-rw-   0        0        0    67134 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/exit.ico
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/forum.ico
+-rw-rw-rw-   0        0        0    21662 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/restore.ico
+-rw-rw-rw-   0        0        0    51774 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/test.ico
+-rw-rw-rw-   0        0        0    67646 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/ico/vnpy.ico
+-rw-rw-rw-   0        0        0    10118 2023-04-26 07:30:10.000000 vnpy-3.7.0/vnpy/trader/ui/mainwindow.py
+-rw-rw-rw-   0        0        0     3919 2023-02-16 05:30:33.000000 vnpy-3.7.0/vnpy/trader/ui/qt.py
+-rw-rw-rw-   0        0        0    43292 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/ui/widget.py
+-rw-rw-rw-   0        0        0    30239 2022-11-12 13:43:34.000000 vnpy-3.7.0/vnpy/trader/utility.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:30:52.640354 vnpy-3.7.0/vnpy.egg-info/
+-rw-rw-rw-   0        0        0    18628 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1234 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       99 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-26 07:30:52.000000 vnpy-3.7.0/vnpy.egg-info/top_level.txt
```

### Comparing `vnpy-3.6.0/LICENSE` & `vnpy-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/PKG-INFO` & `vnpy-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: vnpy
-Version: 3.6.0
+Version: 3.7.0
 Summary: A framework for developing quant trading systems.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Project-URL: Documentation, https://www.vnpy.com/docs
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,24 +29,24 @@
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/veighna-logo.png"/>
 </p>
 
 💬 Want to read this in **english** ? Go [**here**](README_ENG.md)
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.6.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.7.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/actions/workflow/status/vnpy/vnpy/pythonapp.yml?branch=master"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 VeighNa是一套基于Python的开源量化交易系统开发框架，在开源社区持续不断的贡献下一步步成长为多功能量化交易平台，自发布以来已经积累了众多来自金融机构或相关领域的用户，包括私募基金、证券公司、期货公司等。
 
-&#x1F393;&#x1F393;&#x1F393; **《VeighNa实战进阶》系列在线课程，已经在官方微信公众号[VeighNa开源量化]上线，覆盖30天入门、CTA实战、海龟策略、期权波动率交易等内容。购买请扫描下方二维码关注后，点击菜单栏的【进阶资料】按钮即可**：
+:rocket: :rocket: :rocket: **面向专业交易员的【VeighNa Elite量化终端】已经正式发布，针对专业交易员群体在海量策略并发、智能移仓换月、算法拆单执行、多账户交易支持等方面的需求提供了完善支持。了解更详细的信息请扫描下方二维码关注后，点击菜单栏的【社区交流 -> Elite会员服务】即可**：
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy_qr.jpg"/>
 </p>
 
 在使用VeighNa进行二次开发（策略、模块等）的过程中有任何疑问，请查看[**VeighNa项目文档**](https://www.vnpy.com/docs/cn/index.html)，如果无法解决请前往[**官方社区论坛**](https://www.vnpy.com/forum/)的【提问求助】板块寻求帮助，也欢迎在【经验分享】板块分享你的使用心得！
 
@@ -211,15 +210,15 @@
 
 11. 官方交流群262656087（QQ），管理严格（定期清除长期潜水的成员），入群费将捐赠给VeighNa社区基金。
 
 注：以上关于功能特点的说明为根据说明文档发布时情况罗列，后续可能存在更新或调整。若功能描述同实际存在出入，欢迎通过Issue联系进行调整。
 
 ## 环境准备
 
-* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.6.0](https://download.vnpy.com/veighna_studio-3.6.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
+* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.7.0](https://download.vnpy.com/veighna_studio-3.7.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
 * 支持的系统版本：Windows 10以上 / Windows Server 2016以上 / Ubuntu 20.04 LTS以上
 * 支持的Python版本：Python 3.7/ 3.8 / 3.9 / 3.10 64位（**推荐使用Python 3.10**）
 
 ## 安装步骤
 
 在[这里](https://github.com/vnpy/vnpy/releases)下载Release发布版本，解压后运行以下命令安装：
 
@@ -325,9 +324,7 @@
 * [社区行为准则](https://github.com/vnpy/vnpy/blob/dev/.github/CODE_OF_CONDUCT.md)
 * [Issue模板](https://github.com/vnpy/vnpy/blob/dev/.github/ISSUE_TEMPLATE.md)
 * [PR模板](https://github.com/vnpy/vnpy/blob/dev/.github/PULL_REQUEST_TEMPLATE.md)
 
 ## 版权说明
 
 MIT
-
-
```

### Comparing `vnpy-3.6.0/README.md` & `vnpy-3.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/veighna-logo.png"/>
 </p>
 
 💬 Want to read this in **english** ? Go [**here**](README_ENG.md)
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.6.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.7.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/actions/workflow/status/vnpy/vnpy/pythonapp.yml?branch=master"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 VeighNa是一套基于Python的开源量化交易系统开发框架，在开源社区持续不断的贡献下一步步成长为多功能量化交易平台，自发布以来已经积累了众多来自金融机构或相关领域的用户，包括私募基金、证券公司、期货公司等。
 
-&#x1F393;&#x1F393;&#x1F393; **《VeighNa实战进阶》系列在线课程，已经在官方微信公众号[VeighNa开源量化]上线，覆盖30天入门、CTA实战、海龟策略、期权波动率交易等内容。购买请扫描下方二维码关注后，点击菜单栏的【进阶资料】按钮即可**：
+:rocket: :rocket: :rocket: **面向专业交易员的【VeighNa Elite量化终端】已经正式发布，针对专业交易员群体在海量策略并发、智能移仓换月、算法拆单执行、多账户交易支持等方面的需求提供了完善支持。了解更详细的信息请扫描下方二维码关注后，点击菜单栏的【社区交流 -> Elite会员服务】即可**：
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy_qr.jpg"/>
 </p>
 
 在使用VeighNa进行二次开发（策略、模块等）的过程中有任何疑问，请查看[**VeighNa项目文档**](https://www.vnpy.com/docs/cn/index.html)，如果无法解决请前往[**官方社区论坛**](https://www.vnpy.com/forum/)的【提问求助】板块寻求帮助，也欢迎在【经验分享】板块分享你的使用心得！
 
@@ -184,15 +184,15 @@
 
 11. 官方交流群262656087（QQ），管理严格（定期清除长期潜水的成员），入群费将捐赠给VeighNa社区基金。
 
 注：以上关于功能特点的说明为根据说明文档发布时情况罗列，后续可能存在更新或调整。若功能描述同实际存在出入，欢迎通过Issue联系进行调整。
 
 ## 环境准备
 
-* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.6.0](https://download.vnpy.com/veighna_studio-3.6.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
+* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.7.0](https://download.vnpy.com/veighna_studio-3.7.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
 * 支持的系统版本：Windows 10以上 / Windows Server 2016以上 / Ubuntu 20.04 LTS以上
 * 支持的Python版本：Python 3.7/ 3.8 / 3.9 / 3.10 64位（**推荐使用Python 3.10**）
 
 ## 安装步骤
 
 在[这里](https://github.com/vnpy/vnpy/releases)下载Release发布版本，解压后运行以下命令安装：
```

### Comparing `vnpy-3.6.0/setup.cfg` & `vnpy-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/__init__.py` & `vnpy-3.7.0/vnpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 
-__version__ = "3.6.0"
+__version__ = "3.7.0"
```

### Comparing `vnpy-3.6.0/vnpy/chart/axis.py` & `vnpy-3.7.0/vnpy/chart/axis.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/chart/item.py` & `vnpy-3.7.0/vnpy/chart/item.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/chart/manager.py` & `vnpy-3.7.0/vnpy/chart/manager.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/chart/widget.py` & `vnpy-3.7.0/vnpy/chart/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/event/engine.py` & `vnpy-3.7.0/vnpy/event/engine.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/rpc/client.py` & `vnpy-3.7.0/vnpy/rpc/client.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/rpc/server.py` & `vnpy-3.7.0/vnpy/rpc/server.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/app.py` & `vnpy-3.7.0/vnpy/trader/app.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/constant.py` & `vnpy-3.7.0/vnpy/trader/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,16 @@
     CZCE = "CZCE"           # Zhengzhou Commodity Exchange
     DCE = "DCE"             # Dalian Commodity Exchange
     INE = "INE"             # Shanghai International Energy Exchange
     GFEX = "GFEX"           # Guangzhou Futures Exchange
     SSE = "SSE"             # Shanghai Stock Exchange
     SZSE = "SZSE"           # Shenzhen Stock Exchange
     BSE = "BSE"             # Beijing Stock Exchange
+    SHHK = "SHHK"           # Shanghai-HK Stock Connect
+    SZHK = "SZHK"           # Shenzhen-HK Stock Connect
     SGE = "SGE"             # Shanghai Gold Exchange
     WXE = "WXE"             # Wuxi Steel Exchange
     CFETS = "CFETS"         # CFETS Bond Market Maker Trading System
     XBOND = "XBOND"         # CFETS X-Bond Anonymous Trading System
 
     # Global
     SMART = "SMART"         # Smart Router for US stocks
```

### Comparing `vnpy-3.6.0/vnpy/trader/converter.py` & `vnpy-3.7.0/vnpy/trader/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
         holding: PositionHolding = self.get_position_holding(req.vt_symbol)
 
         if lock:
             return holding.convert_order_request_lock(req)
         elif net:
             return holding.convert_order_request_net(req)
-        elif req.exchange in [Exchange.SHFE, Exchange.INE]:
+        elif req.exchange in {Exchange.SHFE, Exchange.INE}:
             return holding.convert_order_request_shfe(req)
         else:
             return [req]
 
     def is_convert_required(self, vt_symbol: str) -> bool:
         """
         Check if the contract needs offset convert.
@@ -160,15 +160,15 @@
             if trade.offset == Offset.OPEN:
                 self.long_td += trade.volume
             elif trade.offset == Offset.CLOSETODAY:
                 self.short_td -= trade.volume
             elif trade.offset == Offset.CLOSEYESTERDAY:
                 self.short_yd -= trade.volume
             elif trade.offset == Offset.CLOSE:
-                if trade.exchange in [Exchange.SHFE, Exchange.INE]:
+                if trade.exchange in {Exchange.SHFE, Exchange.INE}:
                     self.short_yd -= trade.volume
                 else:
                     self.short_td -= trade.volume
 
                     if self.short_td < 0:
                         self.short_yd += self.short_td
                         self.short_td = 0
@@ -176,15 +176,15 @@
             if trade.offset == Offset.OPEN:
                 self.short_td += trade.volume
             elif trade.offset == Offset.CLOSETODAY:
                 self.long_td -= trade.volume
             elif trade.offset == Offset.CLOSEYESTERDAY:
                 self.long_yd -= trade.volume
             elif trade.offset == Offset.CLOSE:
-                if trade.exchange in [Exchange.SHFE, Exchange.INE]:
+                if trade.exchange in {Exchange.SHFE, Exchange.INE}:
                     self.long_yd -= trade.volume
                 else:
                     self.long_td -= trade.volume
 
                     if self.long_td < 0:
                         self.long_yd += self.long_td
                         self.long_td = 0
```

### Comparing `vnpy-3.6.0/vnpy/trader/database.py` & `vnpy-3.7.0/vnpy/trader/database.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/datafeed.py` & `vnpy-3.7.0/vnpy/trader/datafeed.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/engine.py` & `vnpy-3.7.0/vnpy/trader/engine.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/gateway.py` & `vnpy-3.7.0/vnpy/trader/gateway.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/object.py` & `vnpy-3.7.0/vnpy/trader/object.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/optimize.py` & `vnpy-3.7.0/vnpy/trader/optimize.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/setting.py` & `vnpy-3.7.0/vnpy/trader/setting.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/about.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/about.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/connect.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/connect.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/contract.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/contract.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/database.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/database.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/editor.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/editor.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/email.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/email.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/exit.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/exit.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/forum.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/forum.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/restore.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/restore.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/test.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/test.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/ico/vnpy.ico` & `vnpy-3.7.0/vnpy/trader/ui/ico/vnpy.ico`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/mainwindow.py` & `vnpy-3.7.0/vnpy/trader/ui/mainwindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         return widget, dock
 
     def connect(self, gateway_name: str) -> None:
         """
         Open connect dialog for gateway connection.
         """
         dialog: ConnectDialog = ConnectDialog(self.main_engine, gateway_name)
-        dialog.exec_()
+        dialog.exec()
 
     def closeEvent(self, event: QtGui.QCloseEvent) -> None:
         """
         Call main engine close function before exit.
         """
         reply = QtWidgets.QMessageBox.question(
             self,
@@ -273,15 +273,15 @@
         """
         widget: QtWidgets.QWidget = self.widgets.get(name, None)
         if not widget:
             widget = widget_class(self.main_engine, self.event_engine)
             self.widgets[name] = widget
 
         if isinstance(widget, QtWidgets.QDialog):
-            widget.exec_()
+            widget.exec()
         else:
             widget.show()
 
     def save_window_setting(self, name: str) -> None:
         """
         Save current window size and state by trader path and setting name.
         """
@@ -319,8 +319,8 @@
         """
         webbrowser.open("https://www.vnpy.com/forum/")
 
     def edit_global_setting(self) -> None:
         """
         """
         dialog: GlobalDialog = GlobalDialog()
-        dialog.exec_()
+        dialog.exec()
```

### Comparing `vnpy-3.6.0/vnpy/trader/ui/qt.py` & `vnpy-3.7.0/vnpy/trader/ui/qt.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/ui/widget.py` & `vnpy-3.7.0/vnpy/trader/ui/widget.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy/trader/utility.py` & `vnpy-3.7.0/vnpy/trader/utility.py`

 * *Files identical despite different names*

### Comparing `vnpy-3.6.0/vnpy.egg-info/PKG-INFO` & `vnpy-3.7.0/vnpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: vnpy
-Version: 3.6.0
+Version: 3.7.0
 Summary: A framework for developing quant trading systems.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Project-URL: Documentation, https://www.vnpy.com/docs
 Keywords: quant,quantitative,investment,trading,algotrading
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -30,24 +29,24 @@
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/veighna-logo.png"/>
 </p>
 
 💬 Want to read this in **english** ? Go [**here**](README_ENG.md)
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-3.6.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-3.7.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
     <img src ="https://img.shields.io/badge/python-3.7|3.8|3.9|3.10-blue.svg" />
     <img src ="https://img.shields.io/github/actions/workflow/status/vnpy/vnpy/pythonapp.yml?branch=master"/>
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 VeighNa是一套基于Python的开源量化交易系统开发框架，在开源社区持续不断的贡献下一步步成长为多功能量化交易平台，自发布以来已经积累了众多来自金融机构或相关领域的用户，包括私募基金、证券公司、期货公司等。
 
-&#x1F393;&#x1F393;&#x1F393; **《VeighNa实战进阶》系列在线课程，已经在官方微信公众号[VeighNa开源量化]上线，覆盖30天入门、CTA实战、海龟策略、期权波动率交易等内容。购买请扫描下方二维码关注后，点击菜单栏的【进阶资料】按钮即可**：
+:rocket: :rocket: :rocket: **面向专业交易员的【VeighNa Elite量化终端】已经正式发布，针对专业交易员群体在海量策略并发、智能移仓换月、算法拆单执行、多账户交易支持等方面的需求提供了完善支持。了解更详细的信息请扫描下方二维码关注后，点击菜单栏的【社区交流 -> Elite会员服务】即可**：
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy_qr.jpg"/>
 </p>
 
 在使用VeighNa进行二次开发（策略、模块等）的过程中有任何疑问，请查看[**VeighNa项目文档**](https://www.vnpy.com/docs/cn/index.html)，如果无法解决请前往[**官方社区论坛**](https://www.vnpy.com/forum/)的【提问求助】板块寻求帮助，也欢迎在【经验分享】板块分享你的使用心得！
 
@@ -211,15 +210,15 @@
 
 11. 官方交流群262656087（QQ），管理严格（定期清除长期潜水的成员），入群费将捐赠给VeighNa社区基金。
 
 注：以上关于功能特点的说明为根据说明文档发布时情况罗列，后续可能存在更新或调整。若功能描述同实际存在出入，欢迎通过Issue联系进行调整。
 
 ## 环境准备
 
-* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.6.0](https://download.vnpy.com/veighna_studio-3.6.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
+* 推荐使用VeighNa团队为量化交易专门打造的Python发行版[VeighNa Studio-3.7.0](https://download.vnpy.com/veighna_studio-3.7.0.exe)，集成内置了VeighNa框架以及VeighNa Station量化管理平台，无需手动安装
 * 支持的系统版本：Windows 10以上 / Windows Server 2016以上 / Ubuntu 20.04 LTS以上
 * 支持的Python版本：Python 3.7/ 3.8 / 3.9 / 3.10 64位（**推荐使用Python 3.10**）
 
 ## 安装步骤
 
 在[这里](https://github.com/vnpy/vnpy/releases)下载Release发布版本，解压后运行以下命令安装：
 
@@ -325,9 +324,7 @@
 * [社区行为准则](https://github.com/vnpy/vnpy/blob/dev/.github/CODE_OF_CONDUCT.md)
 * [Issue模板](https://github.com/vnpy/vnpy/blob/dev/.github/ISSUE_TEMPLATE.md)
 * [PR模板](https://github.com/vnpy/vnpy/blob/dev/.github/PULL_REQUEST_TEMPLATE.md)
 
 ## 版权说明
 
 MIT
-
-
```

### Comparing `vnpy-3.6.0/vnpy.egg-info/SOURCES.txt` & `vnpy-3.7.0/vnpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

