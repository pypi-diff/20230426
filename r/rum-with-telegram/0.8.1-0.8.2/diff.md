# Comparing `tmp/rum_with_telegram-0.8.1.tar.gz` & `tmp/rum_with_telegram-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rum_with_telegram-0.8.1.tar", last modified: Tue Apr 25 15:54:07 2023, max compression
+gzip compressed data, was "rum_with_telegram-0.8.2.tar", last modified: Wed Apr 26 09:35:07 2023, max compression
```

## Comparing `rum_with_telegram-0.8.1.tar` & `rum_with_telegram-0.8.2.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 15:54:07.209745 rum_with_telegram-0.8.1/
--rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.1/LICENSE
--rw-rw-rw-   0        0        0     1032 2023-04-25 15:54:07.208739 rum_with_telegram-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.1/README.md
--rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-04-25 15:54:07.193780 rum_with_telegram-0.8.1/rum_with_telegram/
--rw-rw-rw-   0        0        0      215 2023-04-25 15:52:44.000000 rum_with_telegram-0.8.1/rum_with_telegram/__init__.py
--rw-rw-rw-   0        0        0    22324 2023-04-25 15:52:55.000000 rum_with_telegram-0.8.1/rum_with_telegram/data_exchanger.py
--rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.1/rum_with_telegram/db_handle.py
--rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.1/rum_with_telegram/module.py
-drwxrwxrwx   0        0        0        0 2023-04-25 15:54:07.207743 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/
--rw-rw-rw-   0        0        0     1032 2023-04-25 15:54:07.000000 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-04-25 15:54:07.000000 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 15:54:07.000000 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-04-25 15:54:07.000000 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-04-25 15:54:07.000000 rum_with_telegram-0.8.1/rum_with_telegram.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 15:54:07.210732 rum_with_telegram-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1453 2023-04-25 15:52:44.000000 rum_with_telegram-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.946800 rum_with_telegram-0.8.2/
+-rw-rw-rw-   0        0        0     1087 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.2/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-04-26 09:35:07.944806 rum_with_telegram-0.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0       19 2023-03-22 04:17:54.000000 rum_with_telegram-0.8.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.917877 rum_with_telegram-0.8.2/local_test/
+-rw-rw-rw-   0        0        0       27 2023-04-26 08:37:26.000000 rum_with_telegram-0.8.2/local_test/__init__.py
+-rw-rw-rw-   0        0        0     1559 2023-04-26 08:37:39.000000 rum_with_telegram-0.8.2/local_test/config.py
+-rw-rw-rw-   0        0        0      101 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.2/local_test/local_test.py
+-rw-rw-rw-   0        0        0      143 2023-04-26 08:37:24.000000 rum_with_telegram-0.8.2/local_test/local_test_rum.py
+-rw-rw-rw-   0        0        0      163 2023-04-25 07:27:09.000000 rum_with_telegram-0.8.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.929846 rum_with_telegram-0.8.2/rum_with_telegram/
+-rw-rw-rw-   0        0        0      215 2023-04-26 09:34:21.000000 rum_with_telegram-0.8.2/rum_with_telegram/__init__.py
+-rw-rw-rw-   0        0        0     1038 2023-04-26 09:33:02.000000 rum_with_telegram-0.8.2/rum_with_telegram/config.py
+-rw-rw-rw-   0        0        0    23598 2023-04-26 09:33:06.000000 rum_with_telegram-0.8.2/rum_with_telegram/data_exchanger.py
+-rw-rw-rw-   0        0        0     2821 2023-04-25 07:27:11.000000 rum_with_telegram-0.8.2/rum_with_telegram/db_handle.py
+-rw-rw-rw-   0        0        0     1635 2023-04-19 05:46:46.000000 rum_with_telegram-0.8.2/rum_with_telegram/module.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:35:07.942815 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-04-26 09:35:07.000000 rum_with_telegram-0.8.2/rum_with_telegram.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:35:07.946800 rum_with_telegram-0.8.2/setup.cfg
+-rw-rw-rw-   0        0        0     1453 2023-04-26 09:34:33.000000 rum_with_telegram-0.8.2/setup.py
```

### Comparing `rum_with_telegram-0.8.1/LICENSE` & `rum_with_telegram-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.1/PKG-INFO` & `rum_with_telegram-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum_with_telegram
-Version: 0.8.1
+Version: 0.8.2
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.1/rum_with_telegram/data_exchanger.py` & `rum_with_telegram-0.8.2/rum_with_telegram/data_exchanger.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,31 @@
 
 from quorum_data_py import feed, get_trx_type, util
 from quorum_mininode_py import MiniNode
 from quorum_mininode_py.crypto import account
 from telegram import Bot, Update
 from telegram.ext import Application, CommandHandler, ContextTypes, MessageHandler, filters
 
+from rum_with_telegram.config import get_config
 from rum_with_telegram.db_handle import DBHandle
 from rum_with_telegram.module import Relation
 
 logger = logging.getLogger(__name__)
 
 
 class DataExchanger:
     """the data exchanger between telegram bot/channel/chat-group and rum group-chain"""
 
-    def __init__(self, config):
-        self.config = config
+    def __init__(self, config: dict = None, json_config_file: str = None):
+        if isinstance(config, str):
+            json_config_file = config
+            config = None
+        self.config = config or get_config(json_config_file)
+        if not self.config:
+            raise Exception("config is None")
         self.rum = MiniNode(self.config.RUM_SEED, self.config.ETH_PVTKEY)
         self.app = Application.builder().token(self.config.TG_BOT_TOKEN).build()
         self.db = DBHandle(self.config.DB_URL, echo=self.config.DB_ECHO)
         self.start_trx = None
 
     def _get_origin_post_id(self, rum_post_id: str):
         """get the origin post id for trx"""
@@ -61,14 +67,15 @@
             image = bytes(await image.download_as_bytearray())
         else:
             image = None
         images = [image] if image else None
         if reply_id:
             data = feed.reply(content=text, images=images, reply_id=reply_id)
         else:
+            text += f" {self.config.RUM_POST_FOOTER}"
             data = feed.new_post(content=text, images=images)
         if origin:
             data["origin"] = {
                 "type": "telegram",
                 "name": self.config.TG_CHANNEL_NAME,
                 "url": f"{self.config.TG_CHANNEL_URL}/{origin}",
             }
@@ -92,14 +99,16 @@
         context,
         extend_text: str,
         userid,
         reply_to_message_id,
         rum_post_url,
     ):
         """reply to user with rum post url"""
+        if not self.config.TG_REPLY_POSTURL:
+            return
         reply = f"⚜️ Success to blockchain.\n👉[{self.config.FEED_TITLE}]({rum_post_url})\n" + (
             extend_text or ""
         )
         await context.bot.send_message(
             chat_id=userid,
             text=reply,
             parse_mode="Markdown",
@@ -491,43 +500,63 @@
         await context.bot.send_message(
             chat_id=chat_id,
             text=text,
             reply_to_message_id=message_id,
             parse_mode="Markdown",
         )
 
+    async def command_my_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
+        logger.info("start command_my_nft")
+        # TODO
+
+    async def command_grant_nft(self, update: Update, context: ContextTypes.DEFAULT_TYPE):
+        logger.info("start command_grant_nft")
+        userid = update.message.from_user.id
+        if userid not in self.config.ADMIN_USERIDS:
+            reply = "You are not admin."
+            await context.bot.send_message(
+                chat_id=update.message.chat_id,
+                text=reply,
+                reply_to_message_id=update.message.message_id,
+            )
+            return
+        # TODO
+
     def run(self):
         self.app.add_handler(CommandHandler("start", self.command_start))
         self.app.add_handler(CommandHandler("profile", self.command_profile))
         self.app.add_handler(CommandHandler("show_pvtkey", self.command_show_pvtkey))
         # TODO: add logs to map userid and pvtkey
         self.app.add_handler(CommandHandler("new_pvtkey", self.command_new_pvtkey))
         self.app.add_handler(CommandHandler("import_pvtkey", self.command_import_pvtkey))
+        # TODO:
+        self.app.add_handler(CommandHandler("my_nft", self.command_my_nft))
+        self.app.add_handler(CommandHandler("grant_nft", self.command_grant_nft))
 
-        content_handle = (filters.TEXT | filters.PHOTO) & ~filters.COMMAND
+        content_filter = (filters.TEXT | filters.PHOTO) & ~filters.COMMAND
         # private chat message:
         # send to tg channel and rum group as new post
         # reply the feed_post_url to user in private chat and the comment of the channel post
         self.app.add_handler(
             MessageHandler(
-                content_handle & filters.ChatType.PRIVATE,
+                content_filter & filters.ChatType.PRIVATE,
                 self.handle_private_chat,
             )
         )
         # channel message:
         # send to rum group as new post; and reply to user in group chat
         self.app.add_handler(
             MessageHandler(
-                content_handle & filters.SenderChat(self.config.TG_CHANNEL_ID),
+                content_filter & filters.SenderChat(self.config.TG_CHANNEL_ID),
                 self.handle_channel_message,
             )
         )
         # group message:
         # send to rum group as comment of the pinned post or the reply-to post
         self.app.add_handler(
             MessageHandler(
-                content_handle & filters.SenderChat.SUPER_GROUP,
+                content_filter & filters.SenderChat.SUPER_GROUP,
                 self.handle_group_message,
             )
         )
 
         self.app.run_polling()
```

### Comparing `rum_with_telegram-0.8.1/rum_with_telegram/db_handle.py` & `rum_with_telegram-0.8.2/rum_with_telegram/db_handle.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.1/rum_with_telegram/module.py` & `rum_with_telegram-0.8.2/rum_with_telegram/module.py`

 * *Files identical despite different names*

### Comparing `rum_with_telegram-0.8.1/rum_with_telegram.egg-info/PKG-INFO` & `rum_with_telegram-0.8.2/rum_with_telegram.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rum-with-telegram
-Version: 0.8.1
+Version: 0.8.2
 Summary: A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.
 Home-page: https://github.com/liujuanjuan1984/rum_with_telegram
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/rum_with_telegram
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/rum_with_telegram/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `rum_with_telegram-0.8.1/setup.py` & `rum_with_telegram-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rum_with_telegram",
-    version="0.8.1",
+    version="0.8.2",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="A bot, send telegram update to rum group as trx, and get new trx from rum group to channel.",
     keywords=["python-telegram-bot", "rumsystem", "quorum"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/rum_with_telegram",
```

