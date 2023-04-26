# Comparing `tmp/tableX-0.1.2.tar.gz` & `tmp/tableX-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableX-0.1.2.tar", last modified: Thu Jul 21 08:12:34 2022, max compression
+gzip compressed data, was "tableX-0.1.3.tar", last modified: Wed Apr 26 07:32:42 2023, max compression
```

## Comparing `tableX-0.1.2.tar` & `tableX-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-07-21 08:12:34.067909 tableX-0.1.2/
--rw-rw-rw-   0        0        0   212458 2022-07-21 08:12:34.066910 tableX-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-07-21 08:12:34.067909 tableX-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      940 2022-07-21 08:11:58.000000 tableX-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-21 08:12:34.026910 tableX-0.1.2/tableX/
--rw-rw-rw-   0        0        0       36 2022-07-21 07:57:38.000000 tableX-0.1.2/tableX/__init__.py
--rw-rw-rw-   0        0        0    12469 2022-07-21 08:01:43.000000 tableX-0.1.2/tableX/table2json.py
--rw-rw-rw-   0        0        0    10361 2022-07-21 07:57:38.000000 tableX-0.1.2/tableX/table2parser.py
--rw-rw-rw-   0        0        0     9402 2022-07-21 07:57:38.000000 tableX-0.1.2/tableX/tableparser.py
-drwxrwxrwx   0        0        0        0 2022-07-21 08:12:34.040910 tableX-0.1.2/tableX.egg-info/
--rw-rw-rw-   0        0        0   212458 2022-07-21 08:12:33.000000 tableX-0.1.2/tableX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2022-07-21 08:12:33.000000 tableX-0.1.2/tableX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-21 08:12:33.000000 tableX-0.1.2/tableX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2022-07-21 08:12:33.000000 tableX-0.1.2/tableX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-07-21 08:12:33.000000 tableX-0.1.2/tableX.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-21 08:12:34.062911 tableX-0.1.2/test/
--rw-rw-rw-   0        0        0   150224 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test.py
--rw-rw-rw-   0        0        0    23738 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test2.py
--rw-rw-rw-   0        0        0    21590 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test3.py
--rw-rw-rw-   0        0        0    23675 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test4.py
--rw-rw-rw-   0        0        0    24719 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test5.py
--rw-rw-rw-   0        0        0    57369 2022-07-21 07:57:38.000000 tableX-0.1.2/test/test_yj.py
--rw-rw-rw-   0        0        0    24729 2022-07-21 07:57:38.000000 tableX-0.1.2/test/testjjw.py
--rw-rw-rw-   0        0        0     6234 2022-07-21 07:57:38.000000 tableX-0.1.2/test/testth.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:32:42.607411 tableX-0.1.3/
+-rw-rw-rw-   0        0        0   229789 2023-04-26 07:32:42.606413 tableX-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-26 07:32:42.607411 tableX-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      960 2023-04-26 07:32:14.000000 tableX-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:32:42.574498 tableX-0.1.3/tableX/
+-rw-rw-rw-   0        0        0       36 2023-04-26 06:34:03.000000 tableX-0.1.3/tableX/__init__.py
+-rw-rw-rw-   0        0        0     1612 2023-04-26 05:22:17.000000 tableX-0.1.3/tableX/combining.py
+-rw-rw-rw-   0        0        0    12469 2023-04-26 06:34:03.000000 tableX-0.1.3/tableX/table2json.py
+-rw-rw-rw-   0        0        0    10361 2023-04-26 06:34:03.000000 tableX-0.1.3/tableX/table2parser.py
+-rw-rw-rw-   0        0        0     9402 2023-04-26 06:34:03.000000 tableX-0.1.3/tableX/tableparser.py
+drwxrwxrwx   0        0        0        0 2023-04-26 07:32:42.585469 tableX-0.1.3/tableX.egg-info/
+-rw-rw-rw-   0        0        0   229789 2023-04-26 07:32:42.000000 tableX-0.1.3/tableX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-04-26 07:32:42.000000 tableX-0.1.3/tableX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 07:32:42.000000 tableX-0.1.3/tableX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-26 07:32:42.000000 tableX-0.1.3/tableX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-26 07:32:42.000000 tableX-0.1.3/tableX.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 07:32:42.603422 tableX-0.1.3/test/
+-rw-rw-rw-   0        0        0   150224 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test.py
+-rw-rw-rw-   0        0        0    23738 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test2.py
+-rw-rw-rw-   0        0        0    21590 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test3.py
+-rw-rw-rw-   0        0        0    23675 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test4.py
+-rw-rw-rw-   0        0        0    24719 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test5.py
+-rw-rw-rw-   0        0        0    57369 2023-04-26 06:34:03.000000 tableX-0.1.3/test/test_yj.py
+-rw-rw-rw-   0        0        0    24729 2023-04-26 06:34:03.000000 tableX-0.1.3/test/testjjw.py
+-rw-rw-rw-   0        0        0     6234 2023-04-26 06:34:03.000000 tableX-0.1.3/test/testth.py
```

### Comparing `tableX-0.1.2/PKG-INFO` & `tableX-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tableX
-Version: 0.1.2
+Version: 0.1.3
 Summary: 针对前端table 工具类
 Home-page: https://www.github/buliqioqiolibusdo/tablex
 Author: xcc
 Author-email: xinchacha@xcc.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 
 ### tableX为操作前端table的工具集
 
 ### 版本说明
 	* v0.1.2 update 2022/7/21
@@ -88,15 +86,15 @@
         <tr><td>TO-251</td><td>N</td><td>250</td><td>8</td><td>0.36</td><td>0.47</td><td>-</td><td>-</td><td>2</td><td>4</td><td>12.8</td><td>557.9</td><td><a href="./202006/P020200630519802803185.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-3P(N)</td><td>N</td><td>200</td><td>60</td><td>39</td><td>46</td><td>-</td><td>-</td><td>2</td><td>4</td><td>56.9</td><td>3308</td><td><a href="./202006/P020200630518254400632.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220F</td><td>N</td><td>200</td><td>30</td><td>70</td><td>80</td><td>-</td><td>-</td><td>2</td><td>4</td><td>38</td><td>1945</td><td><a href="./202006/P020200630515454053403.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220F</td><td>N</td><td>200</td><td>9</td><td>0.22</td><td>0.28</td><td>-</td><td>-</td><td>1</td><td>3</td><td>14.6</td><td>673</td><td><a href="./202006/P020200630493232631450.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>200</td><td>9</td><td>0.22</td><td>0.28</td><td>-</td><td>-</td><td>1</td><td>3</td><td>14.6</td><td>673</td><td><a href="./202006/P020200630491951045852.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT-223-3L</td><td>N</td><td>200</td><td>3</td><td>1.2</td><td>1.5</td><td>-</td><td>-</td><td>2</td><td>4</td><td>4.3</td><td>101</td><td><a href="./202006/P020200630487520952738.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOP8-Dual</td><td>N</td><td>150</td><td>2</td><td>230</td><td>300</td><td>250</td><td>330</td><td>1.7</td><td>2.8</td><td>11.6</td><td>549.5</td><td><a href="./202006/P020200619558321389451.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-263</td><td>N</td><td>150</td><td>135</td><td>5.9</td><td>7</td><td>-</td><td>-</td><td>2</td><td>4</td><td>79</td><td>5416</td><td><a href="./202006/P020200619550316827004.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>120</td><td>50</td><td>15</td><td>20</td><td>15.5</td><td>23</td><td>1</td><td>2.5</td><td>96.88</td><td>4281</td><td><a href="./202006/P020200629531162576114.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220</td><td>N</td><td>120</td><td>130</td><td>4.8</td><td>5.8</td><td>-</td><td>-</td><td>2</td><td>4</td><td>80.07</td><td>5548</td><td><a href="./202006/P020200619541347828194.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>100</td><td>14</td><td>113</td><td>150</td><td>135</td><td>190</td><td>1.8</td><td>2.9</td><td>11.5</td><td>556.5</td><td><a href="./202006/P020200619409377584999.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>100</td><td>25</td><td>29</td><td>36</td><td>30.5</td><td>39</td><td>1</td><td>2</td><td>60</td><td>2359</td><td><a href="./202006/P020200629527605923542.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220AB</td><td>N</td><td>100</td><td>80</td><td>14</td><td>23</td><td>-</td><td>-</td><td>2</td><td>4</td><td>72</td><td>3901</td><td><a href="./202006/P020200629525836031796.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>30</td><td>130</td><td>1.9</td><td>2.5</td><td>2.6</td><td>3.3</td><td>1</td><td>3</td><td>79.1</td><td>4893</td><td><a href="./202006/P020200629506247629877.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>PDFN5*6</td><td>N</td><td>30</td><td>300</td><td>0.75</td><td>1</td><td>1.2</td><td>1.5</td><td>0.9</td><td>1.8</td><td>92.5</td><td>4849</td><td><a href="./202006/P020200629504792927704.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TSSOP-8</td><td>N+N</td><td>20</td><td>10</td><td>-</td><td>-</td><td>18</td><td>25</td><td>0.45</td><td>1</td><td>14.9</td><td>568</td><td><a href="./202006/P020200617573639199664.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT23-6</td><td>N+N</td><td>20</td><td>7</td><td>-</td><td>-</td><td>19</td><td>25</td><td>0.45</td><td>1</td><td>14.9</td><td>568</td><td><a href="./202006/P020200617573081059435.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT23-3</td><td>N</td><td>20</td><td>8</td><td>-</td><td>-</td><td>12</td><td>15</td><td>0.4</td><td>1</td><td>23</td><td>770</td><td><a href="./202006/P020200617572324291547.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>20</td><td>80</td><td>3.6</td><td>5</td><td>3</td><td>4.5</td><td>0.4</td><td>1</td><td>104</td><td>3386</td><td><a href="./202006/P020200617538395463092.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TSSOP-8</td><td>N</td><td>20</td><td>10</td><td>12</td><td>15</td><td>16</td><td>20</td><td>0.45</td><td>1</td><td>21.7</td><td>758</td><td><a href="./202006/P020200617538124632205.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr></tbody>
     </table>
     ''']
     json = table2json.table2json(text, [0, 1, 2], [3])
     print(json)
 
 示例二:
-```python
+​```python
 	"""
 	author:tieyongjie
 	desc: html_是带有图片,pdf的的html文本,获取到类似{'Image':'/upload/category/module_1.gif',
 	'DataSheet': '/download.asp?STARCAP_Datasheet_SM_20180710.pdf'}
 	"""
 
 	from table.tableX import table2parser
@@ -1327,8 +1325,27 @@
     # json = table2json.table2jsonStr(text, [0, 1, 2], [3])
     print(json)
 ```
 
 ### 2、table2jsonStr方法
 说明：跟table2json类似，只是返回参数是json字符串
 
+### 3、combining_json方法
+
+```
+from tableX.combining import combining_json
+table_html = """
+<table style="width: 100%;"><tbody><tr style="height:27px" class="firstRow"><td width="366" valign="top" colspan="3" style="padding: 0px 7px; border-width: 1px; border-color: windowtext; word-break: break-word;"><p>Item</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Specifications</p></td></tr><tr style="height:18px"><td width="129" valign="top" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="10" colspan="1"><p>GPS&nbsp;Antenna</p></td><td width="71" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5" colspan="1"><p>Dielectric</p><p>Antenna</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency&nbsp;Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>1575.42±3MHz</p></td></tr><tr style="height:18px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>RHCP</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2dBic（Zenith）</p></td></tr><tr style="height:11px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜1.5</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td width="71" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext; word-break: break-word;" rowspan="5" colspan="1"><p>LNA</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext; word-break: break-word;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>28±2dB</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Noise Figure</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜1.5dB</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜2.0</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Supply Voltage</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>3~5V DC</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Current Consumption</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜15mA</p></td></tr><tr style="height:27px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>LTE&nbsp;Antenna&nbsp;MAIN</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>698~960MHz/1710~2690MHz</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜3.0</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Linear</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2.5dBi（Zenith）</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>LTE&nbsp;Antenna&nbsp;AUX</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>698~960MHz/1710~2690MHz</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜3.0</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Linear</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2.0dBi（Zenith）</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="4"><p>Mechanical</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Cable</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>RG174</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Connector</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>SMA/FAKRA or others</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Material</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>ABS</p></td></tr><tr style="height:13px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Mounting Method</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Adhesive/Magnet</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>Environmental</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Operating Temperature</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>-40℃~+85℃</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Relative Humidity</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Up to 95%</p></td></tr><tr style="height:12px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Ingress Protection</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>IP67</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Vibration</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>10 to 55Hz with 1.5mm amplitude 2hours</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Environmentally Friendly</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>ROHS Compliant</p></td></tr></tbody></table>
+"""
+
+if __name__ == '__main__':
+    json_dic_s = combining_json(table_html, col=[0,1,2], tagSep=';',keySep='|')
+    print(json_dic_s)
+```
+
+**tagSep**:多value合并时切分符号,默认";"
+**keySep:** 多个key值合并时分隔符,默认空格
+
+**col**:列表,需要合并的列号,默认合并首列
 
+**table_html**: 输入需要转成json的列table
+**return** : 返回的字典组成的列表
```

### Comparing `tableX-0.1.2/setup.py` & `tableX-0.1.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     with io.open(os.path.join(here, 'tableX.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = ''
 
 setup(
     name='tableX',     # 包名字
-    version='0.1.2',   # 包版本
+    version='0.1.3',   # 包版本
     description='针对前端table 工具类',   # 简单描述
     author='xcc',  # 作者
     author_email='xinchacha@xcc.com',  # 作者邮箱
     url='https://www.github/buliqioqiolibusdo/tablex',      # 包的主页
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['tableX'],                 # 包
     install_requires=[
          # 'collections',
+         'pandas',
          'lxml >= 4.4.1',
          'json5 >= 0.8.5',
          'w3lib >= 1.22.0',
     ]   #依赖
 )
```

### Comparing `tableX-0.1.2/tableX/table2json.py` & `tableX-0.1.3/tableX/table2json.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/tableX/table2parser.py` & `tableX-0.1.3/tableX/table2parser.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/tableX/tableparser.py` & `tableX-0.1.3/tableX/tableparser.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/tableX.egg-info/PKG-INFO` & `tableX-0.1.3/tableX.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: tableX
-Version: 0.1.2
+Version: 0.1.3
 Summary: 针对前端table 工具类
 Home-page: https://www.github/buliqioqiolibusdo/tablex
 Author: xcc
 Author-email: xinchacha@xcc.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 
 ### tableX为操作前端table的工具集
 
 ### 版本说明
 	* v0.1.2 update 2022/7/21
@@ -88,15 +86,15 @@
         <tr><td>TO-251</td><td>N</td><td>250</td><td>8</td><td>0.36</td><td>0.47</td><td>-</td><td>-</td><td>2</td><td>4</td><td>12.8</td><td>557.9</td><td><a href="./202006/P020200630519802803185.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-3P(N)</td><td>N</td><td>200</td><td>60</td><td>39</td><td>46</td><td>-</td><td>-</td><td>2</td><td>4</td><td>56.9</td><td>3308</td><td><a href="./202006/P020200630518254400632.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220F</td><td>N</td><td>200</td><td>30</td><td>70</td><td>80</td><td>-</td><td>-</td><td>2</td><td>4</td><td>38</td><td>1945</td><td><a href="./202006/P020200630515454053403.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220F</td><td>N</td><td>200</td><td>9</td><td>0.22</td><td>0.28</td><td>-</td><td>-</td><td>1</td><td>3</td><td>14.6</td><td>673</td><td><a href="./202006/P020200630493232631450.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>200</td><td>9</td><td>0.22</td><td>0.28</td><td>-</td><td>-</td><td>1</td><td>3</td><td>14.6</td><td>673</td><td><a href="./202006/P020200630491951045852.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT-223-3L</td><td>N</td><td>200</td><td>3</td><td>1.2</td><td>1.5</td><td>-</td><td>-</td><td>2</td><td>4</td><td>4.3</td><td>101</td><td><a href="./202006/P020200630487520952738.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOP8-Dual</td><td>N</td><td>150</td><td>2</td><td>230</td><td>300</td><td>250</td><td>330</td><td>1.7</td><td>2.8</td><td>11.6</td><td>549.5</td><td><a href="./202006/P020200619558321389451.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-263</td><td>N</td><td>150</td><td>135</td><td>5.9</td><td>7</td><td>-</td><td>-</td><td>2</td><td>4</td><td>79</td><td>5416</td><td><a href="./202006/P020200619550316827004.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>120</td><td>50</td><td>15</td><td>20</td><td>15.5</td><td>23</td><td>1</td><td>2.5</td><td>96.88</td><td>4281</td><td><a href="./202006/P020200629531162576114.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220</td><td>N</td><td>120</td><td>130</td><td>4.8</td><td>5.8</td><td>-</td><td>-</td><td>2</td><td>4</td><td>80.07</td><td>5548</td><td><a href="./202006/P020200619541347828194.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>100</td><td>14</td><td>113</td><td>150</td><td>135</td><td>190</td><td>1.8</td><td>2.9</td><td>11.5</td><td>556.5</td><td><a href="./202006/P020200619409377584999.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>100</td><td>25</td><td>29</td><td>36</td><td>30.5</td><td>39</td><td>1</td><td>2</td><td>60</td><td>2359</td><td><a href="./202006/P020200629527605923542.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-220AB</td><td>N</td><td>100</td><td>80</td><td>14</td><td>23</td><td>-</td><td>-</td><td>2</td><td>4</td><td>72</td><td>3901</td><td><a href="./202006/P020200629525836031796.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-251</td><td>N</td><td>30</td><td>130</td><td>1.9</td><td>2.5</td><td>2.6</td><td>3.3</td><td>1</td><td>3</td><td>79.1</td><td>4893</td><td><a href="./202006/P020200629506247629877.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>PDFN5*6</td><td>N</td><td>30</td><td>300</td><td>0.75</td><td>1</td><td>1.2</td><td>1.5</td><td>0.9</td><td>1.8</td><td>92.5</td><td>4849</td><td><a href="./202006/P020200629504792927704.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TSSOP-8</td><td>N+N</td><td>20</td><td>10</td><td>-</td><td>-</td><td>18</td><td>25</td><td>0.45</td><td>1</td><td>14.9</td><td>568</td><td><a href="./202006/P020200617573639199664.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT23-6</td><td>N+N</td><td>20</td><td>7</td><td>-</td><td>-</td><td>19</td><td>25</td><td>0.45</td><td>1</td><td>14.9</td><td>568</td><td><a href="./202006/P020200617573081059435.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>SOT23-3</td><td>N</td><td>20</td><td>8</td><td>-</td><td>-</td><td>12</td><td>15</td><td>0.4</td><td>1</td><td>23</td><td>770</td><td><a href="./202006/P020200617572324291547.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TO-252</td><td>N</td><td>20</td><td>80</td><td>3.6</td><td>5</td><td>3</td><td>4.5</td><td>0.4</td><td>1</td><td>104</td><td>3386</td><td><a href="./202006/P020200617538395463092.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr><tr><td>TSSOP-8</td><td>N</td><td>20</td><td>10</td><td>12</td><td>15</td><td>16</td><td>20</td><td>0.45</td><td>1</td><td>21.7</td><td>758</td><td><a href="./202006/P020200617538124632205.pdf" class="crm-search-bro" target="_blank">预览</a></td></tr></tbody>
     </table>
     ''']
     json = table2json.table2json(text, [0, 1, 2], [3])
     print(json)
 
 示例二:
-```python
+​```python
 	"""
 	author:tieyongjie
 	desc: html_是带有图片,pdf的的html文本,获取到类似{'Image':'/upload/category/module_1.gif',
 	'DataSheet': '/download.asp?STARCAP_Datasheet_SM_20180710.pdf'}
 	"""
 
 	from table.tableX import table2parser
@@ -1327,8 +1325,27 @@
     # json = table2json.table2jsonStr(text, [0, 1, 2], [3])
     print(json)
 ```
 
 ### 2、table2jsonStr方法
 说明：跟table2json类似，只是返回参数是json字符串
 
+### 3、combining_json方法
+
+```
+from tableX.combining import combining_json
+table_html = """
+<table style="width: 100%;"><tbody><tr style="height:27px" class="firstRow"><td width="366" valign="top" colspan="3" style="padding: 0px 7px; border-width: 1px; border-color: windowtext; word-break: break-word;"><p>Item</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Specifications</p></td></tr><tr style="height:18px"><td width="129" valign="top" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="10" colspan="1"><p>GPS&nbsp;Antenna</p></td><td width="71" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5" colspan="1"><p>Dielectric</p><p>Antenna</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency&nbsp;Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>1575.42±3MHz</p></td></tr><tr style="height:18px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>RHCP</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2dBic（Zenith）</p></td></tr><tr style="height:11px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜1.5</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td width="71" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext; word-break: break-word;" rowspan="5" colspan="1"><p>LNA</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext; word-break: break-word;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>28±2dB</p></td></tr><tr style="height:15px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Noise Figure</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜1.5dB</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜2.0</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Supply Voltage</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>3~5V DC</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Current Consumption</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜15mA</p></td></tr><tr style="height:27px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>LTE&nbsp;Antenna&nbsp;MAIN</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top-width: 1px; border-top-color: windowtext; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>698~960MHz/1710~2690MHz</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜3.0</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Linear</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2.5dBi（Zenith）</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>LTE&nbsp;Antenna&nbsp;AUX</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Frequency Range</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>698~960MHz/1710~2690MHz</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>V.S.W.R</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>＜3.0</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Polarization</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Linear</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Gain</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>2.0dBi（Zenith）</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Impedance</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>50Ω</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="4"><p>Mechanical</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Cable</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>RG174</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Connector</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>SMA/FAKRA or others</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Material</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>ABS</p></td></tr><tr style="height:13px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Mounting Method</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Adhesive/Magnet</p></td></tr><tr style="height:6px"><td valign="top" colspan="2" style="padding: 0px 7px; border-left-width: 1px; border-left-color: windowtext; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;" rowspan="5"><p>Environmental</p></td><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Operating Temperature</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>-40℃~+85℃</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Relative Humidity</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Up to 95%</p></td></tr><tr style="height:12px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Ingress Protection</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>IP67</p></td></tr><tr style="height:6px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Vibration</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>10 to 55Hz with 1.5mm amplitude 2hours</p></td></tr><tr style="height:27px"><td width="166" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>Environmentally Friendly</p></td><td width="251" valign="top" style="padding: 0px 7px; border-left: none; border-right-width: 1px; border-right-color: windowtext; border-top: none; border-bottom-width: 1px; border-bottom-color: windowtext;"><p>ROHS Compliant</p></td></tr></tbody></table>
+"""
+
+if __name__ == '__main__':
+    json_dic_s = combining_json(table_html, col=[0,1,2], tagSep=';',keySep='|')
+    print(json_dic_s)
+```
+
+**tagSep**:多value合并时切分符号,默认";"
+**keySep:** 多个key值合并时分隔符,默认空格
+
+**col**:列表,需要合并的列号,默认合并首列
 
+**table_html**: 输入需要转成json的列table
+**return** : 返回的字典组成的列表
```

### Comparing `tableX-0.1.2/test/test.py` & `tableX-0.1.3/test/test.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/test2.py` & `tableX-0.1.3/test/test2.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/test3.py` & `tableX-0.1.3/test/test3.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/test4.py` & `tableX-0.1.3/test/test4.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/test5.py` & `tableX-0.1.3/test/test5.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/test_yj.py` & `tableX-0.1.3/test/test_yj.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/testjjw.py` & `tableX-0.1.3/test/testjjw.py`

 * *Files identical despite different names*

### Comparing `tableX-0.1.2/test/testth.py` & `tableX-0.1.3/test/testth.py`

 * *Files identical despite different names*

