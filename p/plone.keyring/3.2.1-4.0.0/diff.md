# Comparing `tmp/plone.keyring-3.2.1.tar.gz` & `tmp/plone.keyring-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.keyring-3.2.1.tar", last modified: Tue Mar 21 22:51:05 2023, max compression
+gzip compressed data, was "plone.keyring-4.0.0.tar", last modified: Wed Apr 26 21:50:02 2023, max compression
```

## Comparing `plone.keyring-3.2.1.tar` & `plone.keyring-4.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.595036 plone.keyring-3.2.1/
--rw-r--r--   0 maurits    (501) staff       (20)     2637 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      148 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     4934 2023-03-21 22:51:05.595273 plone.keyring-3.2.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1215 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.586665 plone.keyring-3.2.1/docs/
--rw-r--r--   0 maurits    (501) staff       (20)     3124 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.586952 plone.keyring-3.2.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)      244 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.592609 plone.keyring-3.2.1/plone/keyring/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)      606 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     2941 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/django_random.py
--rw-r--r--   0 maurits    (501) staff       (20)     1247 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     1299 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/keymanager.py
--rw-r--r--   0 maurits    (501) staff       (20)     1418 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/keyring.py
--rw-r--r--   0 maurits    (501) staff       (20)      263 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/meta.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.583627 plone.keyring-3.2.1/plone/keyring/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.593387 plone.keyring-3.2.1/plone/keyring/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      227 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/profiles/default/componentregistry.xml
--rw-r--r--   0 maurits    (501) staff       (20)       87 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/profiles/default/metadata.xml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.594641 plone.keyring-3.2.1/plone/keyring/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        2 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     4294 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/tests/testKeymanager.py
--rw-r--r--   0 maurits    (501) staff       (20)     1762 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/plone/keyring/tests/testKeyring.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-03-21 22:51:05.589850 plone.keyring-3.2.1/plone.keyring.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     4934 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      779 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)       60 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-03-21 22:51:05.000000 plone.keyring-3.2.1/plone.keyring.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)      397 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       67 2023-03-21 22:51:05.595744 plone.keyring-3.2.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1563 2023-03-21 22:51:04.000000 plone.keyring-3.2.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.232847 plone.keyring-4.0.0/
+-rw-r--r--   0 maurits    (501) staff       (20)     2813 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      148 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)     4889 2023-04-26 21:50:02.232975 plone.keyring-4.0.0/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1215 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.226833 plone.keyring-4.0.0/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)     3124 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.227228 plone.keyring-4.0.0/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.231292 plone.keyring-4.0.0/plone/keyring/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)      611 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     2723 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/django_random.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1214 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/keymanager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1391 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/keyring.py
+-rw-r--r--   0 maurits    (501) staff       (20)      292 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/meta.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.223332 plone.keyring-4.0.0/plone/keyring/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.231803 plone.keyring-4.0.0/plone/keyring/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      237 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/profiles/default/componentregistry.xml
+-rw-r--r--   0 maurits    (501) staff       (20)       87 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/profiles/default/metadata.xml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.232648 plone.keyring-4.0.0/plone/keyring/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        2 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4190 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/tests/testKeymanager.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1782 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/plone/keyring/tests/testKeyring.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-26 21:50:02.229256 plone.keyring-4.0.0/plone.keyring.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)     4889 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      779 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)       66 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-26 21:50:02.000000 plone.keyring-4.0.0/plone.keyring.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2908 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2023-04-26 21:50:02.233509 plone.keyring-4.0.0/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1349 2023-04-26 21:50:01.000000 plone.keyring-4.0.0/setup.py
```

### Comparing `plone.keyring-3.2.1/CHANGES.rst` & `plone.keyring-4.0.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,31 @@
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
 3.2.1 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.keyring-3.2.1/PKG-INFO` & `plone.keyring-4.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.keyring
-Version: 3.2.1
+Version: 4.0.0
 Summary: Manage secrets
 Home-page: https://pypi.org/project/plone.keyring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: secret key keyring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 
 Introduction
 ============
 
 *plone.keyring* contains a Zope utility that facilitates handling of
 secrets in an application. Secrets are very important in modern applications,
 which is why a shared tool to manage them is useful.
@@ -71,14 +67,31 @@
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
 3.2.1 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.keyring-3.2.1/README.rst` & `plone.keyring-4.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `plone.keyring-3.2.1/docs/LICENSE.txt` & `plone.keyring-4.0.0/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.keyring-3.2.1/plone/keyring/configure.zcml` & `plone.keyring-4.0.0/plone/keyring/configure.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 <configure
     xmlns="http://namespaces.zope.org/zope"
-    xmlns:zcml="http://namespaces.zope.org/zcml"
     xmlns:genericsetup="http://namespaces.zope.org/genericsetup"
-    i18n_domain="plone.keyring">
+    xmlns:zcml="http://namespaces.zope.org/zcml"
+    i18n_domain="plone.keyring"
+    >
 
   <genericsetup:registerProfile
-      zcml:condition="installed Products.GenericSetup"
       name="default"
-      directory="profiles/default"
       title="plone.keyring KeyManager registration"
       description="Registers a persistent plone.keyring KeyManager"
       provides="Products.GenericSetup.interfaces.EXTENSION"
       for="zope.interface.interfaces.IComponentRegistry"
+      directory="profiles/default"
+      zcml:condition="installed Products.GenericSetup"
       />
 
 </configure>
```

### Comparing `plone.keyring-3.2.1/plone/keyring/django_random.py` & `plone.keyring-4.0.0/plone/keyring/django_random.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,50 +24,43 @@
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
 ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
+from hashlib import sha256 as sha
+
 import random
+import time
+
+
 try:
     random = random.SystemRandom()
     using_sysrandom = True
 except NotImplementedError:
     using_sysrandom = False
 
-try:
-    from hashlib import sha256 as sha
-except ImportError:
-    from sha import sha
-
-import time
-
 
 # generated when process started, hard to guess
 SECRET = random.randint(0, 1000000)
 
 
-def get_random_string(length=12,
-                      allowed_chars='abcdefghijklmnopqrstuvwxyz'
-                                    'ABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'):
+def get_random_string(
+    length=12,
+    allowed_chars="abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789",
+):
     """
     Returns a securely generated random string.
 
     The default length of 12 with the a-z, A-Z, 0-9 character set returns
     a 71-bit value. log_2((26+26+10)^12) =~ 71 bits
     """
     if not using_sysrandom:
         # This is ugly, and a hack, but it makes things better than
         # the alternative of predictability. This re-seeds the PRNG
         # using a value that is hard for an attacker to predict, every
         # time a random string is required. This may change the
         # properties of the chosen random sequence slightly, but this
         # is better than absolute predictability.
-        random.seed(
-            sha(
-                "%s%s%s" % (
-                    random.getstate(),
-                    time.time(),
-                    SECRET)
-                ).digest())
-    return ''.join([random.choice(allowed_chars) for i in range(length)])
+        random.seed(sha(f"{random.getstate()}{time.time()}{SECRET}").digest())
+    return "".join([random.choice(allowed_chars) for i in range(length)])
```

### Comparing `plone.keyring-3.2.1/plone/keyring/interfaces.py` & `plone.keyring-4.0.0/plone/keyring/interfaces.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 from zope.container.constraints import contains
 from zope.container.interfaces import IContainer
 from zope.interface import Attribute
 from zope.interface.common.sequence import IFiniteSequence
 from zope.location.interfaces import IContained
 
 
-
 class IKeyManager(IContainer):
     contains("plone.keyring.interfaces.IKeyring")
 
-    def clear(ring=u"_system"):
+    def clear(ring="_system"):
         """Clear all keys on a given ring. By default the system ring
         is cleader.  If None is used as ring id all rings are cleared.
         """
 
-    def rotate(ring=u"_system"):
+    def rotate(ring="_system"):
         """Rotate a given ring. By default rotates the system ring.
         If None is used as ring id all rings are rotated.
         """
 
-    def secret(ring=u"_system"):
+    def secret(ring="_system"):
         """Return the current secret for a given ring. If no ring
         is given the secret for the system ring is returned"""
 
 
-
 class IKeyring(IContained, IFiniteSequence):
     current = Attribute("The current (ie latest) secret in the ring.")
 
     def __init__(size=5):
-        """Construct a new keyring for a specified number of keys.
-        """
+        """Construct a new keyring for a specified number of keys."""
 
     def clear():
-        """Remove all keys from the ring.
-        """
+        """Remove all keys from the ring."""
 
     def rotate():
-        """Add a new secret to the ring, pushing out the oldest secret.
-        """
-
+        """Add a new secret to the ring, pushing out the oldest secret."""
```

### Comparing `plone.keyring-3.2.1/plone/keyring/keymanager.py` & `plone.keyring-4.0.0/plone/keyring/keymanager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from persistent.mapping import PersistentMapping
-from zope.container.sample import SampleContainer
-from zope.interface import implementer
-
 from plone.keyring.interfaces import IKeyManager
 from plone.keyring.keyring import Keyring
+from zope.container.sample import SampleContainer
+from zope.interface import implementer
 
 
 @implementer(IKeyManager)
 class KeyManager(SampleContainer):
-
     def __init__(self, keyring_size=5):
         SampleContainer.__init__(self)
 
         if keyring_size < 1:
             keyring_size = 5  # prevent not having any keys
 
-        self[u"_system"] = Keyring(keyring_size)
-        self[u"_system"].fill()
+        self["_system"] = Keyring(keyring_size)
+        self["_system"].fill()
 
         # to be used with anonymous users
-        self[u'_anon'] = Keyring(keyring_size)
-        self[u'_anon'].fill()
+        self["_anon"] = Keyring(keyring_size)
+        self["_anon"].fill()
 
         # to be used with forms, plone.protect here..
-        self[u'_forms'] = Keyring(keyring_size)
-        self[u'_forms'].fill()
+        self["_forms"] = Keyring(keyring_size)
+        self["_forms"].fill()
 
     def _newContainerData(self):
         return PersistentMapping()
 
-    def clear(self, ring=u"_system"):
+    def clear(self, ring="_system"):
         if ring is None:
             for ring in self.values():
                 ring.clear()
         else:
             self[ring].clear()
 
-    def rotate(self, ring=u"_system"):
+    def rotate(self, ring="_system"):
         if ring is None:
             for ring in self.values():
                 ring.rotate()
         else:
             self[ring].rotate()
 
-    def secret(self, ring=u"_system"):
+    def secret(self, ring="_system"):
         return self[ring].current
```

### Comparing `plone.keyring-3.2.1/plone/keyring/keyring.py` & `plone.keyring-4.0.0/plone/keyring/keyring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-import time
-from random import choice
-
 from persistent.list import PersistentList
+from plone.keyring import django_random
+from plone.keyring.interfaces import IKeyring
+from random import choice
 from zope.interface import implementer
 from zope.location.interfaces import IContained
 
-from plone.keyring.interfaces import IKeyring
-from plone.keyring import django_random
+import time
 
 
 def GenerateSecret(length=64):
     return django_random.get_random_string(length)
 
 
 @implementer(IKeyring, IContained)
 class Keyring(PersistentList):
-
     __parent__ = __name__ = None
 
     last_rotation = 0
 
     def __init__(self, size=5):
         PersistentList.__init__(self)
         for i in range(size):
             self.append(None)
 
     def __iter__(self):
-        for item in self.data:
-            yield item
+        yield from self.data
 
     def clear(self):
         for i in range(len(self)):
             self[i] = None
 
     def rotate(self):
         self.pop()
```

### Comparing `plone.keyring-3.2.1/plone/keyring/tests/testKeymanager.py` & `plone.keyring-4.0.0/plone/keyring/tests/testKeymanager.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,124 +1,114 @@
-from unittest import makeSuite
-from unittest import TestCase
-from unittest import TestSuite
 from persistent.mapping import PersistentMapping
-from zope.interface.verify import verifyClass
 from plone.keyring.interfaces import IKeyManager
 from plone.keyring.keymanager import KeyManager
 from plone.keyring.keyring import Keyring
+from unittest import makeSuite
+from unittest import TestCase
+from unittest import TestSuite
+from zope.interface.verify import verifyClass
 
 
-marker=[]
+marker = []
 
 
 class KeyManagerTests(TestCase):
     def setUp(self):
-        self.mgr=KeyManager()
-        del self.mgr[u"_system"]
-        self.mgr[u"_system"]=Keyring()
-        self.mgr[u"_system"].rotate()
-        self.mgr[u"one"]=Keyring()
-        self.mgr[u"one"].rotate()
-        self.mgr[u"two"]=Keyring()
-        self.mgr[u"two"].rotate()
-
+        self.mgr = KeyManager()
+        del self.mgr["_system"]
+        self.mgr["_system"] = Keyring()
+        self.mgr["_system"].rotate()
+        self.mgr["one"] = Keyring()
+        self.mgr["one"].rotate()
+        self.mgr["two"] = Keyring()
+        self.mgr["two"].rotate()
 
     def testInterface(self):
         verifyClass(IKeyManager, KeyManager)
 
-
     def testSystemKeyringCreated(self):
-        mgr=KeyManager()
-        self.assertEqual(set(mgr), {u"_anon", u"_forms", u"_system"})
-        self.assertTrue(mgr[u"_system"].current is not None)
-
+        mgr = KeyManager()
+        self.assertEqual(set(mgr), {"_anon", "_forms", "_system"})
+        self.assertTrue(mgr["_system"].current is not None)
 
     def testContainerIsPersistent(self):
-        mgr=KeyManager()
-        self.assertTrue(isinstance(mgr.__dict__["_SampleContainer__data"],
-                                   PersistentMapping))
-
+        mgr = KeyManager()
+        self.assertTrue(
+            isinstance(mgr.__dict__["_SampleContainer__data"], PersistentMapping)
+        )
 
     def testClear(self):
         self.mgr.clear()
-        self.assertEqual(set(self.mgr[u"_system"]), set([None]))
-        self.assertNotEqual(set(self.mgr[u"one"]), set([None]))
-        self.assertNotEqual(set(self.mgr[u"two"]), set([None]))
-
+        self.assertEqual(set(self.mgr["_system"]), {None})
+        self.assertNotEqual(set(self.mgr["one"]), {None})
+        self.assertNotEqual(set(self.mgr["two"]), {None})
 
     def testClearGivenRing(self):
-        self.mgr.clear(u"one")
-        self.assertNotEqual(set(self.mgr[u"_system"]), set([None]))
-        self.assertEqual(set(self.mgr[u"one"]), set([None]))
-        self.assertNotEqual(set(self.mgr[u"two"]), set([None]))
-
+        self.mgr.clear("one")
+        self.assertNotEqual(set(self.mgr["_system"]), {None})
+        self.assertEqual(set(self.mgr["one"]), {None})
+        self.assertNotEqual(set(self.mgr["two"]), {None})
 
     def testClearAll(self):
         self.mgr.clear(None)
-        self.assertEqual(set(self.mgr[u"_system"]), set([None]))
-        self.assertEqual(set(self.mgr[u"one"]), set([None]))
-        self.assertEqual(set(self.mgr[u"two"]), set([None]))
-
+        self.assertEqual(set(self.mgr["_system"]), {None})
+        self.assertEqual(set(self.mgr["one"]), {None})
+        self.assertEqual(set(self.mgr["two"]), {None})
 
     def testClearUnknownRing(self):
-        self.assertRaises(KeyError, self.mgr.clear, u"missing")
-
+        self.assertRaises(KeyError, self.mgr.clear, "missing")
 
     def testRotate(self):
-        current_sys = self.mgr[u"_system"].current
-        current_one = self.mgr[u"one"].current
-        current_two = self.mgr[u"two"].current
+        current_sys = self.mgr["_system"].current
+        current_one = self.mgr["one"].current
+        current_two = self.mgr["two"].current
         self.mgr.rotate()
-        self.assertNotEqual(self.mgr[u"_system"].current, current_sys)
-        self.assertEqual(self.mgr[u"_system"][1], current_sys)
-        self.assertEqual(self.mgr[u"one"].current, current_one)
-        self.assertEqual(self.mgr[u"one"][1], None)
-        self.assertEqual(self.mgr[u"two"].current, current_two)
-        self.assertEqual(self.mgr[u"two"][1], None)
-
+        self.assertNotEqual(self.mgr["_system"].current, current_sys)
+        self.assertEqual(self.mgr["_system"][1], current_sys)
+        self.assertEqual(self.mgr["one"].current, current_one)
+        self.assertEqual(self.mgr["one"][1], None)
+        self.assertEqual(self.mgr["two"].current, current_two)
+        self.assertEqual(self.mgr["two"][1], None)
 
     def testRotateGivenRing(self):
-        current_sys = self.mgr[u"_system"].current
-        current_one = self.mgr[u"one"].current
-        current_two = self.mgr[u"two"].current
-        self.mgr.rotate(u"one")
-        self.assertEqual(self.mgr[u"_system"].current, current_sys)
-        self.assertEqual(self.mgr[u"_system"][1], None)
-        self.assertNotEqual(self.mgr[u"one"].current, current_one)
-        self.assertEqual(self.mgr[u"one"][1], current_one)
-        self.assertEqual(self.mgr[u"two"].current, current_two)
-        self.assertEqual(self.mgr[u"two"][1], None)
-
+        current_sys = self.mgr["_system"].current
+        current_one = self.mgr["one"].current
+        current_two = self.mgr["two"].current
+        self.mgr.rotate("one")
+        self.assertEqual(self.mgr["_system"].current, current_sys)
+        self.assertEqual(self.mgr["_system"][1], None)
+        self.assertNotEqual(self.mgr["one"].current, current_one)
+        self.assertEqual(self.mgr["one"][1], current_one)
+        self.assertEqual(self.mgr["two"].current, current_two)
+        self.assertEqual(self.mgr["two"][1], None)
 
     def testRotateAll(self):
-        current_sys = self.mgr[u"_system"].current
-        current_one = self.mgr[u"one"].current
-        current_two = self.mgr[u"two"].current
+        current_sys = self.mgr["_system"].current
+        current_one = self.mgr["one"].current
+        current_two = self.mgr["two"].current
         self.mgr.rotate(None)
-        self.assertNotEqual(self.mgr[u"_system"].current, current_sys)
-        self.assertEqual(self.mgr[u"_system"][1], current_sys)
-        self.assertNotEqual(self.mgr[u"one"].current, current_one)
-        self.assertEqual(self.mgr[u"one"][1], current_one)
-        self.assertNotEqual(self.mgr[u"two"].current, current_two)
-        self.assertEqual(self.mgr[u"two"][1], current_two)
-
+        self.assertNotEqual(self.mgr["_system"].current, current_sys)
+        self.assertEqual(self.mgr["_system"][1], current_sys)
+        self.assertNotEqual(self.mgr["one"].current, current_one)
+        self.assertEqual(self.mgr["one"][1], current_one)
+        self.assertNotEqual(self.mgr["two"].current, current_two)
+        self.assertEqual(self.mgr["two"][1], current_two)
 
     def testRotateUnknownRing(self):
-        self.assertRaises(KeyError, self.mgr.clear, u"missing")
-
+        self.assertRaises(KeyError, self.mgr.clear, "missing")
 
     def testSecret(self):
-        self.mgr[u"_system"][0]=marker
+        self.mgr["_system"][0] = marker
         self.assertTrue(self.mgr.secret() is marker)
 
     def testSecretGivenRing(self):
-        self.mgr[u"one"][0]=marker
-        self.assertTrue(self.mgr.secret(u"one") is marker)
+        self.mgr["one"][0] = marker
+        self.assertTrue(self.mgr.secret("one") is marker)
 
     def testSecretUnknownRing(self):
-        self.assertRaises(KeyError, self.mgr.secret, u"missing")
+        self.assertRaises(KeyError, self.mgr.secret, "missing")
+
 
 def test_suite():
-    suite=TestSuite()
+    suite = TestSuite()
     suite.addTest(makeSuite(KeyManagerTests))
     return suite
```

### Comparing `plone.keyring-3.2.1/plone/keyring/tests/testKeyring.py` & `plone.keyring-4.0.0/plone/keyring/tests/testKeyring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,64 @@
-import types
+from plone.keyring.interfaces import IKeyring
+from plone.keyring.keyring import Keyring
 from unittest import makeSuite
 from unittest import TestCase
 from unittest import TestSuite
 from zope.interface.verify import verifyClass
-from plone.keyring.interfaces import IKeyring
-from plone.keyring.keyring import Keyring
+
+import types
+
 
 class KeyringTests(TestCase):
     def testInterface(self):
         verifyClass(IKeyring, Keyring)
 
     def testConstructionDefaultSize(self):
-        ring=Keyring()
+        ring = Keyring()
         self.assertEqual(len(ring), 5)
 
     def testConstructionSize(self):
-        ring=Keyring(3)
+        ring = Keyring(3)
         self.assertEqual(len(ring), 3)
 
     def testKeyringStartsEmpty(self):
-        ring=Keyring()
-        self.assertEqual(set(list(ring)), set([None]))
+        ring = Keyring()
+        self.assertEqual(set(list(ring)), {None})
 
     def testIterate(self):
-        ring=Keyring()
-        ring.data=[0, 1, 2, 3, 4]
-        iterator=ring.__iter__()
+        ring = Keyring()
+        ring.data = [0, 1, 2, 3, 4]
+        iterator = ring.__iter__()
         self.assertTrue(isinstance(iterator, types.GeneratorType))
         self.assertEqual(list(iterator), [0, 1, 2, 3, 4])
 
     def testClear(self):
-        ring=Keyring()
-        ring.data=[0, 1, 2]
+        ring = Keyring()
+        ring.data = [0, 1, 2]
         ring.clear()
-        self.assertEqual(ring.data, [ None, None, None ])
+        self.assertEqual(ring.data, [None, None, None])
 
     def testRotate(self):
-        ring=Keyring()
+        ring = Keyring()
         ring.rotate()
         self.assertFalse(ring.current is None)
-        self.assertEqual(ring.data[1:], [ None, None, None, None])
+        self.assertEqual(ring.data[1:], [None, None, None, None])
 
     def testRotateTwice(self):
-        ring=Keyring()
+        ring = Keyring()
         ring.rotate()
         ring.rotate()
         self.assertTrue(ring.data[0] is not None)
         self.assertTrue(ring.data[1] is not None)
-        self.assertEqual(ring.data[2:], [ None, None, None])
+        self.assertEqual(ring.data[2:], [None, None, None])
 
     def testCurrent(self):
-        ring=Keyring()
-        marker=[]
-        ring.data=[marker, 1, 2, 3]
+        ring = Keyring()
+        marker = []
+        ring.data = [marker, 1, 2, 3]
         self.assertTrue(ring.current is marker)
 
 
 def test_suite():
-    suite=TestSuite()
+    suite = TestSuite()
     suite.addTest(makeSuite(KeyringTests))
     return suite
-
```

### Comparing `plone.keyring-3.2.1/plone.keyring.egg-info/PKG-INFO` & `plone.keyring-4.0.0/plone.keyring.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 Metadata-Version: 2.1
 Name: plone.keyring
-Version: 3.2.1
+Version: 4.0.0
 Summary: Manage secrets
 Home-page: https://pypi.org/project/plone.keyring
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: BSD
 Keywords: secret key keyring
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Plone
-Classifier: Framework :: Plone :: 5.2
 Classifier: Framework :: Plone :: 6.0
 Classifier: Framework :: Plone :: Core
-Classifier: Framework :: Zope :: 4
 Classifier: Framework :: Zope :: 5
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Requires-Python: >=3.8
 
 Introduction
 ============
 
 *plone.keyring* contains a Zope utility that facilitates handling of
 secrets in an application. Secrets are very important in modern applications,
 which is why a shared tool to manage them is useful.
@@ -71,14 +67,31 @@
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
 3.2.1 (2023-03-21)
 ------------------
 
 Bug fixes:
 
 
 - Use `ZODB` as dependency rather than the deprecated `ZODB3`.
```

### Comparing `plone.keyring-3.2.1/plone.keyring.egg-info/SOURCES.txt` & `plone.keyring-4.0.0/plone.keyring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.keyring-3.2.1/setup.py` & `plone.keyring-4.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
-version = '3.2.1'
+
+version = "4.0.0"
 
 setup(
-    name='plone.keyring',
+    name="plone.keyring",
     version=version,
     description="Manage secrets",
-    long_description=(open("README.rst").read() + "\n" +
-                      open("CHANGES.rst").read()),
+    long_description=(open("README.rst").read() + "\n" + open("CHANGES.rst").read()),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
-        "Framework :: Plone :: 5.2",
         "Framework :: Plone :: 6.0",
         "Framework :: Plone :: Core",
-        "Framework :: Zope :: 4",
         "Framework :: Zope :: 5",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    keywords='secret key keyring',
-    author='Plone Foundation',
-    author_email='plone-developers@lists.sourceforge.net',
-    url='https://pypi.org/project/plone.keyring',
-    license='BSD',
+    keywords="secret key keyring",
+    author="Plone Foundation",
+    author_email="plone-developers@lists.sourceforge.net",
+    url="https://pypi.org/project/plone.keyring",
+    license="BSD",
     packages=find_packages(),
-    namespace_packages=['plone'],
+    namespace_packages=["plone"],
     include_package_data=True,
     zip_safe=False,
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*",
+    python_requires=">=3.8",
     install_requires=[
-        'setuptools',
-        'ZODB',
-        'zope.container',
-        'zope.interface',
-        'zope.location',
+        "persistent",
+        "setuptools",
+        "zope.container",
+        "zope.interface",
+        "zope.location",
     ],
-    )
+)
```

