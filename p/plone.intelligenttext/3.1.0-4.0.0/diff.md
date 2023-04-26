# Comparing `tmp/plone.intelligenttext-3.1.0.tar.gz` & `tmp/plone.intelligenttext-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/plone.intelligenttext-3.1.0.tar", last modified: Mon Apr 20 20:40:12 2020, max compression
+gzip compressed data, was "plone.intelligenttext-4.0.0.tar", last modified: Wed Apr 26 21:51:10 2023, max compression
```

## Comparing `plone.intelligenttext-3.1.0.tar` & `plone.intelligenttext-4.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/
--rw-r--r--   0 maurits    (501) staff       (20)     7329 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/PKG-INFO
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     7329 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)      593 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)       11 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       70 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      397 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      149 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/MANIFEST.in
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      683 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/docs/LICENSE.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1912 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/setup.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       80 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/intelligenttext/
--rw-r--r--   0 maurits    (501) staff       (20)     7249 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/intelligenttext/transforms.py
--rw-r--r--   0 maurits    (501) staff       (20)       24 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/intelligenttext/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)    13726 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/intelligenttext/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      442 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/plone/intelligenttext/tests.py
--rw-r--r--   0 maurits    (501) staff       (20)      153 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      406 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3723 2020-04-20 20:40:12.000000 plone.intelligenttext-3.1.0/CHANGES.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:10.359843 plone.intelligenttext-4.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     3898 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     5427 2023-04-26 21:51:10.359968 plone.intelligenttext-4.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      406 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:10.355139 plone.intelligenttext-4.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      683 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:10.355394 plone.intelligenttext-4.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:10.359540 plone.intelligenttext-4.0.0/plone/intelligenttext/
+-rw-r--r--   0 maurits    (501) staff       (20)    13726 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/plone/intelligenttext/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/plone/intelligenttext/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      405 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/plone/intelligenttext/tests.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6910 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/plone/intelligenttext/transforms.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:51:10.357797 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     5427 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      593 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       11 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:51:10.000000 plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2864 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 21:51:10.360434 plone.intelligenttext-4.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1574 2023-04-26 21:51:09.000000 plone.intelligenttext-4.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `plone.intelligenttext-3.1.0/plone.intelligenttext.egg-info/SOURCES.txt` & `plone.intelligenttext-4.0.0/plone.intelligenttext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.intelligenttext-3.1.0/docs/LICENSE.GPL` & `plone.intelligenttext-4.0.0/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.intelligenttext-3.1.0/docs/LICENSE.txt` & `plone.intelligenttext-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.intelligenttext-3.1.0/setup.py` & `plone.intelligenttext-4.0.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,44 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-version = '3.1.0'
+
+version = "4.0.0"
 
 setup(
-    name='plone.intelligenttext',
+    name="plone.intelligenttext",
     version=version,
     description="Provides transforms from text/x-web-intelligent to "
-                "text/html and vice versa.",
-    long_description=(
-        open("README.rst").read() +
-        "\n" +
-        open("CHANGES.rst").read()
-    ),
+    "text/html and vice versa.",
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 4.0",
-        "Framework :: Plone :: 4.1",
-        "Framework :: Plone :: 4.2",
-        "Framework :: Plone :: 4.3",
-        "Framework :: Plone :: 5.0",
-        "Framework :: Plone :: 5.1",
-        "Framework :: Plone :: 5.2",
+        "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
-        "Framework :: Zope2",
-        "Framework :: Zope :: 4",
+        "Framework :: Zope :: 5",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
-      ],
-    keywords='transform intelligenttext',
-    author='Plone Foundation',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://pypi.org/project/plone.intelligenttext',
-    license='GPL version 2',
+    ],
+    keywords="transform intelligenttext",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/plone.intelligenttext",
+    license="GPL version 2",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
+    python_requires=">=3.8",
     test_suite="plone.intelligenttext.tests.test_suite",
     install_requires=[
-      'setuptools',
+        "setuptools",
     ],
 )
```

### Comparing `plone.intelligenttext-3.1.0/plone/intelligenttext/transforms.py` & `plone.intelligenttext-4.0.0/plone/intelligenttext/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,216 +1,197 @@
-# -*- coding: utf-8 -*-
-import re
-import sys
+from html.entities import name2codepoint
 
-PY3 = sys.version_info[0] == 3
-if PY3:
-    from html.entities import name2codepoint
-    unicode = str
-    unichr = chr
-else:
-    from htmlentitydefs import name2codepoint
+import re
 
 
-def safe_decode(s, encoding='utf-8', errors='strict'):
-    if isinstance(s, unicode):
+def safe_decode(s, encoding="utf-8", errors="strict"):
+    if isinstance(s, str):
         return s
     return s.decode(encoding)
 
 
-class WebIntelligentToHtmlConverter(object):
+class WebIntelligentToHtmlConverter:
     urlRegexp = re.compile(
         r'((?:ftp|https?)://(localhost|([12]?[0-9]{1,2}.){3}([12]?[0-9]{1,2})|(?:[a-z0-9](?:[-a-z0-9]*[a-z0-9])?\.)+(?:com|edu|biz|org|gov|int|info|mil|net|name|museum|coop|aero|[a-z][a-z]))\b(?::\d+)?(?:\/[^"\'<>()\[\]{}\s\x7f-\xff]*(?:[.,?]+[^"\'<>()\[\]{}\s\x7f-\xff]+)*)?)',
-        re.I | re.S | re.U
+        re.I | re.S | re.U,
     )
     emailRegexp = re.compile(
-        r'["=]?(\b[A-Z0-9._%-]+@[A-Z0-9._%-]+\.[A-Z]{2,4}\b)',
-        re.I | re.S | re.U
+        r'["=]?(\b[A-Z0-9._%-]+@[A-Z0-9._%-]+\.[A-Z]{2,4}\b)', re.I | re.S | re.U
     )
-    indentRegexp = re.compile(r'^(\s+)', re.M | re.U)
+    indentRegexp = re.compile(r"^(\s+)", re.M | re.U)
 
     def __init__(self, orig, tab_width=4):
         self.orig = orig
         self.tab_width = tab_width
 
     def __call__(self):
         text = self.orig
         if text is None:
-            text = ''
-        text = safe_decode(text, errors='replace')
+            text = ""
+        text = safe_decode(text, errors="replace")
 
         # Do &amp; separately, else, it may replace an already-inserted & from
         # an entity with &amp;, so < becomes &lt; becomes &amp;lt;
-        text = text.replace('&', '&amp;')
+        text = text.replace("&", "&amp;")
         # Make funny characters into html entity defs
         for entity, codepoint in name2codepoint.items():
-            if entity != 'amp':
-                text = text.replace(unichr(codepoint), '&' + entity + ';')
+            if entity != "amp":
+                text = text.replace(chr(codepoint), "&" + entity + ";")
 
         text = self.urlRegexp.subn(self.replaceURL, text)[0]
         text = self.emailRegexp.subn(self.replaceEmail, text)[0]
         text = self.indentRegexp.subn(self.indentWhitespace, text)[0]
 
         # convert windows line endings
-        text = text.replace('\r\n', '\n')
+        text = text.replace("\r\n", "\n")
         # Finally, make \n's into br's
-        text = text.replace('\n', '<br />')
-
-        if not PY3:
-            text = text.encode('utf-8')
+        text = text.replace("\n", "<br />")
 
         return text
 
     @staticmethod
     def abbreviateUrl(url, max=60, ellipsis="[&hellip;]"):
-        """very long urls are abbreviated to allow nicer layout
-        """
+        """very long urls are abbreviated to allow nicer layout"""
         if len(url) < max:
             return url
         protocol = ""
         protocolend = url.find("//")
         if protocolend != -1:
-            protocol = url[0:protocolend+2]
-            url = url[protocolend+2:]
+            protocol = url[0 : protocolend + 2]
+            url = url[protocolend + 2 :]
         list = url.split("/")
         if len(list) < 3 or len(list[0]) + len(list[-1]) > max:
             url = protocol + url
-            center = (max-5) // 2
+            center = (max - 5) // 2
             return url[:center] + ellipsis + url[-center:]
 
         return protocol + list[0] + "/" + ellipsis + "/" + list[-1]
 
     @classmethod
     def replaceURL(cls, match):
-        """Replace hyperlinks with clickable <a> tags
-        """
+        """Replace hyperlinks with clickable <a> tags"""
         url = match.groups()[0]
         linktext = cls.abbreviateUrl(url)
         # Also with <some link> we should only link to some link, not
         # including the brackets.
-        end = ''
+        end = ""
         # XXX Probably better to fix the regex above.  Maurits
-        if url.endswith('&gt;'):
-            url = url[:-len('&gt;')]
-            linktext = linktext[:-len('&gt;')]
-            end = '&gt;'
-        elif url.endswith('.') or url.endswith('?') or url.endswith('!'):
+        if url.endswith("&gt;"):
+            url = url[: -len("&gt;")]
+            linktext = linktext[: -len("&gt;")]
+            end = "&gt;"
+        elif url.endswith(".") or url.endswith("?") or url.endswith("!"):
             end = url[-1]
             url = url[:-1]
             linktext = linktext[:-1]
 
         # rel="nofollow" shall avoid spamming
-        return '<a href="%s" rel="nofollow">%s</a>%s' % (url, linktext, end)
+        return f'<a href="{url}" rel="nofollow">{linktext}</a>{end}'
 
     @staticmethod
     def replaceEmail(match):
-        """Replace email strings with mailto: links
-        """
+        """Replace email strings with mailto: links"""
         url = match.groups()[0]
         # following unicode substitutions shall avoid email spam
         # crawlers to pickup email addresses
-        url = url.replace('@', '&#0064;')
-        return '<a href="&#0109;ailto&#0058;%s">%s</a>' % (url, url)
+        url = url.replace("@", "&#0064;")
+        return f'<a href="&#0109;ailto&#0058;{url}">{url}</a>'
 
     def indentWhitespace(self, match):
-        """Make leading whitespace on a line into &nbsp; to preserve indents
-        """
+        """Make leading whitespace on a line into &nbsp; to preserve indents"""
         indent = match.groups()[0]
-        indent = indent.replace(' ', '&nbsp;')
-        return indent.replace('\t', '&nbsp;' * self.tab_width)
+        indent = indent.replace(" ", "&nbsp;")
+        return indent.replace("\t", "&nbsp;" * self.tab_width)
 
 
 def convertWebIntelligentPlainTextToHtml(orig, tab_width=4):
-    """Converts text/x-web-intelligent to text/html
-    """
+    """Converts text/x-web-intelligent to text/html"""
     try:
         # tab_width could be a string like '4'
         tab_width = int(tab_width)
     except ValueError:
         tab_width = 4
 
     return WebIntelligentToHtmlConverter(orig, tab_width)()
 
 
 def convertHtmlToWebIntelligentPlainText(orig):
-    """Converts text/html to text/x-web-intelligent.
-    """
-    preRegex = re.compile(r'<\s*pre[^>]*>(.*?)<\s*/pre\s*>', re.I | re.S)
-
-    tagWhitespaceRegex = re.compile(r'\s+((<[^>]+>)\s+)+')
-    whitespaceRegex = re.compile(r'\s+')
-
-    tdRegex = re.compile(r'<\s*(td)([^>])*>', re.I)
-    breakRegex = re.compile(r'<\s*(br)\s*/?>', re.I)
-    startBlockRegex = re.compile(r'<\s*(dt)[^>]*>', re.I)
-    endBlockRegex = re.compile(r'<\s*/\s*(p|div|tr|ul|ol|dl)[^>]*>', re.I)
-    indentBlockRegex = re.compile(r'<\s*(blockquote|dd)[^>]*>', re.I)
-    listBlockRegex = re.compile(r'<\s*(li)[^>]*>', re.I)
+    """Converts text/html to text/x-web-intelligent."""
+    preRegex = re.compile(r"<\s*pre[^>]*>(.*?)<\s*/pre\s*>", re.I | re.S)
+
+    tagWhitespaceRegex = re.compile(r"\s+((<[^>]+>)\s+)+")
+    whitespaceRegex = re.compile(r"\s+")
+
+    tdRegex = re.compile(r"<\s*(td)([^>])*>", re.I)
+    breakRegex = re.compile(r"<\s*(br)\s*/?>", re.I)
+    startBlockRegex = re.compile(r"<\s*(dt)[^>]*>", re.I)
+    endBlockRegex = re.compile(r"<\s*/\s*(p|div|tr|ul|ol|dl)[^>]*>", re.I)
+    indentBlockRegex = re.compile(r"<\s*(blockquote|dd)[^>]*>", re.I)
+    listBlockRegex = re.compile(r"<\s*(li)[^>]*>", re.I)
 
-    tagRegex = re.compile(r'<[^>]+>', re.I | re.M)
+    tagRegex = re.compile(r"<[^>]+>", re.I | re.M)
 
     # Save all <pre> sections and restore after other transforms
     preSections = {}
 
     def savePres(match):
-        marker = '__pre_marker__%d__' % len(preSections)
+        marker = "__pre_marker__%d__" % len(preSections)
         preSections[marker] = match.group(1)
         return marker
+
     if orig is None:
-        orig = ''
+        orig = ""
     text = preRegex.sub(savePres, orig)
 
     def fixTagWhitespace(match):
         """Make whitespace-tag-whitespace into whitespace-tag.
         Repeat this in case there are directly nested tags.
         """
         # Remove any superfluous whitespace, but preserve one leading space
-        return ' ' + whitespaceRegex.sub('', match.group(0))
+        return " " + whitespaceRegex.sub("", match.group(0))
+
     text = tagWhitespaceRegex.sub(fixTagWhitespace, text)
 
     # Make all whitespace into a single space
-    text = whitespaceRegex.sub(' ', text)
+    text = whitespaceRegex.sub(" ", text)
 
     # Fix entities
-    text = text.replace('&nbsp;', ' ')
+    text = text.replace("&nbsp;", " ")
     for entity, codepoint in name2codepoint.items():
         # Do &lt; and &gt; later, else we may be creating what looks like
         # tags
-        if entity != 'lt' and entity != 'gt' and entity != 'amp':
-            text = text.replace(
-                '&' + entity + ';',
-                '&#' + str(codepoint) + ';'
-            )
+        if entity != "lt" and entity != "gt" and entity != "amp":
+            text = text.replace("&" + entity + ";", "&#" + str(codepoint) + ";")
 
     # XXX: Remove <head>, <script>, <style> ?
 
     # Make tabs out of td's
-    text = tdRegex.sub('\t', text)
+    text = tdRegex.sub("\t", text)
 
     # Make br's and li's into newlines
-    text = breakRegex.sub('\n', text)
+    text = breakRegex.sub("\n", text)
 
     # Make the start of list blocks into paragraphs
-    text = startBlockRegex.sub('\n\n', text)
+    text = startBlockRegex.sub("\n\n", text)
 
     # Make the close of p's, div's and tr's into paragraphs
-    text = endBlockRegex.sub('\n\n', text)
+    text = endBlockRegex.sub("\n\n", text)
 
     # Make blockquotes and dd blocks indented
-    text = indentBlockRegex.sub('\n\n  ', text)
+    text = indentBlockRegex.sub("\n\n  ", text)
 
     # Make list items indented and prefixed with -
-    text = listBlockRegex.sub('\n\n  - ', text)
+    text = listBlockRegex.sub("\n\n  - ", text)
 
     # Remove other tags
-    text = tagRegex.sub('', text)
+    text = tagRegex.sub("", text)
 
     # Fix < and > entities
-    text = text.replace('&lt;', '<')
-    text = text.replace('&gt;', '>')
-    text = text.replace('&amp;', '&')
+    text = text.replace("&lt;", "<")
+    text = text.replace("&gt;", ">")
+    text = text.replace("&amp;", "&")
 
-    # Restore pres
+    # Restore `pre`s
     for marker, section in preSections.items():
-        text = text.replace(marker, '\n\n' + section + '\n\n')
+        text = text.replace(marker, "\n\n" + section + "\n\n")
 
     return text
```

### Comparing `plone.intelligenttext-3.1.0/plone/intelligenttext/README.rst` & `plone.intelligenttext-4.0.0/plone/intelligenttext/README.rst`

 * *Files identical despite different names*

### Comparing `plone.intelligenttext-3.1.0/CHANGES.rst` & `plone.intelligenttext-4.0.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,31 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.0 (2023-04-26)
+------------------
+
+Breaking changes:
+
+
+- Drop python 2.7 support.
+  [gforcada] (#1)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (2ed8f544)
+
+
 3.1.0 (2020-04-20)
 ------------------
 
 New features:
 
 
 - Drop Python 2.6 support from tests.
@@ -188,14 +205,14 @@
   [diefenbach]
 
 
 0.1
 ---
 
 - Initial development by Martin Aspeli (optilude@gmx.net). For further
-  informations see http://dev.plone.org/collective/browser/intelligenttext/
+  information see http://dev.plone.org/collective/browser/intelligenttext/
 
 - The transform was originally based on the url_to_hyperlink transform from
   Ploneboard by Plone Solutions and others.
 
 - Initial package structure.
   [zopeskel]
```

