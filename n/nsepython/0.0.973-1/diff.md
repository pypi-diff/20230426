# Comparing `tmp/nsepython-0.0.973.tar.gz` & `tmp/nsepython-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsepython-0.0.973.tar", last modified: Wed Sep 28 22:38:46 2022, max compression
+gzip compressed data, was "nsepython-1.tar", last modified: Wed Apr 26 20:37:01 2023, max compression
```

## Comparing `nsepython-0.0.973.tar` & `nsepython-1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-28 22:38:46.094884 nsepython-0.0.973/
--rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-0.0.973/LICENSE
--rw-rw-rw-   0        0        0     2415 2022-09-28 22:38:46.092368 nsepython-0.0.973/PKG-INFO
--rw-rw-rw-   0        0        0     1719 2022-09-28 21:31:36.000000 nsepython-0.0.973/README.md
-drwxrwxrwx   0        0        0        0 2022-09-28 22:38:46.055726 nsepython-0.0.973/nsepython/
--rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-0.0.973/nsepython/__init__.py
--rw-rw-rw-   0        0        0    33536 2022-09-28 20:08:56.000000 nsepython-0.0.973/nsepython/rahu.py
-drwxrwxrwx   0        0        0        0 2022-09-28 22:38:46.090375 nsepython-0.0.973/nsepython.egg-info/
--rw-rw-rw-   0        0        0     2415 2022-09-28 22:38:45.000000 nsepython-0.0.973/nsepython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2022-09-28 22:38:45.000000 nsepython-0.0.973/nsepython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-28 22:38:45.000000 nsepython-0.0.973/nsepython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2022-09-28 22:38:45.000000 nsepython-0.0.973/nsepython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-28 22:38:45.000000 nsepython-0.0.973/nsepython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-28 22:38:46.094884 nsepython-0.0.973/setup.cfg
--rw-rw-rw-   0        0        0     1014 2022-09-28 22:36:55.000000 nsepython-0.0.973/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.128758 nsepython-1/
+-rw-rw-rw-   0        0        0    35176 2021-05-30 09:46:07.000000 nsepython-1/LICENSE
+-rw-rw-rw-   0        0        0     2372 2023-04-26 20:37:01.126130 nsepython-1/PKG-INFO
+-rw-rw-rw-   0        0        0     1682 2023-04-26 20:24:52.000000 nsepython-1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.076778 nsepython-1/nsepython/
+-rw-rw-rw-   0        0        0       44 2021-05-30 09:46:07.000000 nsepython-1/nsepython/__init__.py
+-rw-rw-rw-   0        0        0    36359 2023-04-26 20:23:32.000000 nsepython-1/nsepython/rahu.py
+-rw-rw-rw-   0        0        0    36357 2023-04-26 20:27:16.000000 nsepython-1/nsepython/rahuserver.py
+drwxrwxrwx   0        0        0        0 2023-04-26 20:37:01.119524 nsepython-1/nsepython.egg-info/
+-rw-rw-rw-   0        0        0     2372 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 20:36:54.000000 nsepython-1/nsepython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 20:37:01.129277 nsepython-1/setup.cfg
+-rw-rw-rw-   0        0        0     1008 2023-04-26 20:25:51.000000 nsepython-1/setup.py
```

### Comparing `nsepython-0.0.973/LICENSE` & `nsepython-1/LICENSE`

 * *Files identical despite different names*

### Comparing `nsepython-0.0.973/PKG-INFO` & `nsepython-1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 0.0.973
+Version: 1
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -26,32 +26,29 @@
 
 <p align="left">
   <a href="https://unofficed.com/nse-python/documentation/" target="_blank">
     <img width="200" src="https://github.com/aeron7/nsepython/blob/master/button_read-the-documentation.png" alt="logo">
   </a>
 </p>
 
-The library gets constant updates based on feedbacks. <br/>
-So many of the functions are in beta phase. <br/>
-But to see all beta functions You can see - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
 
 ## Installation
 
 Use the package manager [pip](https://pypi.org/project/nsepython/) to install nsepython.
 
 ```bash
 pip install nsepython
 ```
 ## Cross Library Migration
 All the functions of the two famous packages NsepY and NSETools are also migrated here with same function name. <br/>
 They were both unmaintained since long time.
 
-## Advanced Usecases 
+## Advanced Usecases
 [Calculate any Option Greek using Black Scholes Formula in Python](https://unofficed.com/black-scholes-formula-in-python/)
 
 [ How to find the beta of Indian stocks using Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-python/)
 
+[How to get Historical PE, PB and Dividend Ratio of any index using Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+
 ## Contributing
 For Discussion and Improving this Code, Join - https://www.unofficed.com/chat/
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: nsepython Version: 0.0.973 Summary: Python library
-for NSE India APIs Home-page: https://github.com/aeron7/nsepython Author:
-Aeron7 Author-email: dexter@unofficed.com Keywords:
+Metadata-Version: 2.1 Name: nsepython Version: 1 Summary: Python library for
+NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
+Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Description-Content-Type: text/markdown License-
 File: LICENSE
 [logo]
 #### NSEPython is a Python library to get publicly available data on the
 current [NSEIndia](https://nseindia.com) and [NIFTY Indices](https://
 www.niftyindices.com/) site by communicating with their REST APIs.
 [logo]
-The library gets constant updates based on feedbacks.
-So many of the functions are in beta phase.
-But to see all beta functions You can see - [https://forum.unofficed.com/t/
-nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-
-documentation/376/107) ## Installation Use the package manager [pip](https://
-pypi.org/project/nsepython/) to install nsepython. ```bash pip install
-nsepython ``` ## Cross Library Migration All the functions of the two famous
-packages NsepY and NSETools are also migrated here with same function name.
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-
+documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/
+376/107) ## Installation Use the package manager [pip](https://pypi.org/
+project/nsepython/) to install nsepython. ```bash pip install nsepython ``` ##
+Cross Library Migration All the functions of the two famous packages NsepY and
+NSETools are also migrated here with same function name.
 They were both unmaintained since long time. ## Advanced Usecases [Calculate
 any Option Greek using Black Scholes Formula in Python](https://unofficed.com/
 black-scholes-formula-in-python/) [ How to find the beta of Indian stocks using
 Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-
-python/) ## Contributing For Discussion and Improving this Code, Join - https:/
-/www.unofficed.com/chat/ ## License [MIT](https://choosealicense.com/licenses/
-mit/)
+python/) [How to get Historical PE, PB and Dividend Ratio of any index using
+Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+## Contributing For Discussion and Improving this Code, Join - https://
+www.unofficed.com/chat/
```

### Comparing `nsepython-0.0.973/README.md` & `nsepython-1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,29 @@
 
 <p align="left">
   <a href="https://unofficed.com/nse-python/documentation/" target="_blank">
     <img width="200" src="https://github.com/aeron7/nsepython/blob/master/button_read-the-documentation.png" alt="logo">
   </a>
 </p>
 
-The library gets constant updates based on feedbacks. <br/>
-So many of the functions are in beta phase. <br/>
-But to see all beta functions You can see - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
 
 ## Installation
 
 Use the package manager [pip](https://pypi.org/project/nsepython/) to install nsepython.
 
 ```bash
 pip install nsepython
 ```
 ## Cross Library Migration
 All the functions of the two famous packages NsepY and NSETools are also migrated here with same function name. <br/>
 They were both unmaintained since long time.
 
-## Advanced Usecases 
+## Advanced Usecases
 [Calculate any Option Greek using Black Scholes Formula in Python](https://unofficed.com/black-scholes-formula-in-python/)
 
 [ How to find the beta of Indian stocks using Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-python/)
 
+[How to get Historical PE, PB and Dividend Ratio of any index using Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+
 ## Contributing
 For Discussion and Improving this Code, Join - https://www.unofficed.com/chat/
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
 [logo]
 #### NSEPython is a Python library to get publicly available data on the
 current [NSEIndia](https://nseindia.com) and [NIFTY Indices](https://
 www.niftyindices.com/) site by communicating with their REST APIs.
 [logo]
-The library gets constant updates based on feedbacks.
-So many of the functions are in beta phase.
-But to see all beta functions You can see - [https://forum.unofficed.com/t/
-nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-
-documentation/376/107) ## Installation Use the package manager [pip](https://
-pypi.org/project/nsepython/) to install nsepython. ```bash pip install
-nsepython ``` ## Cross Library Migration All the functions of the two famous
-packages NsepY and NSETools are also migrated here with same function name.
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-
+documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/
+376/107) ## Installation Use the package manager [pip](https://pypi.org/
+project/nsepython/) to install nsepython. ```bash pip install nsepython ``` ##
+Cross Library Migration All the functions of the two famous packages NsepY and
+NSETools are also migrated here with same function name.
 They were both unmaintained since long time. ## Advanced Usecases [Calculate
 any Option Greek using Black Scholes Formula in Python](https://unofficed.com/
 black-scholes-formula-in-python/) [ How to find the beta of Indian stocks using
 Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-
-python/) ## Contributing For Discussion and Improving this Code, Join - https:/
-/www.unofficed.com/chat/ ## License [MIT](https://choosealicense.com/licenses/
-mit/)
+python/) [How to get Historical PE, PB and Dividend Ratio of any index using
+Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+## Contributing For Discussion and Improving this Code, Join - https://
+www.unofficed.com/chat/
```

### Comparing `nsepython-0.0.973/nsepython/rahu.py` & `nsepython-1/nsepython/rahu.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,55 +6,61 @@
 import pandas as pd
 import json
 import random
 import datetime,time
 import logging
 import re
 
-mode ='local'
-
-if(mode=='local'):
 
-    headers = {
-        'Connection': 'keep-alive',
-        'Cache-Control': 'max-age=0',
-        'DNT': '1',
-        'Upgrade-Insecure-Requests': '1',
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.79 Safari/537.36',
-        'Sec-Fetch-User': '?1',
-        'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
-        'Sec-Fetch-Site': 'none',
-        'Sec-Fetch-Mode': 'navigate',
-        'Accept-Encoding': 'gzip, deflate, br',
-        'Accept-Language': 'en-US,en;q=0.9,hi;q=0.8',
-    }
+mode ='local'
 
+if(mode=='vpn'):
     def nsefetch(payload):
+        if (("%26" in payload) or ("%20" in payload)):
+            encoded_url = payload
+        else:
+            encoded_url = urllib.parse.quote(payload, safe=':/?&=')
+        payload_var = 'curl -b cookies.txt "' + encoded_url + '"' + curl_headers + ''
         try:
-            output = requests.get(payload,headers=headers).json()
-            #print(output)
-        except ValueError:
-            s =requests.Session()
-            output = s.get("http://nseindia.com",headers=headers)
-            output = s.get(payload,headers=headers).json()
+            output = os.popen(payload_var).read()
+            output=json.loads(output)
+        except ValueError:  # includes simplejson.decoder.JSONDecodeError:
+            payload2 = "https://www.nseindia.com"
+            output2 = os.popen('curl -c cookies.txt "'+payload2+'"'+curl_headers+'').read()
+    
+            output = os.popen(payload_var).read()
+            output=json.loads(output)
+        return output
+if(mode=='local'):
+    def nsefetch(payload):
+        output = requests.get(payload,headers=headers).json()
         return output
-
-run_time=datetime.datetime.now()
-
-#Constants
-indices = ['NIFTY','FINNIFTY','BANKNIFTY']
-
-
-
-
 
 
+headers = {
+    'Connection': 'keep-alive',
+    'Cache-Control': 'max-age=0',
+    'DNT': '1',
+    'Upgrade-Insecure-Requests': '1',
+    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.79 Safari/537.36',
+    'Sec-Fetch-User': '?1',
+    'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9',
+    'Sec-Fetch-Site': 'none',
+    'Sec-Fetch-Mode': 'navigate',
+    'Accept-Encoding': 'gzip, deflate, br',
+    'Accept-Language': 'en-US,en;q=0.9,hi;q=0.8',
+}
 
+#Curl headers
+curl_headers = ''' -H "authority: beta.nseindia.com" -H "cache-control: max-age=0" -H "dnt: 1" -H "upgrade-insecure-requests: 1" -H "user-agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.117 Safari/537.36" -H "sec-fetch-user: ?1" -H "accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9" -H "sec-fetch-site: none" -H "sec-fetch-mode: navigate" -H "accept-encoding: gzip, deflate, br" -H "accept-language: en-US,en;q=0.9,hi;q=0.8" --compressed'''
 
+run_time=datetime.datetime.now()
 
+#Constants
+indices = ['NIFTY','FINNIFTY','BANKNIFTY']
 
 def running_status():
     start_now=datetime.datetime.now().replace(hour=9, minute=15, second=0, microsecond=0)
     end_now=datetime.datetime.now().replace(hour=15, minute=30, second=0, microsecond=0)
     return start_now<datetime.datetime.now()<end_now
 
 #Getting FNO Symboles
@@ -81,15 +87,15 @@
     if any(x in symbol for x in indices):
         payload = nsefetch('https://www.nseindia.com/api/option-chain-indices?symbol='+symbol)
     else:
         payload = nsefetch('https://www.nseindia.com/api/option-chain-equities?symbol='+symbol)
     return payload
 
 
-def oi_chain_builder (symbol,expiry="latest",oi_mode="full"):
+def oi_chain_builder(symbol,expiry="latest",oi_mode="full"):
 
     payload = nse_optionchain_scrapper(symbol)
 
     if(oi_mode=='compact'):
         col_names = ['CALLS_OI','CALLS_Chng in OI','CALLS_Volume','CALLS_IV','CALLS_LTP','CALLS_Net Chng','Strike Price','PUTS_OI','PUTS_Chng in OI','PUTS_Volume','PUTS_IV','PUTS_LTP','PUTS_Net Chng']
     if(oi_mode=='full'):
         col_names = ['CALLS_Chart','CALLS_OI','CALLS_Chng in OI','CALLS_Volume','CALLS_IV','CALLS_LTP','CALLS_Net Chng','CALLS_Bid Qty','CALLS_Bid Price','CALLS_Ask Price','CALLS_Ask Qty','Strike Price','PUTS_Bid Qty','PUTS_Bid Price','PUTS_Ask Price','PUTS_Ask Qty','PUTS_Net Chng','PUTS_LTP','PUTS_IV','PUTS_Volume','PUTS_Chng in OI','PUTS_OI','PUTS_Chart']
@@ -140,27 +146,39 @@
                     if(oi_mode=='full'):
                         oi_row['PUTS_Bid Qty'],oi_row['PUTS_Bid Price'],oi_row['PUTS_Ask Price'],oi_row['PUTS_Ask Qty']=0,0,0,0
             else:
                 logging.info(m)
 
             if(oi_mode=='full'):
                 oi_row['CALLS_Chart'],oi_row['PUTS_Chart']=0,0
-            oi_data = oi_data.append(oi_row, ignore_index=True)
+            #oi_data = oi_data.append(oi_row, ignore_index=True)
+            #oi_data = pd.concat([oi_data, oi_row], ignore_index=True)
+            oi_data = pd.concat([oi_data, pd.DataFrame([oi_row])], ignore_index=True)
 
+
+
+            oi_data['time_stamp']=payload['records']['timestamp']
     return oi_data,float(payload['records']['underlyingValue']),payload['records']['timestamp']
 
 
-def nse_quote(symbol):
+def nse_quote(symbol,section=""):
+    #https://forum.unofficed.com/t/nsetools-get-quote-is-not-fetching-delivery-data-and-delivery-can-you-include-this-as-part-of-feature-request/1115/4    
     symbol = nsesymbolpurify(symbol)
 
-    if any(x in symbol for x in fnolist()):
-        payload = nsefetch('https://www.nseindia.com/api/quote-derivative?symbol='+symbol)
-    else:
-        payload = nsefetch('https://www.nseindia.com/api/quote-equity?symbol='+symbol)
-    return payload
+    if(section==""):
+        if any(x in symbol for x in fnolist()):
+            payload = nsefetch('https://www.nseindia.com/api/quote-derivative?symbol='+symbol)
+        else:
+            payload = nsefetch('https://www.nseindia.com/api/quote-equity?symbol='+symbol)
+        return payload
+    
+    if(section!=""):
+        payload = nsefetch('https://www.nseindia.com/api/quote-equity?symbol='+symbol+'&section='+section)            
+        return payload
+
 
 def nse_expirydetails(payload,i=0):
     currentExpiry = payload['records']['expiryDates'][i]
     currentExpiry = datetime.datetime.strptime(currentExpiry,'%d-%b-%Y').date()  # converting json datetime to alice datetime
     date_today = run_time.strftime('%Y-%m-%d')  # required to remove hh:mm:ss
     date_today = datetime.datetime.strptime(date_today,'%Y-%m-%d').date()
     dte = (currentExpiry - date_today).days
@@ -506,15 +524,17 @@
   vega = ((1/100)*S0*math.exp(-r*t)*math.sqrt(t))*(1/(math.sqrt(2*math.pi))*math.exp(-(d1*d1)/2))
   call_rho =(1/100)*X*t*math.exp(-r*t)*norm.cdf(d2)
   put_rho =(-1/100)*X*t*math.exp(-r*t)*norm.cdf(-d2)
 
   return call_theta,put_theta,call_premium,put_premium,call_delta,put_delta,gamma,vega,call_rho,put_rho
 
 def equity_history_virgin(symbol,series,start_date,end_date):
-    url="https://www.nseindia.com/api/historical/cm/equity?symbol="+symbol+"&series=[%22"+series+"%22]&from="+str(start_date)+"&to="+str(end_date)+""
+    #url="https://www.nseindia.com/api/historical/cm/equity?symbol="+symbol+"&series=[%22"+series+"%22]&from="+str(start_date)+"&to="+str(end_date)+""
+    url = 'https://www.nseindia.com/api/historical/cm/equity?symbol=' + symbol + '&series=["' + series + '"]&from=' + start_date + '&to=' + end_date
+
     payload = nsefetch(url)
     return pd.DataFrame.from_records(payload["data"])
 
 # You shall see beautiful use the logger function.
 def equity_history(symbol,series,start_date,end_date):
     #We are getting the input in text. So it is being converted to Datetime object from String.
     start_date = datetime.datetime.strptime(start_date, "%d-%m-%Y")
@@ -537,15 +557,18 @@
 
         logging.info("Loop = "+str(i))
         logging.info("====")
         logging.info("Starting Date: "+str(start_date))
         logging.info("Ending Date: "+str(temp_date))
         logging.info("====")
 
-        total=total.append(equity_history_virgin(symbol,series,start_date,temp_date))
+        #total=total.append(equity_history_virgin(symbol,series,start_date,temp_date))
+        #total=total.concat(equity_history_virgin(symbol,series,start_date,temp_date))
+        total = pd.concat([total, equity_history_virgin(symbol, series, start_date, temp_date)])
+
 
         logging.info("Length of the Table: "+ str(len(total)))
 
         #Preparation for the next loop
         start_date = datetime.datetime.strptime(temp_date, "%d-%m-%Y")
 
 
@@ -554,15 +577,18 @@
 
     logging.info("End Loop")
     logging.info("====")
     logging.info("Starting Date: "+str(start_date))
     logging.info("Ending Date: "+str(end_date))
     logging.info("====")
 
-    total=total.append(equity_history_virgin(symbol,series,start_date,end_date))
+    #total=total.append(equity_history_virgin(symbol,series,start_date,end_date))
+    #total=total.concat(equity_history_virgin(symbol,series,start_date,end_date))
+    total = pd.concat([total, equity_history_virgin(symbol, series, start_date, end_date)])
+
 
     logging.info("Finale")
     logging.info("Length of the Total Dataset: "+ str(len(total)))
     payload = total.iloc[::-1].reset_index(drop=True)
     return payload
 
 def derivative_history_virgin(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice="",optionType=""):
@@ -578,14 +604,15 @@
 
     if(((instrumentType=="OPTIDX")or (instrumentType=="OPTSTK")) and (expiry_date!="")):
         strikePrice = "%.2f" % strikePrice
         strikePrice = str(strikePrice)
 
     nsefetch_url = "https://www.nseindia.com/api/historical/fo/derivatives?&from="+str(start_date)+"&to="+str(end_date)+"&optionType="+optionType+"&strikePrice="+strikePrice+"&expiryDate="+expiry_date+"&instrumentType="+instrumentType+"&symbol="+symbol+""
     payload = nsefetch(nsefetch_url)
+    logging.info(nsefetch_url)
     logging.info(payload)
     return pd.DataFrame.from_records(payload["data"])
 
 def derivative_history(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice="",optionType=""):
     #We are getting the input in text. So it is being converted to Datetime object from String.
     start_date = datetime.datetime.strptime(start_date, "%d-%m-%Y")
     end_date = datetime.datetime.strptime(end_date, "%d-%m-%Y")
@@ -607,15 +634,18 @@
 
         logging.info("Loop = "+str(i))
         logging.info("====")
         logging.info("Starting Date: "+str(start_date))
         logging.info("Ending Date: "+str(temp_date))
         logging.info("====")
 
-        total=total.append(derivative_history_virgin(symbol,start_date,temp_date,instrumentType,expiry_date,strikePrice,optionType))
+        #total=total.append(derivative_history_virgin(symbol,start_date,temp_date,instrumentType,expiry_date,strikePrice,optionType))
+        #total=total.concat([total, derivative_history_virgin(symbol,start_date,temp_date,instrumentType,expiry_date,strikePrice,optionType)])
+        total = pd.concat([total, derivative_history_virgin(symbol, start_date, temp_date, instrumentType, expiry_date, strikePrice, optionType)])
+
 
         logging.info("Length of the Table: "+ str(len(total)))
 
         #Preparation for the next loop
         start_date = datetime.datetime.strptime(temp_date, "%d-%m-%Y")
 
 
@@ -624,15 +654,19 @@
 
     logging.info("End Loop")
     logging.info("====")
     logging.info("Starting Date: "+str(start_date))
     logging.info("Ending Date: "+str(end_date))
     logging.info("====")
 
-    total=total.append(derivative_history_virgin(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice,optionType))
+    #total=total.append(derivative_history_virgin(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice,optionType))
+    #total = total.concat([total, derivative_history_virgin(symbol,start_date,end_date,instrumentType,expiry_date,strikePrice,optionType)])
+    total = pd.concat([total, derivative_history_virgin(symbol, start_date, end_date, instrumentType, expiry_date, strikePrice, optionType)])
+
+
 
     logging.info("Finale")
     logging.info("Length of the Total Dataset: "+ str(len(total)))
     payload = total.iloc[::-1].reset_index(drop=True)
     return payload
 
 
@@ -766,7 +800,10 @@
 # sort = "volume"
 # sort = "value"
 
 def nse_most_active(type="securities",sort="value"):
     payload = nsefetch("https://www.nseindia.com/api/live-analysis-most-active-"+type+"?index="+sort+"")
     payload = pd.DataFrame(payload["data"])
     return payload
+
+
+def nse_eq_symbols():
```

### Comparing `nsepython-0.0.973/nsepython.egg-info/PKG-INFO` & `nsepython-1/nsepython.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nsepython
-Version: 0.0.973
+Version: 1
 Summary: Python library for NSE India APIs
 Home-page: https://github.com/aeron7/nsepython
 Author: Aeron7
 Author-email: dexter@unofficed.com
 Keywords: nseindia,nse,python,sdk,trading,stock markets
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
@@ -26,32 +26,29 @@
 
 <p align="left">
   <a href="https://unofficed.com/nse-python/documentation/" target="_blank">
     <img width="200" src="https://github.com/aeron7/nsepython/blob/master/button_read-the-documentation.png" alt="logo">
   </a>
 </p>
 
-The library gets constant updates based on feedbacks. <br/>
-So many of the functions are in beta phase. <br/>
-But to see all beta functions You can see - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/376/107)
 
 ## Installation
 
 Use the package manager [pip](https://pypi.org/project/nsepython/) to install nsepython.
 
 ```bash
 pip install nsepython
 ```
 ## Cross Library Migration
 All the functions of the two famous packages NsepY and NSETools are also migrated here with same function name. <br/>
 They were both unmaintained since long time.
 
-## Advanced Usecases 
+## Advanced Usecases
 [Calculate any Option Greek using Black Scholes Formula in Python](https://unofficed.com/black-scholes-formula-in-python/)
 
 [ How to find the beta of Indian stocks using Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-python/)
 
+[How to get Historical PE, PB and Dividend Ratio of any index using Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+
 ## Contributing
 For Discussion and Improving this Code, Join - https://www.unofficed.com/chat/
-
-## License
-[MIT](https://choosealicense.com/licenses/mit/)
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: nsepython Version: 0.0.973 Summary: Python library
-for NSE India APIs Home-page: https://github.com/aeron7/nsepython Author:
-Aeron7 Author-email: dexter@unofficed.com Keywords:
+Metadata-Version: 2.1 Name: nsepython Version: 1 Summary: Python library for
+NSE India APIs Home-page: https://github.com/aeron7/nsepython Author: Aeron7
+Author-email: dexter@unofficed.com Keywords:
 nseindia,nse,python,sdk,trading,stock markets Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: Implementation :: PyPy Classifier: Topic :: Software Development ::
 Libraries :: Python Modules Description-Content-Type: text/markdown License-
 File: LICENSE
 [logo]
 #### NSEPython is a Python library to get publicly available data on the
 current [NSEIndia](https://nseindia.com) and [NIFTY Indices](https://
 www.niftyindices.com/) site by communicating with their REST APIs.
 [logo]
-The library gets constant updates based on feedbacks.
-So many of the functions are in beta phase.
-But to see all beta functions You can see - [https://forum.unofficed.com/t/
-nsepython-documentation/376/107](https://forum.unofficed.com/t/nsepython-
-documentation/376/107) ## Installation Use the package manager [pip](https://
-pypi.org/project/nsepython/) to install nsepython. ```bash pip install
-nsepython ``` ## Cross Library Migration All the functions of the two famous
-packages NsepY and NSETools are also migrated here with same function name.
+For Support and Beta Functions - [https://forum.unofficed.com/t/nsepython-
+documentation/376/107](https://forum.unofficed.com/t/nsepython-documentation/
+376/107) ## Installation Use the package manager [pip](https://pypi.org/
+project/nsepython/) to install nsepython. ```bash pip install nsepython ``` ##
+Cross Library Migration All the functions of the two famous packages NsepY and
+NSETools are also migrated here with same function name.
 They were both unmaintained since long time. ## Advanced Usecases [Calculate
 any Option Greek using Black Scholes Formula in Python](https://unofficed.com/
 black-scholes-formula-in-python/) [ How to find the beta of Indian stocks using
 Python?](https://unofficed.com/how-to-find-the-beta-of-indian-stocks-using-
-python/) ## Contributing For Discussion and Improving this Code, Join - https:/
-/www.unofficed.com/chat/ ## License [MIT](https://choosealicense.com/licenses/
-mit/)
+python/) [How to get Historical PE, PB and Dividend Ratio of any index using
+Python](https://unofficed.com/nse-python/documentation/nsepy/#index_pe_pb_div)
+## Contributing For Discussion and Improving this Code, Join - https://
+www.unofficed.com/chat/
```

### Comparing `nsepython-0.0.973/setup.py` & `nsepython-1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'nsepython',
     packages=setuptools.find_packages(),
-    version = '0.0.973',
+    version = '1',
     include_package_data=True,
     description = 'Python library for NSE India APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Aeron7',
     author_email = 'dexter@unofficed.com',
     url = 'https://github.com/aeron7/nsepython',
     install_requires=['requests', 'pandas','scipy'],
```

