# Comparing `tmp/chatgpt-tool-hub-0.4.2.tar.gz` & `tmp/chatgpt-tool-hub-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-tool-hub-0.4.2.tar", last modified: Tue Apr 25 16:32:19 2023, max compression
+gzip compressed data, was "chatgpt-tool-hub-0.4.3.tar", last modified: Tue Apr 25 17:39:22 2023, max compression
```

## Comparing `chatgpt-tool-hub-0.4.2.tar` & `chatgpt-tool-hub-0.4.3.tar`

### file list

```diff
@@ -1,157 +1,157 @@
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.300943 chatgpt-tool-hub-0.4.2/
--rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.2/LICENSE
--rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 16:32:19.300611 chatgpt-tool-hub-0.4.2/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)    13295 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/README.md
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.283072 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.284496 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/
--rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2517 2023-04-25 14:38:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2661 2023-04-25 16:04:49.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/app_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/lite_app.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 16:03:00.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/victorinox.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.284726 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/
--rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/all_bot_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.285076 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    11283 2023-04-25 16:07:11.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-25 13:40:57.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.285397 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4981 2023-04-24 14:53:16.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.285927 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/
--rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.286407 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/
--rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 16:07:11.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-24 14:28:40.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/llm.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.288355 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/cache.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/calculate_token.py
--rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/callbacks.py
--rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/config.py
--rw-r--r--   0 goldfish   (502) staff       (20)      168 2023-04-16 00:10:23.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/constants.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/document.py
--rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/formatting.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/input.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/json_utils.py
--rw-r--r--   0 goldfish   (502) staff       (20)      640 2023-04-25 16:28:12.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/log.py
--rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/schema.py
--rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/singleton.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/text_splitter.py
--rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.288907 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/
--rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 13:49:31.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/chat_memory.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/token_buffer.py
--rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/utils.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.289460 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/
--rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12841 2023-04-25 15:51:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/bot.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/initialize.py
--rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-25 16:07:11.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/tool_engine.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.290018 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/
--rw-r--r--   0 goldfish   (502) staff       (20)     2142 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/base.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.290592 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/
--rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15107 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/chatgpt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/model_factory.py
--rw-r--r--   0 goldfish   (502) staff       (20)    28103 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/openai.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.291287 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/
--rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-24 14:28:40.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/chat.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/prompt.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.292067 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/
--rw-r--r--   0 goldfish   (502) staff       (20)     1396 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/all_tool_list.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.292529 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/
--rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 14:48:46.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2892 2023-04-25 15:51:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 14:38:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/base_tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.292932 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.293274 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/load_tools.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.293614 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/
--rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5158 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1922 2023-04-25 16:10:37.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.293841 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/
--rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/__init__.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.294132 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/finance_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/finance_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/finance_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.295006 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/
--rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3205 2023-04-25 14:19:06.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.295349 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/
--rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 15:20:23.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 16:10:37.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2277 2023-04-25 15:02:33.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.295575 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/python/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/python/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/python/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.295947 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/
--rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.296399 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/
--rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/map_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/reduce_prompt.py
--rw-r--r--   0 goldfish   (502) staff       (20)     7354 2023-04-25 16:07:11.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/tool.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.296768 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/
--rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/answer_user.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/debug.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.296997 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/terminal/
--rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/terminal/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/terminal/base.py
--rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/tool.py
--rw-r--r--   0 goldfish   (502) staff       (20)      784 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/tool_register.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.297334 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/visual_dl/
--rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/visual_dl/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2349 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/visual_dl/text2image.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.298694 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/
--rw-r--r--   0 goldfish   (502) staff       (20)     2365 2023-04-25 15:51:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-04-25 14:05:22.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/browser.py
--rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/delete.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 14:00:32.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/get.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/patch.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/post.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/put.py
--rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-24 14:17:41.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.299624 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/
--rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 13:23:32.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
--rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 14:00:32.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/wrapper.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.300296 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/
--rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 15:29:22.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
--rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
--rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-25 16:31:02.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/version.py
-drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 16:32:19.283862 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/
--rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 16:32:19.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/PKG-INFO
--rw-r--r--   0 goldfish   (502) staff       (20)     4862 2023-04-25 16:32:19.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/SOURCES.txt
--rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-25 16:32:19.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/dependency_links.txt
--rw-r--r--   0 goldfish   (502) staff       (20)      245 2023-04-25 16:32:19.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/requires.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-25 16:32:19.000000 chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/top_level.txt
--rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-25 16:32:19.300993 chatgpt-tool-hub-0.4.2/setup.cfg
--rw-r--r--   0 goldfish   (502) staff       (20)     1962 2023-04-24 15:05:59.000000 chatgpt-tool-hub-0.4.2/setup.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.793435 chatgpt-tool-hub-0.4.3/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1068 2023-03-27 01:02:03.000000 chatgpt-tool-hub-0.4.3/LICENSE
+-rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 17:39:22.793220 chatgpt-tool-hub-0.4.3/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)    13295 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/README.md
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.770038 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772043 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/
+-rw-r--r--   0 goldfish   (502) staff       (20)       99 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2517 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2661 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1921 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/lite_app.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5190 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/victorinox.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772419 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/
+-rw-r--r--   0 goldfish   (502) staff       (20)      150 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      210 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/all_bot_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.772875 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    11283 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1935 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.773255 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4981 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.773961 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/
+-rw-r--r--   0 goldfish   (502) staff       (20)      155 2023-04-08 18:26:04.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.774633 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/
+-rw-r--r--   0 goldfish   (502) staff       (20)      138 2023-04-08 18:27:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4749 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1273 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    10572 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7498 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/llm.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.777465 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-03-26 14:32:25.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5081 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/cache.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2079 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/calculate_token.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    24793 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/callbacks.py
+-rw-r--r--   0 goldfish   (502) staff       (20)        0 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/config.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      168 2023-04-16 00:10:23.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/constants.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1256 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/document.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      968 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/formatting.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1020 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/input.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5776 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/json_utils.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      640 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/log.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     8577 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/schema.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      630 2023-03-27 14:21:20.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/singleton.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6621 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/text_splitter.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      882 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.778330 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/
+-rw-r--r--   0 goldfish   (502) staff       (20)      133 2023-03-27 18:19:31.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1696 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/chat_memory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2388 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/token_buffer.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      526 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/utils.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.779193 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/
+-rw-r--r--   0 goldfish   (502) staff       (20)      103 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12841 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/bot.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2071 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/initialize.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    13050 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/tool_engine.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.780048 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2142 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    12913 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/base.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.781690 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/
+-rw-r--r--   0 goldfish   (502) staff       (20)       89 2023-03-27 18:19:49.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5393 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15107 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/chatgpt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      521 2023-04-08 08:53:56.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/model_factory.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    28103 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/openai.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.782602 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/
+-rw-r--r--   0 goldfish   (502) staff       (20)      751 2023-03-27 18:21:02.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6359 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     6316 2023-03-27 18:25:43.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/chat.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4323 2023-03-30 16:33:18.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/prompt.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.783656 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/
+-rw-r--r--   0 goldfish   (502) staff       (20)     1396 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      321 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/all_tool_list.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.784246 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)       63 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1700 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2892 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3219 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4140 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/base_tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.784869 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      140 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1476 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3427 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.785412 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      165 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2290 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3552 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2608 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/load_tools.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786033 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/
+-rw-r--r--   0 goldfish   (502) staff       (20)       62 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5158 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1922 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786306 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/
+-rw-r--r--   0 goldfish   (502) staff       (20)      883 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/__init__.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.786692 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1349 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.787391 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/
+-rw-r--r--   0 goldfish   (502) staff       (20)       74 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      639 2023-04-11 16:17:29.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3205 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.787800 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/
+-rw-r--r--   0 goldfish   (502) staff       (20)       66 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2709 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1826 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2277 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.788053 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2375 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.788542 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/
+-rw-r--r--   0 goldfish   (502) staff       (20)      169 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2323 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)    15639 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.789124 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/
+-rw-r--r--   0 goldfish   (502) staff       (20)      196 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      665 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/map_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      464 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/reduce_prompt.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     7354 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/tool.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.789710 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/
+-rw-r--r--   0 goldfish   (502) staff       (20)      127 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1046 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/answer_user.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1329 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/debug.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.790078 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/
+-rw-r--r--   0 goldfish   (502) staff       (20)       61 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4412 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/base.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     3667 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      784 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool_register.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.790488 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/
+-rw-r--r--   0 goldfish   (502) staff       (20)       73 2023-04-09 04:05:39.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2349 2023-04-22 18:14:42.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/text2image.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.791941 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/
+-rw-r--r--   0 goldfish   (502) staff       (20)     2365 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     5094 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/browser.py
+-rw-r--r--   0 goldfish   (502) staff       (20)      753 2023-04-18 18:03:30.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/delete.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2117 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/get.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1231 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/patch.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2054 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/post.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1215 2023-03-27 18:20:27.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/put.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     4629 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.792497 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/
+-rw-r--r--   0 goldfish   (502) staff       (20)      142 2023-04-04 16:47:52.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1372 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wikipedia.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     2494 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wrapper.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.792993 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/
+-rw-r--r--   0 goldfish   (502) staff       (20)      166 2023-04-08 17:59:17.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/__init__.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1511 2023-04-25 17:37:12.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py
+-rw-r--r--   0 goldfish   (502) staff       (20)     1896 2023-04-23 17:58:59.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py
+-rw-r--r--   0 goldfish   (502) staff       (20)       22 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/version.py
+drwxr-xr-x   0 goldfish   (502) staff       (20)        0 2023-04-25 17:39:22.770817 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/
+-rw-r--r--   0 goldfish   (502) staff       (20)    14090 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/PKG-INFO
+-rw-r--r--   0 goldfish   (502) staff       (20)     4862 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)        1 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)      250 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/requires.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       17 2023-04-25 17:39:22.000000 chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/top_level.txt
+-rw-r--r--   0 goldfish   (502) staff       (20)       38 2023-04-25 17:39:22.793477 chatgpt-tool-hub-0.4.3/setup.cfg
+-rw-r--r--   0 goldfish   (502) staff       (20)     1977 2023-04-25 17:38:17.000000 chatgpt-tool-hub-0.4.3/setup.py
```

### Comparing `chatgpt-tool-hub-0.4.2/LICENSE` & `chatgpt-tool-hub-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/PKG-INFO` & `chatgpt-tool-hub-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.2
+Version: 0.4.3
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.2/README.md` & `chatgpt-tool-hub-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/app.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/app_factory.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/app_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/lite_app.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/lite_app.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/apps/victorinox.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/apps/victorinox.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/chat_bot/prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/chat_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/bots/qa_bot/prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/bots/qa_bot/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/api/prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/api/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/chains/llm.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/chains/llm.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/cache.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/cache.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/calculate_token.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/calculate_token.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/callbacks.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/callbacks.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/document.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/document.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/formatting.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/formatting.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/input.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/input.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/json_utils.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/json_utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/log.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/log.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/schema.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/schema.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/singleton.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/singleton.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/text_splitter.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/text_splitter.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/common/utils.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/common/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/chat_memory.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/chat_memory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/token_buffer.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/token_buffer.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/database/utils.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/database/utils.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/bot.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/bot.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/initialize.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/initialize.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/engine/tool_engine.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/engine/tool_engine.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/__init__.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/chatgpt/chatgpt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/chatgpt/chatgpt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/model_factory.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/models/openai.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/models/openai.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/__init__.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/chat.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/chat.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/prompts/prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/__init__.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/api_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/arxiv_search/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/arxiv_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/base_tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/bing_search/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/bing_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/google_search/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/google_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/load_tools.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/load_tools.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/docs_prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/meteo/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/meteo/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/__init__.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/finance_news/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/finance_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/morning_news/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/morning_news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/docs_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/news_api/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/news_api/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/news/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/news/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/python/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/python/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/searxng_search/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/searxng_search/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/map_prompt.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/map_prompt.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/summary/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/summary/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/answer_user.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/answer_user.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/system/debug.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/system/debug.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/terminal/base.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/terminal/base.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/tool.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/tool_register.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/tool_register.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/visual_dl/text2image.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/visual_dl/text2image.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/__init__.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/browser.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/browser.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/delete.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/delete.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/get.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/get.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/patch.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/patch.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/post.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/post.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/put.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/put.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/web_requests/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/web_requests/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/wikipedia.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wikipedia/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wikipedia/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub/tools/wolfram_alpha/wrapper.py`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/PKG-INFO` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-tool-hub
-Version: 0.4.2
+Version: 0.4.3
 Summary: An open-source chatgpt tool ecosystem where you can combine tools with chatgpt and use natural language to do anything.
 Home-page: https://github.com/goldfishh/chatgpt-tool-hub
 Author: goldfishh
 Author-email: goldfish.buaa@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `chatgpt-tool-hub-0.4.2/chatgpt_tool_hub.egg-info/SOURCES.txt` & `chatgpt-tool-hub-0.4.3/chatgpt_tool_hub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chatgpt-tool-hub-0.4.2/setup.py` & `chatgpt-tool-hub-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
         "wolframalpha",
         'aiohttp~=3.8.4',
         'requests~=2.28.2',
         "google-api-python-client",
         "SQLAlchemy~=2.0.7",
         "selenium",
         "webdriver_manager",
+        "rich"
     ],
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

