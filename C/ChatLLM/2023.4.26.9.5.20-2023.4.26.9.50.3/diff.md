# Comparing `tmp/ChatLLM-2023.4.26.9.5.20.tar.gz` & `tmp/ChatLLM-2023.4.26.9.50.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.26.9.5.20.tar", last modified: Wed Apr 26 01:05:20 2023, max compression
+gzip compressed data, was "ChatLLM-2023.4.26.9.50.3.tar", last modified: Wed Apr 26 01:50:03 2023, max compression
```

## Comparing `ChatLLM-2023.4.26.9.5.20.tar` & `ChatLLM-2023.4.26.9.50.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.410218 ChatLLM-2023.4.26.9.5.20/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.26.9.5.20/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.379128 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     2127 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1604 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-26 01:05:20.000000 ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     2127 2023-04-26 01:05:20.410047 ChatLLM-2023.4.26.9.5.20/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1312 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.5.20/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/README.rst
--rw-r--r--   0 betterme   (501) staff       (20)       97 2023-04-25 11:54:57.000000 ChatLLM-2023.4.26.9.5.20/TODO.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.379570 ChatLLM-2023.4.26.9.5.20/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.381792 ChatLLM-2023.4.26.9.5.20/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     2851 2023-04-26 01:04:59.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      542 2023-04-25 08:23:38.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.26.9.5.20/chatllm/applications/pipeline.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.382336 ChatLLM-2023.4.26.9.5.20/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      571 2023-04-25 02:29:53.000000 ChatLLM-2023.4.26.9.5.20/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1429 2023-04-25 08:29:49.000000 ChatLLM-2023.4.26.9.5.20/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.383284 ChatLLM-2023.4.26.9.5.20/chatllm/his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.26.9.5.20/chatllm/his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.5.20/chatllm/his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.5.20/chatllm/his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.5.20/chatllm/his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.383799 ChatLLM-2023.4.26.9.5.20/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.26.9.5.20/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.26.9.5.20/chatllm/parse_utils/doc_parse.py
--rw-r--r--   0 betterme   (501) staff       (20)     3326 2023-04-26 00:57:53.000000 ChatLLM-2023.4.26.9.5.20/chatllm/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.385172 ChatLLM-2023.4.26.9.5.20/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1446 2023-04-25 10:54:31.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      221 2023-04-25 11:01:07.000000 ChatLLM-2023.4.26.9.5.20/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.389086 ChatLLM-2023.4.26.9.5.20/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.392853 ChatLLM-2023.4.26.9.5.20/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.26.9.5.20/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.26.9.5.20/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.5.20/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.5.20/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.5.20/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.26.9.5.20/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.5.20/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.409388 ChatLLM-2023.4.26.9.5.20/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     1342 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.5.20/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.26.9.5.20/docs/img.png
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatLLM-2023.4.26.9.5.20/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatLLM-2023.4.26.9.5.20/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.26.9.5.20/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-26 01:05:20.410279 ChatLLM-2023.4.26.9.5.20/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-04-25 02:27:49.000000 ChatLLM-2023.4.26.9.5.20/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:05:20.409721 ChatLLM-2023.4.26.9.5.20/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.5.20/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726815 ChatLLM-2023.4.26.9.50.3/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.26.9.50.3/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.696066 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     1789 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1604 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       49 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)       43 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-26 01:50:03.000000 ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1789 2023-04-26 01:50:03.726660 ChatLLM-2023.4.26.9.50.3/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      974 2023-04-26 01:32:56.000000 ChatLLM-2023.4.26.9.50.3/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      844 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/README.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       97 2023-04-25 11:54:57.000000 ChatLLM-2023.4.26.9.50.3/TODO.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.696487 ChatLLM-2023.4.26.9.50.3/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.698805 ChatLLM-2023.4.26.9.50.3/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      775 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3307 2023-04-26 01:49:42.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      542 2023-04-25 08:23:38.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.26.9.50.3/chatllm/applications/pipeline.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.699767 ChatLLM-2023.4.26.9.50.3/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      571 2023-04-25 02:29:53.000000 ChatLLM-2023.4.26.9.50.3/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1429 2023-04-25 08:29:49.000000 ChatLLM-2023.4.26.9.50.3/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.701014 ChatLLM-2023.4.26.9.50.3/chatllm/his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      285 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2492 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/chatllm/his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.701713 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.26.9.50.3/chatllm/parse_utils/doc_parse.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3326 2023-04-26 00:57:53.000000 ChatLLM-2023.4.26.9.50.3/chatllm/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.703247 ChatLLM-2023.4.26.9.50.3/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1446 2023-04-25 10:54:31.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      221 2023-04-25 11:01:07.000000 ChatLLM-2023.4.26.9.50.3/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.706999 ChatLLM-2023.4.26.9.50.3/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.710586 ChatLLM-2023.4.26.9.50.3/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.26.9.50.3/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.26.9.50.3/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.26.9.50.3/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.26.9.50.3/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726076 ChatLLM-2023.4.26.9.50.3/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     1342 2023-04-25 08:31:06.000000 ChatLLM-2023.4.26.9.50.3/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)   257150 2023-04-20 11:45:08.000000 ChatLLM-2023.4.26.9.50.3/docs/img.png
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1122 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      237 2023-04-20 11:28:30.000000 ChatLLM-2023.4.26.9.50.3/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       55 2023-04-21 04:00:06.000000 ChatLLM-2023.4.26.9.50.3/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-25 02:57:55.000000 ChatLLM-2023.4.26.9.50.3/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-26 01:50:03.726864 ChatLLM-2023.4.26.9.50.3/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1554 2023-04-25 02:27:49.000000 ChatLLM-2023.4.26.9.50.3/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-26 01:50:03.726406 ChatLLM-2023.4.26.9.50.3/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.26.9.50.3/tox.ini
```

### Comparing `ChatLLM-2023.4.26.9.5.20/.gitignore` & `ChatLLM-2023.4.26.9.50.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/.travis.yml` & `ChatLLM-2023.4.26.9.50.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/CONTRIBUTING.rst` & `ChatLLM-2023.4.26.9.50.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.4.26.9.50.3/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/LICENSE` & `ChatLLM-2023.4.26.9.50.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/Makefile` & `ChatLLM-2023.4.26.9.50.3/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/README.md` & `ChatLLM-2023.4.26.9.50.3/docs/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 ![image](https://img.shields.io/pypi/v/llm4gpt.svg) ![image](https://img.shields.io/travis/yuanjie-ai/llm4gpt.svg) ![image](https://readthedocs.org/projects/llm4gpt/badge/?version=latest)
 
 
 
-<h1 align = "center">🔥ChatLLM🔥</h1>
+<h1 align = "center">🔥LLM4GPT 为大模型而生🔥</h1>
 
 ---
 
 # Install
 
 ```python
 pip install -U llm4gpt
 ```
 
-# [Docs](https://jie-yuan.github.io/llm4gpt/)
+# [Docs](https://yuanjie-ai.github.io/LLM4GPT/)
 
 # Usages
 
 ```python
 from chatllm.his._qa import QA
-from chatllm.his import FaissANN
-from chatllm.his._chatllm import ChatLLM
 from chatllm.utils import llm_load
+from chatllm.his._chatllm import ChatLLM
+from chatllm.his.FaissANN import FaissANN
 
 from meutils.pipe import *
 
 # 解析知识库
 texts = []
 metadatas = []
 for p in Path('data').glob('*.txt'):
```

### Comparing `ChatLLM-2023.4.26.9.5.20/README.rst` & `ChatLLM-2023.4.26.9.50.3/README.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatann.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatbase.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatbase.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 # @WeChat       : meutils
 # @Software     : PyCharm
 # @Description  :
 import types
 from meutils.pipe import *
 from meutils.decorators import clear_cuda_cache
 
+from chatllm.utils import DEVICE, load_llm4chat
+
 
 class ChatBase(object):
 
-    def __init__(self, chat_func, prompt_template=None):
+    def __init__(self, chat_func=None, prompt_template=None, role='你扮演的角色是ChatLLM项目助理，由Betterme开发'):
         self.chat_func = chat_func
         self.prompt_template = prompt_template if prompt_template else self.default_document_prompt
+        self.role = role
 
         #
         self.history = []
         self.knowledge_base = None
 
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
@@ -29,19 +32,19 @@
         """可重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
     def set_chat_kwargs(self, **kwargs):
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
-    def _qa(self, query, knowledge_base='', max_turns=1):
+    def _qa(self, query, knowledge_base='请自由回答', max_turns=1):
 
         if knowledge_base:
             self.knowledge_base = knowledge_base
-            query = self.prompt_template.format(context=knowledge_base, question=query)
+            query = self.prompt_template.format(context=knowledge_base, question=query, role=self.role)
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
 
         if isinstance(result, types.GeneratorType):
             return self._stream(result)
         else:  # list(self._stream(result)) 想办法合并
@@ -55,30 +58,34 @@
         bar = tqdm(result, ascii=True)  # ncols
         for response, history in bar:
             bar.set_description(response)
             yield response, history
         # self.history_ = history  # 历史所有
         self.history += [[None, response]]  # 置空知识
 
+    def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
+        assert not self.chat_func, "overwrite chat_func"
+        self.chat_func = load_llm4chat(model_name_or_path, device, stream, **kwargs)
+
     @property
     def default_document_prompt(self):
         prompt_template = """
-            基于以下已知信息，简洁和专业的来回答问题。
-            如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的相关信息"，不允许在答案中添加编造成分，答案请使用中文。
+            {role} 基于以下已知信息，简洁和专业的来回答问题。
+            如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的信息"，不允许在答案中添加编造成分，答案请使用中文。
             已知信息: {context}
             问题: {question}
             """.strip()
 
         return prompt_template
 
 
 if __name__ == '__main__':
-    from chatllm.utils import load_llm4chat
+    from chatllm.applications import ChatBase
 
-    chat_func = load_llm4chat(
-        model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
-    )
-
-    qa = ChatBase(chat_func=chat_func)
+    qa = ChatBase()
+    qa.load_llm4chat(model_name_or_path="/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm")
 
     for i, _ in qa(query='周杰伦是谁', knowledge_base='周杰伦是傻子'):
-        print(_, flush=True)
+        pass
+
+    for i, _ in qa(query='你是谁', knowledge_base='自由回答'):
+        pass
```

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/applications/chatpdf.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/clis/cli.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/embedding.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/his/FaissANN.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/his/_chatllm.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/his/_qa.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/utils.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/webui/chatbase.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/webui/chatpdf.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/chatllm/webui/nice_ui.py` & `ChatLLM-2023.4.26.9.50.3/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/医/500种中药现代研究.txt` & `ChatLLM-2023.4.26.9.50.3/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/医/古今医统大全.txt` & `ChatLLM-2023.4.26.9.50.3/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/姚明.txt` & `ChatLLM-2023.4.26.9.50.3/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/王治郅.txt` & `ChatLLM-2023.4.26.9.50.3/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/科比.txt` & `ChatLLM-2023.4.26.9.50.3/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/data/财报.pdf` & `ChatLLM-2023.4.26.9.50.3/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/docs/Makefile` & `ChatLLM-2023.4.26.9.50.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/docs/conf.py` & `ChatLLM-2023.4.26.9.50.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/docs/img.png` & `ChatLLM-2023.4.26.9.50.3/docs/img.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/docs/installation.rst` & `ChatLLM-2023.4.26.9.50.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/docs/make.bat` & `ChatLLM-2023.4.26.9.50.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/setup.py` & `ChatLLM-2023.4.26.9.50.3/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.26.9.5.20/tests/test_llm4gpt.py` & `ChatLLM-2023.4.26.9.50.3/tests/test_llm4gpt.py`

 * *Files identical despite different names*

