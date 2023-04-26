# Comparing `tmp/shadpy-2.1.5.tar.gz` & `tmp/shadpy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadpy-2.1.5.tar", last modified: Mon Apr 24 22:41:18 2023, max compression
+gzip compressed data, was "shadpy-2.2.0.tar", last modified: Tue Apr 25 22:37:29 2023, max compression
```

## Comparing `shadpy-2.1.5.tar` & `shadpy-2.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.832350 shadpy-2.1.5/
--rw-rw-rw-   0        0        0     3366 2023-04-24 22:41:18.832350 shadpy-2.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2023-04-24 22:36:07.000000 shadpy-2.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 22:41:18.832350 shadpy-2.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1542 2023-04-24 22:41:13.000000 shadpy-2.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.801107 shadpy-2.1.5/shadpy/
--rw-rw-rw-   0        0        0      240 2023-04-24 22:38:01.000000 shadpy-2.1.5/shadpy/__init__.py
--rw-rw-rw-   0        0        0    32368 2023-04-24 20:56:07.000000 shadpy-2.1.5/shadpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.816730 shadpy-2.1.5/shadpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.816730 shadpy-2.1.5/shadpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 shadpy-2.1.5/shadpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25831 2023-04-24 22:38:49.000000 shadpy-2.1.5/shadpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 shadpy-2.1.5/shadpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.816730 shadpy-2.1.5/shadpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/network/__init__.py
--rw-rw-rw-   0        0        0    10591 2023-04-15 19:45:40.000000 shadpy-2.1.5/shadpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.816730 shadpy-2.1.5/shadpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.832350 shadpy-2.1.5/shadpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 shadpy-2.1.5/shadpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 shadpy-2.1.5/shadpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-24 22:41:18.816730 shadpy-2.1.5/shadpy.egg-info/
--rw-rw-rw-   0        0        0     3366 2023-04-24 22:41:18.000000 shadpy-2.1.5/shadpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-04-24 22:41:18.000000 shadpy-2.1.5/shadpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 22:41:18.000000 shadpy-2.1.5/shadpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-24 22:41:18.000000 shadpy-2.1.5/shadpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-24 22:41:18.000000 shadpy-2.1.5/shadpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.505554 shadpy-2.2.0/
+-rw-rw-rw-   0        0        0     3349 2023-04-25 22:37:29.505554 shadpy-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2205 2023-04-25 22:33:18.000000 shadpy-2.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 22:37:29.505554 shadpy-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-04-25 22:37:09.000000 shadpy-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.458300 shadpy-2.2.0/shadpy/
+-rw-rw-rw-   0        0        0      240 2023-04-25 22:06:08.000000 shadpy-2.2.0/shadpy/__init__.py
+-rw-rw-rw-   0        0        0    41244 2023-04-25 22:35:54.000000 shadpy-2.2.0/shadpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.473923 shadpy-2.2.0/shadpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.492548 shadpy-2.2.0/shadpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 shadpy-2.2.0/shadpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25831 2023-04-25 22:34:50.000000 shadpy-2.2.0/shadpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 shadpy-2.2.0/shadpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.492548 shadpy-2.2.0/shadpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10587 2023-04-25 22:36:56.000000 shadpy-2.2.0/shadpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.505554 shadpy-2.2.0/shadpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.505554 shadpy-2.2.0/shadpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 shadpy-2.2.0/shadpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 shadpy-2.2.0/shadpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-25 22:37:29.473923 shadpy-2.2.0/shadpy.egg-info/
+-rw-rw-rw-   0        0        0     3349 2023-04-25 22:37:29.000000 shadpy-2.2.0/shadpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-04-25 22:37:29.000000 shadpy-2.2.0/shadpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 22:37:29.000000 shadpy-2.2.0/shadpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-25 22:37:29.000000 shadpy-2.2.0/shadpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-25 22:37:29.000000 shadpy-2.2.0/shadpy.egg-info/top_level.txt
```

### Comparing `shadpy-2.1.5/PKG-INFO` & `shadpy-2.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadpy
-Version: 2.1.5
+Version: 2.2.0
 Summary: This is an unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: shad,rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -43,53 +43,53 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## ShadPy
 
 > Elegant, modern and asynchronous Shad API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from shadpy import Client, handlers, Message
+from shadpy import Client, handlers
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(message: Message):
+        async def updates(update):
             await update.reply('`hello` __from__ **shadpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from shadpy import Client
 from asyncio import run
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         result = await client.send_message('me', '`hello` __from__ **shadpy**')
         print(result)
 
 run(main())
 ```
 
 **ShadPy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Shad API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
 
-- **Ready**: Install Rubpy with pip and start building your applications right away.
+- **Ready**: Install ShadPy with pip and start building your applications right away.
 - **Easy**: Makes the Shad API simple and intuitive, while still allowing advanced usages.
 - **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Shad's API to execute any official client action and more.
 
 ### Installing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shadpy Version: 2.1.5 Summary: This is an
+Metadata-Version: 2.1 Name: shadpy Version: 2.2.0 Summary: This is an
 unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 shad,rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
@@ -12,27 +12,27 @@
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Software Development :: Libraries :: Application Frameworks Requires-Python:
 ~=3.7 Description-Content-Type: text/markdown Provides-Extra: opencv-python
                                    [Rubpy]
                         Shad API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
-## Rubpy > Elegant, modern and asynchronous Shad API framework in Python for
+## ShadPy > Elegant, modern and asynchronous Shad API framework in Python for
 users and bots ### Accounts ```python import asyncio from shadpy import Client,
-handlers, Message async def main(): async with Client(session='ShadPy') as
-client: @client.on(handlers.MessageUpdates()) async def updates(message:
-Message): await update.reply('`hello` __from__ **shadpy**') await
-client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
-```python from shadpy import Client from asyncio import run async def main():
-async with Client(session='ShadPy') as client: result = await
-client.send_message('me', '`hello` __from__ **shadpy**') print(result) run(main
-()) ``` **ShadPy** is a modern, elegant and asynchronous framework. It enables
-you to easily interact with the main Shad API through a user account (custom
-client) or a bot identity (bot API alternative) using Python. ### Key Features
-- **Ready**: Install Rubpy with pip and start building your applications right
-away. - **Easy**: Makes the Shad API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Shad's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U shadpy ```
+handlers async def main(): async with Client(session='shadpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **shadpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from shadpy import
+Client from asyncio import run async def main(): async with Client
+(session='shadpy') as client: result = await client.send_message('me', '`hello`
+__from__ **shadpy**') print(result) run(main()) ``` **ShadPy** is a modern,
+elegant and asynchronous framework. It enables you to easily interact with the
+main Shad API through a user account (custom client) or a bot identity (bot API
+alternative) using Python. ### Key Features - **Ready**: Install ShadPy with
+pip and start building your applications right away. - **Easy**: Makes the Shad
+API simple and intuitive, while still allowing advanced usages. - **Elegant**:
+Low-level details are abstracted and re-presented in a more convenient way. -
+**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
+written in C. - **Async**: Fully asynchronous (also usable synchronously if
+wanted, for convenience). - **Powerful**: Full access to Shad's API to execute
+any official client action and more. ### Installing ``` bash pip3 install -
+U shadpy ```
```

### Comparing `shadpy-2.1.5/README.md` & `shadpy-2.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -18,53 +18,53 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## ShadPy
 
 > Elegant, modern and asynchronous Shad API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from shadpy import Client, handlers, Message
+from shadpy import Client, handlers
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(message: Message):
+        async def updates(update):
             await update.reply('`hello` __from__ **shadpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from shadpy import Client
 from asyncio import run
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         result = await client.send_message('me', '`hello` __from__ **shadpy**')
         print(result)
 
 run(main())
 ```
 
 **ShadPy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Shad API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
 
-- **Ready**: Install Rubpy with pip and start building your applications right away.
+- **Ready**: Install ShadPy with pip and start building your applications right away.
 - **Easy**: Makes the Shad API simple and intuitive, while still allowing advanced usages.
 - **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Shad's API to execute any official client action and more.
 
 ### Installing
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
                                    [Rubpy]
                         Shad API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
-## Rubpy > Elegant, modern and asynchronous Shad API framework in Python for
+## ShadPy > Elegant, modern and asynchronous Shad API framework in Python for
 users and bots ### Accounts ```python import asyncio from shadpy import Client,
-handlers, Message async def main(): async with Client(session='ShadPy') as
-client: @client.on(handlers.MessageUpdates()) async def updates(message:
-Message): await update.reply('`hello` __from__ **shadpy**') await
-client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
-```python from shadpy import Client from asyncio import run async def main():
-async with Client(session='ShadPy') as client: result = await
-client.send_message('me', '`hello` __from__ **shadpy**') print(result) run(main
-()) ``` **ShadPy** is a modern, elegant and asynchronous framework. It enables
-you to easily interact with the main Shad API through a user account (custom
-client) or a bot identity (bot API alternative) using Python. ### Key Features
-- **Ready**: Install Rubpy with pip and start building your applications right
-away. - **Easy**: Makes the Shad API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Shad's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U shadpy ```
+handlers async def main(): async with Client(session='shadpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **shadpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from shadpy import
+Client from asyncio import run async def main(): async with Client
+(session='shadpy') as client: result = await client.send_message('me', '`hello`
+__from__ **shadpy**') print(result) run(main()) ``` **ShadPy** is a modern,
+elegant and asynchronous framework. It enables you to easily interact with the
+main Shad API through a user account (custom client) or a bot identity (bot API
+alternative) using Python. ### Key Features - **Ready**: Install ShadPy with
+pip and start building your applications right away. - **Easy**: Makes the Shad
+API simple and intuitive, while still allowing advanced usages. - **Elegant**:
+Low-level details are abstracted and re-presented in a more convenient way. -
+**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
+written in C. - **Async**: Fully asynchronous (also usable synchronously if
+wanted, for convenience). - **Powerful**: Full access to Shad's API to execute
+any official client action and more. ### Installing ``` bash pip3 install -
+U shadpy ```
```

### Comparing `shadpy-2.1.5/setup.py` & `shadpy-2.2.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
-requirements = ['aiohttp', 'pycryptodome']
+requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'shadpy',
-    version = '2.1.5',
+    version = '2.2.0',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Shad accounts.',
     keywords = ['shad', 'rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

### Comparing `shadpy-2.1.5/shadpy/client.py` & `shadpy-2.2.0/shadpy/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import os
+import io
+import aiofiles
 import logging
 from .crypto import Crypto
 from .structs import Struct
 from . import __name__ as logger_name
 from .network import Connection, Proxies
 from .gadgets import exceptions, methods, thumbnail
 from .sessions import StringSession, SQLiteSession
 
 
 class Client:
     configuire = {
-        'package': 'web.rubika.ir',
+        'package': 'web.shad.ir',
         'platform': 'Web',
         'app_name': 'Main',
         'user_agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
                        'AppleWebKit/537.36 (KHTML, like Gecko)'
                        'Chrome/102.0.0.0 Safari/537.36'),
         'api_version': '5',
-        'app_version': '4.2.0'
+        'app_version': '4.1.16'
     }
 
     def __init__(self,
         session,
         proxy=None,
         logger=None,
         timeout=20,
@@ -474,14 +476,268 @@
         return await self(
             methods.messages.SendMessage(
                 object_guid,
                 message=message,
                 file_inline=file_inline,
                 reply_to_message_id=reply_to_message_id))
 
+    async def send_photo(self,
+        object_guid: str,
+        photo: bytes,
+        caption: str = None,
+        file_name: str = None,
+        width: int = None,
+        height: int = None,
+        thumb: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(photo) != bytes:
+            async with aiofiles.open(photo, 'rb') as file:
+                file_name = os.path.basename(photo)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                photo = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        thumb = thumbnail.MakeThumbnail(photo)
+
+        file_inline = await self.upload(photo, *args, **kwargs)
+        file_inline['type'] = 'Image'
+
+        if thumb and width and height != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_file(self,
+        object_guid: str,
+        file: bytes,
+        caption: str = None,
+        file_name: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(file) != bytes:
+            async with aiofiles.open(file, 'rb') as ofile:
+                file_name = os.path.basename(file)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await ofile.read()
+                await ofile.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(file, *args, **kwargs)
+        file_inline['type'] = 'File'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_gif(self,
+        object_guid: str,
+        gif: bytes,
+        caption: str = None,
+        file_name: str = None,
+        thumb: str = None,
+        time: str = None,
+        width: int = None,
+        height: int = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(gif) != bytes:
+            async with aiofiles.open(gif, 'rb') as file:
+                file_name = os.path.basename(gif)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(gif, *args, **kwargs)
+        file_inline['type'] = 'Gif'
+
+        thumb = thumbnail.MakeThumbnail.from_video(gif)
+
+        if thumb and width and height and time != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+            file_inline['time'] = time
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['time'] = thumb.seconds
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_video(self,
+        object_guid: str,
+        video: bytes,
+        caption: str = None,
+        file_name: str = None,
+        thumb: str = None,
+        time: str = None,
+        width: int = None,
+        height: int = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(video) != bytes:
+            async with aiofiles.open(video, 'rb') as file:
+                file_name = os.path.basename(video)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(video, *args, **kwargs)
+        file_inline['type'] = 'Video'
+
+        thumb = thumbnail.MakeThumbnail.from_video(video)
+
+        if thumb and width and height and time != None:
+            file_inline['width'] = width
+            file_inline['height'] = height
+            file_inline['thumb_inline'] = thumb
+            file_inline['time'] = time
+        else:
+            if isinstance(thumb, thumbnail.Thumbnail):
+                file_inline['time'] = thumb.seconds
+                file_inline['width'] = thumb.width
+                file_inline['height'] = thumb.height
+                file_inline['thumb_inline'] = thumb.to_base64()
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_music(self,
+        object_guid: str,
+        music: bytes,
+        caption: str = None,
+        file_name: str = None,
+        time: str = None,
+        music_performer: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(music) != bytes:
+            async with aiofiles.open(music, 'rb') as file:
+                file_name = os.path.basename(music)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(music, *args, **kwargs)
+        file_inline['type'] = 'Music'
+        file_inline['auto_play'] = False
+        file_inline['music_performer'] = kwargs.get('performer', music_performer or '')
+
+        if time != None:
+            file_inline['time'] = time
+        else:
+            file_inline['time'] = '60'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
+    async def send_voice(self,
+        object_guid: str,
+        music: bytes,
+        caption: str = None,
+        file_name: str = None,
+        time: str = None,
+        reply_to_message_id: str = None,
+        *args,
+        **kwargs,
+    ):
+        if object_guid.lower() in ('me', 'self', 'cloud'):
+            object_guid = self._guid
+
+        if type(music) != bytes:
+            async with aiofiles.open(music, 'rb') as file:
+                file_name = os.path.basename(music)
+                kwargs['file_name'] = kwargs.get('file_name', file_name)
+                file = await file.read()
+                await file.close()
+        else:
+            kwargs['file_name'] = kwargs.get('file_name', file_name)
+
+        file_inline = await self.upload(music, *args, **kwargs)
+        file_inline['type'] = 'Voice'
+        file_inline['mime'] = 'ogg'
+        file_inline['auto_play'] = False
+
+        if time != None:
+            file_inline['time'] = time
+        else:
+            file_inline['time'] = '60'
+
+        return await self(
+            methods.messages.SendMessage(
+                object_guid,
+                message=caption,
+                file_inline=file_inline,
+                reply_to_message_id=reply_to_message_id))
+
     async def edit_message(self, object_guid: str, message_id: str, text: str):
         return await self(methods.messages.EditMessage(object_guid, message_id, text))
 
     async def delete_messages(self, object_guid: str, message_ids: list, type: str = 'Global'):
         return await self(methods.messages.DeleteMessages(object_guid, message_ids, type))
 
     async def request_send_file(self, file_name: str, size: int, mime: str):
```

### Comparing `shadpy-2.1.5/shadpy/crypto/crypto.py` & `shadpy-2.2.0/shadpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/gadgets/classino.py` & `shadpy-2.2.0/shadpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/gadgets/exceptions.py` & `shadpy-2.2.0/shadpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/gadgets/grouping.py` & `shadpy-2.2.0/shadpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/gadgets/methods.py` & `shadpy-2.2.0/shadpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/gadgets/thumbnail.py` & `shadpy-2.2.0/shadpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/network/connection.py` & `shadpy-2.2.0/shadpy/network/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     """Internal class"""
 
     def __init__(self, client):
         self._client = client
         self._connection = aiohttp.ClientSession(
             connector=self._client._proxy,
             headers={'user-agent': self._client._user_agent,
-            	'origin': 'https://web.rubika.ir',
-            	'referer': 'https://web.rubika.ir/'},
+            	'origin': 'https://web.shad.ir',
+            	'referer': 'https://web.shad.ir/'},
             timeout=aiohttp.ClientTimeout(total=self._client._timeout))
 
     async def _dcs(self):
         if not self._client._dcs:
             self._client._dcs = await self.execute(
                 methods.authorisations.GetDCs())
```

### Comparing `shadpy-2.1.5/shadpy/network/proxies.py` & `shadpy-2.2.0/shadpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/sessions/sqliteSession.py` & `shadpy-2.2.0/shadpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/sessions/stringSession.py` & `shadpy-2.2.0/shadpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/structs/handlers.py` & `shadpy-2.2.0/shadpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/structs/models.py` & `shadpy-2.2.0/shadpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/structs/results.py` & `shadpy-2.2.0/shadpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy/structs/struct.py` & `shadpy-2.2.0/shadpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `shadpy-2.1.5/shadpy.egg-info/PKG-INFO` & `shadpy-2.2.0/shadpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadpy
-Version: 2.1.5
+Version: 2.2.0
 Summary: This is an unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: shad,rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -43,53 +43,53 @@
     </a>
     •
     <a href="https://t.me/rubika_library">
         News
     </a>
 </p>
 
-## Rubpy
+## ShadPy
 
 > Elegant, modern and asynchronous Shad API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from shadpy import Client, handlers, Message
+from shadpy import Client, handlers
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(message: Message):
+        async def updates(update):
             await update.reply('`hello` __from__ **shadpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from shadpy import Client
 from asyncio import run
 
 async def main():
-    async with Client(session='ShadPy') as client:
+    async with Client(session='shadpy') as client:
         result = await client.send_message('me', '`hello` __from__ **shadpy**')
         print(result)
 
 run(main())
 ```
 
 **ShadPy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Shad API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
 
 
 ### Key Features
 
-- **Ready**: Install Rubpy with pip and start building your applications right away.
+- **Ready**: Install ShadPy with pip and start building your applications right away.
 - **Easy**: Makes the Shad API simple and intuitive, while still allowing advanced usages.
 - **Elegant**: Low-level details are abstracted and re-presented in a more convenient way.
 - **Fast**: Boosted up by pycryptodome, a high-performance cryptography library written in C.
 - **Async**: Fully asynchronous (also usable synchronously if wanted, for convenience).
 - **Powerful**: Full access to Shad's API to execute any official client action and more.
 
 ### Installing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shadpy Version: 2.1.5 Summary: This is an
+Metadata-Version: 2.1 Name: shadpy Version: 2.2.0 Summary: This is an
 unofficial library and fastest library for deploying robots on Shad accounts.
 Home-page: https://github.com/shayanheidari01/rubika Author: Shayan Heidari
 Author-email: contact@shayanheidari.info Keywords:
 shad,rubika,rubpy,chat,bot,robot,asyncio Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
@@ -12,27 +12,27 @@
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic ::
 Software Development :: Libraries :: Application Frameworks Requires-Python:
 ~=3.7 Description-Content-Type: text/markdown Provides-Extra: opencv-python
                                    [Rubpy]
                         Shad API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
-## Rubpy > Elegant, modern and asynchronous Shad API framework in Python for
+## ShadPy > Elegant, modern and asynchronous Shad API framework in Python for
 users and bots ### Accounts ```python import asyncio from shadpy import Client,
-handlers, Message async def main(): async with Client(session='ShadPy') as
-client: @client.on(handlers.MessageUpdates()) async def updates(message:
-Message): await update.reply('`hello` __from__ **shadpy**') await
-client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
-```python from shadpy import Client from asyncio import run async def main():
-async with Client(session='ShadPy') as client: result = await
-client.send_message('me', '`hello` __from__ **shadpy**') print(result) run(main
-()) ``` **ShadPy** is a modern, elegant and asynchronous framework. It enables
-you to easily interact with the main Shad API through a user account (custom
-client) or a bot identity (bot API alternative) using Python. ### Key Features
-- **Ready**: Install Rubpy with pip and start building your applications right
-away. - **Easy**: Makes the Shad API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
-asynchronous (also usable synchronously if wanted, for convenience). -
-**Powerful**: Full access to Shad's API to execute any official client action
-and more. ### Installing ``` bash pip3 install -U shadpy ```
+handlers async def main(): async with Client(session='shadpy') as client:
+@client.on(handlers.MessageUpdates()) async def updates(update): await
+update.reply('`hello` __from__ **shadpy**') await client.run_until_disconnected
+() asyncio.run(main()) ``` **Another example:** ```python from shadpy import
+Client from asyncio import run async def main(): async with Client
+(session='shadpy') as client: result = await client.send_message('me', '`hello`
+__from__ **shadpy**') print(result) run(main()) ``` **ShadPy** is a modern,
+elegant and asynchronous framework. It enables you to easily interact with the
+main Shad API through a user account (custom client) or a bot identity (bot API
+alternative) using Python. ### Key Features - **Ready**: Install ShadPy with
+pip and start building your applications right away. - **Easy**: Makes the Shad
+API simple and intuitive, while still allowing advanced usages. - **Elegant**:
+Low-level details are abstracted and re-presented in a more convenient way. -
+**Fast**: Boosted up by pycryptodome, a high-performance cryptography library
+written in C. - **Async**: Fully asynchronous (also usable synchronously if
+wanted, for convenience). - **Powerful**: Full access to Shad's API to execute
+any official client action and more. ### Installing ``` bash pip3 install -
+U shadpy ```
```

### Comparing `shadpy-2.1.5/shadpy.egg-info/SOURCES.txt` & `shadpy-2.2.0/shadpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

