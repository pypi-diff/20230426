# Comparing `tmp/usefulib-1.0.2.tar.gz` & `tmp/usefulib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usefulib-1.0.2.tar", last modified: Fri Apr 21 10:08:26 2023, max compression
+gzip compressed data, was "usefulib-1.0.3.tar", last modified: Wed Apr 26 16:23:25 2023, max compression
```

## Comparing `usefulib-1.0.2.tar` & `usefulib-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 10:08:26.746216 usefulib-1.0.2/
--rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1721 2023-04-21 10:08:26.746216 usefulib-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-04-21 10:06:52.000000 usefulib-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-04-21 10:08:26.746216 usefulib-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1962 2023-04-21 10:04:02.000000 usefulib-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:08:26.730566 usefulib-1.0.2/usefulib/
--rw-rw-rw-   0        0        0      210 2023-04-21 10:04:14.000000 usefulib-1.0.2/usefulib/__init__.py
--rw-rw-rw-   0        0        0     3734 2023-04-21 10:04:19.000000 usefulib-1.0.2/usefulib/_usefulibs.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:08:26.746216 usefulib-1.0.2/usefulib/temp_data/
--rw-rw-rw-   0        0        0      238 2023-04-21 10:04:28.000000 usefulib-1.0.2/usefulib/temp_data/__init__.py
--rw-rw-rw-   0        0        0     3086 2023-04-21 10:04:23.000000 usefulib-1.0.2/usefulib/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-21 10:08:26.730566 usefulib-1.0.2/usefulib.egg-info/
--rw-rw-rw-   0        0        0     1721 2023-04-21 10:08:26.000000 usefulib-1.0.2/usefulib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-04-21 10:08:26.000000 usefulib-1.0.2/usefulib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 10:08:26.000000 usefulib-1.0.2/usefulib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 10:08:26.000000 usefulib-1.0.2/usefulib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.691342 usefulib-1.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-04-18 17:53:04.000000 usefulib-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     3150 2023-04-26 16:23:25.690344 usefulib-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2434 2023-04-26 16:22:01.000000 usefulib-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-26 16:23:25.691342 usefulib-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     3391 2023-04-26 16:20:23.000000 usefulib-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.660328 usefulib-1.0.3/usefulib/
+-rw-rw-rw-   0        0        0      210 2023-04-26 16:20:46.000000 usefulib-1.0.3/usefulib/__init__.py
+-rw-rw-rw-   0        0        0     4246 2023-04-26 16:20:39.000000 usefulib-1.0.3/usefulib/_usefulibs.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.689359 usefulib-1.0.3/usefulib/temp_data/
+-rw-rw-rw-   0        0        0      238 2023-04-21 10:04:28.000000 usefulib-1.0.3/usefulib/temp_data/__init__.py
+-rw-rw-rw-   0        0        0     3276 2023-04-26 16:20:34.000000 usefulib-1.0.3/usefulib/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-26 16:23:25.682761 usefulib-1.0.3/usefulib.egg-info/
+-rw-rw-rw-   0        0        0     3150 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 16:23:25.000000 usefulib-1.0.3/usefulib.egg-info/top_level.txt
```

### Comparing `usefulib-1.0.2/LICENSE` & `usefulib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `usefulib-1.0.2/setup.py` & `usefulib-1.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,72 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.2'
+VERSION = '1.0.3'
 DESCRIPTION = 'A collection of assorted methods to make small tasks easier..'
 LONG_DESCRIPTION = """
-# usefulib v1.0.2
-A useful library for Python with assorted functions to make small tasks easier.
+<div align="center">
+  <img src="https://github.com/hamdivazim/usefulib/raw/main/logo.png">
+</div>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/Python- >= 2.7 -blue?style=plastic.svg" alt="python versions" /></a>
+<a style="display:inline;" href="#"><img src="https://badge.fury.io/py/usefulib.svg" alt="pypi version" /></a>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/first timer-friendly-4DC71F?style=plastic.svg" alt="first timer friendly" /></a>
+<a style="display:inline;" href="https://github.com/hamdivazim/usefulib/labels/usefulib-idea"><img src="https://img.shields.io/github/issues-raw/hamdivazim/usefulib/usefulib-idea?color=4DC71F&label=usefulib%20ideas" alt="usefulib ideas" /></a>
+<a style="display:inline;" href="#"><img src="https://img.shields.io/badge/tests- all passing -4DC71F?style=plastic.svg" alt="usefulib ideas" /></a>
+
+
+
+<h1>usefulib v1.0.2</h1>
+A useful library for Python with <em>a lot</em> of assorted functions to make numerous small tasks easier.
 
 ### GitHub Page: https://github.com/hamdivazim/usefulib
 
 ## How to install
 Install with pip in your terminal, making sure Python is added to PATH:
 ```
 $ pip install usefulib
 ```
+Alternatively, you can use the git URL to do the same.
+```
+$ pip install "git+https://github.com/hamdivazim/usefulib.git@pip-install#egg=usefulib"
+```
 
 ## How to use
 All you need to do is import the package, and all usefulibs that you may want will come along with it! As an example:
 ```python
 import usefulib
 
 a_string = "abcdef123456"
 reverse_string = usefulib.reverse_string(a_string)
 ```
+If all you need is one usefulib:
+```python
+from usefulib import reverse_string
+
+a_string = "abcdef123456"
+reverse_string = reverse_string(a_string)
+```
 
 ## What can it do?
-usefulib is open-source and can be contributed to by anyone. Therefore, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all fuctions usefulib provides can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
+As an open-source library and can be contributed to by anyone, it offers a lot of simple functions to make writing code easier and quicker. A complete list of all usefulibs that are available can be found [here](https://github.com/hamdivazim/usefulib/blob/main/ALLFUNCTIONS.md).
+
+## Support usefulib
+usefulib is full of contributions from the community! We're beginner-friendly here, so read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and give us your best usefulibs 😃!
+
+## License
+usefulib is licensed under the [GNU General Public License v3.0](https://github.com/hamdivazim/usefulib/blob/main/LICENSE).
 
-## Can I contribute?
-Want to contribute? You rock! Before you do, make sure to read the [contributing guidelines](https://github.com/hamdivazim/usefulib/blob/main/CONTRIBUTING.md) and you should have your PR merged!
 """
 
 # Setting up
 setup(
     name="usefulib",
     version=VERSION,
-    author="Hamdi Vazim",
+    author="Hamd Waseem",
     author_email="<codingboy.cw@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'useful', 'usefulib', 'collection'],
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `usefulib-1.0.2/usefulib/_usefulibs.py` & `usefulib-1.0.3/usefulib/_usefulibs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
-usefulib v1.0.2
+usefulib v1.0.3
 Copyright Hamd Waseem (https://github.com/hamdivazim) under the GNU Public License 3.0.
 
 https://github.com/hamdivazim/usefulib
 
 Add your useful method here if you are contributing. Remember to add unit tests in tests.py :)
 """
 
 """ Setup - add any setup scripts here remembering to put the function(s) they are for. """
 
 import random # generate_random_string()
 import string # generate_random_string()
 import uuid # generateUUID()
 import os # external_verbose_output()
+import hashlib # get_hash()
 
 """"""
 
 def reverse_string(string):
     """ @hamdivazim - Reverses a string. """
 
     return string[::-1]
@@ -129,8 +130,18 @@
     """ @hamdivazim - if you are printing a lot of data, you can use this method to write the output to log file. """
 
     if not os.path.exists(path):
         open(path, "x").close()
 
     with open(path, "w") as f:
         f.write("# Logged by usefulibs.external_verbose_output()\n\n")
-        f.write(data)
+        f.write(data)
+
+def get_hash(string):
+    """
+    @MKM12345 + @hamdivazim - This function takes a string as input, hashes it using the SHA-256 algorithm, and returns the hexadecimal representation of the hash value. Useful for developers that one to store strings without actually having to store them.
+    """
+
+    if not isinstance(string, str):
+        raise TypeError("get_hash() cannot get the hash of a non-string.")
+
+    return hashlib.sha256(string.encode('utf-8')).hexdigest()
```

### Comparing `usefulib-1.0.2/usefulib/tests.py` & `usefulib-1.0.3/usefulib/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-usefulib v1.0.2
+usefulib v1.0.3
 Copyright Hamd Waseem (https://github.com/hamdivazim) under the GNU Public License 3.0.
 
 https://github.com/hamdivazim/usefulib
 
 
 This is where you should write unit tests for your useful method. If you can't do so for any reason, mention so in your PR so I can help.
 """
@@ -70,10 +70,14 @@
     def test_external_verbose_output(self):
         """ @hamdivazim """
         external_verbose_output("Test Data\n1 2 3\na b c", R"usefulib\temp_data\ext_verbose_test.log")
 
         with open(R"usefulib\temp_data\ext_verbose_test.log", "r") as f:
             self.assertEqual(f.read(), "# Logged by usefulibs.external_verbose_output()\n\nTest Data\n1 2 3\na b c")
 
+    def test_get_hash(self):
+        """ @MKM12345 + @hamdivazim """
+        self.assertEqual(get_hash("abc123"), get_hash("abc123"))
+        self.assertRaises(TypeError, get_hash, 1)
 
 if __name__ == "__main__":
-    unittest.main()
+    unittest.main()
```

