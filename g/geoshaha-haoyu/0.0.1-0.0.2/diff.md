# Comparing `tmp/geoshaha-haoyu-0.0.1.tar.gz` & `tmp/geoshaha-haoyu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoshaha-haoyu-0.0.1.tar", last modified: Tue Apr 25 21:36:49 2023, max compression
+gzip compressed data, was "geoshaha-haoyu-0.0.2.tar", last modified: Wed Apr 26 18:03:33 2023, max compression
```

## Comparing `geoshaha-haoyu-0.0.1.tar` & `geoshaha-haoyu-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:49.799323 geoshaha-haoyu-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1271 2023-04-25 21:36:49.799323 geoshaha-haoyu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      480 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:49.791803 geoshaha-haoyu-0.0.1/geoshaha_haoyu/
--rw-rw-rw-   0        0        0      129 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu/__init__.py
--rw-rw-rw-   0        0        0      194 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu/common.py
--rw-rw-rw-   0        0        0       20 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu/geoshaha_haoyu.py
-drwxrwxrwx   0        0        0        0 2023-04-25 21:36:49.798321 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/
--rw-rw-rw-   0        0        0     1271 2023-04-25 21:36:49.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-25 21:36:49.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 21:36:49.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-25 21:36:49.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       15 2023-04-25 21:36:49.000000 geoshaha-haoyu-0.0.1/geoshaha_haoyu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0      422 2023-04-25 21:36:49.800319 geoshaha-haoyu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1820 2023-04-25 21:33:17.000000 geoshaha-haoyu-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:03:33.920383 geoshaha-haoyu-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-26 18:03:33.924383 geoshaha-haoyu-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:03:33.920383 geoshaha-haoyu-0.0.2/geoshaha_haoyu/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu/geoshaha_haoyu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:03:33.920383 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-26 18:03:33.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-26 18:03:33.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:03:33.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:03:33.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 18:03:33.000000 geoshaha-haoyu-0.0.2/geoshaha_haoyu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-04-26 18:03:33.924383 geoshaha-haoyu-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-26 18:03:16.000000 geoshaha-haoyu-0.0.2/setup.py
```

### Comparing `geoshaha-haoyu-0.0.1/LICENSE` & `geoshaha-haoyu-0.0.2/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-MIT License
-
-Copyright (c) 2023, Haoyu Niu
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+MIT License
+
+Copyright (c) 2023, Haoyu Niu
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

### Comparing `geoshaha-haoyu-0.0.1/setup.py` & `geoshaha-haoyu-0.0.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-#!/usr/bin/env python
-
-"""The setup script."""
-
-import io
-from os import path as op
-from setuptools import setup, find_packages
-
-with open('README.md') as readme_file:
-    readme = readme_file.read()
-
-here = op.abspath(op.dirname(__file__))
-
-# get the dependencies and installs
-with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
-    all_reqs = f.read().split("\n")
-
-install_requires = [x.strip() for x in all_reqs if "git+" not in x]
-dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
-
-requirements = [ ]
-
-setup_requirements = [ ]
-
-test_requirements = [ ]
-
-setup(
-    author="Haoyu Niu",
-    author_email='hniu@tamu.edu',
-    python_requires='>=3.8',
-    classifiers=[
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: MIT License',
-        'Natural Language :: English',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: 3.11',
-    ],
-    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
-    install_requires=install_requires,
-    dependency_links=dependency_links,
-    license="MIT license",
-    long_description=readme,
-    long_description_content_type='text/markdown',
-    include_package_data=True,
-    keywords='geoshaha_haoyu',
-    name='geoshaha-haoyu',
-    packages=find_packages(include=['geoshaha_haoyu', 'geoshaha_haoyu.*']),
-    setup_requires=setup_requirements,
-    test_suite='tests',
-    tests_require=test_requirements,
-    url='https://github.com/hniu-tamu/geoshaha-haoyu',
-    version='0.0.1',
-    zip_safe=False,
-)
+#!/usr/bin/env python
+
+"""The setup script."""
+
+import io
+from os import path as op
+from setuptools import setup, find_packages
+
+with open('README.md') as readme_file:
+    readme = readme_file.read()
+
+here = op.abspath(op.dirname(__file__))
+
+# get the dependencies and installs
+with io.open(op.join(here, "requirements.txt"), encoding="utf-8") as f:
+    all_reqs = f.read().split("\n")
+
+install_requires = [x.strip() for x in all_reqs if "git+" not in x]
+dependency_links = [x.strip().replace("git+", "") for x in all_reqs if "git+" not in x]
+
+requirements = [ ]
+
+setup_requirements = [ ]
+
+test_requirements = [ ]
+
+setup(
+    author="Haoyu Niu",
+    author_email='hniu@tamu.edu',
+    python_requires='>=3.8',
+    classifiers=[
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: English',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+    ],
+    description="Python Boilerplate contains all the boilerplate you need to create a Python package.",
+    install_requires=install_requires,
+    dependency_links=dependency_links,
+    license="MIT license",
+    long_description=readme,
+    long_description_content_type='text/markdown',
+    include_package_data=True,
+    keywords='geoshaha_haoyu',
+    name='geoshaha-haoyu',
+    packages=find_packages(include=['geoshaha_haoyu', 'geoshaha_haoyu.*']),
+    setup_requires=setup_requirements,
+    test_suite='tests',
+    tests_require=test_requirements,
+    url='https://github.com/hniu-tamu/geoshaha-haoyu',
+    version='0.0.2',
+    zip_safe=False,
+)
```

