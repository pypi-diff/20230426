# Comparing `tmp/yeref-0.1.45.tar.gz` & `tmp/yeref-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.45.tar", last modified: Sun Apr 23 14:48:57 2023, max compression
+gzip compressed data, was "yeref-0.1.46.tar", last modified: Tue Apr 25 13:56:56 2023, max compression
```

## Comparing `yeref-0.1.45.tar` & `yeref-0.1.46.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 14:48:57.930731 yeref-0.1.45/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 14:48:57.930948 yeref-0.1.45/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-23 14:48:57.931816 yeref-0.1.45/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-23 14:48:44.000000 yeref-0.1.45/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 14:48:57.925196 yeref-0.1.45/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.45/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   101605 2023-04-23 12:10:51.000000 yeref-0.1.45/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   188506 2023-04-23 14:46:03.000000 yeref-0.1.45/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-23 14:48:57.930108 yeref-0.1.45/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-23 14:48:57.000000 yeref-0.1.45/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-23 14:48:57.000000 yeref-0.1.45/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-23 14:48:57.000000 yeref-0.1.45/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-23 14:48:57.000000 yeref-0.1.45/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.913917 yeref-0.1.46/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-25 13:56:56.914094 yeref-0.1.46/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-04-25 13:56:56.914938 yeref-0.1.46/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1154 2023-04-25 13:56:43.000000 yeref-0.1.46/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.908894 yeref-0.1.46/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.46/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   162440 2023-04-25 13:55:33.000000 yeref-0.1.46/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   188525 2023-04-24 20:15:25.000000 yeref-0.1.46/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-04-25 13:56:56.913071 yeref-0.1.46/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-04-25 13:56:56.000000 yeref-0.1.46/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.45/setup.py` & `yeref-0.1.46/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.45',
+      version='0.1.46',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,10 +39,10 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.44-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.46-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
```

### Comparing `yeref-0.1.45/yeref/yeref.py` & `yeref-0.1.46/yeref/yeref.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 lkjhgfdsa_channel_id = -1001657854832
 lkjhgfdsa_channel_un = "lkjhgfdsa_channel"
 tg_ch_ads_un = 'kiejakn3_djdjn4m_ads'
 tg_ch_ads_id = -1001921910898
 price_one = 200
 price_all = 500
 
-TGPH_TOKEN_BAN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
+TGPH_TOKEN_MAIN = 'a9335172886eae62ec0743bf8a4e195286ec30cff067da5fd1db2899d008'
 TGPH_TOKEN_BROADCAST = 'b348a7a3964bbb4df2b66f8dbcd142e9dbf22ce58478a96bab3761dba51c'
 pp = 'https://telegra.ph/broadcasting-04-22'
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
@@ -198,15 +198,15 @@
 # endregion
 
 
 # region menu
 async def is_ban_menu(chat_id):
     result = False
     try:
-        telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
@@ -214,15 +214,15 @@
                     if str(chat_id) in ban_ids:
                         return True
                     break
             except Exception as e:
                 logger.info(log_ % str(e))
                 await asyncio.sleep(round(random.uniform(0, 1), 2))
 
-        # telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        # telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         # html_ = {'one': '1', 'two': '2'}
         # html_ = json.dumps(html_, ensure_ascii=False)
         # page_ = telegraph_.create_page(title='broadcasting', html_content=html_, author_name='bot_username', author_url='https://t.me/bot_username', return_content=True)
         # page_url = page_['url']
     except TelegramRetryAfter as e:
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
@@ -233,15 +233,15 @@
         return result
 
 
 async def ban_handler_menu(bot, chat_id, prepare_ids):
     try:
         prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
         if not len(prepare_ids): return
-        telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
@@ -269,15 +269,15 @@
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def unban_handler_menu(bot, chat_id, prepare_ids):
     try:
         prepare_ids = [prepare_id for prepare_id in prepare_ids if prepare_id.isdigit()]
         if not len(prepare_ids): return
-        telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'ban-04-11-7':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=True)
                     ban_ids = str(page['content']).split()
@@ -303,15 +303,15 @@
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
 async def check_tgph_posts(bot_username, BASE_D):
     try:
-        telegraph_ = Telegraph(access_token=TGPH_TOKEN_BAN)
+        telegraph_ = Telegraph(access_token=TGPH_TOKEN_MAIN)
         pages = telegraph_.get_page_list()
 
         for item in pages['pages']:
             try:
                 if item['path'] == 'broadcasting-04-22':
                     page = telegraph_.get_page(path=item['path'], return_content=True, return_html=False)
                     content_json = json.loads(str(page['content'][0]))
@@ -1792,15 +1792,15 @@
         logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
 
 
-async def edit_inline_admin(post_id, inline_message_id, current, len_):
+async def edit_inline_admin(bot, post_id, inline_message_id, current, len_, BASE_D):
     result = None
     try:
         sql = "SELECT POST_TEXT, POST_MEDIATYPE, POST_FILEID, POST_FILEIDNOTE, POST_BUTTON, POST_ISBUTTON, " \
               "POST_TGPHLINK, POST_ISTGPH, POST_ISGALLERY, POST_ISSPOILER FROM POST WHERE POST_ID=?"
         data_posts = await db_select(sql, (post_id,), BASE_D)
         if not len(data_posts): return
         item = data_posts[0]
```

