# Comparing `tmp/Flask-Liquid-1.1.0.tar.gz` & `tmp/flask_liquid-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Liquid-1.1.0.tar", last modified: Sat Nov  5 10:51:59 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `Flask-Liquid-1.1.0.tar` & `flask_liquid-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,8 @@
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/
--rw-r--r--   0 james     (1000) james     (1000)     1287 2022-11-05 10:45:09.000000 Flask-Liquid-1.1.0/CHANGES.rst
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)     3193 2022-11-05 10:51:59.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      473 2022-11-05 10:51:59.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/SOURCES.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2022-11-05 10:51:59.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/dependency_links.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2022-11-05 10:51:58.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/not-zip-safe
--rw-r--r--   0 james     (1000) james     (1000)       50 2022-11-05 10:51:59.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/requires.txt
--rw-r--r--   0 james     (1000) james     (1000)       13 2022-11-05 10:51:59.000000 Flask-Liquid-1.1.0/Flask_Liquid.egg-info/top_level.txt
--rw-r--r--   0 james     (1000) james     (1000)     1067 2021-02-23 16:47:38.000000 Flask-Liquid-1.1.0/LICENSE
--rw-r--r--   0 james     (1000) james     (1000)      119 2021-12-26 09:35:50.000000 Flask-Liquid-1.1.0/MANIFEST.in
--rw-r--r--   0 james     (1000) james     (1000)     3193 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      484 2022-11-05 08:26:57.000000 Flask-Liquid-1.1.0/Pipfile
--rw-r--r--   0 james     (1000) james     (1000)    58866 2022-11-05 08:27:18.000000 Flask-Liquid-1.1.0/Pipfile.lock
--rw-r--r--   0 james     (1000) james     (1000)     2109 2022-11-05 10:47:13.000000 Flask-Liquid-1.1.0/README.rst
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/flask_liquid/
--rw-r--r--   0 james     (1000) james     (1000)      442 2022-11-05 10:41:03.000000 Flask-Liquid-1.1.0/flask_liquid/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)    15222 2022-11-05 10:29:46.000000 Flask-Liquid-1.1.0/flask_liquid/flask_liquid.py
--rw-r--r--   0 james     (1000) james     (1000)        0 2021-12-25 11:24:57.000000 Flask-Liquid-1.1.0/flask_liquid/py.typed
--rw-r--r--   0 james     (1000) james     (1000)      100 2022-11-05 08:27:57.000000 Flask-Liquid-1.1.0/pyproject.toml
--rw-r--r--   0 james     (1000) james     (1000)     2026 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/setup.cfg
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/tests/
--rw-r--r--   0 james     (1000) james     (1000)        0 2021-02-24 17:05:05.000000 Flask-Liquid-1.1.0/tests/__init__.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2022-11-05 10:51:59.032039 Flask-Liquid-1.1.0/tests/templates/
--rw-r--r--   0 james     (1000) james     (1000)       15 2021-02-24 17:11:46.000000 Flask-Liquid-1.1.0/tests/templates/index.html
--rw-r--r--   0 james     (1000) james     (1000)       20 2021-12-25 11:55:27.000000 Flask-Liquid-1.1.0/tests/templates/snippet.html
--rw-r--r--   0 james     (1000) james     (1000)    14218 2022-11-05 08:32:23.000000 Flask-Liquid-1.1.0/tests/test_liquid.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/flask_liquid/__init__.py
+-rw-r--r--   0        0        0    15294 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/flask_liquid/flask_liquid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/flask_liquid/py.typed
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/README.md
+-rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 flask_liquid-1.2.0/PKG-INFO
```

### Comparing `Flask-Liquid-1.1.0/LICENSE` & `flask_liquid-1.2.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 James Prior
+Copyright (c) 2023 James Prior
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `Flask-Liquid-1.1.0/README.rst` & `flask_liquid-1.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,132 +1,173 @@
-00000000: 0a2e 2e20 5f4c 6971 7569 643a 2068 7474  ... _Liquid: htt
-00000010: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000020: 6a67 2d72 702f 6c69 7175 6964 0a2e 2e20  jg-rp/liquid... 
-00000030: 5f50 6970 656e 763a 2068 7474 7073 3a2f  _Pipenv: https:/
-00000040: 2f70 6970 656e 762e 7079 7061 2e69 6f2f  /pipenv.pypa.io/
-00000050: 656e 2f6c 6174 6573 742f 0a0a 466c 6173  en/latest/..Flas
-00000060: 6b2d 4c69 7175 6964 0a3d 3d3d 3d3d 3d3d  k-Liquid.=======
-00000070: 3d3d 3d3d 3d0a 0a41 2060 466c 6173 6b20  =====..A `Flask 
-00000080: 3c68 7474 7073 3a2f 2f70 616c 6c65 7473  <https://pallets
-00000090: 7072 6f6a 6563 7473 2e63 6f6d 2f70 2f66  projects.com/p/f
-000000a0: 6c61 736b 2f3e 605f 2065 7874 656e 7369  lask/>`_ extensi
-000000b0: 6f6e 2066 6f72 2060 4c69 7175 6964 605f  on for `Liquid`_
-000000c0: 2e20 5265 6e64 6572 204c 6971 7569 640a  . Render Liquid.
-000000d0: 7465 6d70 6c61 7465 7320 696e 2079 6f75  templates in you
-000000e0: 7220 466c 6173 6b20 6170 706c 6963 6174  r Flask applicat
-000000f0: 696f 6e73 2e0a 0a2e 2e20 696d 6167 653a  ions..... image:
-00000100: 3a20 6874 7470 733a 2f2f 696d 672e 7368  : https://img.sh
-00000110: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
-00000120: 666c 6173 6b2d 6c69 7175 6964 2e73 7667  flask-liquid.svg
-00000130: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
-00000140: 7265 0a20 2020 203a 7461 7267 6574 3a20  re.    :target: 
-00000150: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-00000160: 2f70 726f 6a65 6374 2f66 6c61 736b 2d6c  /project/flask-l
-00000170: 6971 7569 642f 0a20 2020 203a 616c 743a  iquid/.    :alt:
-00000180: 2056 6572 7369 6f6e 0a0a 2e2e 2069 6d61   Version.... ima
-00000190: 6765 3a3a 2068 7474 7073 3a2f 2f69 6d67  ge:: https://img
-000001a0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
-000001b0: 7562 2f77 6f72 6b66 6c6f 772f 7374 6174  ub/workflow/stat
-000001c0: 7573 2f6a 672d 7270 2f66 6c61 736b 2d6c  us/jg-rp/flask-l
-000001d0: 6971 7569 642f 5465 7374 732f 6d61 696e  iquid/Tests/main
-000001e0: 3f6c 6162 656c 3d74 6573 7473 2673 7479  ?label=tests&sty
-000001f0: 6c65 3d66 6c61 742d 7371 7561 7265 0a20  le=flat-square. 
-00000200: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-00000210: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
-00000220: 672d 7270 2f66 6c61 736b 2d6c 6971 7569  g-rp/flask-liqui
-00000230: 642f 7472 6565 2f6d 6169 6e2f 7465 7374  d/tree/main/test
-00000240: 730a 2020 2020 3a61 6c74 3a20 5465 7374  s.    :alt: Test
-00000250: 730a 0a2e 2e20 696d 6167 653a 3a20 6874  s.... image:: ht
-00000260: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000270: 732e 696f 2f70 7970 692f 6c2f 666c 6173  s.io/pypi/l/flas
-00000280: 6b2d 6c69 7175 6964 2e73 7667 3f73 7479  k-liquid.svg?sty
-00000290: 6c65 3d66 6c61 742d 7371 7561 7265 0a20  le=flat-square. 
-000002a0: 2020 203a 7461 7267 6574 3a20 6874 7470     :target: http
-000002b0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000002c0: 6a65 6374 2f66 6c61 736b 2d6c 6971 7569  ject/flask-liqui
-000002d0: 642f 0a20 2020 203a 616c 743a 204c 6963  d/.    :alt: Lic
-000002e0: 656e 6365 0a0a 2e2e 2069 6d61 6765 3a3a  ence.... image::
-000002f0: 2068 7474 7073 3a2f 2f69 6d67 2e73 6869   https://img.shi
-00000300: 656c 6473 2e69 6f2f 7079 7069 2f70 7976  elds.io/pypi/pyv
-00000310: 6572 7369 6f6e 732f 666c 6173 6b2d 6c69  ersions/flask-li
-00000320: 7175 6964 2e73 7667 3f73 7479 6c65 3d66  quid.svg?style=f
-00000330: 6c61 742d 7371 7561 7265 0a20 2020 203a  lat-square.    :
-00000340: 7461 7267 6574 3a20 6874 7470 733a 2f2f  target: https://
-00000350: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000360: 2f66 6c61 736b 2d6c 6971 7569 642f 0a20  /flask-liquid/. 
-00000370: 2020 203a 616c 743a 2050 7974 686f 6e20     :alt: Python 
-00000380: 7665 7273 696f 6e73 0a0a 2e2e 2069 6d61  versions.... ima
-00000390: 6765 3a3a 2068 7474 7073 3a2f 2f69 6d67  ge:: https://img
-000003a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000003b0: 652f 7079 7079 2d33 2e37 2532 3025 3743  e/pypy-3.7%20%7C
-000003c0: 2532 3033 2e38 2d62 6c75 653f 7374 796c  %203.8-blue?styl
-000003d0: 653d 666c 6174 2d73 7175 6172 650a 2020  e=flat-square.  
-000003e0: 2020 3a74 6172 6765 743a 2068 7474 7073    :target: https
-000003f0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00000400: 6563 742f 666c 6173 6b2d 6c69 7175 6964  ect/flask-liquid
-00000410: 2f0a 2020 2020 3a61 6c74 3a20 5079 5079  /.    :alt: PyPy
-00000420: 2076 6572 7369 6f6e 730a 0a49 6e73 7461   versions..Insta
-00000430: 6c6c 696e 670a 2d2d 2d2d 2d2d 2d2d 2d2d  lling.----------
-00000440: 0a0a 496e 7374 616c 6c20 466c 6173 6b20  ..Install Flask 
-00000450: 4c69 7175 6964 2075 7369 6e67 2060 5069  Liquid using `Pi
-00000460: 7065 6e76 605f 3a0a 0a2e 2e20 636f 6465  penv`_:.... code
-00000470: 2d62 6c6f 636b 3a3a 2074 6578 740a 0a20  -block:: text.. 
-00000480: 2020 2024 2070 6970 656e 7620 696e 7374     $ pipenv inst
-00000490: 616c 6c20 666c 6173 6b2d 6c69 7175 6964  all flask-liquid
-000004a0: 0a0a 4f72 2060 7069 7020 3c68 7474 7073  ..Or `pip <https
-000004b0: 3a2f 2f70 6970 2e70 7970 612e 696f 2f65  ://pip.pypa.io/e
-000004c0: 6e2f 7374 6162 6c65 2f67 6574 7469 6e67  n/stable/getting
-000004d0: 2d73 7461 7274 6564 2f3e 605f 3a0a 0a2e  -started/>`_:...
-000004e0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2074  . code-block:: t
-000004f0: 6578 740a 0a20 2020 2024 2070 7974 686f  ext..    $ pytho
-00000500: 6e20 2d6d 2070 6970 2069 6e73 7461 6c6c  n -m pip install
-00000510: 202d 5520 666c 6173 6b2d 6c69 7175 6964   -U flask-liquid
-00000520: 0a0a 4c69 6e6b 730a 2d2d 2d2d 2d0a 0a2d  ..Links.-----..-
-00000530: 2044 6f63 756d 656e 7461 7469 6f6e 3a20   Documentation: 
-00000540: 6874 7470 733a 2f2f 6a67 2d72 702e 6769  https://jg-rp.gi
-00000550: 7468 7562 2e69 6f2f 6c69 7175 6964 2f67  thub.io/liquid/g
-00000560: 7569 6465 732f 666c 6173 6b2d 6c69 7175  uides/flask-liqu
-00000570: 6964 0a2d 2043 6861 6e67 6520 4c6f 673a  id.- Change Log:
-00000580: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000590: 636f 6d2f 6a67 2d72 702f 466c 6173 6b2d  com/jg-rp/Flask-
-000005a0: 4c69 7175 6964 2f62 6c6f 622f 6d61 696e  Liquid/blob/main
-000005b0: 2f43 4841 4e47 4553 2e72 7374 0a2d 2050  /CHANGES.rst.- P
-000005c0: 7950 693a 2068 7474 7073 3a2f 2f70 7970  yPi: https://pyp
-000005d0: 692e 6f72 672f 7072 6f6a 6563 742f 466c  i.org/project/Fl
-000005e0: 6173 6b2d 4c69 7175 6964 2f0a 2d20 536f  ask-Liquid/.- So
-000005f0: 7572 6365 2043 6f64 653a 2068 7474 7073  urce Code: https
-00000600: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
-00000610: 2d72 702f 466c 6173 6b2d 4c69 7175 6964  -rp/Flask-Liquid
-00000620: 0a2d 2049 7373 7565 2054 7261 636b 6572  .- Issue Tracker
-00000630: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000640: 2e63 6f6d 2f6a 672d 7270 2f66 6c61 736b  .com/jg-rp/flask
-00000650: 2d4c 6971 7569 642f 6973 7375 6573 0a0a  -Liquid/issues..
-00000660: 436f 6e74 7269 6275 7469 6e67 0a2d 2d2d  Contributing.---
-00000670: 2d2d 2d2d 2d2d 2d2d 2d0a 0a2d 2049 6e73  ---------..- Ins
-00000680: 7461 6c6c 2064 6576 656c 6f70 6d65 6e74  tall development
-00000690: 2064 6570 656e 6465 6e63 6965 7320 7769   dependencies wi
-000006a0: 7468 2060 5069 7065 6e76 605f 0a0a 2d20  th `Pipenv`_..- 
-000006b0: 466c 6173 6b20 4c69 7175 6964 2075 7365  Flask Liquid use
-000006c0: 7320 7479 7065 2068 696e 7473 2061 6e64  s type hints and
-000006d0: 2073 7461 7469 6320 7479 7065 2063 6865   static type che
-000006e0: 636b 696e 672e 2052 756e 2060 606d 7970  cking. Run ``myp
-000006f0: 7960 6020 6f72 2020 0a20 2060 6074 6f78  y`` or  .  ``tox
-00000700: 202d 6520 7479 7069 6e67 6060 2074 6f20   -e typing`` to 
-00000710: 6368 6563 6b20 666f 7220 7479 7069 6e67  check for typing
-00000720: 2069 7373 7565 732e 0a0a 2d20 466f 726d   issues...- Form
-00000730: 6174 2063 6f64 6520 7573 696e 6720 6062  at code using `b
-00000740: 6c61 636b 203c 6874 7470 733a 2f2f 6769  lack <https://gi
-00000750: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-00000760: 636b 3e60 5f2e 0a0a 2d20 5772 6974 6520  ck>`_...- Write 
-00000770: 7465 7374 7320 7573 696e 6720 6060 756e  tests using ``un
-00000780: 6974 7465 7374 2e54 6573 7443 6173 6560  ittest.TestCase`
-00000790: 602e 0a0a 2d20 5275 6e20 7465 7374 7320  `...- Run tests 
-000007a0: 7769 7468 2060 606d 616b 6520 7465 7374  with ``make test
-000007b0: 6060 206f 7220 6060 7079 7468 6f6e 202d  `` or ``python -
-000007c0: 6d20 756e 6974 7465 7374 6060 206f 7220  m unittest`` or 
-000007d0: 6060 7079 7465 7374 6060 2e0a 0a2d 2043  ``pytest``...- C
-000007e0: 6865 636b 2074 6573 7420 636f 7665 7261  heck test covera
-000007f0: 6765 2077 6974 6820 6060 6d61 6b65 2063  ge with ``make c
-00000800: 6f76 6572 6167 6560 6020 616e 6420 6f70  overage`` and op
-00000810: 656e 2060 6068 746d 6c63 6f76 2f69 6e64  en ``htmlcov/ind
-00000820: 6578 2e68 746d 6c60 6020 696e 2079 6f75  ex.html`` in you
-00000830: 720a 2020 6272 6f77 7365 722e 0a         r.  browser..
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 466c 6173  : 2.1.Name: Flas
+00000020: 6b2d 4c69 7175 6964 0a56 6572 7369 6f6e  k-Liquid.Version
+00000030: 3a20 312e 322e 300a 5375 6d6d 6172 793a  : 1.2.0.Summary:
+00000040: 2041 2046 6c61 736b 2065 7874 656e 7369   A Flask extensi
+00000050: 6f6e 2066 6f72 2072 656e 6465 7269 6e67  on for rendering
+00000060: 204c 6971 7569 6420 7465 6d70 6c61 7465   Liquid template
+00000070: 732e 0a50 726f 6a65 6374 2d55 524c 3a20  s..Project-URL: 
+00000080: 4368 616e 6765 204c 6f67 2c20 6874 7470  Change Log, http
+00000090: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6a  s://github.com/j
+000000a0: 672d 7270 2f66 6c61 736b 2d6c 6971 7569  g-rp/flask-liqui
+000000b0: 642f 626c 6f62 2f6d 6169 6e2f 4348 414e  d/blob/main/CHAN
+000000c0: 4745 532e 6d64 0a50 726f 6a65 6374 2d55  GES.md.Project-U
+000000d0: 524c 3a20 446f 6375 6d65 6e74 6174 696f  RL: Documentatio
+000000e0: 6e2c 2068 7474 7073 3a2f 2f6a 672d 7270  n, https://jg-rp
+000000f0: 2e67 6974 6875 622e 696f 2f6c 6971 7569  .github.io/liqui
+00000100: 642f 6775 6964 6573 2f66 6c61 736b 2d6c  d/guides/flask-l
+00000110: 6971 7569 640a 5072 6f6a 6563 742d 5552  iquid.Project-UR
+00000120: 4c3a 2048 6f6d 6570 6167 652c 2068 7474  L: Homepage, htt
+00000130: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000140: 6a67 2d72 702f 666c 6173 6b2d 6c69 7175  jg-rp/flask-liqu
+00000150: 6964 0a50 726f 6a65 6374 2d55 524c 3a20  id.Project-URL: 
+00000160: 4973 7375 6520 5472 6163 6b65 722c 2068  Issue Tracker, h
+00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000180: 6d2f 6a67 2d72 702f 666c 6173 6b2d 6c69  m/jg-rp/flask-li
+00000190: 7175 6964 2f69 7373 7565 730a 5072 6f6a  quid/issues.Proj
+000001a0: 6563 742d 5552 4c3a 2053 6f75 7263 6520  ect-URL: Source 
+000001b0: 436f 6465 2c20 6874 7470 733a 2f2f 6769  Code, https://gi
+000001c0: 7468 7562 2e63 6f6d 2f6a 672d 7270 2f66  thub.com/jg-rp/f
+000001d0: 6c61 736b 2d6c 6971 7569 640a 4c69 6365  lask-liquid.Lice
+000001e0: 6e73 652d 4578 7072 6573 7369 6f6e 3a20  nse-Expression: 
+000001f0: 4d49 540a 4c69 6365 6e73 652d 4669 6c65  MIT.License-File
+00000200: 3a20 4c49 4345 4e53 450a 436c 6173 7369  : LICENSE.Classi
+00000210: 6669 6572 3a20 4465 7665 6c6f 706d 656e  fier: Developmen
+00000220: 7420 5374 6174 7573 203a 3a20 3520 2d20  t Status :: 5 - 
+00000230: 5072 6f64 7563 7469 6f6e 2f53 7461 626c  Production/Stabl
+00000240: 650a 436c 6173 7369 6669 6572 3a20 496e  e.Classifier: In
+00000250: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+00000260: 3a3a 2044 6576 656c 6f70 6572 730a 436c  :: Developers.Cl
+00000270: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+00000280: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+00000290: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000002a0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000002b0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002c0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000002d0: 0a43 6c61 7373 6966 6965 723a 2050 726f  .Classifier: Pro
+000002e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000002f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000300: 2e37 0a43 6c61 7373 6966 6965 723a 2050  .7.Classifier: P
+00000310: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000320: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000330: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
+00000340: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000350: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000360: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
+00000370: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00000380: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00000390: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
+000003a0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
+000003b0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000003c0: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
+000003d0: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+000003e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000003f0: 2050 7974 686f 6e20 3a3a 2049 6d70 6c65   Python :: Imple
+00000400: 6d65 6e74 6174 696f 6e20 3a3a 2043 5079  mentation :: CPy
+00000410: 7468 6f6e 0a52 6571 7569 7265 732d 5079  thon.Requires-Py
+00000420: 7468 6f6e 3a20 3e3d 332e 370a 5265 7175  thon: >=3.7.Requ
+00000430: 6972 6573 2d44 6973 743a 2066 6c61 736b  ires-Dist: flask
+00000440: 3e3d 322e 300a 5265 7175 6972 6573 2d44  >=2.0.Requires-D
+00000450: 6973 743a 206d 6172 6b75 7073 6166 653e  ist: markupsafe>
+00000460: 3d32 2e30 2e30 0a52 6571 7569 7265 732d  =2.0.0.Requires-
+00000470: 4469 7374 3a20 7079 7468 6f6e 2d6c 6971  Dist: python-liq
+00000480: 7569 643e 3d31 2e31 2e30 0a44 6573 6372  uid>=1.1.0.Descr
+00000490: 6970 7469 6f6e 2d43 6f6e 7465 6e74 2d54  iption-Content-T
+000004a0: 7970 653a 2074 6578 742f 6d61 726b 646f  ype: text/markdo
+000004b0: 776e 0a0a 3c68 3120 616c 6967 6e3d 2263  wn..<h1 align="c
+000004c0: 656e 7465 7222 3e46 6c61 736b 204c 6971  enter">Flask Liq
+000004d0: 7569 643c 2f68 313e 0a0a 3c70 2061 6c69  uid</h1>..<p ali
+000004e0: 676e 3d22 6365 6e74 6572 223e 0a41 203c  gn="center">.A <
+000004f0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000500: 7061 6c6c 6574 7370 726f 6a65 6374 732e  palletsprojects.
+00000510: 636f 6d2f 702f 666c 6173 6b2f 223e 466c  com/p/flask/">Fl
+00000520: 6173 6b3c 2f61 3e20 6578 7465 6e73 696f  ask</a> extensio
+00000530: 6e20 666f 7220 3c61 2068 7265 663d 2268  n for <a href="h
+00000540: 7474 7073 3a2f 2f6a 672d 7270 2e67 6974  ttps://jg-rp.git
+00000550: 6875 622e 696f 2f6c 6971 7569 642f 223e  hub.io/liquid/">
+00000560: 4c69 7175 6964 3c2f 613e 2e20 5265 6e64  Liquid</a>. Rend
+00000570: 6572 204c 6971 7569 6420 7465 6d70 6c61  er Liquid templa
+00000580: 7465 7320 696e 2079 6f75 7220 466c 6173  tes in your Flas
+00000590: 6b20 6170 706c 6963 6174 696f 6e73 2e0a  k applications..
+000005a0: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d22  </p>..<p align="
+000005b0: 6365 6e74 6572 223e 0a20 203c 6120 6872  center">.  <a hr
+000005c0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+000005d0: 7562 2e63 6f6d 2f6a 672d 7270 2f66 6c61  ub.com/jg-rp/fla
+000005e0: 736b 2d6c 6971 7569 642f 626c 6f62 2f6d  sk-liquid/blob/m
+000005f0: 6169 6e2f 4c49 4345 4e53 4522 3e0a 2020  ain/LICENSE">.  
+00000600: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+00000610: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000620: 696f 2f70 7970 692f 6c2f 666c 6173 6b2d  io/pypi/l/flask-
+00000630: 6c69 7175 6964 2e73 7667 3f73 7479 6c65  liquid.svg?style
+00000640: 3d66 6c61 742d 7371 7561 7265 2220 616c  =flat-square" al
+00000650: 743d 224c 6963 656e 7365 223e 0a20 203c  t="License">.  <
+00000660: 2f61 3e0a 2020 3c61 2068 7265 663d 2268  /a>.  <a href="h
+00000670: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000680: 6d2f 6a67 2d72 702f 6c69 7175 6964 2f61  m/jg-rp/liquid/a
+00000690: 6374 696f 6e73 2f77 6f72 6b66 6c6f 7773  ctions/workflows
+000006a0: 2f74 6573 7473 2e79 616d 6c22 3e0a 2020  /tests.yaml">.  
+000006b0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
+000006c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000006d0: 696f 2f67 6974 6875 622f 6163 7469 6f6e  io/github/action
+000006e0: 732f 776f 726b 666c 6f77 2f73 7461 7475  s/workflow/statu
+000006f0: 732f 6a67 2d72 702f 6c69 7175 6964 2f74  s/jg-rp/liquid/t
+00000700: 6573 7473 2e79 616d 6c3f 6272 616e 6368  ests.yaml?branch
+00000710: 3d6d 6169 6e26 6c61 6265 6c3d 7465 7374  =main&label=test
+00000720: 7326 7374 796c 653d 666c 6174 2d73 7175  s&style=flat-squ
+00000730: 6172 6522 2061 6c74 3d22 5465 7374 7322  are" alt="Tests"
+00000740: 3e0a 2020 3c2f 613e 0a20 203c 6272 3e0a  >.  </a>.  <br>.
+00000750: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+00000760: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000770: 6563 742f 666c 6173 6b2d 6c69 7175 6964  ect/flask-liquid
+00000780: 2f22 3e0a 2020 2020 3c69 6d67 2073 7263  /">.    <img src
+00000790: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+000007a0: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+000007b0: 666c 6173 6b2d 6c69 7175 6964 2e73 7667  flask-liquid.svg
+000007c0: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+000007d0: 7265 2220 616c 743d 2250 7950 6920 2d20  re" alt="PyPi - 
+000007e0: 5665 7273 696f 6e22 3e0a 2020 3c2f 613e  Version">.  </a>
+000007f0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
+00000800: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000810: 6a65 6374 2f66 6c61 736b 2d6c 6971 7569  ject/flask-liqui
+00000820: 642f 223e 0a20 2020 203c 696d 6720 7372  d/">.    <img sr
+00000830: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000840: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
+00000850: 7976 6572 7369 6f6e 732f 666c 6173 6b2d  yversions/flask-
+00000860: 6c69 7175 6964 2e73 7667 3f73 7479 6c65  liquid.svg?style
+00000870: 3d66 6c61 742d 7371 7561 7265 2220 616c  =flat-square" al
+00000880: 743d 2250 7974 686f 6e20 7665 7273 696f  t="Python versio
+00000890: 6e73 223e 0a20 203c 2f61 3e0a 3c2f 703e  ns">.  </a>.</p>
+000008a0: 0a0a 2d2d 2d0a 0a23 2320 496e 7374 616c  ..---..## Instal
+000008b0: 6c0a 0a49 6e73 7461 6c6c 2046 6c61 736b  l..Install Flask
+000008c0: 204c 6971 7569 6420 7573 696e 6720 5b70   Liquid using [p
+000008d0: 6970 5d28 6874 7470 733a 2f2f 7069 702e  ip](https://pip.
+000008e0: 7079 7061 2e69 6f2f 656e 2f73 7461 626c  pypa.io/en/stabl
+000008f0: 652f 6765 7474 696e 672d 7374 6172 7465  e/getting-starte
+00000900: 642f 293a 0a0a 6060 6063 6f6e 736f 6c65  d/):..```console
+00000910: 0a70 6970 2069 6e73 7461 6c6c 2066 6c61  .pip install fla
+00000920: 736b 2d6c 6971 7569 640a 6060 600a 0a4f  sk-liquid.```..O
+00000930: 7220 5b50 6970 656e 765d 2868 7474 7073  r [Pipenv](https
+00000940: 3a2f 2f70 6970 656e 762e 7079 7061 2e69  ://pipenv.pypa.i
+00000950: 6f2f 656e 2f6c 6174 6573 742f 293a 0a0a  o/en/latest/):..
+00000960: 6060 6063 6f6e 736f 6c65 0a70 6970 656e  ```console.pipen
+00000970: 7620 696e 7374 616c 6c20 2d75 2066 6c61  v install -u fla
+00000980: 736b 2d6c 6971 7569 640a 6060 600a 0a23  sk-liquid.```..#
+00000990: 2320 4c69 6e6b 730a 0a2d 2044 6f63 756d  # Links..- Docum
+000009a0: 656e 7461 7469 6f6e 3a20 6874 7470 733a  entation: https:
+000009b0: 2f2f 6a67 2d72 702e 6769 7468 7562 2e69  //jg-rp.github.i
+000009c0: 6f2f 6c69 7175 6964 2f67 7569 6465 732f  o/liquid/guides/
+000009d0: 666c 6173 6b2d 6c69 7175 6964 0a2d 2043  flask-liquid.- C
+000009e0: 6861 6e67 6520 4c6f 673a 2068 7474 7073  hange Log: https
+000009f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+00000a00: 2d72 702f 666c 6173 6b2d 6c69 7175 6964  -rp/flask-liquid
+00000a10: 2f62 6c6f 622f 6d61 696e 2f43 4841 4e47  /blob/main/CHANG
+00000a20: 4553 2e6d 640a 2d20 5079 5069 3a20 6874  ES.md.- PyPi: ht
+00000a30: 7470 733a 2f2f 7079 7069 2e6f 7267 2f70  tps://pypi.org/p
+00000a40: 726f 6a65 6374 2f66 6c61 736b 2d6c 6971  roject/flask-liq
+00000a50: 7569 642f 0a2d 2053 6f75 7263 6520 436f  uid/.- Source Co
+00000a60: 6465 3a20 6874 7470 733a 2f2f 6769 7468  de: https://gith
+00000a70: 7562 2e63 6f6d 2f6a 672d 7270 2f66 6c61  ub.com/jg-rp/fla
+00000a80: 736b 2d6c 6971 7569 640a 2d20 4973 7375  sk-liquid.- Issu
+00000a90: 6520 5472 6163 6b65 723a 2068 7474 7073  e Tracker: https
+00000aa0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6a67  ://github.com/jg
+00000ab0: 2d72 702f 666c 6173 6b2d 6c69 7175 6964  -rp/flask-liquid
+00000ac0: 2f69 7373 7565 730a                      /issues.
```

### Comparing `Flask-Liquid-1.1.0/flask_liquid/flask_liquid.py` & `flask_liquid-1.2.0/flask_liquid/flask_liquid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Add Liquid templates to a Flask application."""
 from __future__ import annotations
 
+import warnings
 from contextlib import contextmanager
 from itertools import chain
-
+from typing import TYPE_CHECKING
 from typing import Any
 from typing import Callable
-from typing import cast
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import Mapping
 from typing import Optional
 from typing import Type
+from typing import cast
 
 from flask import Flask
+from flask import before_render_template
 from flask import current_app
-from flask import signals_available
 from flask import template_rendered
-from flask import before_render_template
 from flask.ctx import RequestContext
 
+with warnings.catch_warnings():
+    warnings.simplefilter("ignore", category=DeprecationWarning)
+    try:
+        from flask import signals_available
+    except ImportError:
+        signals_available = True
+
 try:
     from flask.globals import request_ctx
 
     def _request_ctx() -> RequestContext:
         return request_ctx
 
 except ImportError:
@@ -33,20 +40,19 @@
     def _request_ctx() -> RequestContext:
         return cast(RequestContext, _request_ctx_stack.top)
 
 
 from liquid import Environment
 from liquid import Mode
 from liquid import Undefined
-
-from liquid.template import BoundTemplate
-
 from liquid.loaders import BaseLoader
 from liquid.loaders import FileSystemLoader
 
+if TYPE_CHECKING:
+    from liquid.template import BoundTemplate
 
 TemplateContextProcessorCallable = Callable[[], Dict[str, Any]]
 
 
 class Liquid:
     """The Liquid template extension for Flask.
 
@@ -112,15 +118,14 @@
     :type globals: dict
     :param flask_context_processors: If set to `True` Flask context processors
         will be applied to Liquid every render context. Defaults to `False`.
     :param flask_signals: If set to `True` the `template_rendered` and
         `before_template_rendered` signals will be emitted for Liquid templates.
     """
 
-    # pylint: disable=redefined-builtin too-many-arguments too-many-locals
     def __init__(
         self,
         app: Optional[Flask] = None,
         *,
         tag_start_string: str = r"{%",
         tag_end_string: str = r"%}",
         statement_start_string: str = r"{{",
@@ -130,15 +135,15 @@
         comment_end_string: str = "#}",
         tolerance: Mode = Mode.STRICT,
         loader: Optional[BaseLoader] = None,
         undefined: Type[Undefined] = Undefined,
         strict_filters: bool = True,
         autoescape: bool = True,
         auto_reload: bool = True,
-        globals: Optional[Mapping[str, object]] = None,
+        globals: Optional[Mapping[str, object]] = None,  # noqa: A002
         flask_context_processors: bool = False,
         flask_signals: bool = True,
         cache_size: int = 300,
         expression_cache_size: int = 0,
     ):
         self.app = app
 
@@ -259,15 +264,16 @@
         if not self.env.template_comments:
             self.env.comment_start_string = ""
             self.env.comment_end_string = ""
 
         self.env.set_expression_cache_size(app.config["LIQUID_EXPRESSION_CACHE_SIZE"])
 
         # Just in case init_app is called late and templates have already been loaded.
-        self.env.cache.clear()
+        if self.env.cache:
+            self.env.cache.clear()
 
         app.extensions["flask_liquid"] = self
         self.app = app
 
     def _make_context(self, context: Dict[str, object]) -> Dict[str, object]:
         """Add the result of Flask context processors to the given context."""
         # NOTE: We're not using `app.update_template_context` because we don't want
@@ -311,47 +317,39 @@
 
     def render_template(self, template_name: str, **context: object) -> str:
         """Render a Liquid template from the configured template loader."""
         context = self._make_context(context)
         template = self.env.get_template(template_name)
 
         with self._signals(template, context):
-            rendered = template.render(**context)
-
-        return rendered
+            return template.render(**context)
 
     async def render_template_async(self, template_name: str, **context: object) -> str:
         """Render a Liquid template from the configured template loader."""
         context = self._make_context(context)
         template = await self.env.get_template_async(template_name)
 
         with self._signals(template, context):
-            rendered = await template.render_async(**context)
-
-        return rendered
+            return await template.render_async(**context)
 
     def render_template_string(self, source: str, **context: object) -> str:
         """Render a Liquid template from a template string."""
         context = self._make_context(context)
         template = self.env.from_string(source)
 
         with self._signals(template, context):
-            rendered = template.render(**context)
-
-        return rendered
+            return template.render(**context)
 
     async def render_template_string_async(self, source: str, **context: object) -> str:
         """Render a Liquid template from a template string."""
         context = self._make_context(context)
         template = self.env.from_string(source)
 
         with self._signals(template, context):
-            rendered = await template.render_async(**context)
-
-        return rendered
+            return await template.render_async(**context)
 
 
 def render_template(template_name: str, **context: object) -> str:
     """Render a Liquid template in the current Flask application context."""
     ext: Liquid = current_app.extensions["flask_liquid"]
     return ext.render_template(template_name, **context)
 
@@ -359,18 +357,16 @@
 async def render_template_async(template_name: str, **context: object) -> str:
     """Render a Liquid template in the current Flask application context."""
     ext: Liquid = current_app.extensions["flask_liquid"]
     return await ext.render_template_async(template_name, **context)
 
 
 def render_template_string(source: str, **context: object) -> str:
-    """Render a Liquid template from a string in the current Flask application
-    context."""
+    """Render a template from a string in the current Flask application context."""
     ext: Liquid = current_app.extensions["flask_liquid"]
     return ext.render_template_string(source, **context)
 
 
 async def render_template_string_async(source: str, **context: object) -> str:
-    """Render a Liquid template from a string in the current Flask application
-    context."""
+    """Render a template from a string in the current Flask application context."""
     ext: Liquid = current_app.extensions["flask_liquid"]
     return await ext.render_template_string_async(source, **context)
```

