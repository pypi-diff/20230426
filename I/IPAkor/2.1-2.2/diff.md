# Comparing `tmp/IPAkor-2.1.tar.gz` & `tmp/IPAkor-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPAkor-2.1.tar", last modified: Wed Apr 26 04:08:37 2023, max compression
+gzip compressed data, was "IPAkor-2.2.tar", last modified: Wed Apr 26 04:37:41 2023, max compression
```

## Comparing `IPAkor-2.1.tar` & `IPAkor-2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:08:37.733771 IPAkor-2.1/
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:08:37.730339 IPAkor-2.1/IPAkor/
--rw-r--r--   0 eneminova   (501) staff       (20)       63 2023-04-25 19:57:07.000000 IPAkor-2.1/IPAkor/__init__.py
--rw-r--r--   0 eneminova   (501) staff       (20)     3912 2023-04-25 19:32:13.000000 IPAkor-2.1/IPAkor/border_maker.py
--rw-r--r--   0 eneminova   (501) staff       (20)     8605 2023-04-26 04:07:45.000000 IPAkor-2.1/IPAkor/rules.py
-drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:08:37.733428 IPAkor-2.1/IPAkor.egg-info/
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:08:37.000000 IPAkor-2.1/IPAkor.egg-info/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)      235 2023-04-26 04:08:37.000000 IPAkor-2.1/IPAkor.egg-info/SOURCES.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-26 04:08:37.000000 IPAkor-2.1/IPAkor.egg-info/dependency_links.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-26 04:08:37.000000 IPAkor-2.1/IPAkor.egg-info/requires.txt
--rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-26 04:08:37.000000 IPAkor-2.1/IPAkor.egg-info/top_level.txt
--rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:08:37.733957 IPAkor-2.1/PKG-INFO
--rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.1/README.md
--rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-26 04:08:37.734692 IPAkor-2.1/setup.cfg
--rw-r--r--   0 eneminova   (501) staff       (20)      564 2023-04-26 04:08:19.000000 IPAkor-2.1/setup.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.156512 IPAkor-2.2/
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.153366 IPAkor-2.2/IPAkor/
+-rw-r--r--   0 eneminova   (501) staff       (20)       63 2023-04-25 19:57:07.000000 IPAkor-2.2/IPAkor/__init__.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     4065 2023-04-26 04:36:37.000000 IPAkor-2.2/IPAkor/border_maker.py
+-rw-r--r--   0 eneminova   (501) staff       (20)     8605 2023-04-26 04:36:37.000000 IPAkor-2.2/IPAkor/rules.py
+drwxr-xr-x   0 eneminova   (501) staff       (20)        0 2023-04-26 04:37:41.156221 IPAkor-2.2/IPAkor.egg-info/
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)      235 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/SOURCES.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        1 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/dependency_links.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)       12 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/requires.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)        7 2023-04-26 04:37:41.000000 IPAkor-2.2/IPAkor.egg-info/top_level.txt
+-rw-r--r--   0 eneminova   (501) staff       (20)      244 2023-04-26 04:37:41.156638 IPAkor-2.2/PKG-INFO
+-rw-r--r--   0 eneminova   (501) staff       (20)     1422 2023-04-25 19:58:38.000000 IPAkor-2.2/README.md
+-rw-r--r--   0 eneminova   (501) staff       (20)       38 2023-04-26 04:37:41.157646 IPAkor-2.2/setup.cfg
+-rw-r--r--   0 eneminova   (501) staff       (20)      572 2023-04-26 04:36:37.000000 IPAkor-2.2/setup.py
```

### Comparing `IPAkor-2.1/IPAkor/border_maker.py` & `IPAkor-2.2/IPAkor/border_maker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # ЭТОТ КОД ДЕЛАЕТ РАЗНЫЕ ВИДЫ ГРАНИЦ МЕЖДУ СЛОГАМИ, КЛИТИКАМИ,
 # СЛОВАМИ И СИНТАГМАМИ
 # подробнее: https://colab.research.google.com/drive/1F6rf_Difpv1sYtp2X1PNsvUi3ARu0b07#scrollTo=KE5t4CsRGmzl
 from konlpy.tag import Twitter
 from konlpy.tag import Kkma
 import csv
 import re
+import wget
+
 
 class BorderMaker():
 
     def __init__(self):
         self.twitter = Twitter()
-        #hello world
+        self.kkma = Kkma()
 
         self.final_trans = dict()
-        with open('final_trans.csv', 'r', encoding='utf-8') as ft_file:
-          spamreader = csv.reader(ft_file)
-          for row in spamreader:
-              self.final_trans[row[0]] = row[2]
+        self.filename = wget.download(
+            'https://raw.githubusercontent.com/Ne-minus/kor_to_phonemes/main/IPAkor/final_trans.csv')
+        with open(self.filename, encoding='utf-8') as ft_file:
+            spamreader = csv.reader(ft_file)
 
+            for row in spamreader:
+                self.final_trans[row[0]] = row[2]
 
     def intruser(self, word: str) -> str:
         ready_word = ''
         for char in word:
             ready_word += '-' + self.final_trans[char]
         return ready_word.strip('-')
 
     def separator(self, text: str) -> str:
         syll_dict = dict()
 
-        with open('final_trans.csv') as csvfile:
+        with open(self.filename) as csvfile:
             spamreader = csv.reader(csvfile)
             sylls = list(spamreader)
             for s in sylls:
                 syll_dict[s[0]] = s[2]
 
         good_text = ' '
         twit_morph = self.twitter.pos(text, norm=True)
```

### Comparing `IPAkor-2.1/IPAkor/rules.py` & `IPAkor-2.2/IPAkor/rules.py`

 * *Files identical despite different names*

### Comparing `IPAkor-2.1/README.md` & `IPAkor-2.2/README.md`

 * *Files identical despite different names*

### Comparing `IPAkor-2.1/setup.py` & `IPAkor-2.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 setuptools.setup(name='IPAkor',
-                 version='2.1',
+                 version='2.2',
                  packages=setuptools.find_packages(),
                  include_package_data=True,
                  classifiers=[
                      'Programming Language :: Python :: 3',
                      'Operating System :: OS Independent',
                      'Topic :: Scientific/Engineering'
                  ],
-                 install_requires=['konlpy'],
+                 install_requires=['konlpy', 'wget'],
                  python_requires='>=3',
                  author_email='neminova2.0@gmail.com'
                  )
```

