# Comparing `tmp/cs.htmlmailer-2.0.tar.gz` & `tmp/cs.htmlmailer-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cs.htmlmailer-2.0.tar", last modified: Mon Feb 10 14:01:48 2020, max compression
+gzip compressed data, was "cs.htmlmailer-2.1.tar", last modified: Wed Apr 26 07:58:09 2023, max compression
```

## Comparing `cs.htmlmailer-2.0.tar` & `cs.htmlmailer-2.1.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/
--rw-r--r--   0 erral     (1000) erral     (1000)      575 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/README.txt
--rw-r--r--   0 erral     (1000) erral     (1000)       29 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/MANIFEST.in
--rw-r--r--   0 erral     (1000) erral     (1000)     1305 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/PKG-INFO
--rw-r--r--   0 erral     (1000) erral     (1000)      912 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/setup.py
--rw-r--r--   0 erral     (1000) erral     (1000)       38 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/setup.cfg
-drwxr-xr-x   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs/
-drwxr-xr-x   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs/htmlmailer/
--rw-r--r--   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs/htmlmailer/__init__.py
--rw-r--r--   0 erral     (1000) erral     (1000)     2430 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs/htmlmailer/mailer.py
--rw-r--r--   0 erral     (1000) erral     (1000)      244 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs/__init__.py
-drwxr-xr-x   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/docs/
--rw-r--r--   0 erral     (1000) erral     (1000)      157 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/docs/HISTORY.txt
-drwxr-xr-x   0 erral     (1000) erral     (1000)        0 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/
--rw-r--r--   0 erral     (1000) erral     (1000)        1 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/dependency_links.txt
--rw-r--r--   0 erral     (1000) erral     (1000)       37 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/entry_points.txt
--rw-r--r--   0 erral     (1000) erral     (1000)        3 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/top_level.txt
--rw-r--r--   0 erral     (1000) erral     (1000)     1305 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/PKG-INFO
--rw-r--r--   0 erral     (1000) erral     (1000)        1 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/not-zip-safe
--rw-r--r--   0 erral     (1000) erral     (1000)       11 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/requires.txt
--rw-r--r--   0 erral     (1000) erral     (1000)      419 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/SOURCES.txt
--rw-r--r--   0 erral     (1000) erral     (1000)        3 2020-02-10 14:01:48.000000 cs.htmlmailer-2.0/cs.htmlmailer.egg-info/namespace_packages.txt
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:09.670937 cs.htmlmailer-2.1/
+-rw-rw-r--   0 erral     (1000) erral     (1000)       29 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/MANIFEST.in
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1338 2023-04-26 07:58:09.666937 cs.htmlmailer-2.1/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)      575 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/README.txt
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:09.666937 cs.htmlmailer-2.1/cs/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      245 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/cs/__init__.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:09.666937 cs.htmlmailer-2.1/cs/htmlmailer/
+-rw-rw-r--   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/cs/htmlmailer/__init__.py
+-rw-rw-r--   0 erral     (1000) erral     (1000)     2358 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/cs/htmlmailer/mailer.py
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:09.666937 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1338 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/PKG-INFO
+-rw-rw-r--   0 erral     (1000) erral     (1000)      379 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/SOURCES.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/dependency_links.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        3 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/namespace_packages.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        1 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/not-zip-safe
+-rw-rw-r--   0 erral     (1000) erral     (1000)       11 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/requires.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)        3 2023-04-26 07:58:09.000000 cs.htmlmailer-2.1/cs.htmlmailer.egg-info/top_level.txt
+drwxrwxr-x   0 erral     (1000) erral     (1000)        0 2023-04-26 07:58:09.666937 cs.htmlmailer-2.1/docs/
+-rw-rw-r--   0 erral     (1000) erral     (1000)      241 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/docs/HISTORY.txt
+-rw-rw-r--   0 erral     (1000) erral     (1000)       38 2023-04-26 07:58:09.670937 cs.htmlmailer-2.1/setup.cfg
+-rw-rw-r--   0 erral     (1000) erral     (1000)     1056 2023-04-26 07:58:07.000000 cs.htmlmailer-2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cs.htmlmailer-2.0/README.txt` & `cs.htmlmailer-2.1/README.txt`

 * *Files identical despite different names*

### Comparing `cs.htmlmailer-2.0/setup.py` & `cs.htmlmailer-2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
 import os
 
-version = "2.0"
+version = "2.1"
 
 setup(
     name="cs.htmlmailer",
     version=version,
     description="A library to send emails with HTML and Text mixed content",
     long_description=open("README.txt").read()
     + "\n"
     + open(os.path.join("docs", "HISTORY.txt")).read(),
-    # Get more strings from
-    # http://pypi.python.org/pypi?:action=list_classifiers
-    classifiers=["Programming Language :: Python"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ],
     keywords="",
     author="Mikel Larreategi",
     author_email="mlarreategi@codesyntax.com",
     url="https://github.com/codesyntax/cs.htmlmailer/",
     license="GPL",
     packages=find_packages(exclude=["ez_setup"]),
     namespace_packages=["cs"],
```

### Comparing `cs.htmlmailer-2.0/cs/htmlmailer/mailer.py` & `cs.htmlmailer-2.1/cs/htmlmailer/mailer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 __doc__ = """ Mailer stolen from collective.singing """
 
 from email.header import Header
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate
-from email.utils import make_msgid
 from html.parser import HTMLParser
 
 
 class HTMLFilter(HTMLParser):
     text = ""
     anchorlist = []
 
@@ -60,15 +59,14 @@
     # maybe later :)  msg['From'] = Header("%s <%s>" % (send_from_name, send_from), encoding)
     msg["Subject"] = Header(subject, encoding)
     msg["From"] = from_addr
     msg["To"] = to_addr
     if cc_addrs:
         msg["Cc"] = ", ".join(cc_addrs)
     msg["Date"] = formatdate(localtime=True)
-    msg["Message-ID"] = make_msgid()
     if headers:
         for key, value in headers.items():
             msg[key] = value
     msg.preamble = "This is a multi-part message in MIME format."
 
     alternatives = MIMEMultipart("alternative")
     msg.attach(alternatives)
```

