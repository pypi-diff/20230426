# Comparing `tmp/rubpy-6.1.5.tar.gz` & `tmp/rubpy-6.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.1.5.tar", last modified: Wed Apr 26 15:08:29 2023, max compression
+gzip compressed data, was "rubpy-6.1.6.tar", last modified: Wed Apr 26 17:37:56 2023, max compression
```

## Comparing `rubpy-6.1.5.tar` & `rubpy-6.1.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.415061 rubpy-6.1.5/
--rw-rw-rw-   0        0        0     3347 2023-04-26 15:08:29.415061 rubpy-6.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2207 2023-04-24 00:06:56.000000 rubpy-6.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.305405 rubpy-6.1.5/rubpy/
--rw-rw-rw-   0        0        0      240 2023-04-26 15:08:14.000000 rubpy-6.1.5/rubpy/__init__.py
--rw-rw-rw-   0        0        0    41309 2023-04-26 15:05:42.000000 rubpy-6.1.5/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.389678 rubpy-6.1.5/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.399726 rubpy-6.1.5/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.5/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.5/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14190 2023-04-23 23:43:50.000000 rubpy-6.1.5/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.405264 rubpy-6.1.5/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    10949 2023-04-26 14:44:17.000000 rubpy-6.1.5/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.405264 rubpy-6.1.5/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.415061 rubpy-6.1.5/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.5/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.5/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:08:29.385368 rubpy-6.1.5/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3347 2023-04-26 15:08:29.000000 rubpy-6.1.5/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-04-26 15:08:29.000000 rubpy-6.1.5/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:08:29.000000 rubpy-6.1.5/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-26 15:08:29.000000 rubpy-6.1.5/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-26 15:08:29.000000 rubpy-6.1.5/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 15:08:29.415061 rubpy-6.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-04-26 15:08:04.000000 rubpy-6.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.847161 rubpy-6.1.6/
+-rw-rw-rw-   0        0        0     3378 2023-04-26 17:37:56.847161 rubpy-6.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.733400 rubpy-6.1.6/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-04-26 15:08:14.000000 rubpy-6.1.6/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    41309 2023-04-26 17:32:17.000000 rubpy-6.1.6/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.796291 rubpy-6.1.6/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     1531 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.811914 rubpy-6.1.6/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      907 2023-04-23 17:54:16.000000 rubpy-6.1.6/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2122 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    25829 2023-04-24 20:54:14.000000 rubpy-6.1.6/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.1.6/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.811914 rubpy-6.1.6/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    10949 2023-04-26 14:44:17.000000 rubpy-6.1.6/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.827536 rubpy-6.1.6/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2235 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.843153 rubpy-6.1.6/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.1.6/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.1.6/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-04-26 17:37:56.796291 rubpy-6.1.6/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-26 17:37:56.000000 rubpy-6.1.6/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 17:37:56.847161 rubpy-6.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-04-26 17:32:31.000000 rubpy-6.1.6/setup.py
```

### Comparing `rubpy-6.1.5/PKG-INFO` & `rubpy-6.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.5
+Version: 6.1.6
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
-        <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
+        <img src="https://raw.githubusercontent.com/shayanheidari01/rubika/master/icon.png" alt="Rubpy" width="128">
     </a>
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
@@ -50,34 +50,34 @@
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from rubpy import Client, handlers
+from rubpy import Client, handlers, Message
 
 async def main():
     async with Client(session='rubpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(update):
-            await update.reply('`hello` __from__ **rubpy**')
+        async def updates(message: Message):
+            await message.reply('`hello` __from__ **rubpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from rubpy import Client
 from asyncio import run
 
 async def main():
     async with Client(session='rubpy') as client:
-        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        result = await client.send_message('me', '`hello` __from__ **rubpy**')
         print(result)
 
 run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.6 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -14,25 +14,25 @@
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Accounts ```python import asyncio from rubpy import Client,
-handlers async def main(): async with Client(session='rubpy') as client:
-@client.on(handlers.MessageUpdates()) async def updates(update): await
-update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
-() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
-Client from asyncio import run async def main(): async with Client
-(session='rubpy') as client: result = await client.send_message('GUID',
-'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
-modern, elegant and asynchronous framework. It enables you to easily interact
-with the main Rubika API through a user account (custom client) or a bot
-identity (bot API alternative) using Python. ### Key Features - **Ready**:
-Install Rubpy with pip and start building your applications right away. -
-**Easy**: Makes the Rubika API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
+handlers, Message async def main(): async with Client(session='rubpy') as
+client: @client.on(handlers.MessageUpdates()) async def updates(message:
+Message): await message.reply('`hello` __from__ **rubpy**') await
+client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
+```python from rubpy import Client from asyncio import run async def main():
+async with Client(session='rubpy') as client: result = await
+client.send_message('me', '`hello` __from__ **rubpy**') print(result) run(main
+()) ``` **Rubpy** is a modern, elegant and asynchronous framework. It enables
+you to easily interact with the main Rubika API through a user account (custom
+client) or a bot identity (bot API alternative) using Python. ### Key Features
+- **Ready**: Install Rubpy with pip and start building your applications right
+away. - **Easy**: Makes the Rubika API simple and intuitive, while still
+allowing advanced usages. - **Elegant**: Low-level details are abstracted and
+re-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome,
+a high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
 and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.1.5/README.md` & `rubpy-6.1.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
     <a href="github.address">
-        <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
+        <img src="https://raw.githubusercontent.com/shayanheidari01/rubika/master/icon.png" alt="Rubpy" width="128">
     </a>
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
@@ -25,34 +25,34 @@
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from rubpy import Client, handlers
+from rubpy import Client, handlers, Message
 
 async def main():
     async with Client(session='rubpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(update):
-            await update.reply('`hello` __from__ **rubpy**')
+        async def updates(message: Message):
+            await message.reply('`hello` __from__ **rubpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from rubpy import Client
 from asyncio import run
 
 async def main():
     async with Client(session='rubpy') as client:
-        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        result = await client.send_message('me', '`hello` __from__ **rubpy**')
         print(result)
 
 run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Accounts ```python import asyncio from rubpy import Client,
-handlers async def main(): async with Client(session='rubpy') as client:
-@client.on(handlers.MessageUpdates()) async def updates(update): await
-update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
-() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
-Client from asyncio import run async def main(): async with Client
-(session='rubpy') as client: result = await client.send_message('GUID',
-'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
-modern, elegant and asynchronous framework. It enables you to easily interact
-with the main Rubika API through a user account (custom client) or a bot
-identity (bot API alternative) using Python. ### Key Features - **Ready**:
-Install Rubpy with pip and start building your applications right away. -
-**Easy**: Makes the Rubika API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
+handlers, Message async def main(): async with Client(session='rubpy') as
+client: @client.on(handlers.MessageUpdates()) async def updates(message:
+Message): await message.reply('`hello` __from__ **rubpy**') await
+client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
+```python from rubpy import Client from asyncio import run async def main():
+async with Client(session='rubpy') as client: result = await
+client.send_message('me', '`hello` __from__ **rubpy**') print(result) run(main
+()) ``` **Rubpy** is a modern, elegant and asynchronous framework. It enables
+you to easily interact with the main Rubika API through a user account (custom
+client) or a bot identity (bot API alternative) using Python. ### Key Features
+- **Ready**: Install Rubpy with pip and start building your applications right
+away. - **Easy**: Makes the Rubika API simple and intuitive, while still
+allowing advanced usages. - **Elegant**: Low-level details are abstracted and
+re-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome,
+a high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
 and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.1.5/rubpy/client.py` & `rubpy-6.1.6/rubpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -938,22 +938,22 @@
 
     async def add_folder(self,
             include_chat_types: list = None,
             exclude_chat_types: list = None,
             include_object_guids: list = None,
             exclude_object_guids: list = None
     ):
-        return await self(methods.contacts.AddFolder(
+        return await self(methods.settings.AddFolder(
             include_chat_types,
             exclude_chat_types,
             include_object_guids,
             exclude_object_guids))
 
     async def get_folders(self, last_state: int):
-        return await self(methods.contacts.GetFolders(last_state))
+        return await self(methods.settings.GetFolders(last_state))
 
     async def edit_folder(self,
             include_chat_types: list = None,
             exclude_chat_types: list = None,
             include_object_guids: list = None,
             exclude_object_guids: list = None
     ):
@@ -964,59 +964,59 @@
         if exclude_chat_types:
             updated_parameters.append('exclude_chat_types')
         if include_object_guids:
             updated_parameters.append('include_object_guids')
         if exclude_object_guids:
             updated_parameters.append('exclude_object_guids')
 
-        return await self(methods.contacts.EditFolder(
+        return await self(methods.settings.EditFolder(
             updated_parameters,
             include_chat_types,
             exclude_chat_types,
             include_object_guids,
             exclude_object_guids))
 
     async def delete_folder(self, folder_id: str):
-        return await self(methods.contacts.DeleteFolder(folder_id))
+        return await self(methods.settings.DeleteFolder(folder_id))
 
     async def update_profile(self, first_name: str = None, last_name: str = None, bio: str = None):
         updated_parameters = []
 
         if first_name:
             updated_parameters.append('first_name')
         if last_name:
             updated_parameters.append('last_name')
         if bio:
             updated_parameters.append('bio')
 
-        return await self(methods.contacts.UpdateProfile(updated_parameters, first_name, last_name, bio))
+        return await self(methods.settings.UpdateProfile(updated_parameters, first_name, last_name, bio))
 
     async def update_username(self, username: str):
-        return await self(methods.contacts.UpdateUsername(username))
+        return await self(methods.settings.UpdateUsername(username))
 
     async def get_two_passcode_status(self):
-        return await self(methods.contacts.GetTwoPasscodeStatus())
+        return await self(methods.settings.GetTwoPasscodeStatus())
 
     async def get_suggested_folders(self):
-        return await self(methods.contacts.GetSuggestedFolders())
+        return await self(methods.settings.GetSuggestedFolders())
 
     async def get_privacy_setting(self):
-        return await self(methods.contacts.GetPrivacySetting())
+        return await self(methods.settings.GetPrivacySetting())
 
     async def get_blocked_users(self):
-        return await self(methods.contacts.GetBlockedUsers())
+        return await self(methods.settings.GetBlockedUsers())
 
     async def get_my_sessions(self):
-        return await self(methods.contacts.GetMySessions())
+        return await self(methods.settings.GetMySessions())
 
     async def terminate_session(self, session_key: str):
-        return await self(methods.contacts.TerminateSession(session_key))
+        return await self(methods.settings.TerminateSession(session_key))
 
     async def setup_two_step_verification(self, password: str, hint: str, recovery_email: str):
-        return await self(methods.contacts.SetupTwoStepVerification(password, hint, recovery_email))
+        return await self(methods.settings.SetupTwoStepVerification(password, hint, recovery_email))
 
 # ---------------- Stickers Methods ----------------
 
     async def get_my_sticker_sets(self):
         return await self(methods.stickers.GetMyStickerSets())
 
     async def search_stickers(self, search_text: str = '', start_id: int = None):
```

### Comparing `rubpy-6.1.5/rubpy/crypto/crypto.py` & `rubpy-6.1.6/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/gadgets/classino.py` & `rubpy-6.1.6/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/gadgets/exceptions.py` & `rubpy-6.1.6/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/gadgets/grouping.py` & `rubpy-6.1.6/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/gadgets/methods.py` & `rubpy-6.1.6/rubpy/gadgets/methods.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -404,8 +404,8 @@
     def __dir__(self):
         return grouping.keys()
 
     def __getattr__(self, name) -> BaseGrouping:
         group = self.create(name, (BaseGrouping,), dir(self))
         return group(methods=grouping[group.__name__])
 
-sys.modules[__name__] = Methods(__name__)
+sys.modules[__name__] = Methods(__name__)
```

### Comparing `rubpy-6.1.5/rubpy/gadgets/thumbnail.py` & `rubpy-6.1.6/rubpy/gadgets/thumbnail.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/network/connection.py` & `rubpy-6.1.6/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/network/proxies.py` & `rubpy-6.1.6/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/sessions/sqliteSession.py` & `rubpy-6.1.6/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/sessions/stringSession.py` & `rubpy-6.1.6/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/structs/handlers.py` & `rubpy-6.1.6/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/structs/models.py` & `rubpy-6.1.6/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/structs/results.py` & `rubpy-6.1.6/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy/structs/struct.py` & `rubpy-6.1.6/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/rubpy.egg-info/PKG-INFO` & `rubpy-6.1.6/rubpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.1.5
+Version: 6.1.6
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -21,15 +21,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: opencv-python
 
 <p align="center">
     <a href="github.address">
-        <img src="https://upcdn.io/W142hJk/thumbnail/demo/4mrDXtYPJA.png.crop" alt="Rubpy" width="128">
+        <img src="https://raw.githubusercontent.com/shayanheidari01/rubika/master/icon.png" alt="Rubpy" width="128">
     </a>
     <br>
     <b>Rubika API Framework for Python</b>
     <br>
     <a href="https://github.com/shayanheidari01/rubika">
         Homepage
     </a>
@@ -50,34 +50,34 @@
 ## Rubpy
 
 > Elegant, modern and asynchronous Rubika API framework in Python for users and bots
 
 ### Accounts
 ```python
 import asyncio
-from rubpy import Client, handlers
+from rubpy import Client, handlers, Message
 
 async def main():
     async with Client(session='rubpy') as client:
         @client.on(handlers.MessageUpdates())
-        async def updates(update):
-            await update.reply('`hello` __from__ **rubpy**')
+        async def updates(message: Message):
+            await message.reply('`hello` __from__ **rubpy**')
         await client.run_until_disconnected()
 
 asyncio.run(main())
 ```
 
 **Another example:**
 ```python
 from rubpy import Client
 from asyncio import run
 
 async def main():
     async with Client(session='rubpy') as client:
-        result = await client.send_message('GUID', '`hello` __from__ **rubpy**')
+        result = await client.send_message('me', '`hello` __from__ **rubpy**')
         print(result)
 
 run(main())
 ```
 
 **Rubpy** is a modern, elegant and asynchronous framework. It enables you to easily interact with the main Rubika API through a user account (custom client) or a bot
 identity (bot API alternative) using Python.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.1.5 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.1.6 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -14,25 +14,25 @@
 Application Frameworks Requires-Python: ~=3.7 Description-Content-Type: text/
 markdown Provides-Extra: opencv-python
                                    [Rubpy]
                        Rubika API Framework for Python
                Homepage â¢ Documentation â¢ Releases â¢ News
 ## Rubpy > Elegant, modern and asynchronous Rubika API framework in Python for
 users and bots ### Accounts ```python import asyncio from rubpy import Client,
-handlers async def main(): async with Client(session='rubpy') as client:
-@client.on(handlers.MessageUpdates()) async def updates(update): await
-update.reply('`hello` __from__ **rubpy**') await client.run_until_disconnected
-() asyncio.run(main()) ``` **Another example:** ```python from rubpy import
-Client from asyncio import run async def main(): async with Client
-(session='rubpy') as client: result = await client.send_message('GUID',
-'`hello` __from__ **rubpy**') print(result) run(main()) ``` **Rubpy** is a
-modern, elegant and asynchronous framework. It enables you to easily interact
-with the main Rubika API through a user account (custom client) or a bot
-identity (bot API alternative) using Python. ### Key Features - **Ready**:
-Install Rubpy with pip and start building your applications right away. -
-**Easy**: Makes the Rubika API simple and intuitive, while still allowing
-advanced usages. - **Elegant**: Low-level details are abstracted and re-
-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome, a
-high-performance cryptography library written in C. - **Async**: Fully
+handlers, Message async def main(): async with Client(session='rubpy') as
+client: @client.on(handlers.MessageUpdates()) async def updates(message:
+Message): await message.reply('`hello` __from__ **rubpy**') await
+client.run_until_disconnected() asyncio.run(main()) ``` **Another example:**
+```python from rubpy import Client from asyncio import run async def main():
+async with Client(session='rubpy') as client: result = await
+client.send_message('me', '`hello` __from__ **rubpy**') print(result) run(main
+()) ``` **Rubpy** is a modern, elegant and asynchronous framework. It enables
+you to easily interact with the main Rubika API through a user account (custom
+client) or a bot identity (bot API alternative) using Python. ### Key Features
+- **Ready**: Install Rubpy with pip and start building your applications right
+away. - **Easy**: Makes the Rubika API simple and intuitive, while still
+allowing advanced usages. - **Elegant**: Low-level details are abstracted and
+re-presented in a more convenient way. - **Fast**: Boosted up by pycryptodome,
+a high-performance cryptography library written in C. - **Async**: Fully
 asynchronous (also usable synchronously if wanted, for convenience). -
 **Powerful**: Full access to Rubika's API to execute any official client action
 and more. ### Installing ``` bash pip3 install -U rubpy ```
```

### Comparing `rubpy-6.1.5/rubpy.egg-info/SOURCES.txt` & `rubpy-6.1.6/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.1.5/setup.py` & `rubpy-6.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.1.5',
+    version = '6.1.6',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

