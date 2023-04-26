# Comparing `tmp/bingpython-0.0.19.tar.gz` & `tmp/bingpython-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingpython-0.0.19.tar", last modified: Wed Mar 22 20:19:30 2023, max compression
+gzip compressed data, was "bingpython-0.0.20.tar", last modified: Wed Apr 26 09:08:11 2023, max compression
```

## Comparing `bingpython-0.0.19.tar` & `bingpython-0.0.20.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.628166 bingpython-0.0.19/
--rw-rw-rw-   0        0        0     1509 2023-03-22 20:19:30.628166 bingpython-0.0.19/PKG-INFO
--rw-rw-rw-   0        0        0      713 2023-03-22 20:04:30.000000 bingpython-0.0.19/README.md
--rw-rw-rw-   0        0        0      111 2023-03-22 20:19:30.629176 bingpython-0.0.19/setup.cfg
--rw-rw-rw-   0        0        0     1228 2023-03-22 20:07:17.000000 bingpython-0.0.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.614009 bingpython-0.0.19/src/
--rw-rw-rw-   0        0        0     7440 2023-03-22 20:19:16.000000 bingpython-0.0.19/src/BingPython.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:19:30.628166 bingpython-0.0.19/src/bingpython.egg-info/
--rw-rw-rw-   0        0        0     1509 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-03-22 20:19:30.000000 bingpython-0.0.19/src/bingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 09:08:11.628652 bingpython-0.0.20/
+-rw-rw-rw-   0        0        0    16725 2023-04-25 12:00:52.000000 bingpython-0.0.20/LICENSE
+-rw-rw-rw-   0        0        0     1532 2023-04-26 09:08:11.629649 bingpython-0.0.20/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2023-04-25 12:00:52.000000 bingpython-0.0.20/README.md
+-rw-rw-rw-   0        0        0      111 2023-04-26 09:08:11.634636 bingpython-0.0.20/setup.cfg
+-rw-rw-rw-   0        0        0     1195 2023-04-25 12:00:52.000000 bingpython-0.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:08:11.600533 bingpython-0.0.20/src/
+-rw-rw-rw-   0        0        0     7448 2023-04-25 12:00:52.000000 bingpython-0.0.20/src/BingPython.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:08:11.625657 bingpython-0.0.20/src/bingpython.egg-info/
+-rw-rw-rw-   0        0        0     1532 2023-04-26 09:08:11.000000 bingpython-0.0.20/src/bingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-04-26 09:08:11.000000 bingpython-0.0.20/src/bingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:08:11.000000 bingpython-0.0.20/src/bingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-26 09:08:11.000000 bingpython-0.0.20/src/bingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 09:08:11.000000 bingpython-0.0.20/src/bingpython.egg-info/top_level.txt
```

### Comparing `bingpython-0.0.19/PKG-INFO` & `bingpython-0.0.20/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: bingpython
-Version: 0.0.19
+Version: 0.0.20
 Summary: Bing AI Chat API
 Home-page: https://github.com/alicangnll/BingGPT-Python
 Author: Ali Can Gönüllü
 Author-email: alicangonullu@yahoo.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-Python/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # BingGPT - Bing AI API on Python
 You can use BingGPT AI API on Python!
 # Requirements
 <ul>
   <li>Python 3.8+</li>
 </ul>
 <h1>Installation</h1>
 <ul>
   <li>pip install -r requirements.txt</li>
-  <li>pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install bingpython</li>
+  <li>pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install bingpython</li>
 </ul>
 <h1>Pictures</h1>
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png" />
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png" />
 <h1>Example</h1>
 <a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example.py">Example Code</a>
 <br><a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example2.py">Example Code 2</a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: bingpython Version: 0.0.19 Summary: Bing AI Chat
+Metadata-Version: 2.1 Name: bingpython Version: 0.0.20 Summary: Bing AI Chat
 API Home-page: https://github.com/alicangnll/BingGPT-Python Author: Ali Can
 GÃ¶nÃ¼llÃ¼ Author-email: alicangonullu@yahoo.com License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-
 Python/issues/new Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-# BingGPT - Bing AI API on Python You can use BingGPT AI API on Python! #
-Requirements
+License-File: LICENSE # BingGPT - Bing AI API on Python You can use BingGPT AI
+API on Python! # Requirements
     * Python 3.8+
 ****** Installation ******
     * pip install -r requirements.txt
-    * pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install
+    * pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install
       bingpython
 ****** Pictures ******
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png]
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png]
 ****** Example ******
 Example_Code
 Example_Code_2
```

### Comparing `bingpython-0.0.19/README.md` & `bingpython-0.0.20/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Requirements
 <ul>
   <li>Python 3.8+</li>
 </ul>
 <h1>Installation</h1>
 <ul>
   <li>pip install -r requirements.txt</li>
-  <li>pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install bingpython</li>
+  <li>pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install bingpython</li>
 </ul>
 <h1>Pictures</h1>
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png" />
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png" />
 <h1>Example</h1>
 <a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example.py">Example Code</a>
 <br><a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example2.py">Example Code 2</a>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # BingGPT - Bing AI API on Python You can use BingGPT AI API on Python! #
 Requirements
     * Python 3.8+
 ****** Installation ******
     * pip install -r requirements.txt
-    * pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install
+    * pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install
       bingpython
 ****** Pictures ******
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png]
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png]
 ****** Example ******
 Example_Code
 Example_Code_2
```

### Comparing `bingpython-0.0.19/setup.py` & `bingpython-0.0.20/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import find_packages
-from setuptools import setup
-
-setup(
-    name="bingpython",
-    version="0.0.19",
-    license="GNU General Public License v2.0",
-    author="Ali Can Gönüllü",
-    author_email="alicangonullu@yahoo.com",
-    description="Bing AI Chat API",
-    packages=find_packages("src"),
-    package_dir={"": "src"},
-    url="https://github.com/alicangnll/BingGPT-Python",
-    project_urls={"Bug Report": "https://github.com/alicangnll/BingGPT-Python/issues/new"},
-    install_requires=[
-        "asyncio",
-        "requests",
-        "websockets",
-        "rich",
-        "certifi",
-        "uuid"
-    ],
-    long_description=open("README.md", encoding="utf-8").read(),
-    long_description_content_type="text/markdown",
-    py_modules=["BingPython"],
-    classifiers=[
-        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-        "Intended Audience :: Developers",
-        "Topic :: Software Development :: Libraries :: Python Modules",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
-)
+from setuptools import find_packages
+from setuptools import setup
+
+setup(
+    name="bingpython",
+    version="0.0.20",
+    license="GNU General Public License v2.0",
+    author="Ali Can Gönüllü",
+    author_email="alicangonullu@yahoo.com",
+    description="Bing AI Chat API",
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    url="https://github.com/alicangnll/BingGPT-Python",
+    project_urls={"Bug Report": "https://github.com/alicangnll/BingGPT-Python/issues/new"},
+    install_requires=[
+        "asyncio",
+        "requests",
+        "websockets",
+        "rich",
+        "certifi",
+        "uuid"
+    ],
+    long_description=open("README.md", encoding="utf-8").read(),
+    long_description_content_type="text/markdown",
+    py_modules=["BingPython"],
+    classifiers=[
+        "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
+)
```

### Comparing `bingpython-0.0.19/src/BingPython.py` & `bingpython-0.0.20/src/BingPython.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,347 +119,348 @@
 00000760: 2070 7269 6e74 2827 2d2d 2d20 436f 6e6e   print('--- Conn
 00000770: 6563 7469 6f6e 2061 7265 2075 6e64 6572  ection are under
 00000780: 2063 6f6e 7472 6f6c 2e20 4c6f 6164 696e   control. Loadin
 00000790: 672e 2e2e 202d 2d2d 2729 0a20 2020 2020  g... ---').     
 000007a0: 2020 2020 2020 2061 7761 6974 2061 7379         await asy
 000007b0: 6e63 696f 2e73 6c65 6570 2835 290a 0a20  ncio.sleep(5).. 
 000007c0: 2020 2061 7379 6e63 2064 6566 2073 656e     async def sen
-000007d0: 6463 6f6d 286c 6f61 6464 6174 612c 2071  dcom(loaddata, q
-000007e0: 7565 7374 696f 6e29 3a0a 2020 2020 2020  uestion):.      
-000007f0: 2020 2320 4a53 4f4e 204c 6f61 640a 2020    # JSON Load.  
-00000800: 2020 2020 2020 6a73 3120 3d20 6a73 6f6e        js1 = json
-00000810: 2e6c 6f61 6473 286c 6f61 6464 6174 6129  .loads(loaddata)
-00000820: 0a0a 2020 2020 2020 2020 2320 5353 4c20  ..        # SSL 
-00000830: 436f 6e74 6578 740a 2020 2020 2020 2020  Context.        
-00000840: 7373 6c5f 636f 6e74 6578 7420 3d20 7373  ssl_context = ss
-00000850: 6c2e 6372 6561 7465 5f64 6566 6175 6c74  l.create_default
-00000860: 5f63 6f6e 7465 7874 2829 0a20 2020 2020  _context().     
-00000870: 2020 2073 736c 5f63 6f6e 7465 7874 2e6c     ssl_context.l
-00000880: 6f61 645f 7665 7269 6679 5f6c 6f63 6174  oad_verify_locat
-00000890: 696f 6e73 2863 6572 7469 6669 2e77 6865  ions(certifi.whe
-000008a0: 7265 2829 290a 0a20 2020 2020 2020 2023  re())..        #
-000008b0: 2048 6561 6465 7273 2061 6e64 2049 5020   Headers and IP 
-000008c0: 4164 6472 6573 7365 730a 2020 2020 2020  Addresses.      
-000008d0: 2020 464f 5257 4152 4445 445f 4950 203d    FORWARDED_IP =
-000008e0: 2028 6622 3133 2e7b 7261 6e64 6f6d 2e72   (f"13.{random.r
-000008f0: 616e 6469 6e74 2831 3034 2c20 3130 3729  andint(104, 107)
-00000900: 7d2e 7b72 616e 646f 6d2e 7261 6e64 696e  }.{random.randin
-00000910: 7428 302c 2032 3535 297d 2e7b 7261 6e64  t(0, 255)}.{rand
-00000920: 6f6d 2e72 616e 6469 6e74 2830 2c20 3235  om.randint(0, 25
-00000930: 3529 7d22 290a 2020 2020 2020 2020 4845  5)}").        HE
-00000940: 4144 4552 5320 3d20 7b0a 2020 2020 2020  ADERS = {.      
-00000950: 2020 2020 2020 2261 6363 6570 7422 3a20        "accept": 
-00000960: 2261 7070 6c69 6361 7469 6f6e 2f6a 736f  "application/jso
-00000970: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00000980: 2261 6363 6570 742d 6c61 6e67 7561 6765  "accept-language
-00000990: 223a 2022 656e 2d55 532c 656e 3b71 3d30  ": "en-US,en;q=0
-000009a0: 2e39 222c 0a20 2020 2020 2020 2020 2020  .9",.           
-000009b0: 2022 636f 6e74 656e 742d 7479 7065 223a   "content-type":
-000009c0: 2022 6170 706c 6963 6174 696f 6e2f 6a73   "application/js
-000009d0: 6f6e 222c 0a20 2020 2020 2020 2020 2020  on",.           
-000009e0: 2022 7365 632d 6368 2d75 6122 3a20 2722   "sec-ch-ua": '"
-000009f0: 4e6f 745f 4120 4272 616e 6422 3b76 3d22  Not_A Brand";v="
-00000a00: 3939 222c 2022 4d69 6372 6f73 6f66 7420  99", "Microsoft 
-00000a10: 4564 6765 223b 763d 2231 3130 222c 2022  Edge";v="110", "
-00000a20: 4368 726f 6d69 756d 223b 763d 2231 3130  Chromium";v="110
-00000a30: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00000a40: 2273 6563 2d63 682d 7561 2d61 7263 6822  "sec-ch-ua-arch"
-00000a50: 3a20 2722 7838 3622 272c 0a20 2020 2020  : '"x86"',.     
-00000a60: 2020 2020 2020 2022 7365 632d 6368 2d75         "sec-ch-u
-00000a70: 612d 6269 746e 6573 7322 3a20 2722 3634  a-bitness": '"64
-00000a80: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
-00000a90: 2273 6563 2d63 682d 7561 2d66 756c 6c2d  "sec-ch-ua-full-
-00000aa0: 7665 7273 696f 6e22 3a20 2722 3130 392e  version": '"109.
-00000ab0: 302e 3135 3138 2e37 3822 272c 0a20 2020  0.1518.78"',.   
-00000ac0: 2020 2020 2020 2020 2022 7365 632d 6368           "sec-ch
-00000ad0: 2d75 612d 6675 6c6c 2d76 6572 7369 6f6e  -ua-full-version
-00000ae0: 2d6c 6973 7422 3a20 2722 4368 726f 6d69  -list": '"Chromi
-00000af0: 756d 223b 763d 2231 3130 2e30 2e35 3438  um";v="110.0.548
-00000b00: 312e 3139 3222 2c20 224e 6f74 2041 2842  1.192", "Not A(B
-00000b10: 7261 6e64 223b 763d 2232 342e 302e 302e  rand";v="24.0.0.
-00000b20: 3022 2c20 224d 6963 726f 736f 6674 2045  0", "Microsoft E
-00000b30: 6467 6522 3b76 3d22 3131 302e 302e 3135  dge";v="110.0.15
-00000b40: 3837 2e36 3922 272c 0a20 2020 2020 2020  87.69"',.       
-00000b50: 2020 2020 2022 7365 632d 6368 2d75 612d       "sec-ch-ua-
-00000b60: 6d6f 6269 6c65 223a 2022 3f30 222c 0a20  mobile": "?0",. 
-00000b70: 2020 2020 2020 2020 2020 2022 7365 632d             "sec-
-00000b80: 6368 2d75 612d 6d6f 6465 6c22 3a20 2222  ch-ua-model": ""
-00000b90: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
-00000ba0: 6563 2d63 682d 7561 2d70 6c61 7466 6f72  ec-ch-ua-platfor
-00000bb0: 6d22 3a20 2722 5769 6e64 6f77 7322 272c  m": '"Windows"',
-00000bc0: 0a20 2020 2020 2020 2020 2020 2022 7365  .            "se
-00000bd0: 632d 6368 2d75 612d 706c 6174 666f 726d  c-ch-ua-platform
-00000be0: 2d76 6572 7369 6f6e 223a 2027 2231 352e  -version": '"15.
-00000bf0: 302e 3022 272c 0a20 2020 2020 2020 2020  0.0"',.         
-00000c00: 2020 2022 7365 632d 6665 7463 682d 6465     "sec-fetch-de
-00000c10: 7374 223a 2022 656d 7074 7922 2c0a 2020  st": "empty",.  
-00000c20: 2020 2020 2020 2020 2020 2273 6563 2d66            "sec-f
-00000c30: 6574 6368 2d6d 6f64 6522 3a20 2263 6f72  etch-mode": "cor
-00000c40: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
-00000c50: 2273 6563 2d66 6574 6368 2d73 6974 6522  "sec-fetch-site"
-00000c60: 3a20 2273 616d 652d 6f72 6967 696e 222c  : "same-origin",
-00000c70: 0a20 2020 2020 2020 2020 2020 2022 782d  .            "x-
-00000c80: 6d73 2d63 6c69 656e 742d 7265 7175 6573  ms-client-reques
-00000c90: 742d 6964 223a 2073 7472 2875 7569 642e  t-id": str(uuid.
-00000ca0: 7575 6964 3428 2929 2c0a 2020 2020 2020  uuid4()),.      
-00000cb0: 2020 2020 2020 2278 2d6d 732d 7573 6572        "x-ms-user
-00000cc0: 6167 656e 7422 3a20 2261 7a73 646b 2d6a  agent": "azsdk-j
-00000cd0: 732d 6170 692d 636c 6965 6e74 2d66 6163  s-api-client-fac
-00000ce0: 746f 7279 2f31 2e30 2e30 2d62 6574 612e  tory/1.0.0-beta.
-00000cf0: 3120 636f 7265 2d72 6573 742d 7069 7065  1 core-rest-pipe
-00000d00: 6c69 6e65 2f31 2e31 302e 3020 4f53 2f57  line/1.10.0 OS/W
-00000d10: 696e 3332 222c 0a20 2020 2020 2020 2020  in32",.         
-00000d20: 2020 2022 5265 6665 7265 7222 3a20 2268     "Referer": "h
-00000d30: 7474 7073 3a2f 2f77 7777 2e62 696e 672e  ttps://www.bing.
-00000d40: 636f 6d2f 7365 6172 6368 3f71 3d42 696e  com/search?q=Bin
-00000d50: 672b 4149 2673 686f 7763 6f6e 763d 3126  g+AI&showconv=1&
-00000d60: 464f 524d 3d68 7063 6f64 7822 2c0a 2020  FORM=hpcodx",.  
-00000d70: 2020 2020 2020 2020 2020 2252 6566 6572            "Refer
-00000d80: 7265 722d 506f 6c69 6379 223a 2022 6f72  rer-Policy": "or
-00000d90: 6967 696e 2d77 6865 6e2d 6372 6f73 732d  igin-when-cross-
-00000da0: 6f72 6967 696e 222c 0a20 2020 2020 2020  origin",.       
-00000db0: 2020 2020 2022 782d 666f 7277 6172 6465       "x-forwarde
-00000dc0: 642d 666f 7222 3a20 464f 5257 4152 4445  d-for": FORWARDE
-00000dd0: 445f 4950 2c0a 2020 2020 2020 2020 2020  D_IP,.          
-00000de0: 2020 7d0a 2020 2020 2020 2020 6966 206a    }.        if j
-00000df0: 7331 5b22 7265 7375 6c74 225d 5b22 7661  s1["result"]["va
-00000e00: 6c75 6522 5d20 3d3d 2022 556e 6175 7468  lue"] == "Unauth
-00000e10: 6f72 697a 6564 5265 7175 6573 7422 3a0a  orizedRequest":.
-00000e20: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00000e30: 6520 4e6f 7441 6c6c 6f77 6564 546f 4163  e NotAllowedToAc
-00000e40: 6365 7373 286a 7331 5b22 7265 7375 6c74  cess(js1["result
-00000e50: 225d 5b22 6d65 7373 6167 6522 5d29 0a20  "]["message"]). 
-00000e60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000e70: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00000e80: 2020 2020 2020 2020 2020 2020 2020 7773                ws
-00000e90: 7363 6f6e 203d 2061 7761 6974 2077 6562  scon = await web
-00000ea0: 736f 636b 6574 732e 636f 6e6e 6563 7428  sockets.connect(
-00000eb0: 2777 7373 3a2f 2f73 7964 6e65 792e 6269  'wss://sydney.bi
-00000ec0: 6e67 2e63 6f6d 2f73 7964 6e65 792f 4368  ng.com/sydney/Ch
-00000ed0: 6174 4875 6227 2c20 6578 7472 615f 6865  atHub', extra_he
-00000ee0: 6164 6572 733d 4845 4144 4552 532c 206d  aders=HEADERS, m
-00000ef0: 6178 5f73 697a 653d 4e6f 6e65 2c20 7373  ax_size=None, ss
-00000f00: 6c3d 7373 6c5f 636f 6e74 6578 742c 2074  l=ssl_context, t
-00000f10: 696d 656f 7574 3d39 3939 392c 2063 6c6f  imeout=9999, clo
-00000f20: 7365 5f74 696d 656f 7574 3d39 3939 3929  se_timeout=9999)
-00000f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000f40: 2061 7761 6974 2077 7373 636f 6e2e 7365   await wsscon.se
-00000f50: 6e64 2827 7b22 7072 6f74 6f63 6f6c 223a  nd('{"protocol":
-00000f60: 226a 736f 6e22 2c22 7665 7273 696f 6e22  "json","version"
-00000f70: 3a31 7d1e 2729 0a20 2020 2020 2020 2020  :1}.').         
-00000f80: 2020 2020 2020 2061 7761 6974 2077 7373         await wss
-00000f90: 636f 6e2e 7265 6376 2829 0a20 2020 2020  con.recv().     
-00000fa0: 2020 2020 2020 2020 2020 2061 7761 6974             await
-00000fb0: 2077 7373 636f 6e2e 7365 6e64 2827 7b22   wsscon.send('{"
-00000fc0: 7479 7065 223a 367d 1e27 290a 2020 2020  type":6}.').    
-00000fd0: 2020 2020 2020 2020 2020 2020 6177 6169              awai
-00000fe0: 7420 7773 7363 6f6e 2e72 6563 7628 290a  t wsscon.recv().
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 6177 6169 7420 7773 7363 6f6e 2e73 656e  await wsscon.sen
-00001010: 6428 277b 2261 7267 756d 656e 7473 223a  d('{"arguments":
-00001020: 5b7b 2273 6f75 7263 6522 3a22 6369 6222  [{"source":"cib"
-00001030: 2c22 6f70 7469 6f6e 7353 6574 7322 3a5b  ,"optionsSets":[
-00001040: 226e 6c75 5f64 6972 6563 745f 7265 7370  "nlu_direct_resp
-00001050: 6f6e 7365 5f66 696c 7465 7222 2c22 6465  onse_filter","de
-00001060: 6570 6c65 6f22 2c22 6469 7361 626c 655f  epleo","disable_
-00001070: 656d 6f6a 695f 7370 6f6b 656e 5f74 6578  emoji_spoken_tex
-00001080: 7422 2c22 7265 7370 6f6e 7369 626c 655f  t","responsible_
-00001090: 6169 5f70 6f6c 6963 795f 3233 3522 2c22  ai_policy_235","
-000010a0: 656e 6162 6c65 6d6d 222c 2268 6172 6d6f  enablemm","harmo
-000010b0: 6e79 7633 222c 2267 6c70 726f 6d70 7476  nyv3","glpromptv
-000010c0: 3122 2c22 6361 6368 6577 7269 7465 6578  1","cachewriteex
-000010d0: 7422 2c22 6532 6563 6163 6865 7772 6974  t","e2ecachewrit
-000010e0: 6522 2c22 6476 3373 7567 6722 5d2c 2261  e","dv3sugg"],"a
-000010f0: 6c6c 6f77 6564 4d65 7373 6167 6554 7970  llowedMessageTyp
-00001100: 6573 223a 5b22 4368 6174 222c 2249 6e74  es":["Chat","Int
-00001110: 6572 6e61 6c53 6561 7263 6851 7565 7279  ernalSearchQuery
-00001120: 222c 2249 6e74 6572 6e61 6c53 6561 7263  ","InternalSearc
-00001130: 6852 6573 756c 7422 2c22 4469 7365 6e67  hResult","Diseng
-00001140: 6167 6564 222c 2249 6e74 6572 6e61 6c4c  aged","InternalL
-00001150: 6f61 6465 724d 6573 7361 6765 222c 2252  oaderMessage","R
-00001160: 656e 6465 7243 6172 6452 6571 7565 7374  enderCardRequest
-00001170: 222c 2241 6473 5175 6572 7922 2c22 5365  ","AdsQuery","Se
-00001180: 6d61 6e74 6963 5365 7270 222c 2247 656e  manticSerp","Gen
-00001190: 6572 6174 6543 6f6e 7465 6e74 5175 6572  erateContentQuer
-000011a0: 7922 2c22 5365 6172 6368 5175 6572 7922  y","SearchQuery"
-000011b0: 5d2c 2273 6c69 6365 4964 7322 3a5b 2263  ],"sliceIds":["c
-000011c0: 7265 6174 6f72 7632 6322 2c22 7365 6d73  reatorv2c","sems
-000011d0: 6572 7062 7074 6632 222c 2270 6572 6669  erpbptf2","perfi
-000011e0: 6e73 7463 6622 2c22 7379 6470 6572 6669  nstcf","sydperfi
-000011f0: 6e70 7574 222c 2233 3134 7364 7072 6322  nput","314sdprc"
-00001200: 2c22 3331 3473 6470 7263 222c 2230 3331  ,"314sdprc","031
-00001210: 3077 6c74 6872 6f74 7330 222c 2270 726f  0wlthrots0","pro
-00001220: 6431 3134 6366 222c 2233 3137 676c 706d  d114cf","317glpm
-00001230: 7476 3122 2c22 3331 3665 3265 6361 6368  tv1","316e2ecach
-00001240: 6522 5d2c 2274 7261 6365 4964 223a 2236  e"],"traceId":"6
-00001250: 3431 3938 3730 6136 6536 3834 3530 3339  419870a6e6845039
-00001260: 3731 3266 3765 3537 3934 3532 3539 3522  712f7e579452595"
-00001270: 2c22 6973 5374 6172 744f 6653 6573 7369  ,"isStartOfSessi
-00001280: 6f6e 223a 7472 7565 2c22 6d65 7373 6167  on":true,"messag
-00001290: 6522 3a7b 226c 6f63 616c 6522 3a22 7472  e":{"locale":"tr
-000012a0: 2d54 5222 2c22 6d61 726b 6574 223a 2274  -TR","market":"t
-000012b0: 722d 5452 222c 2272 6567 696f 6e22 3a22  r-TR","region":"
-000012c0: 5452 222c 226c 6f63 6174 696f 6e22 3a22  TR","location":"
-000012d0: 6c61 743a 3437 2e36 3339 3535 373b 6c6f  lat:47.639557;lo
-000012e0: 6e67 3a2d 3132 322e 3132 3831 3539 3b72  ng:-122.128159;r
-000012f0: 653d 3130 3030 6d3b 222c 226c 6f63 6174  e=1000m;","locat
-00001300: 696f 6e48 696e 7473 223a 5b7b 2243 656e  ionHints":[{"Cen
-00001310: 7465 7222 3a7b 224c 6174 6974 7564 6522  ter":{"Latitude"
-00001320: 3a34 302c 224c 6f6e 6769 7475 6465 223a  :40,"Longitude":
-00001330: 3238 7d2c 2252 6567 696f 6e54 7970 6522  28},"RegionType"
-00001340: 3a32 2c22 536f 7572 6365 5479 7065 223a  :2,"SourceType":
-00001350: 3131 7d2c 7b22 636f 756e 7472 7922 3a22  11},{"country":"
-00001360: 5475 726b 6579 222c 2273 7461 7465 223a  Turkey","state":
-00001370: 2242 7572 7361 222c 2263 6974 7922 3a22  "Bursa","city":"
-00001380: 4d75 6461 6e79 6122 2c22 7a69 7063 6f64  Mudanya","zipcod
-00001390: 6522 3a22 3136 3937 3022 2c22 7469 6d65  e":"16970","time
-000013a0: 7a6f 6e65 6f66 6673 6574 223a 332c 2263  zoneoffset":3,"c
-000013b0: 6f75 6e74 7279 436f 6e66 6964 656e 6365  ountryConfidence
-000013c0: 223a 382c 2263 6974 7943 6f6e 6669 6465  ":8,"cityConfide
-000013d0: 6e63 6522 3a35 2c22 4365 6e74 6572 223a  nce":5,"Center":
-000013e0: 7b22 4c61 7469 7475 6465 223a 3430 2c22  {"Latitude":40,"
-000013f0: 4c6f 6e67 6974 7564 6522 3a32 387d 2c22  Longitude":28},"
-00001400: 5265 6769 6f6e 5479 7065 223a 322c 2253  RegionType":2,"S
-00001410: 6f75 7263 6554 7970 6522 3a31 7d5d 2c22  ourceType":1}],"
-00001420: 7469 6d65 7374 616d 7022 3a22 3230 3233  timestamp":"2023
-00001430: 2d30 332d 3231 5431 333a 3239 3a33 342b  -03-21T13:29:34+
-00001440: 3033 3a30 3022 2c22 6175 7468 6f72 223a  03:00","author":
-00001450: 2275 7365 7222 2c22 696e 7075 744d 6574  "user","inputMet
-00001460: 686f 6422 3a22 4b65 7962 6f61 7264 222c  hod":"Keyboard",
-00001470: 2274 6578 7422 3a22 2720 2b20 4269 6e67  "text":"' + Bing
-00001480: 5079 7468 6f6e 2e61 7969 6b6c 6128 7175  Python.ayikla(qu
-00001490: 6573 7469 6f6e 2920 2b20 2722 2c22 6d65  estion) + '","me
-000014a0: 7373 6167 6554 7970 6522 3a22 4368 6174  ssageType":"Chat
-000014b0: 227d 2c22 636f 6e76 6572 7361 7469 6f6e  "},"conversation
-000014c0: 5369 676e 6174 7572 6522 3a22 2720 2b20  Signature":"' + 
-000014d0: 7374 7228 6a73 315b 2263 6f6e 7665 7273  str(js1["convers
-000014e0: 6174 696f 6e53 6967 6e61 7475 7265 225d  ationSignature"]
-000014f0: 2920 2b20 2722 2c22 7061 7274 6963 6970  ) + '","particip
-00001500: 616e 7422 3a7b 2269 6422 3a22 2720 2b20  ant":{"id":"' + 
-00001510: 7374 7228 6a73 315b 2263 6c69 656e 7449  str(js1["clientI
-00001520: 6422 5d29 202b 2027 227d 2c22 636f 6e76  d"]) + '"},"conv
-00001530: 6572 7361 7469 6f6e 4964 223a 2227 202b  ersationId":"' +
-00001540: 2073 7472 286a 7331 5b22 636f 6e76 6572   str(js1["conver
-00001550: 7361 7469 6f6e 4964 225d 2920 2b20 2722  sationId"]) + '"
-00001560: 7d5d 2c22 696e 766f 6361 7469 6f6e 4964  }],"invocationId
-00001570: 223a 2230 222c 2274 6172 6765 7422 3a22  ":"0","target":"
-00001580: 6368 6174 222c 2274 7970 6522 3a34 7d1e  chat","type":4}.
-00001590: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
-000015a0: 2020 2074 6173 6b20 3d20 6173 796e 6369     task = asynci
-000015b0: 6f2e 6372 6561 7465 5f74 6173 6b28 4269  o.create_task(Bi
-000015c0: 6e67 5079 7468 6f6e 2e70 696e 6728 7773  ngPython.ping(ws
-000015d0: 7363 6f6e 2929 0a20 2020 2020 2020 2020  scon)).         
-000015e0: 2020 2065 7863 6570 7428 7765 6273 6f63     except(websoc
-000015f0: 6b65 7473 2e65 7863 6570 7469 6f6e 732e  kets.exceptions.
-00001600: 436f 6e6e 6563 7469 6f6e 436c 6f73 6564  ConnectionClosed
-00001610: 4572 726f 7229 3a0a 2020 2020 2020 2020  Error):.        
-00001620: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00001630: 5765 6253 6f63 6b65 7420 436f 6e6e 6563  WebSocket Connec
-00001640: 7469 6f6e 436c 6f73 6564 4572 726f 7221  tionClosedError!
-00001650: 202d 2054 4552 4d49 4e41 5445 4421 220a   - TERMINATED!".
-00001660: 2020 2020 2020 2020 2020 2020 6669 6e61              fina
-00001670: 6c20 3d20 4661 6c73 650a 2020 2020 2020  l = False.      
-00001680: 2020 2020 2020 7768 696c 6520 6e6f 7420        while not 
-00001690: 6669 6e61 6c3a 0a20 2020 2020 2020 2020  final:.         
-000016a0: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 6f62 6a65 6374 7320 3d20 7374 7228 6177  objects = str(aw
-000016d0: 6169 7420 7773 7363 6f6e 2e72 6563 7628  ait wsscon.recv(
-000016e0: 2929 2e73 706c 6974 2822 1e22 290a 2020  )).split(".").  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00001700: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
-00001710: 2020 2020 2020 2020 2020 6669 6e61 6c20            final 
-00001720: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00001730: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
-00001740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001750: 2020 2020 2020 2020 7265 7475 726e 2022          return "
-00001760: 416e 7377 6572 203a 2022 202b 2076 6572  Answer : " + ver
-00001770: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-00001780: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 2020 2020 7265 7475 726e 2022 416e        return "An
-000017b0: 2065 7272 6f72 206f 6363 7572 6564 2120   error occured! 
-000017c0: 506c 6561 7365 2074 7279 2061 6761 696e  Please try again
-000017d0: 2122 0a20 2020 2020 2020 2020 2020 2020  !".             
-000017e0: 2020 2066 6f72 206f 626a 2069 6e20 6f62     for obj in ob
-000017f0: 6a65 6374 733a 0a20 2020 2020 2020 2020  jects:.         
-00001800: 2020 2020 2020 2020 2020 2069 6620 6f62             if ob
-00001810: 6a20 6973 204e 6f6e 6520 6f72 206f 626a  j is None or obj
-00001820: 203d 3d20 2222 3a0a 2020 2020 2020 2020   == "":.        
+000007d0: 6463 6f6d 5f73 7964 6e65 7928 6c6f 6164  dcom_sydney(load
+000007e0: 6461 7461 2c20 7175 6573 7469 6f6e 293a  data, question):
+000007f0: 0a20 2020 2020 2020 2023 204a 534f 4e20  .        # JSON 
+00000800: 4c6f 6164 0a20 2020 2020 2020 206a 7331  Load.        js1
+00000810: 203d 206a 736f 6e2e 6c6f 6164 7328 6c6f   = json.loads(lo
+00000820: 6164 6461 7461 290a 0a20 2020 2020 2020  addata)..       
+00000830: 2023 2053 534c 2043 6f6e 7465 7874 0a20   # SSL Context. 
+00000840: 2020 2020 2020 2073 736c 5f63 6f6e 7465         ssl_conte
+00000850: 7874 203d 2073 736c 2e63 7265 6174 655f  xt = ssl.create_
+00000860: 6465 6661 756c 745f 636f 6e74 6578 7428  default_context(
+00000870: 290a 2020 2020 2020 2020 7373 6c5f 636f  ).        ssl_co
+00000880: 6e74 6578 742e 6c6f 6164 5f76 6572 6966  ntext.load_verif
+00000890: 795f 6c6f 6361 7469 6f6e 7328 6365 7274  y_locations(cert
+000008a0: 6966 692e 7768 6572 6528 2929 0a0a 2020  ifi.where())..  
+000008b0: 2020 2020 2020 2320 4865 6164 6572 7320        # Headers 
+000008c0: 616e 6420 4950 2041 6464 7265 7373 6573  and IP Addresses
+000008d0: 0a20 2020 2020 2020 2046 4f52 5741 5244  .        FORWARD
+000008e0: 4544 5f49 5020 3d20 2866 2231 332e 7b72  ED_IP = (f"13.{r
+000008f0: 616e 646f 6d2e 7261 6e64 696e 7428 3130  andom.randint(10
+00000900: 342c 2031 3037 297d 2e7b 7261 6e64 6f6d  4, 107)}.{random
+00000910: 2e72 616e 6469 6e74 2830 2c20 3235 3529  .randint(0, 255)
+00000920: 7d2e 7b72 616e 646f 6d2e 7261 6e64 696e  }.{random.randin
+00000930: 7428 302c 2032 3535 297d 2229 0a20 2020  t(0, 255)}").   
+00000940: 2020 2020 2048 4541 4445 5253 203d 207b       HEADERS = {
+00000950: 0a20 2020 2020 2020 2020 2020 2022 6163  .            "ac
+00000960: 6365 7074 223a 2022 6170 706c 6963 6174  cept": "applicat
+00000970: 696f 6e2f 6a73 6f6e 222c 0a20 2020 2020  ion/json",.     
+00000980: 2020 2020 2020 2022 6163 6365 7074 2d6c         "accept-l
+00000990: 616e 6775 6167 6522 3a20 2265 6e2d 5553  anguage": "en-US
+000009a0: 2c65 6e3b 713d 302e 3922 2c0a 2020 2020  ,en;q=0.9",.    
+000009b0: 2020 2020 2020 2020 2263 6f6e 7465 6e74          "content
+000009c0: 2d74 7970 6522 3a20 2261 7070 6c69 6361  -type": "applica
+000009d0: 7469 6f6e 2f6a 736f 6e22 2c0a 2020 2020  tion/json",.    
+000009e0: 2020 2020 2020 2020 2273 6563 2d63 682d          "sec-ch-
+000009f0: 7561 223a 2027 224e 6f74 5f41 2042 7261  ua": '"Not_A Bra
+00000a00: 6e64 223b 763d 2239 3922 2c20 224d 6963  nd";v="99", "Mic
+00000a10: 726f 736f 6674 2045 6467 6522 3b76 3d22  rosoft Edge";v="
+00000a20: 3131 3022 2c20 2243 6872 6f6d 6975 6d22  110", "Chromium"
+00000a30: 3b76 3d22 3131 3022 272c 0a20 2020 2020  ;v="110"',.     
+00000a40: 2020 2020 2020 2022 7365 632d 6368 2d75         "sec-ch-u
+00000a50: 612d 6172 6368 223a 2027 2278 3836 2227  a-arch": '"x86"'
+00000a60: 2c0a 2020 2020 2020 2020 2020 2020 2273  ,.            "s
+00000a70: 6563 2d63 682d 7561 2d62 6974 6e65 7373  ec-ch-ua-bitness
+00000a80: 223a 2027 2236 3422 272c 0a20 2020 2020  ": '"64"',.     
+00000a90: 2020 2020 2020 2022 7365 632d 6368 2d75         "sec-ch-u
+00000aa0: 612d 6675 6c6c 2d76 6572 7369 6f6e 223a  a-full-version":
+00000ab0: 2027 2231 3039 2e30 2e31 3531 382e 3738   '"109.0.1518.78
+00000ac0: 2227 2c0a 2020 2020 2020 2020 2020 2020  "',.            
+00000ad0: 2273 6563 2d63 682d 7561 2d66 756c 6c2d  "sec-ch-ua-full-
+00000ae0: 7665 7273 696f 6e2d 6c69 7374 223a 2027  version-list": '
+00000af0: 2243 6872 6f6d 6975 6d22 3b76 3d22 3131  "Chromium";v="11
+00000b00: 302e 302e 3534 3831 2e31 3932 222c 2022  0.0.5481.192", "
+00000b10: 4e6f 7420 4128 4272 616e 6422 3b76 3d22  Not A(Brand";v="
+00000b20: 3234 2e30 2e30 2e30 222c 2022 4d69 6372  24.0.0.0", "Micr
+00000b30: 6f73 6f66 7420 4564 6765 223b 763d 2231  osoft Edge";v="1
+00000b40: 3130 2e30 2e31 3538 372e 3639 2227 2c0a  10.0.1587.69"',.
+00000b50: 2020 2020 2020 2020 2020 2020 2273 6563              "sec
+00000b60: 2d63 682d 7561 2d6d 6f62 696c 6522 3a20  -ch-ua-mobile": 
+00000b70: 223f 3022 2c0a 2020 2020 2020 2020 2020  "?0",.          
+00000b80: 2020 2273 6563 2d63 682d 7561 2d6d 6f64    "sec-ch-ua-mod
+00000b90: 656c 223a 2022 222c 0a20 2020 2020 2020  el": "",.       
+00000ba0: 2020 2020 2022 7365 632d 6368 2d75 612d       "sec-ch-ua-
+00000bb0: 706c 6174 666f 726d 223a 2027 2257 696e  platform": '"Win
+00000bc0: 646f 7773 2227 2c0a 2020 2020 2020 2020  dows"',.        
+00000bd0: 2020 2020 2273 6563 2d63 682d 7561 2d70      "sec-ch-ua-p
+00000be0: 6c61 7466 6f72 6d2d 7665 7273 696f 6e22  latform-version"
+00000bf0: 3a20 2722 3135 2e30 2e30 2227 2c0a 2020  : '"15.0.0"',.  
+00000c00: 2020 2020 2020 2020 2020 2273 6563 2d66            "sec-f
+00000c10: 6574 6368 2d64 6573 7422 3a20 2265 6d70  etch-dest": "emp
+00000c20: 7479 222c 0a20 2020 2020 2020 2020 2020  ty",.           
+00000c30: 2022 7365 632d 6665 7463 682d 6d6f 6465   "sec-fetch-mode
+00000c40: 223a 2022 636f 7273 222c 0a20 2020 2020  ": "cors",.     
+00000c50: 2020 2020 2020 2022 7365 632d 6665 7463         "sec-fetc
+00000c60: 682d 7369 7465 223a 2022 7361 6d65 2d6f  h-site": "same-o
+00000c70: 7269 6769 6e22 2c0a 2020 2020 2020 2020  rigin",.        
+00000c80: 2020 2020 2278 2d6d 732d 636c 6965 6e74      "x-ms-client
+00000c90: 2d72 6571 7565 7374 2d69 6422 3a20 7374  -request-id": st
+00000ca0: 7228 7575 6964 2e75 7569 6434 2829 292c  r(uuid.uuid4()),
+00000cb0: 0a20 2020 2020 2020 2020 2020 2022 782d  .            "x-
+00000cc0: 6d73 2d75 7365 7261 6765 6e74 223a 2022  ms-useragent": "
+00000cd0: 617a 7364 6b2d 6a73 2d61 7069 2d63 6c69  azsdk-js-api-cli
+00000ce0: 656e 742d 6661 6374 6f72 792f 312e 302e  ent-factory/1.0.
+00000cf0: 302d 6265 7461 2e31 2063 6f72 652d 7265  0-beta.1 core-re
+00000d00: 7374 2d70 6970 656c 696e 652f 312e 3130  st-pipeline/1.10
+00000d10: 2e30 204f 532f 5769 6e33 3222 2c0a 2020  .0 OS/Win32",.  
+00000d20: 2020 2020 2020 2020 2020 2252 6566 6572            "Refer
+00000d30: 6572 223a 2022 6874 7470 733a 2f2f 7777  er": "https://ww
+00000d40: 772e 6269 6e67 2e63 6f6d 2f73 6561 7263  w.bing.com/searc
+00000d50: 683f 713d 4269 6e67 2b41 4926 7368 6f77  h?q=Bing+AI&show
+00000d60: 636f 6e76 3d31 2646 4f52 4d3d 6870 636f  conv=1&FORM=hpco
+00000d70: 6478 222c 0a20 2020 2020 2020 2020 2020  dx",.           
+00000d80: 2022 5265 6665 7272 6572 2d50 6f6c 6963   "Referrer-Polic
+00000d90: 7922 3a20 226f 7269 6769 6e2d 7768 656e  y": "origin-when
+00000da0: 2d63 726f 7373 2d6f 7269 6769 6e22 2c0a  -cross-origin",.
+00000db0: 2020 2020 2020 2020 2020 2020 2278 2d66              "x-f
+00000dc0: 6f72 7761 7264 6564 2d66 6f72 223a 2046  orwarded-for": F
+00000dd0: 4f52 5741 5244 4544 5f49 502c 0a20 2020  ORWARDED_IP,.   
+00000de0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00000df0: 2020 2069 6620 6a73 315b 2272 6573 756c     if js1["resul
+00000e00: 7422 5d5b 2276 616c 7565 225d 203d 3d20  t"]["value"] == 
+00000e10: 2255 6e61 7574 686f 7269 7a65 6452 6571  "UnauthorizedReq
+00000e20: 7565 7374 223a 0a20 2020 2020 2020 2020  uest":.         
+00000e30: 2020 2072 6169 7365 204e 6f74 416c 6c6f     raise NotAllo
+00000e40: 7765 6454 6f41 6363 6573 7328 6a73 315b  wedToAccess(js1[
+00000e50: 2272 6573 756c 7422 5d5b 226d 6573 7361  "result"]["messa
+00000e60: 6765 225d 290a 2020 2020 2020 2020 656c  ge"]).        el
+00000e70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00000e80: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+00000e90: 2020 2020 2077 7373 636f 6e20 3d20 6177       wsscon = aw
+00000ea0: 6169 7420 7765 6273 6f63 6b65 7473 2e63  ait websockets.c
+00000eb0: 6f6e 6e65 6374 2827 7773 733a 2f2f 7379  onnect('wss://sy
+00000ec0: 646e 6579 2e62 696e 672e 636f 6d2f 7379  dney.bing.com/sy
+00000ed0: 646e 6579 2f43 6861 7448 7562 272c 2065  dney/ChatHub', e
+00000ee0: 7874 7261 5f68 6561 6465 7273 3d48 4541  xtra_headers=HEA
+00000ef0: 4445 5253 2c20 6d61 785f 7369 7a65 3d4e  DERS, max_size=N
+00000f00: 6f6e 652c 2073 736c 3d73 736c 5f63 6f6e  one, ssl=ssl_con
+00000f10: 7465 7874 2c20 7469 6d65 6f75 743d 3939  text, timeout=99
+00000f20: 3939 2c20 636c 6f73 655f 7469 6d65 6f75  99, close_timeou
+00000f30: 743d 3939 3939 290a 2020 2020 2020 2020  t=9999).        
+00000f40: 2020 2020 2020 2020 6177 6169 7420 7773          await ws
+00000f50: 7363 6f6e 2e73 656e 6428 277b 2270 726f  scon.send('{"pro
+00000f60: 746f 636f 6c22 3a22 6a73 6f6e 222c 2276  tocol":"json","v
+00000f70: 6572 7369 6f6e 223a 317d 1e27 290a 2020  ersion":1}.').  
+00000f80: 2020 2020 2020 2020 2020 2020 2020 6177                aw
+00000f90: 6169 7420 7773 7363 6f6e 2e72 6563 7628  ait wsscon.recv(
+00000fa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00000fb0: 2020 6177 6169 7420 7773 7363 6f6e 2e73    await wsscon.s
+00000fc0: 656e 6428 277b 2274 7970 6522 3a36 7d1e  end('{"type":6}.
+00000fd0: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00000fe0: 2020 2061 7761 6974 2077 7373 636f 6e2e     await wsscon.
+00000ff0: 7265 6376 2829 0a20 2020 2020 2020 2020  recv().         
+00001000: 2020 2020 2020 2061 7761 6974 2077 7373         await wss
+00001010: 636f 6e2e 7365 6e64 2827 7b22 6172 6775  con.send('{"argu
+00001020: 6d65 6e74 7322 3a5b 7b22 736f 7572 6365  ments":[{"source
+00001030: 223a 2263 6962 222c 226f 7074 696f 6e73  ":"cib","options
+00001040: 5365 7473 223a 5b22 6e6c 755f 6469 7265  Sets":["nlu_dire
+00001050: 6374 5f72 6573 706f 6e73 655f 6669 6c74  ct_response_filt
+00001060: 6572 222c 2264 6565 706c 656f 222c 2264  er","deepleo","d
+00001070: 6973 6162 6c65 5f65 6d6f 6a69 5f73 706f  isable_emoji_spo
+00001080: 6b65 6e5f 7465 7874 222c 2272 6573 706f  ken_text","respo
+00001090: 6e73 6962 6c65 5f61 695f 706f 6c69 6379  nsible_ai_policy
+000010a0: 5f32 3335 222c 2265 6e61 626c 656d 6d22  _235","enablemm"
+000010b0: 2c22 6861 726d 6f6e 7976 3322 2c22 676c  ,"harmonyv3","gl
+000010c0: 7072 6f6d 7074 7631 222c 2263 6163 6865  promptv1","cache
+000010d0: 7772 6974 6565 7874 222c 2265 3265 6361  writeext","e2eca
+000010e0: 6368 6577 7269 7465 222c 2264 7633 7375  chewrite","dv3su
+000010f0: 6767 225d 2c22 616c 6c6f 7765 644d 6573  gg"],"allowedMes
+00001100: 7361 6765 5479 7065 7322 3a5b 2243 6861  sageTypes":["Cha
+00001110: 7422 2c22 496e 7465 726e 616c 5365 6172  t","InternalSear
+00001120: 6368 5175 6572 7922 2c22 496e 7465 726e  chQuery","Intern
+00001130: 616c 5365 6172 6368 5265 7375 6c74 222c  alSearchResult",
+00001140: 2244 6973 656e 6761 6765 6422 2c22 496e  "Disengaged","In
+00001150: 7465 726e 616c 4c6f 6164 6572 4d65 7373  ternalLoaderMess
+00001160: 6167 6522 2c22 5265 6e64 6572 4361 7264  age","RenderCard
+00001170: 5265 7175 6573 7422 2c22 4164 7351 7565  Request","AdsQue
+00001180: 7279 222c 2253 656d 616e 7469 6353 6572  ry","SemanticSer
+00001190: 7022 2c22 4765 6e65 7261 7465 436f 6e74  p","GenerateCont
+000011a0: 656e 7451 7565 7279 222c 2253 6561 7263  entQuery","Searc
+000011b0: 6851 7565 7279 225d 2c22 736c 6963 6549  hQuery"],"sliceI
+000011c0: 6473 223a 5b22 6372 6561 746f 7276 3263  ds":["creatorv2c
+000011d0: 222c 2273 656d 7365 7270 6270 7466 3222  ","semserpbptf2"
+000011e0: 2c22 7065 7266 696e 7374 6366 222c 2273  ,"perfinstcf","s
+000011f0: 7964 7065 7266 696e 7075 7422 2c22 3331  ydperfinput","31
+00001200: 3473 6470 7263 222c 2233 3134 7364 7072  4sdprc","314sdpr
+00001210: 6322 2c22 3033 3130 776c 7468 726f 7473  c","0310wlthrots
+00001220: 3022 2c22 7072 6f64 3131 3463 6622 2c22  0","prod114cf","
+00001230: 3331 3767 6c70 6d74 7631 222c 2233 3136  317glpmtv1","316
+00001240: 6532 6563 6163 6865 225d 2c22 7472 6163  e2ecache"],"trac
+00001250: 6549 6422 3a22 3634 3139 3837 3061 3665  eId":"6419870a6e
+00001260: 3638 3435 3033 3937 3132 6637 6535 3739  6845039712f7e579
+00001270: 3435 3235 3935 222c 2269 7353 7461 7274  452595","isStart
+00001280: 4f66 5365 7373 696f 6e22 3a74 7275 652c  OfSession":true,
+00001290: 226d 6573 7361 6765 223a 7b22 6c6f 6361  "message":{"loca
+000012a0: 6c65 223a 2274 722d 5452 222c 226d 6172  le":"tr-TR","mar
+000012b0: 6b65 7422 3a22 7472 2d54 5222 2c22 7265  ket":"tr-TR","re
+000012c0: 6769 6f6e 223a 2254 5222 2c22 6c6f 6361  gion":"TR","loca
+000012d0: 7469 6f6e 223a 226c 6174 3a34 372e 3633  tion":"lat:47.63
+000012e0: 3935 3537 3b6c 6f6e 673a 2d31 3232 2e31  9557;long:-122.1
+000012f0: 3238 3135 393b 7265 3d31 3030 306d 3b22  28159;re=1000m;"
+00001300: 2c22 6c6f 6361 7469 6f6e 4869 6e74 7322  ,"locationHints"
+00001310: 3a5b 7b22 4365 6e74 6572 223a 7b22 4c61  :[{"Center":{"La
+00001320: 7469 7475 6465 223a 3430 2c22 4c6f 6e67  titude":40,"Long
+00001330: 6974 7564 6522 3a32 387d 2c22 5265 6769  itude":28},"Regi
+00001340: 6f6e 5479 7065 223a 322c 2253 6f75 7263  onType":2,"Sourc
+00001350: 6554 7970 6522 3a31 317d 2c7b 2263 6f75  eType":11},{"cou
+00001360: 6e74 7279 223a 2254 7572 6b65 7922 2c22  ntry":"Turkey","
+00001370: 7374 6174 6522 3a22 4275 7273 6122 2c22  state":"Bursa","
+00001380: 6369 7479 223a 224d 7564 616e 7961 222c  city":"Mudanya",
+00001390: 227a 6970 636f 6465 223a 2231 3639 3730  "zipcode":"16970
+000013a0: 222c 2274 696d 657a 6f6e 656f 6666 7365  ","timezoneoffse
+000013b0: 7422 3a33 2c22 636f 756e 7472 7943 6f6e  t":3,"countryCon
+000013c0: 6669 6465 6e63 6522 3a38 2c22 6369 7479  fidence":8,"city
+000013d0: 436f 6e66 6964 656e 6365 223a 352c 2243  Confidence":5,"C
+000013e0: 656e 7465 7222 3a7b 224c 6174 6974 7564  enter":{"Latitud
+000013f0: 6522 3a34 302c 224c 6f6e 6769 7475 6465  e":40,"Longitude
+00001400: 223a 3238 7d2c 2252 6567 696f 6e54 7970  ":28},"RegionTyp
+00001410: 6522 3a32 2c22 536f 7572 6365 5479 7065  e":2,"SourceType
+00001420: 223a 317d 5d2c 2274 696d 6573 7461 6d70  ":1}],"timestamp
+00001430: 223a 2232 3032 332d 3033 2d32 3154 3133  ":"2023-03-21T13
+00001440: 3a32 393a 3334 2b30 333a 3030 222c 2261  :29:34+03:00","a
+00001450: 7574 686f 7222 3a22 7573 6572 222c 2269  uthor":"user","i
+00001460: 6e70 7574 4d65 7468 6f64 223a 224b 6579  nputMethod":"Key
+00001470: 626f 6172 6422 2c22 7465 7874 223a 2227  board","text":"'
+00001480: 202b 2042 696e 6750 7974 686f 6e2e 6179   + BingPython.ay
+00001490: 696b 6c61 2871 7565 7374 696f 6e29 202b  ikla(question) +
+000014a0: 2027 222c 226d 6573 7361 6765 5479 7065   '","messageType
+000014b0: 223a 2243 6861 7422 7d2c 2263 6f6e 7665  ":"Chat"},"conve
+000014c0: 7273 6174 696f 6e53 6967 6e61 7475 7265  rsationSignature
+000014d0: 223a 2227 202b 2073 7472 286a 7331 5b22  ":"' + str(js1["
+000014e0: 636f 6e76 6572 7361 7469 6f6e 5369 676e  conversationSign
+000014f0: 6174 7572 6522 5d29 202b 2027 222c 2270  ature"]) + '","p
+00001500: 6172 7469 6369 7061 6e74 223a 7b22 6964  articipant":{"id
+00001510: 223a 2227 202b 2073 7472 286a 7331 5b22  ":"' + str(js1["
+00001520: 636c 6965 6e74 4964 225d 2920 2b20 2722  clientId"]) + '"
+00001530: 7d2c 2263 6f6e 7665 7273 6174 696f 6e49  },"conversationI
+00001540: 6422 3a22 2720 2b20 7374 7228 6a73 315b  d":"' + str(js1[
+00001550: 2263 6f6e 7665 7273 6174 696f 6e49 6422  "conversationId"
+00001560: 5d29 202b 2027 227d 5d2c 2269 6e76 6f63  ]) + '"}],"invoc
+00001570: 6174 696f 6e49 6422 3a22 3022 2c22 7461  ationId":"0","ta
+00001580: 7267 6574 223a 2263 6861 7422 2c22 7479  rget":"chat","ty
+00001590: 7065 223a 347d 1e27 290a 2020 2020 2020  pe":4}.').      
+000015a0: 2020 2020 2020 2020 2020 7461 736b 203d            task =
+000015b0: 2061 7379 6e63 696f 2e63 7265 6174 655f   asyncio.create_
+000015c0: 7461 736b 2842 696e 6750 7974 686f 6e2e  task(BingPython.
+000015d0: 7069 6e67 2877 7373 636f 6e29 290a 2020  ping(wsscon)).  
+000015e0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+000015f0: 2877 6562 736f 636b 6574 732e 6578 6365  (websockets.exce
+00001600: 7074 696f 6e73 2e43 6f6e 6e65 6374 696f  ptions.Connectio
+00001610: 6e43 6c6f 7365 6445 7272 6f72 293a 0a20  nClosedError):. 
+00001620: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001630: 6574 7572 6e20 2257 6562 536f 636b 6574  eturn "WebSocket
+00001640: 2043 6f6e 6e65 6374 696f 6e43 6c6f 7365   ConnectionClose
+00001650: 6445 7272 6f72 2120 2d20 5445 524d 494e  dError! - TERMIN
+00001660: 4154 4544 2122 0a20 2020 2020 2020 2020  ATED!".         
+00001670: 2020 2066 696e 616c 203d 2046 616c 7365     final = False
+00001680: 0a20 2020 2020 2020 2020 2020 2077 6869  .            whi
+00001690: 6c65 206e 6f74 2066 696e 616c 3a0a 2020  le not final:.  
+000016a0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+000016b0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+000016c0: 2020 2020 2020 206f 626a 6563 7473 203d         objects =
+000016d0: 2073 7472 2861 7761 6974 2077 7373 636f   str(await wssco
+000016e0: 6e2e 7265 6376 2829 292e 7370 6c69 7428  n.recv()).split(
+000016f0: 221e 2229 0a20 2020 2020 2020 2020 2020  ".").           
+00001700: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2066 696e 616c 203d 2054 7275 650a 2020   final = True.  
+00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001740: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00001750: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00001760: 6574 7572 6e20 2241 6e73 7765 7220 3a20  eturn "Answer : 
+00001770: 2220 2b20 7665 7269 0a20 2020 2020 2020  " + veri.       
+00001780: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00001790: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
+000017a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000017b0: 7572 6e20 2241 6e20 6572 726f 7220 6f63  urn "An error oc
+000017c0: 6375 7265 6421 2050 6c65 6173 6520 7472  cured! Please tr
+000017d0: 7920 6167 6169 6e21 220a 2020 2020 2020  y again!".      
+000017e0: 2020 2020 2020 2020 2020 666f 7220 6f62            for ob
+000017f0: 6a20 696e 206f 626a 6563 7473 3a0a 2020  j in objects:.  
+00001800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001810: 2020 6966 206f 626a 2069 7320 4e6f 6e65    if obj is None
+00001820: 206f 7220 6f62 6a20 3d3d 2022 223a 0a20   or obj == "":. 
 00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001840: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-00001850: 2020 2020 2020 2020 2020 2020 2072 6573               res
-00001860: 706f 6e73 6520 3d20 6a73 6f6e 2e6c 6f61  ponse = json.loa
-00001870: 6473 286f 626a 290a 2020 2020 2020 2020  ds(obj).        
-00001880: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00001890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000018a0: 2020 2020 2020 2020 2069 6620 7265 7370           if resp
-000018b0: 6f6e 7365 5b22 7479 7065 225d 203d 3d20  onse["type"] == 
-000018c0: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-000018d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000018e0: 6620 7265 7370 6f6e 7365 5b22 6172 6775  f response["argu
-000018f0: 6d65 6e74 7322 5d5b 305d 5b22 6d65 7373  ments"][0]["mess
-00001900: 6167 6573 225d 5b30 5d5b 2274 6578 7422  ages"][0]["text"
-00001910: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00001840: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 2020 7265 7370 6f6e 7365 203d 206a      response = j
+00001870: 736f 6e2e 6c6f 6164 7328 6f62 6a29 0a20  son.loads(obj). 
+00001880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001890: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+000018a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018b0: 6966 2072 6573 706f 6e73 655b 2274 7970  if response["typ
+000018c0: 6522 5d20 3d3d 2031 3a0a 2020 2020 2020  e"] == 1:.      
+000018d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000018e0: 2020 2020 2020 6966 2072 6573 706f 6e73        if respons
+000018f0: 655b 2261 7267 756d 656e 7473 225d 5b30  e["arguments"][0
+00001900: 5d5b 226d 6573 7361 6765 7322 5d5b 305d  ]["messages"][0]
+00001910: 5b22 7465 7874 225d 3a0a 2020 2020 2020  ["text"]:.      
 00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 2069 6620 2253 6561 7263 6869 6e67     if "Searching
-00001940: 2074 6865 2077 6562 2066 6f72 2220 696e   the web for" in
-00001950: 2073 7472 2872 6573 706f 6e73 655b 2261   str(response["a
-00001960: 7267 756d 656e 7473 225d 5b30 5d5b 226d  rguments"][0]["m
-00001970: 6573 7361 6765 7322 5d5b 305d 5b22 7465  essages"][0]["te
-00001980: 7874 225d 293a 0a20 2020 2020 2020 2020  xt"]):.         
+00001930: 2020 2020 2020 2020 2020 6966 2022 5365            if "Se
+00001940: 6172 6368 696e 6720 7468 6520 7765 6220  arching the web 
+00001950: 666f 7222 2069 6e20 7374 7228 7265 7370  for" in str(resp
+00001960: 6f6e 7365 5b22 6172 6775 6d65 6e74 7322  onse["arguments"
+00001970: 5d5b 305d 5b22 6d65 7373 6167 6573 225d  ][0]["messages"]
+00001980: 5b30 5d5b 2274 6578 7422 5d29 3a0a 2020  [0]["text"]):.  
 00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019a0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-000019b0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
 000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000019e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00001a00: 2022 4765 6e65 7261 7469 6e67 2061 6e73   "Generating ans
-00001a10: 7765 7273 2066 6f72 2079 6f75 2e2e 2e22  wers for you..."
-00001a20: 2069 6e20 7374 7228 7265 7370 6f6e 7365   in str(response
-00001a30: 5b22 6172 6775 6d65 6e74 7322 5d5b 305d  ["arguments"][0]
-00001a40: 5b22 6d65 7373 6167 6573 225d 5b30 5d5b  ["messages"][0][
-00001a50: 2274 6578 7422 5d29 3a0a 2020 2020 2020  "text"]):.      
-00001a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+000019e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a00: 2020 2020 2069 6620 2247 656e 6572 6174       if "Generat
+00001a10: 696e 6720 616e 7377 6572 7320 666f 7220  ing answers for 
+00001a20: 796f 752e 2e2e 2220 696e 2073 7472 2872  you..." in str(r
+00001a30: 6573 706f 6e73 655b 2261 7267 756d 656e  esponse["argumen
+00001a40: 7473 225d 5b30 5d5b 226d 6573 7361 6765  ts"][0]["message
+00001a50: 7322 5d5b 305d 5b22 7465 7874 225d 293a  s"][0]["text"]):
+00001a60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00001ab0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00001a80: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00001a90: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ab0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ad0: 2020 2020 2020 2020 2020 2020 206c 656e               len
-00001ae0: 6172 7261 7920 3d20 6c65 6e28 7265 7370  array = len(resp
-00001af0: 6f6e 7365 5b22 6172 6775 6d65 6e74 7322  onse["arguments"
-00001b00: 5d5b 305d 5b22 6d65 7373 6167 6573 225d  ][0]["messages"]
-00001b10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ae0: 2020 2020 6c65 6e61 7272 6179 203d 206c      lenarray = l
+00001af0: 656e 2872 6573 706f 6e73 655b 2261 7267  en(response["arg
+00001b00: 756d 656e 7473 225d 5b30 5d5b 226d 6573  uments"][0]["mes
+00001b10: 7361 6765 7322 5d29 0a20 2020 2020 2020  sages"]).       
 00001b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b30: 2020 2020 2020 2020 2020 7665 7269 203d            veri =
-00001b40: 2073 7472 2872 6573 706f 6e73 655b 2261   str(response["a
-00001b50: 7267 756d 656e 7473 225d 5b30 5d5b 226d  rguments"][0]["m
-00001b60: 6573 7361 6765 7322 5d5b 6c65 6e61 7272  essages"][lenarr
-00001b70: 6179 2d32 5d5b 2274 6578 7422 5d29 0a20  ay-2]["text"]). 
-00001b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b90: 2020 2020 2020 2065 6c69 6620 7265 7370         elif resp
-00001ba0: 6f6e 7365 5b22 7479 7065 225d 203d 3d20  onse["type"] == 
-00001bb0: 323a 0a20 2020 2020 2020 2020 2020 2020  2:.             
+00001b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b40: 2076 6572 6920 3d20 7374 7228 7265 7370   veri = str(resp
+00001b50: 6f6e 7365 5b22 6172 6775 6d65 6e74 7322  onse["arguments"
+00001b60: 5d5b 305d 5b22 6d65 7373 6167 6573 225d  ][0]["messages"]
+00001b70: 5b6c 656e 6172 7261 792d 325d 5b22 7465  [lenarray-2]["te
+00001b80: 7874 225d 290a 2020 2020 2020 2020 2020  xt"]).          
+00001b90: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00001ba0: 6966 2072 6573 706f 6e73 655b 2274 7970  if response["typ
+00001bb0: 6522 5d20 3d3d 2032 3a0a 2020 2020 2020  e"] == 2:.      
 00001bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bd0: 2020 2066 696e 616c 203d 2054 7275 650a     final = True.
-00001be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bd0: 2020 2020 2020 2020 2020 6669 6e61 6c20            final 
+00001be0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
 00001bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c00: 6966 2076 6572 6920 3d3d 2071 7565 7374  if veri == quest
-00001c10: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+00001c00: 2020 2020 2020 2069 6620 7665 7269 203d         if veri =
+00001c10: 3d20 7175 6573 7469 6f6e 3a0a 2020 2020  = question:.    
 00001c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c30: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001c40: 2241 6e20 6572 726f 7220 6f63 6375 7265  "An error occure
-00001c50: 6421 2050 6c65 6173 6520 7472 7920 6167  d! Please try ag
-00001c60: 6169 6e21 220a 2020 2020 2020 2020 2020  ain!".          
+00001c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c40: 7265 7475 726e 2022 416e 2065 7272 6f72  return "An error
+00001c50: 206f 6363 7572 6564 2120 506c 6561 7365   occured! Please
+00001c60: 2074 7279 2061 6761 696e 2122 0a20 2020   try again!".   
 00001c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c80: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00001c90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
 00001ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cb0: 7265 7475 726e 2022 416e 7377 6572 203a  return "Answer :
-00001cc0: 2022 202b 2076 6572 690a 2020 2020 2020   " + veri.      
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00001ce0: 6365 7074 284b 6579 4572 726f 7229 3a0a  cept(KeyError):.
-00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d00: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00001cb0: 2020 2020 2020 2072 6574 7572 6e20 2241         return "A
+00001cc0: 6e73 7765 7220 3a20 2220 2b20 7665 7269  nswer : " + veri
+00001cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ce0: 2020 2020 2065 7863 6570 7428 4b65 7945       except(KeyE
+00001cf0: 7272 6f72 293a 0a20 2020 2020 2020 2020  rror):.         
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00001d10: 6f6e 7469 6e75 650a                      ontinue.
```

### Comparing `bingpython-0.0.19/src/bingpython.egg-info/PKG-INFO` & `bingpython-0.0.20/src/bingpython.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: bingpython
-Version: 0.0.19
+Version: 0.0.20
 Summary: Bing AI Chat API
 Home-page: https://github.com/alicangnll/BingGPT-Python
 Author: Ali Can Gönüllü
 Author-email: alicangonullu@yahoo.com
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-Python/issues/new
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # BingGPT - Bing AI API on Python
 You can use BingGPT AI API on Python!
 # Requirements
 <ul>
   <li>Python 3.8+</li>
 </ul>
 <h1>Installation</h1>
 <ul>
   <li>pip install -r requirements.txt</li>
-  <li>pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install bingpython</li>
+  <li>pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install bingpython</li>
 </ul>
 <h1>Pictures</h1>
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png" />
 <img src="https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png" />
 <h1>Example</h1>
 <a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example.py">Example Code</a>
 <br><a href="https://github.com/alicangnll/BingGPT-Python/blob/main/examples/example2.py">Example Code 2</a>
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: bingpython Version: 0.0.19 Summary: Bing AI Chat
+Metadata-Version: 2.1 Name: bingpython Version: 0.0.20 Summary: Bing AI Chat
 API Home-page: https://github.com/alicangnll/BingGPT-Python Author: Ali Can
 GÃ¶nÃ¼llÃ¼ Author-email: alicangonullu@yahoo.com License: GNU General Public
 License v2.0 Project-URL: Bug Report, https://github.com/alicangnll/BingGPT-
 Python/issues/new Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Intended Audience :: Developers Classifier:
 Topic :: Software Development :: Libraries :: Python Modules Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
-# BingGPT - Bing AI API on Python You can use BingGPT AI API on Python! #
-Requirements
+License-File: LICENSE # BingGPT - Bing AI API on Python You can use BingGPT AI
+API on Python! # Requirements
     * Python 3.8+
 ****** Installation ******
     * pip install -r requirements.txt
-    * pip install dist/binggpt-0.0.18-py3-none-any.whl OR pip install
+    * pip install dist/binggpt-0.0.20-py3-none-any.whl OR pip install
       bingpython
 ****** Pictures ******
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic1.png]
 [https://raw.githubusercontent.com/alicangnll/BingGPT-Python/main/pic/pic2.png]
 ****** Example ******
 Example_Code
 Example_Code_2
```

