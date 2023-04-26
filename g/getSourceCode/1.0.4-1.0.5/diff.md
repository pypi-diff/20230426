# Comparing `tmp/getSourceCode-1.0.4.tar.gz` & `tmp/getSourceCode-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getSourceCode-1.0.4.tar", last modified: Mon Apr 10 08:17:09 2023, max compression
+gzip compressed data, was "getSourceCode-1.0.5.tar", last modified: Tue Apr 25 15:28:56 2023, max compression
```

## Comparing `getSourceCode-1.0.4.tar` & `getSourceCode-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.963257 getSourceCode-1.0.4/
--rw-rw-rw-   0        0        0     7236 2023-04-10 08:17:09.951721 getSourceCode-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5614 2023-04-10 08:16:44.000000 getSourceCode-1.0.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.918842 getSourceCode-1.0.4/getSourceCode/
--rw-rw-rw-   0        0        0    28636 2023-04-10 08:16:33.000000 getSourceCode-1.0.4/getSourceCode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-10 08:17:09.944703 getSourceCode-1.0.4/getSourceCode.egg-info/
--rw-rw-rw-   0        0        0     7236 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-04-10 08:17:09.000000 getSourceCode-1.0.4/getSourceCode.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 08:17:09.964768 getSourceCode-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-04-10 08:16:50.000000 getSourceCode-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.891213 getSourceCode-1.0.5/
+-rw-rw-rw-   0        0        0     7236 2023-04-25 15:28:56.890212 getSourceCode-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5614 2023-04-10 08:16:44.000000 getSourceCode-1.0.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.871693 getSourceCode-1.0.5/getSourceCode/
+-rw-rw-rw-   0        0        0    28916 2023-04-25 15:27:34.000000 getSourceCode-1.0.5/getSourceCode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 15:28:56.887215 getSourceCode-1.0.5/getSourceCode.egg-info/
+-rw-rw-rw-   0        0        0     7236 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-04-25 15:28:56.000000 getSourceCode-1.0.5/getSourceCode.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 15:28:56.891213 getSourceCode-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-04-25 15:28:48.000000 getSourceCode-1.0.5/setup.py
```

### Comparing `getSourceCode-1.0.4/PKG-INFO` & `getSourceCode-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
```

### Comparing `getSourceCode-1.0.4/README.rst` & `getSourceCode-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `getSourceCode-1.0.4/getSourceCode/__init__.py` & `getSourceCode-1.0.5/getSourceCode/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import base64
 import json
 import os
 import re
 
 apiKeys = {
     "cronos": [],
-    "opt":[
+    "opt": [
         "M88PMFFAS2KAAT71X6UP491MHWA9VMU6V6",
         "NW3G4BUUVFD1D1YRFQSYGDWFZ81KY9K758",
         "2CEAVWSQMGTSTA4A6QS95NHYBPU6SDWMMK"
     ],
     "heco": [
         "JCTU517KN68FM9APHJWPQ7FVPHKFIAUCZB",
         "GWB1A9WKKFVQCE572YH8TA6CHRNVE42R41",
@@ -171,14 +171,19 @@
                   "IWZMJSBHN17PGCFHXY1EFTGVXZUSIF7FUC"],
     "moonbeam": ["PPGYVB7AR97IDSVKZZJ7TD67WVNDBM74AY", "IV47Y5R8SRKW9KC5DVDYB5RVC3GCV5IHKA",
                  "MQPRQUKMHEFRE7KK6WFXIHZTDMC8RCWX65"],
     "moonbase": ["", "", ""],
     "boba": ["8KNECUPEU3FW673BA65P5MD13WRHHWVWTX", "UMBCJRG9TNMB4UUPF4CC679AAPZYRXRRH6",
              "UYDGY2WRN29IG27YSVJ5NNQ3792VZQAH2A"],
     "boba-testnet": ["", "", ""],
+    "gnosis": [
+        "RUBJM9NNIX5HK1H7IPBZ9HJQUVDIZPF9H2",
+        "7QQXJ18WJ6RU3EY8C2YXUP6Z3NMPWVQHB2",
+        "S9VEA15ASFT95YJ1H69WH34VCNEFEVQAX4"
+    ]
 }
 
 defaultFolder = "contract"
 
 reqUrl = {
     "heco": "https://api.hecoinfo.com/api?module=contract&action=getsourcecode&address=",
     "opt": "https://api-optimistic.etherscan.io/api?module=contract&action=getsourcecode&address=",
@@ -199,15 +204,16 @@
     "poly-testnet": "https://api-testnet.polygonscan.com/api?module=contract&action=getsourcecode&address=",
     "avax-testnet": "https://api-testnet.snowtrace.io/api?module=contract&action=getsourcecode&address=",
     "arbi-testnet": "https://api-testnet.arbiscan.io/api?module=contract&action=getsourcecode&address=",
     "moonriver": "https://api-moonriver.moonscan.io/api?module=contract&action=getsourcecode&address=",
     "moonbeam": "https://api-moonbeam.moonscan.io/api?module=contract&action=getsourcecode&address=",
     "moonbase": "https://api-moonbase.moonscan.io/api?module=contract&action=getsourcecode&address=",
     "boba": "https://api.bobascan.com/api?module=contract&action=getsourcecode&address=",
-    "boba-testnet": "https://api-testnet.bobascan.com/api?module=contract&action=getsourcecode&address="
+    "boba-testnet": "https://api-testnet.bobascan.com/api?module=contract&action=getsourcecode&address=",
+    "gnosis": "https://api.gnosisscan.io/api?module=contract&action=getsourcecode&address="
 
 }
 
 txhashConfig = {
     'eth': {
         "url": "https://etherscan.io/vmtrace?txhash={}&type=parity#raw",
         "re": r"<preid='editor'>(.*?)</pre>"
@@ -268,17 +274,18 @@
 
 contractIndex = 0
 
 contractInfo = {}
 
 proxyContract = {}
 
+
 def _argparse():
     parser = argparse.ArgumentParser(
-        description="To get contract source code. \n\nSupport network: \nHeco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron\nCronos|moonbeam|moonriver|boba|okex|opt\navax-testnet|arbi-testnet|poly-testnet\nbsc-testnet|heco-testnet|ftm-testnet\nGoerli|Kovan|Rinkeby|Ropsten\nmoonbase|boba-testnet\n\nGet code by tx only supports:\nBSC|ETH|BOBA|ARBI|HECO",
+        description="To get contract source code. \n\nSupport network: \nHeco|ETH|BSC|Fantom|Poly|AVAX|ARBI|Tron\nCronos|moonbeam|moonriver|boba|okex|opt\navax-testnet|arbi-testnet|poly-testnet\nbsc-testnet|heco-testnet|ftm-testnet\nGoerli|Kovan|Rinkeby|Ropsten\nmoonbase|boba-testnet|gnosis\n\nGet code by tx only supports:\nBSC|ETH|BOBA|ARBI|HECO",
         formatter_class=RawTextHelpFormatter)
     parser.add_argument('-i', default='', dest='inputFile', help='Input file path including contract addresses.')
     parser.add_argument('-o', default='', dest='outputFolder', help='Choose a folder to export.')
     parser.add_argument('-a', default='', dest='address', help='A string including contract addresses.')
     parser.add_argument('-n', default='', dest='network', help='Which network to get source code.')
     parser.add_argument('-k', action="store_true", dest='key', help='Provide some api keys.')
     parser.add_argument('-p', default='', dest='proxy', help='Use a proxy.')
@@ -364,15 +371,15 @@
                 addresses = getAddresses(inputFile, False, "")
             elif address != "":
                 addresses = getAddresses("", False, address)
             else:
                 print("Erorr input")
                 os._exit(0)
             if addresses != []:
-                sendRequest(addresses, outputFolder, network,"")
+                sendRequest(addresses, outputFolder, network, "")
             else:
                 print("Erorr address")
                 os._exit(0)
     except Exception as e:
         print("--------------------------------------")
         print("error line:", e.__traceback__.tb_lineno)
         print("error type:", e)
@@ -415,15 +422,15 @@
         print("--------------------------------------")
         print("error line:", e.__traceback__.tb_lineno)
         print("error type:", e)
         print("--------------------------------------")
         os._exit(0)
 
 
-def exportResult(result, outputFolder, network, address,typeOf):
+def exportResult(result, outputFolder, network, address, typeOf):
     global contractIndex
     if "ContractName" not in result.keys():
         return
     try:
         index = 0
         isMultiFile = False
         contractName = result['ContractName']
@@ -462,26 +469,26 @@
             with open(contractFolder + "//" + contractName, "w+", encoding='utf-8') as fw:
                 fw.write(sourceCode.replace('\r\n', '\n'))
             print(f'{contractIndex}: {contractFolder + "/" + contractName}'.replace('//', '/'))
             contractIndex += 1
         if network == "cronos":
             if result["IsProxy"] == True:
                 if typeOf == "bytx":
-                    proxyContract[address]=result['ImplementationAddress']
+                    proxyContract[address] = result['ImplementationAddress']
                     return
                 addresses = []
                 addresses.append(result['ImplementationAddress'])
-                sendRequest(addresses, "ImplementationAddress", network,"")
+                sendRequest(addresses, "ImplementationAddress", network, "")
         elif result['Implementation'] != "":
             if typeOf == "bytx":
                 proxyContract[address] = result['Implementation']
                 return
             addresses = []
             addresses.append(result['Implementation'])
-            sendRequest(addresses, "Implementation", network,"")
+            sendRequest(addresses, "Implementation", network, "")
     except Exception as e:
         print("--------------------------------------")
         print("error line:", e.__traceback__.tb_lineno)
         print("error type:", e)
         print("--------------------------------------")
         os._exit(0)
 
@@ -493,15 +500,15 @@
     if not isExists:
         os.makedirs(path)
         return True
     else:
         return False
 
 
-def sendRequest(addresses, outputFolder, network,typeOf):
+def sendRequest(addresses, outputFolder, network, typeOf):
     try:
         proxies = {
             "https": "http://" + proxy,
             "http": "http://" + proxy
         }
         header = {
             'user-agent': "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36"
@@ -515,15 +522,15 @@
                 req = requests.get(realUrl, headers=header)
             results = json.loads(req.text)['result']
 
             if type(results) == dict:
                 outputData = results
             elif type(results) == list:
                 outputData = results[0]
-            exportResult(outputData, outputFolder, network, address,typeOf)
+            exportResult(outputData, outputFolder, network, address, typeOf)
     except Exception as e:
         print("--------------------------------------")
         print("error line:", e.__traceback__.tb_lineno)
         print("error type:", e)
         print("--------------------------------------")
         os._exit(0)
 
@@ -671,19 +678,19 @@
             #             os._exit(0)
             getCode(inputFile, outputFolder, address, network)
         elif txhash != "":
             traceTransaction(txhash, proxy, network, outputFolder)
         else:
             print("Invalid command")
             os._exit(0)
-        if contractInfo!={}:
+        if contractInfo != {}:
             print("\nAddress => ContractName:")
             for key in contractInfo.keys():
                 print(f"{key}\t{contractInfo[key]}")
-        if proxyContract!={}:
+        if proxyContract != {}:
             print("\nProxy => Implementation:")
             for key in proxyContract.keys():
                 print(f"{key}\t{proxyContract[key]}")
         print('\nSuccess.')
 
     except Exception as e:
         print("--------------------------------------")
```

### Comparing `getSourceCode-1.0.4/getSourceCode.egg-info/PKG-INFO` & `getSourceCode-1.0.5/getSourceCode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: getSourceCode
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple way to get contract source code.
 Home-page: https://hxzy.me
 Author: hxzy
 Author-email: hxzy0220@gmail.com
 License: UNKNOWN
 Description: getSourceCode
         =============
```

