# Comparing `tmp/hyt-gpt-0.2.5.tar.gz` & `tmp/hyt-gpt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyt-gpt-0.2.5.tar", last modified: Mon Apr 10 05:25:44 2023, max compression
+gzip compressed data, was "hyt-gpt-0.2.6.tar", last modified: Tue Apr 25 15:41:43 2023, max compression
```

## Comparing `hyt-gpt-0.2.5.tar` & `hyt-gpt-0.2.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/PKG-INFO
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/hyt_gpt/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.5/hyt_gpt/__init__.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-04-10 05:20:52.000000 hyt-gpt-0.2.5/hyt_gpt/gpt.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.5/hyt_gpt/notion.py
--rw-rw-r--   0 haibin    (1000) haibin    (1000)     6366 2023-04-10 05:21:38.000000 hyt-gpt-0.2.5/hyt_gpt/youtube.py
-drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/hyt_gpt.egg-info/
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/PKG-INFO
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/SOURCES.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/dependency_links.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-10 05:25:44.000000 hyt-gpt-0.2.5/hyt_gpt.egg-info/top_level.txt
--rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-10 05:25:44.227964 hyt-gpt-0.2.5/setup.cfg
--rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-10 05:25:41.000000 hyt-gpt-0.2.5/setup.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/PKG-INFO
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/hyt_gpt/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        0 2023-03-26 03:01:59.000000 hyt-gpt-0.2.6/hyt_gpt/__init__.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     4000 2023-04-12 04:46:33.000000 hyt-gpt-0.2.6/hyt_gpt/gpt.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     2886 2023-03-26 03:01:59.000000 hyt-gpt-0.2.6/hyt_gpt/notion.py
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)     6408 2023-04-25 06:23:34.000000 hyt-gpt-0.2.6/hyt_gpt/youtube.py
+drwxrwxr-x   0 haibin    (1000) haibin    (1000)        0 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/hyt_gpt.egg-info/
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      702 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/PKG-INFO
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      204 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/SOURCES.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        1 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/dependency_links.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)        8 2023-04-25 15:41:43.000000 hyt-gpt-0.2.6/hyt_gpt.egg-info/top_level.txt
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)       38 2023-04-25 15:41:43.174047 hyt-gpt-0.2.6/setup.cfg
+-rw-rw-r--   0 haibin    (1000) haibin    (1000)      837 2023-04-25 15:39:58.000000 hyt-gpt-0.2.6/setup.py
```

### Comparing `hyt-gpt-0.2.5/PKG-INFO` & `hyt-gpt-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.5/hyt_gpt/gpt.py` & `hyt-gpt-0.2.6/hyt_gpt/gpt.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.5/hyt_gpt/notion.py` & `hyt-gpt-0.2.6/hyt_gpt/notion.py`

 * *Files identical despite different names*

### Comparing `hyt-gpt-0.2.5/hyt_gpt/youtube.py` & `hyt-gpt-0.2.6/hyt_gpt/youtube.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,15 +147,15 @@
                     if subtitle.get('ext') == 'vtt':
                         text = self.__get_text_from_url(subtitle.get('url'))
                         subtitles.extend(self.__parse_subtitles(text))
         
         if 'requested_subtitles' in result:
             print('Found requested subtitles.')
             requested_subtitles = result.get('requested_subtitles')
-            if 'en' in requested_subtitles:
+            if isinstance(requested_subtitles, dict) and 'en' in requested_subtitles:
                 subtitle = requested_subtitles['en']
                 if subtitle.get('ext') == 'vtt':
                     print('No subtitles found, fetching requested subtitles.')
                     text = self.__get_text_from_url(subtitle.get('url'))
                     subtitles.extend(self.__parse_requested_subtitles(text))
         print(f'Fetched {len(subtitles)} subtitles.')
         return subtitles
```

### Comparing `hyt-gpt-0.2.5/hyt_gpt.egg-info/PKG-INFO` & `hyt-gpt-0.2.6/hyt_gpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyt-gpt
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library for GPT and Youtube
 Author: Harbin
 Author-email: harbinfate@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hyt-gpt-0.2.5/setup.py` & `hyt-gpt-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name='hyt-gpt',
-    version='0.2.5',
+    version='0.2.6',
     description='A library for GPT and Youtube',
     author='Harbin',
     author_email='harbinfate@gmail.com',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

