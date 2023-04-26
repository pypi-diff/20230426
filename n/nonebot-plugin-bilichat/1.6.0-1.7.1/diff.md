# Comparing `tmp/nonebot_plugin_bilichat-1.6.0.tar.gz` & `tmp/nonebot_plugin_bilichat-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-1.6.0.tar", last modified: Sun Apr 23 05:57:40 2023, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-1.7.1.tar", last modified: Wed Apr 26 17:17:42 2023, max compression
```

## Comparing `nonebot_plugin_bilichat-1.6.0.tar` & `nonebot_plugin_bilichat-1.7.1.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0    34523 2023-04-23 05:57:30.828880 nonebot_plugin_bilichat-1.6.0/LICENSE
--rw-r--r--   0        0        0    11739 2023-04-23 05:57:30.828880 nonebot_plugin_bilichat-1.6.0/README.md
--rw-r--r--   0        0        0     7893 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     4809 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0      513 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6226 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0     4806 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py
--rw-r--r--   0        0        0      927 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/column_resolve.py
--rw-r--r--   0        0        0     5262 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/content_resolve.py
--rw-r--r--   0        0        0     8900 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py
--rw-r--r--   0        0        0     3800 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      399 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     1868 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     4102 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      341 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     2854 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1127 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/cache.py
--rw-r--r--   0        0        0       93 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      261 2023-04-23 05:57:30.836880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0   248896 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg
--rw-r--r--   0        0        0     1045 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     5681 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py
--rw-r--r--   0        0        0     4856 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2359 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1448 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/text_to_image.py
--rw-r--r--   0        0        0     1764 2023-04-23 05:57:30.840880 nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py
--rw-r--r--   0        0        0     1407 2023-04-23 05:57:40.672985 nonebot_plugin_bilichat-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    13028 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-26 17:17:10.874528 nonebot_plugin_bilichat-1.7.1/LICENSE
+-rw-r--r--   0        0        0    11739 2023-04-26 17:17:10.874528 nonebot_plugin_bilichat-1.7.1/README.md
+-rw-r--r--   0        0        0     6000 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     4809 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0      513 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6226 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0     4806 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py
+-rw-r--r--   0        0        0      871 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/column_resolve.py
+-rw-r--r--   0        0        0     6439 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/content_resolve.py
+-rw-r--r--   0        0        0     8900 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py
+-rw-r--r--   0        0        0     3800 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      399 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     1868 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     4102 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      341 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     2854 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1127 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/cache.py
+-rw-r--r--   0        0        0      387 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/content.py
+-rw-r--r--   0        0        0       93 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      261 2023-04-26 17:17:10.882527 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0   248896 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg
+-rw-r--r--   0        0        0     1045 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     5681 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py
+-rw-r--r--   0        0        0     4856 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2359 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1448 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/text_to_image.py
+-rw-r--r--   0        0        0     1068 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/utils.py
+-rw-r--r--   0        0        0     1780 2023-04-26 17:17:10.886528 nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py
+-rw-r--r--   0        0        0     1407 2023-04-26 17:17:42.078955 nonebot_plugin_bilichat-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13028 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-1.7.1/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-1.6.0/LICENSE` & `nonebot_plugin_bilichat-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/README.md` & `nonebot_plugin_bilichat-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,49 +2,48 @@
 import shlex
 from itertools import chain
 from typing import Union, cast
 
 from nonebot.adapters import MessageSegment
 from nonebot.adapters.onebot.v11 import Bot as V11_Bot
 from nonebot.adapters.onebot.v11 import GroupMessageEvent as V11_GME
-from nonebot.adapters.onebot.v11 import Message as V11_Message
 from nonebot.adapters.onebot.v11 import MessageEvent as V11_ME
-from nonebot.adapters.onebot.v11 import MessageSegment as V11_MS
 from nonebot.adapters.onebot.v11 import PrivateMessageEvent as V11_PME
 from nonebot.adapters.onebot.v12 import Bot as V12_Bot
-from nonebot.adapters.onebot.v12 import ChannelMessageEvent as V12_CME
 from nonebot.adapters.onebot.v12 import GroupMessageEvent as V12_GME
 from nonebot.adapters.onebot.v12 import MessageEvent as V12_ME
-from nonebot.adapters.onebot.v12 import MessageSegment as V12_MS
 from nonebot.adapters.onebot.v12 import PrivateMessageEvent as V12_PME
 from nonebot.consts import REGEX_GROUP, REGEX_STR
 from nonebot.exception import FinishedException
 from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Depends
 from nonebot.plugin import PluginMetadata, on_regex
 from nonebot.rule import Rule
 from nonebot.typing import T_State
 
 from .config import __version__, plugin_config
 from .lib.b23_extract import b23_extract
-from .lib.content_resolve import get_video_basic, get_video_cache
+from .lib.content_resolve import get_column_basic, get_content_cache, get_video_basic
 from .model.arguments import Options, parser
 from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
+from .utils import get_image, get_reply
 
 if plugin_config.bilichat_openai_token or plugin_config.bilichat_newbing_cookie:
     ENABLE_SUMMARY = True
     from .summary import summarization
 else:
     ENABLE_SUMMARY = False
 
 if plugin_config.bilichat_word_cloud:
     from .wordcloud.wordcloud import wordcloud
 
+FUTUER_FUCTIONS = ENABLE_SUMMARY or plugin_config.bilichat_word_cloud
+
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="一个通过 OpenAI 来对b站视频进行总结插件",
     usage="直接发送视频链接即可",
     extra={
         "author": "djkcyl & Well404",
         "version": __version__,
@@ -67,15 +66,15 @@
     #     return plugin_config.bilichat_enable_v12_channel
     else:
         state["_uid_"] = "unkown"
         return plugin_config.bilichat_enable_unkown_src
 
 
 bili = on_regex(
-    r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})",
+    r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})",
     block=plugin_config.bilichat_block,
     priority=1,
     rule=Rule(_bili_check),
 )
 
 b23 = on_regex(
     r"b23.(tv|wtf)[\\/]+(\w+)",
@@ -100,123 +99,78 @@
 async def get_bili_number_re(state: T_State):
     state["bili_number"] = state[REGEX_STR]
 
 
 @b23.handle()
 async def get_bili_number_b23(state: T_State):
     if matched := re.search(
-        r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})", await b23_extract(state[REGEX_GROUP])  # type: ignore
+        r"av(\d{1,15})|BV(1[A-Za-z0-9]{2}4.1.7[A-Za-z0-9]{2})|cv(\d{1,16})", await b23_extract(state[REGEX_GROUP])  # type: ignore
     ):
         state["bili_number"] = matched.group()
 
 
 @bili.handle()
 @b23.handle()
-async def video_info_v11(
-    bot: V11_Bot, event: V11_ME, state: T_State, matcher: Matcher, options: Options = Depends(get_args)
+async def video_info(
+    bot: Union[V11_Bot, V12_Bot],
+    event: Union[V11_ME, V12_ME],
+    state: T_State,
+    matcher: Matcher,
+    options: Options = Depends(get_args),
 ):
-    # sourcery skip: raise-from-previous-error
+    reply = await get_reply(event)
     # basic info
-    msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
-    if not msg or not info:
-        await matcher.finish()
-    reply = V11_MS.reply(event.message_id)
-    if not img:
-        await matcher.finish(reply + msg)
-    elif img != "IMG_RENDER_DISABLED":
-        image = V11_MS.image(img)
-        msgid = (await matcher.send(reply + image + msg))["message_id"]
-        if plugin_config.bilichat_reply_to_basic_info:
-            reply = V11_MS.reply(msgid)
+    bili_number, uid = state["bili_number"], state["_uid_"]
+    if bili_number[:2] in ["BV", "bv", "av"]:
+        msg, img, info = await get_video_basic(bili_number, uid)
+        if not msg or not info:
+            raise FinishedException
+        if not img:
+            await matcher.finish(reply + msg)
+        elif img != "IMG_RENDER_DISABLED":
+            image = await get_image(img, bot)
+            msgid = (await matcher.send(reply + image + msg))["message_id"]  # type: ignore
+            if plugin_config.bilichat_reply_to_basic_info:
+                reply = await get_reply(event, msgid)
+    elif bili_number[:2] == "cv" and FUTUER_FUCTIONS:
+        info = await get_column_basic(bili_number, uid)
+        if not info:
+            raise FinishedException
+        elif isinstance(info, str):
+            await matcher.finish(reply + info)
+    else:
+        raise FinishedException
 
     # furtuer fuctions
-    if not ENABLE_SUMMARY and not plugin_config.bilichat_word_cloud:
+    if not FUTUER_FUCTIONS:
         raise FinishedException
 
     # get video cache
     try:
-        cache = await get_video_cache(info, options)
+        cache = await get_content_cache(info, options)
     except AbortError as e:
         logger.exception(e)
         await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
     except Exception as e:
         capture_exception()
         logger.exception(e)
         await matcher.finish(f"{reply}未知错误: {e}")
 
     # wordcloud
     wc_image = ""
     if plugin_config.bilichat_word_cloud:
-        if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-            wc_image = V11_MS.image(image)
+        if image := await wordcloud(cache=cache, cid=str(info.cid)):
+            wc_image = await get_image(image, bot)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
     # summary
     summary = ""
     if ENABLE_SUMMARY:
-        if summary := await summarization(cache=cache, cid=str(info["cid"])):
+        if summary := await summarization(cache=cache, cid=str(info.cid)):
             if isinstance(summary, bytes):
-                summary = V11_MS.image(summary)
+                summary = await get_image(summary, bot)
         else:
             await matcher.finish(f"{reply}视频无有效字幕")
 
     if wc_image or summary:
-        await matcher.finish(reply + wc_image + summary)
-
-
-async def get_image_v12(bot: V12_Bot, bili_number: str, suffix: str, data):
-    fileid = await bot.upload_file(type="data", name=f"{bili_number}_{suffix}.jpg", data=data)
-    return V12_MS.image(file_id=fileid["file_id"])
-
-
-@bili.handle()
-@b23.handle()
-async def video_info_v12(
-    bot: V12_Bot, event: V12_ME, state: T_State, matcher: Matcher, options: Options = Depends(get_args)
-):
-    # basic info
-    msg, img, info = await get_video_basic(state["bili_number"], state["_uid_"])
-    if not msg:
-        await matcher.finish()
-    reply = V12_MS.reply(message_id=event.message_id, user_id=event.get_user_id())
-    if not img or not info:
-        await matcher.finish(reply + msg)
-    elif img != "IMG_RENDER_DISABLED":
-        image = await get_image_v12(bot, state["bili_number"], suffix="basic", data=img)
-        msgid = (await matcher.send(reply + image + msg))["message_id"]
-        if plugin_config.bilichat_reply_to_basic_info:
-            reply = V12_MS.reply(msgid)
-
-    # furtuer fuctions
-    if not ENABLE_SUMMARY and not plugin_config.bilichat_word_cloud:
-        raise FinishedException
-
-    try:
-        cache = await get_video_cache(info, options)
-    except AbortError as e:
-        logger.exception(e)
-        await matcher.finish(f"{reply}视频字幕获取失败: {str(e)}")
-    except Exception as e:
-        capture_exception()
-        logger.exception(e)
-        await matcher.finish(f"{reply}未知错误: {str(e)}")
-
-    # wordcloud
-    wc_image = ""
-    if plugin_config.bilichat_word_cloud:
-        if image := await wordcloud(cache=cache, cid=str(info["cid"])):
-            wc_image = await get_image_v12(bot, state["bili_number"], "wc", data=image)
-        else:
-            await matcher.send(f"{reply}视频无有效字幕")
-
-    # summary
-    summary = ""
-    if ENABLE_SUMMARY:
-        if summary := await summarization(cache=cache, cid=str(info["cid"])):
-            if isinstance(summary, bytes):
-                summary = await get_image_v12(bot, state["bili_number"], "summary", data=summary)
-        else:
-            await matcher.send(f"{reply}视频无有效字幕")
-
-    if wc_image or summary:
         await matcher.finish(reply + wc_image + summary)  # type: ignore
```

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/bilibili_request.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/bilibili_request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/column_resolve.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/column_resolve.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-from typing import Tuple
-
 from lxml import etree
 from lxml.etree import _Element, _ElementUnicodeResult
 
 from ..model.exception import AbortError
 from .bilibili_request import hc
 
 XPATH = "//p//text() | //h1/text() | //h2/text() | //h3/text() | //h4/text() | //h5/text() | //h6/text()"
 
 
-async def get_cv(cvid: str) -> Tuple[str, str]:
+async def get_cv(cvid: str):
     cv = await hc.get(f"https://www.bilibili.com/read/cv{cvid}")
     if cv.status_code != 200:
         raise AbortError("专栏获取失败")
     cv.encoding = "utf-8"
     cv = cv.text
 
     http_parser: _Element = etree.fromstring(cv, etree.HTMLParser(encoding="utf-8"))
     title: str = http_parser.xpath('//h1[@class="title"]/text()')[0]
     main_article: _Element = http_parser.xpath('//div[@id="read-article-holder"]')[0]
     plist: _ElementUnicodeResult = main_article.xpath(XPATH)
     text_list = [text.strip() for text in plist if text.strip()]
-    return title, "\n".join(text_list)
+    return title, text_list
```

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/content_resolve.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/content_resolve.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 from grpc.aio import AioRpcError
 from httpx._exceptions import TimeoutException
 from nonebot.log import logger
 
 from ..config import plugin_config
 from ..model.arguments import Options
 from ..model.cache import Cache, Episode
+from ..model.content import Video, Column
+from ..model.exception import AbortError
 from ..optional import capture_exception  # type: ignore
 from .bilibili_request import get_b23_url, grpc_get_view_info
 from .draw_bili_image import binfo_image_create
 from .video_subtitle import get_subtitle
+from .column_resolve import get_cv
+
 
 cd: Dict[str, int] = {}
 cd_size_limit = plugin_config.bilichat_cd_time // 2
 
 
 def check_cd(uid):
     global cd
@@ -81,64 +85,91 @@
         b23_url = await get_b23_url(f"https://www.bilibili.com/video/{bvid}")
         data = (
             (await binfo_image_create(video_info, b23_url))
             if plugin_config.bilichat_basic_info
             else "IMG_RENDER_DISABLED"
         )
         logger.debug(f"Video parsing complete - aid:{aid} cid:{cid} title:{title}")
-        return (b23_url, data, {"aid": aid, "cid": cid, "title": title})
+        return (b23_url, data, Video(aid, cid, title))
     except TimeoutException:
         logger.warning("Video parsing API call timeout")
         return (f"{bili_number} 视频信息生成超时，请稍后再试。", None, None)
     except Exception as e:  # noqa
         capture_exception()
         logger.exception(f"Video parsing API call error: {e}")
         return (f"视频解析 API 调用出错：{e}", None, None)
 
 
-async def get_video_cache(info: Dict, options: Options):
+async def get_column_basic(bili_number: str, uid: Union[str, int]):
+    try:
+        if not check_cd(f"{bili_number}_{uid}"):
+            logger.warning(f"Duplicate column {bili_number}. Skip the video parsing process")
+            return None
+        cvid = bili_number[2:]
+        cv_title, cv_text = await get_cv(cvid)
+        return Column(int(cvid), cv_title, cv_text)
+    except AbortError:
+        logger.warning("Column not found, might deleted by Uploader")
+        return "未找到此专栏，可能已被 UP 主删除。"
+    except TimeoutException:
+        logger.warning("Column parsing API call timeout")
+        return f"{bili_number} 专栏信息生成超时，请稍后再试。"
+    except Exception as e:  # noqa
+        capture_exception()
+        logger.exception(f"Column parsing API call error: {e}")
+        return f"专栏解析 API 调用出错：{e}"
+
+
+async def get_content_cache(info: Union[Video, Column], options: Options):
     async def create_cache():
         return Cache.create(
-            id=f'av{info["aid"]}',
-            title=info["title"],
+            id=f"{id_}",
+            title=info.title,
             episodes={
-                str(info["cid"]): Episode(
+                str(info.cid): Episode(
                     title=None,
-                    content=await get_subtitle(int(info["aid"]), int(info["cid"])),
+                    content=await get_subtitle(int(info.aid), int(info.cid)) if isinstance(info, Video) else info.text,
                     jieba=None,
                     openai=None,
                     newbing=None,
                 )
             },
             temp=options.no_cache,
         )
 
+    if isinstance(info, Video):
+        id_ = f"av{info.aid}"
+    elif isinstance(info, Column):
+        id_ = f"cv{info.aid}"
+    else:
+        raise ValueError(f"unkown type of content {info}")
+
     if options.no_cache:
-        logger.debug(f'parameter --no-cache of av{info["aid"]} detected, using temporary cache')
+        logger.debug(f"parameter --no-cache of {id_} detected, using temporary cache")
         return await create_cache()
 
-    cache = Cache.get(f'av{info["aid"]}')
+    cache = Cache.get(id_)
     # cache file not exists
     if not cache:
-        logger.debug(f'cache of av{info["aid"]} not exists, create cache')
+        logger.debug(f"cache of {id_} not exists, create cache")
         return await create_cache()
     # cache file exists but cid not found
-    elif str(info["cid"]) not in cache.episodes.keys():
-        logger.debug(f'cache of av{info["aid"]} exists, but cid{info["cid"]} not found, appending cache')
-        cache.episodes[str(info["cid"])] = Episode(
+    elif str(info.cid) not in cache.episodes.keys():
+        logger.debug(f"cache of {id_} exists, but cid{info.cid} not found, appending cache")
+        cache.episodes[str(info.cid)] = Episode(
             title=None,
-            content=await get_subtitle(int(info["aid"]), int(info["cid"])),
+            content=await get_subtitle(int(info.aid), int(info.cid)) if isinstance(info, Video) else info.text,
             jieba=None,
             openai=None,
             newbing=None,
         )
     # all exists but need refresh
     elif options.refresh:
-        logger.debug(f'parameter --refresh of av{info["aid"]} detected, remove summary cache')
-        episode = cache.episodes[str(info["cid"])]
+        logger.debug(f"parameter --refresh of {id_} detected, remove summary cache")
+        episode = cache.episodes[str(info.cid)]
         episode.jieba = None
         episode.openai = None
         episode.newbing = None
     # all exists
     else:
-        logger.debug(f'cache of av{info["aid"]} exists, use cache')
+        logger.debug(f"cache of {id_} exists, use cache")
     return cache
```

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/draw_bili_image.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/draw_bili_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/model/cache.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/model/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/static/bing_apology.jpg` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/static/bing_apology.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/__init__.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/newbing_summarise.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/newbing_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/summary/text_to_image.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/summary/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-1.6.0/nonebot_plugin_bilichat/wordcloud/wordcloud.py` & `nonebot_plugin_bilichat-1.7.1/nonebot_plugin_bilichat/wordcloud/wordcloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from jieba.analyse.tfidf import TFIDF
 from nonebot.log import logger
 from wordcloud import WordCloud
 
 from ..lib.fonts_provider import get_font
 from ..model.cache import Cache
 from ..model.exception import AbortError
-from ..optional import capture_exception
+from ..optional import capture_exception  # type: ignore
 
 tfidf = TFIDF()
 
 
 async def wordcloud(cache: Cache, cid: str = "0"):
     try:
         logger.info(f"Generation wordcloud of Video(Column) {cache.id}")
```

### Comparing `nonebot_plugin_bilichat-1.6.0/pyproject.toml` & `nonebot_plugin_bilichat-1.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "py311",
 ]
 include = "\\.pyi?$"
 extend-exclude = ""
 
 [project]
 name = "nonebot-plugin-bilichat"
-version = "1.6.0"
+version = "1.7.1"
 description = "一个通过 OpenAI 来对b站视频进行总结插件"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "httpx>=0.23.3",
```

### Comparing `nonebot_plugin_bilichat-1.6.0/PKG-INFO` & `nonebot_plugin_bilichat-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 1.6.0
+Version: 1.7.1
 Summary: 一个通过 OpenAI 来对b站视频进行总结插件
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: httpx>=0.23.3
 Requires-Dist: bilireq>=0.2.4
 Requires-Dist: qrcode>=7.4.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.6.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 1.7.1 Summary:
 ä¸ä¸ªéè¿ OpenAI æ¥å¯¹bç«è§é¢è¿è¡æ»ç»æä»¶ Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 httpx>=0.23.3 Requires-Dist: bilireq>=0.2.4 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-
 plugin-localstore>=0.4.1 Requires-Dist: nonebot-adapter-onebot>=2.2.2 Requires-
 Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra" Requires-Dist:
```

