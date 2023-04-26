# Comparing `tmp/PwnModules-1.0.tar.gz` & `tmp/PwnModules-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PwnModules-1.0.tar", last modified: Mon Apr 24 14:31:20 2023, max compression
+gzip compressed data, was "PwnModules-1.1.tar", last modified: Tue Apr 25 14:58:36 2023, max compression
```

## Comparing `PwnModules-1.0.tar` & `PwnModules-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 14:31:20.943480 PwnModules-1.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.0/License.txt
--rw-rw-rw-   0        0        0      747 2023-04-24 14:31:20.942484 PwnModules-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 14:31:20.940489 PwnModules-1.0/PwnModules.egg-info/
--rw-rw-rw-   0        0        0      747 2023-04-24 14:31:20.000000 PwnModules-1.0/PwnModules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-04-24 14:31:20.000000 PwnModules-1.0/PwnModules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 14:31:20.000000 PwnModules-1.0/PwnModules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 14:31:20.000000 PwnModules-1.0/PwnModules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-24 14:31:20.000000 PwnModules-1.0/PwnModules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1818 2023-04-24 14:29:29.000000 PwnModules-1.0/PwnModules.py
--rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-24 14:31:20.943480 PwnModules-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 14:58:36.196752 PwnModules-1.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 12:32:23.000000 PwnModules-1.1/License.txt
+-rw-rw-rw-   0        0        0      747 2023-04-25 14:58:36.195754 PwnModules-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-25 14:58:36.193759 PwnModules-1.1/PwnModules.egg-info/
+-rw-rw-rw-   0        0        0      747 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-04-25 14:58:36.000000 PwnModules-1.1/PwnModules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-25 14:58:35.000000 PwnModules-1.1/PwnModules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2023-04-25 14:47:46.000000 PwnModules-1.1/PwnModules.py
+-rw-rw-rw-   0        0        0       84 2023-04-24 14:25:45.000000 PwnModules-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-25 14:58:36.196752 PwnModules-1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-04-24 14:25:56.000000 PwnModules-1.1/setup.py
```

### Comparing `PwnModules-1.0/License.txt` & `PwnModules-1.1/License.txt`

 * *Files identical despite different names*

### Comparing `PwnModules-1.0/PKG-INFO` & `PwnModules-1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.0
+Version: 1.1
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.0/PwnModules.egg-info/PKG-INFO` & `PwnModules-1.1/PwnModules.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PwnModules
-Version: 1.0
+Version: 1.1
 Summary: A open-source Pwntools Extern Functions.
 Home-page: https://github.com/XKaguya/PwnModules
 Author: RedLeaves
 Author-email: rx700@vip.qq.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PwnModules-1.0/PwnModules.py` & `PwnModules-1.1/PwnModules.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 Pwntools-Extern Functions
 开源包，任何人都可以使用并修改！
 """
 
 from LibcSearcher import *
 from pwn import *
 
-__version__ = '1.0'
+__version__ = '1.1'
 
 def leak_addr(i, io_i):
+    if i == 0:
+        address_internal = u32(io_i.recv(4))
+        return address_internal
     if i == 1:
         address_internal = u64(io_i.recvuntil(b'\x7f')[:6].ljust(8, b'\x00'))
         return address_internal
-    else:
-        address_internal = u32(io_i.recv(4))
-        return address_internal
     if i == 2:
         address_internal = u64(io_i.recvuntil(b'\x7f')[-6:].ljust(8, b'\x00'))
         return address_internal
 
 
 def libc_remastered(func, addr_i):
     libc_i = LibcSearcher(func, addr_i)
```

### Comparing `PwnModules-1.0/setup.py` & `PwnModules-1.1/setup.py`

 * *Files identical despite different names*

