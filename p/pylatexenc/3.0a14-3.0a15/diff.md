# Comparing `tmp/pylatexenc-3.0a14.tar.gz` & `tmp/pylatexenc-3.0a15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylatexenc-3.0a14.tar", max compression
+gzip compressed data, was "pylatexenc-3.0a15.tar", max compression
```

## Comparing `pylatexenc-3.0a14.tar` & `pylatexenc-3.0a15.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0     1086 2023-04-15 20:22:30.680495 pylatexenc-3.0a14/LICENSE.txt
--rw-r--r--   0        0        0     2830 2023-04-15 20:22:30.680495 pylatexenc-3.0a14/README.rst
--rw-r--r--   0        0        0     1326 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/__init__.py
--rw-r--r--   0        0        0     5162 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/_util.py
--rw-r--r--   0        0        0     3766 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/_util_support.py
--rw-r--r--   0        0        0    59269 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/__init__.py
--rw-r--r--   0        0        0    10011 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/__main__.py
--rw-r--r--   0        0        0    94342 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/_defaultspecs.py
--rw-r--r--   0        0        0     2526 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latex2text/_inputlatexfile.py
--rw-r--r--   0        0        0    12944 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/__init__.py
--rw-r--r--   0        0        0     4426 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/__main__.py
--rw-r--r--   0        0        0     4404 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_partial_latex_encoder.py
--rw-r--r--   0        0        0    99833 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap.py
--rw-r--r--   0        0        0    55947 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap_xml.py
--rw-r--r--   0        0        0    26209 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexencode/_unicode_to_latex_encoder.py
--rw-r--r--   0        0        0     2179 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/__init__.py
--rw-r--r--   0        0        0     2197 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_callablespecbase.py
--rw-r--r--   0        0        0    11001 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_exctypes.py
--rw-r--r--   0        0        0     6315 2023-04-15 20:22:30.684495 pylatexenc-3.0a14/pylatexenc/latexnodes/_latexcontextdbbase.py
--rw-r--r--   0        0        0    36489 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_nodescollector.py
--rw-r--r--   0        0        0    10124 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargs.py
--rw-r--r--   0        0        0    11877 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargsinfo.py
--rw-r--r--   0        0        0    17020 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstate.py
--rw-r--r--   0        0        0     7109 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstatedelta.py
--rw-r--r--   0        0        0     8446 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_token.py
--rw-r--r--   0        0        0    27434 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreader.py
--rw-r--r--   0        0        0    10098 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreaderbase.py
--rw-r--r--   0        0        0     4841 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/_walkerbase.py
--rw-r--r--   0        0        0    42174 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/nodes.py
--rw-r--r--   0        0        0     2141 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/__init__.py
--rw-r--r--   0        0        0     5285 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_base.py
--rw-r--r--   0        0        0    41024 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_delimited.py
--rw-r--r--   0        0        0    18288 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_expression.py
--rw-r--r--   0        0        0    12896 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_generalnodes.py
--rw-r--r--   0        0        0     5658 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_math.py
--rw-r--r--   0        0        0     6180 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_optionals.py
--rw-r--r--   0        0        0    22370 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_stdarg.py
--rw-r--r--   0        0        0    11301 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_verbatim.py
--rw-r--r--   0        0        0     4520 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/__init__.py
--rw-r--r--   0        0        0     6214 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/__main__.py
--rw-r--r--   0        0        0    17383 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_defaultspecs.py
--rw-r--r--   0        0        0     2937 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_get_defaultspecs.py
--rw-r--r--   0        0        0     7833 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_helpers.py
--rw-r--r--   0        0        0     7487 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_legacy_py1x.py
--rw-r--r--   0        0        0    52642 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/latexwalker/_walker.py
--rw-r--r--   0        0        0     2341 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/__init__.py
--rw-r--r--   0        0        0     8525 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_argumentsparser.py
--rw-r--r--   0        0        0     7372 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_environmentbodyparser.py
--rw-r--r--   0        0        0    29706 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_latexcontextdb.py
--rw-r--r--   0        0        0    10045 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_macrocallparser.py
--rw-r--r--   0        0        0     1535 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
--rw-r--r--   0        0        0     8866 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
--rw-r--r--   0        0        0    16110 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
--rw-r--r--   0        0        0    15650 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_specclasses.py
--rw-r--r--   0        0        0     8951 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/macrospec/_spechelpers.py
--rw-r--r--   0        0        0     2115 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pylatexenc/version.py
--rw-r--r--   0        0        0     1091 2023-04-15 20:22:30.688495 pylatexenc-3.0a14/pyproject.toml
--rw-r--r--   0        0        0     3984 1970-01-01 00:00:00.000000 pylatexenc-3.0a14/setup.py
--rw-r--r--   0        0        0     3416 1970-01-01 00:00:00.000000 pylatexenc-3.0a14/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-04-15 13:24:30.143033 pylatexenc-3.0a15/LICENSE.txt
+-rw-r--r--   0        0        0     3572 2023-04-18 07:57:57.261013 pylatexenc-3.0a15/README.rst
+-rw-r--r--   0        0        0     1326 2019-07-25 20:20:56.000000 pylatexenc-3.0a15/pylatexenc/__init__.py
+-rw-r--r--   0        0        0     5162 2023-04-15 11:29:53.841130 pylatexenc-3.0a15/pylatexenc/_util.py
+-rw-r--r--   0        0        0     3766 2023-04-15 11:29:53.841423 pylatexenc-3.0a15/pylatexenc/_util_support.py
+-rw-r--r--   0        0        0    59269 2023-04-15 11:57:13.282343 pylatexenc-3.0a15/pylatexenc/latex2text/__init__.py
+-rw-r--r--   0        0        0    10011 2023-04-15 11:55:00.471421 pylatexenc-3.0a15/pylatexenc/latex2text/__main__.py
+-rw-r--r--   0        0        0    94342 2023-04-15 11:29:53.843500 pylatexenc-3.0a15/pylatexenc/latex2text/_defaultspecs.py
+-rw-r--r--   0        0        0     2526 2021-12-17 19:22:56.000000 pylatexenc-3.0a15/pylatexenc/latex2text/_inputlatexfile.py
+-rw-r--r--   0        0        0    12944 2021-03-31 23:28:40.000000 pylatexenc-3.0a15/pylatexenc/latexencode/__init__.py
+-rw-r--r--   0        0        0     4426 2019-08-25 13:06:29.000000 pylatexenc-3.0a15/pylatexenc/latexencode/__main__.py
+-rw-r--r--   0        0        0     4404 2023-04-15 12:03:11.103995 pylatexenc-3.0a15/pylatexenc/latexencode/_partial_latex_encoder.py
+-rw-r--r--   0        0        0    99833 2021-09-15 19:08:59.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap.py
+-rw-r--r--   0        0        0    55947 2019-07-27 15:08:32.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap_xml.py
+-rw-r--r--   0        0        0    26209 2021-04-01 11:51:30.000000 pylatexenc-3.0a15/pylatexenc/latexencode/_unicode_to_latex_encoder.py
+-rw-r--r--   0        0        0     2179 2023-04-15 11:29:53.843788 pylatexenc-3.0a15/pylatexenc/latexnodes/__init__.py
+-rw-r--r--   0        0        0     2197 2023-04-15 17:44:53.955715 pylatexenc-3.0a15/pylatexenc/latexnodes/_callablespecbase.py
+-rw-r--r--   0        0        0    11001 2023-04-15 17:53:09.732071 pylatexenc-3.0a15/pylatexenc/latexnodes/_exctypes.py
+-rw-r--r--   0        0        0     6315 2023-04-15 17:52:07.518222 pylatexenc-3.0a15/pylatexenc/latexnodes/_latexcontextdbbase.py
+-rw-r--r--   0        0        0    36489 2023-04-15 19:46:24.921466 pylatexenc-3.0a15/pylatexenc/latexnodes/_nodescollector.py
+-rw-r--r--   0        0        0    10124 2023-04-15 11:29:53.845301 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargs.py
+-rw-r--r--   0        0        0    11877 2023-04-15 11:29:53.845584 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargsinfo.py
+-rw-r--r--   0        0        0    17020 2023-04-15 17:51:09.423753 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstate.py
+-rw-r--r--   0        0        0     7109 2023-04-15 11:29:53.846228 pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstatedelta.py
+-rw-r--r--   0        0        0     8446 2023-04-15 17:12:48.503604 pylatexenc-3.0a15/pylatexenc/latexnodes/_token.py
+-rw-r--r--   0        0        0    27524 2023-04-26 15:32:16.345591 pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreader.py
+-rw-r--r--   0        0        0    10098 2023-04-15 17:13:31.159345 pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreaderbase.py
+-rw-r--r--   0        0        0     4841 2023-04-15 17:50:19.637390 pylatexenc-3.0a15/pylatexenc/latexnodes/_walkerbase.py
+-rw-r--r--   0        0        0    42174 2023-04-15 16:56:19.119357 pylatexenc-3.0a15/pylatexenc/latexnodes/nodes.py
+-rw-r--r--   0        0        0     2141 2023-04-15 11:29:53.848262 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/__init__.py
+-rw-r--r--   0        0        0     5285 2023-04-15 11:29:53.848639 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_base.py
+-rw-r--r--   0        0        0    41024 2023-04-15 16:46:03.019064 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_delimited.py
+-rw-r--r--   0        0        0    18288 2023-04-15 11:29:53.849524 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_expression.py
+-rw-r--r--   0        0        0    12896 2023-04-15 11:29:53.849773 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_generalnodes.py
+-rw-r--r--   0        0        0     5658 2023-04-15 11:29:53.849985 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_math.py
+-rw-r--r--   0        0        0     6180 2023-04-15 11:29:53.850252 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_optionals.py
+-rw-r--r--   0        0        0    22370 2023-04-15 16:46:34.476752 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_stdarg.py
+-rw-r--r--   0        0        0    11551 2023-04-18 07:57:57.274724 pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_verbatim.py
+-rw-r--r--   0        0        0     4520 2023-04-15 11:29:53.851132 pylatexenc-3.0a15/pylatexenc/latexwalker/__init__.py
+-rw-r--r--   0        0        0     6214 2023-04-15 11:29:53.851406 pylatexenc-3.0a15/pylatexenc/latexwalker/__main__.py
+-rw-r--r--   0        0        0    17597 2023-04-26 15:29:33.456920 pylatexenc-3.0a15/pylatexenc/latexwalker/_defaultspecs.py
+-rw-r--r--   0        0        0     2937 2023-04-15 11:29:53.852111 pylatexenc-3.0a15/pylatexenc/latexwalker/_get_defaultspecs.py
+-rw-r--r--   0        0        0     7833 2023-04-15 11:29:53.852354 pylatexenc-3.0a15/pylatexenc/latexwalker/_helpers.py
+-rw-r--r--   0        0        0     7487 2023-04-15 11:29:53.852626 pylatexenc-3.0a15/pylatexenc/latexwalker/_legacy_py1x.py
+-rw-r--r--   0        0        0    52642 2023-04-15 11:37:07.707893 pylatexenc-3.0a15/pylatexenc/latexwalker/_walker.py
+-rw-r--r--   0        0        0     2414 2023-04-18 07:57:57.275029 pylatexenc-3.0a15/pylatexenc/macrospec/__init__.py
+-rw-r--r--   0        0        0     8819 2023-04-18 07:57:57.275339 pylatexenc-3.0a15/pylatexenc/macrospec/_argumentsparser.py
+-rw-r--r--   0        0        0     7372 2023-04-15 11:29:53.853904 pylatexenc-3.0a15/pylatexenc/macrospec/_environmentbodyparser.py
+-rw-r--r--   0        0        0    29706 2023-04-15 11:29:53.854223 pylatexenc-3.0a15/pylatexenc/macrospec/_latexcontextdb.py
+-rw-r--r--   0        0        0    10046 2023-04-15 20:38:58.126785 pylatexenc-3.0a15/pylatexenc/macrospec/_macrocallparser.py
+-rw-r--r--   0        0        0     1535 2023-04-15 11:29:53.854841 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py
+-rw-r--r--   0        0        0     9488 2023-04-18 07:57:57.275664 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py
+-rw-r--r--   0        0        0    16735 2023-04-18 07:57:57.276084 pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py
+-rw-r--r--   0        0        0    15650 2023-04-15 11:29:53.855594 pylatexenc-3.0a15/pylatexenc/macrospec/_specclasses.py
+-rw-r--r--   0        0        0     8951 2023-04-15 11:29:53.855874 pylatexenc-3.0a15/pylatexenc/macrospec/_spechelpers.py
+-rw-r--r--   0        0        0     2115 2023-04-26 18:27:44.170514 pylatexenc-3.0a15/pylatexenc/version.py
+-rw-r--r--   0        0        0     1091 2023-04-26 18:27:38.171969 pylatexenc-3.0a15/pyproject.toml
+-rw-r--r--   0        0        0     4209 1970-01-01 00:00:00.000000 pylatexenc-3.0a15/PKG-INFO
```

### Comparing `pylatexenc-3.0a14/LICENSE.txt` & `pylatexenc-3.0a15/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/README.rst` & `pylatexenc-3.0a15/README.rst`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,21 @@
    :target: https://pypi.org/project/pylatexenc/
 
 Python: ≥ 3.4 or ≥ 2.7. The library is designed to be as backwards-compatible as
 reasonably possible and is able to run on old python verisons should it be
 necessary. (Use the setup.py script directly if you have python<3.7, poetry
 doesn't seem to work with old python versions.)
 
+**NEW (4/2023)**: *PYLATEXENC 3.0alpha* is in pre-release on PyPI.  See `new features
+and major changes <https://pylatexenc.readthedocs.io/en/latest/new-in-pylatexenc-3/>`_.
+The `documentation <https://pylatexenc.readthedocs.io/en/latest/>`_ is still
+incomplete, and the new APIs are still subject to changes.  The code is meant
+to be as backwards compatible as is reasonably possible.  Feel free to try it
+out & submit feedback!
+
 
 Unicode Text to LaTeX code
 --------------------------
 
 The ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``
 which converts a unicode string into LaTeX text and escape sequences. It should
 recognize accented characters and most math symbols. A couple of switches allow
@@ -69,7 +76,16 @@
 See LICENSE.txt (MIT License).
 
 NOTE: See copyright notice and license information for file
 ``tools/unicode.xml`` provided in ``tools/unicode.xml.LICENSE``.  (The file
 ``tools/unicode.xml`` was downloaded from
 https://www.w3.org/2003/entities/2007xml/unicode.xml as linked from
 https://www.w3.org/TR/xml-entity-names/#source.)
+
+
+Javascript Library
+------------------
+
+Some core parts of this library can be transcribed to JavaScript.  This feature
+is used (and was developed for) my `Flexible Latex-like Markup
+project <https://github.com/phfaist/flm>`_.  See the *js-transcrypt/* folder and
+its `README file <js-transcrypt/README.md>`_.
```

### Comparing `pylatexenc-3.0a14/pylatexenc/__init__.py` & `pylatexenc-3.0a15/pylatexenc/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/_util.py` & `pylatexenc-3.0a15/pylatexenc/_util.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/_util_support.py` & `pylatexenc-3.0a15/pylatexenc/_util_support.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latex2text/__init__.py` & `pylatexenc-3.0a15/pylatexenc/latex2text/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latex2text/__main__.py` & `pylatexenc-3.0a15/pylatexenc/latex2text/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latex2text/_defaultspecs.py` & `pylatexenc-3.0a15/pylatexenc/latex2text/_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latex2text/_inputlatexfile.py` & `pylatexenc-3.0a15/pylatexenc/latex2text/_inputlatexfile.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/__init__.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/__main__.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/_partial_latex_encoder.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/_partial_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/_uni2latexmap_xml.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/_uni2latexmap_xml.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexencode/_unicode_to_latex_encoder.py` & `pylatexenc-3.0a15/pylatexenc/latexencode/_unicode_to_latex_encoder.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/__init__.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_callablespecbase.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_callablespecbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_exctypes.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_exctypes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_latexcontextdbbase.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_latexcontextdbbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_nodescollector.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_nodescollector.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargs.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsedargsinfo.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsedargsinfo.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstate.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstate.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_parsingstatedelta.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_parsingstatedelta.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_token.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_token.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreader.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreader.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,30 +253,32 @@
                 # get_specials_spec() on failed lookup
                 if sspec is not None and sspec.specials_chars == '\n\n':
                     return self.make_token(tok='specials',
                                            arg=sspec,
                                            pos=newpar_pos_start,
                                            pos_end=newpar_pos_end,
                                            pre_space=pre_space)
-            return self.make_token(tok='char', arg='\n\n',
+
+            par_space_tokens = s[newpar_pos_start:newpar_pos_end]
+            return self.make_token(tok='char', arg=par_space_tokens, #'\n\n',
                                    pos=newpar_pos_start,
                                    pos_end=newpar_pos_end,
                                    pre_space=pre_space)
 
         # if all we could read is whitespsace (w/o 2+ newlines), and we're at
         # the end of the stream, we raise LatexWalkerEndOfStream.
         pos = space_pos_end
         if pos >= len_s:
             raise LatexWalkerEndOfStream(final_space=pre_space)
 
         # inspect the next character --
 
         c = s[pos]
 
-        logger.debug("Char at %d: %r", pos, c)
+        #logger.debug("Char at %d: %r", pos, c)
 
         # check if we have a math mode delimiter
         if c in parsing_state._math_delims_info_startchars and parsing_state.enable_math:
             t = self.impl_maybe_read_math_mode_delimiter(s, pos, parsing_state, pre_space)
             if t is not None:
                 return t
             # continue, we have some other token ->
@@ -288,16 +290,16 @@
                 if s.startswith('begin', pos+1):
                     beginend = 'begin'
                 elif s.startswith('end', pos+1):
                     beginend = 'end'
                 else:
                     beginend = None
 
-                logger.debug("beginend=%r; s.startswith('begin',pos+1)=%r; s[pos+1:pos+7]=%r",
-                             beginend, s.startswith('begin', pos+1), s[pos+1:pos+7])
+                #logger.debug("beginend=%r; s.startswith('begin',pos+1)=%r; s[pos+1:pos+7]=%r",
+                #             beginend, s.startswith('begin', pos+1), s[pos+1:pos+7])
 
                 if beginend:
                     pastbeginendpos = pos+1+len(beginend)
                     if pastbeginendpos >= len(s) \
                        or s[pastbeginendpos] not in parsing_state.macro_alpha_chars:
                         # \begin{environment} and not e.g. \beginmetastate, or
                         # \end{environment} and not e.g. \endcsname
@@ -331,15 +333,15 @@
                 return self.make_token(tok='brace_close', arg=c, pos=pos, pos_end=pos+1,
                                        pre_space=pre_space)
 
         if parsing_state.latex_context is not None and parsing_state.enable_specials:
             sspec = parsing_state.latex_context.test_for_specials(
                 s, pos, parsing_state=parsing_state
             )
-            logger.debug("tested for specials at ‘%s’ -> %r", s[pos:pos+3]+'...', sspec)
+            #logger.debug("tested for specials at ‘%s’ -> %r", s[pos:pos+3]+'...', sspec)
             #logger.debug("get_specials_spec('&') -> %r", parsing_state.latex_context.get_specials_spec('&'))
             if sspec is not None:
                 return self.make_token(tok='specials', arg=sspec,
                                        pos=pos, pos_end=pos+len(sspec.specials_chars),
                                        pre_space=pre_space)
 
         # otherwise, the token is a normal 'char' type.
```

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_tokenreaderbase.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_tokenreaderbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/_walkerbase.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/_walkerbase.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/nodes.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/nodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/__init__.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_base.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_base.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_delimited.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_delimited.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_expression.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_expression.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_generalnodes.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_generalnodes.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_math.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_math.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_optionals.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_optionals.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_stdarg.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_stdarg.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexnodes/parsers/_verbatim.py` & `pylatexenc-3.0a15/pylatexenc/latexnodes/parsers/_verbatim.py`

 * *Files 5% similar despite different names*

```diff
@@ -150,14 +150,21 @@
                                              verbatim_info=verbatim_info )
         
         return nodes, None
 
 
 
 class LatexDelimitedVerbatimParser(LatexVerbatimBaseParser):
+    r"""
+    Parse verbatim content specified between token delimiters (e.g.,
+    ``\verb|...|``).
+
+    Doc..................
+    """
+
     def __init__(self,
                  delimiters=None,
                  auto_delimiters=None,
                  **kwargs):
         super(LatexDelimitedVerbatimParser, self).__init__(**kwargs)
 
         self.delimiters = delimiters
@@ -251,14 +258,19 @@
         )
 
         return nodes, None
 
 
 
 class LatexVerbatimEnvironmentContentsParser(LatexVerbatimBaseParser):
+    r"""
+    Parse verbatim content given as an environment body contents.
+
+    Doc.......................
+    """
     def __init__(self, environment_name='verbatim', **kwargs):
         super(LatexVerbatimEnvironmentContentsParser, self).__init__(**kwargs)
         self.environment_name = environment_name
 
     def new_char_check_stop_condition(self, char, verbatim_string, verbatim_info,
                                       parsing_state):
```

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/__init__.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/__main__.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/_defaultspecs.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/_defaultspecs.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,25 @@
     MacroSpec, EnvironmentSpec, MacroStandardArgsParser,
     VerbatimArgsParser, LstListingArgsParser,
 )
 
 
 specs = [
     #
+    # CATEGORY: latex-paragraph
+    #
+    ('latex-paragraph', {
+        'macros': [],
+        'environments': [],
+        'specials': [
+            std_specials('\n\n'), # paragraph break
+        ],
+    }),
+
+    #
     # CATEGORY: latex-base
     #
     ('latex-base', {
         'macros': [
 
             std_macro('documentclass', True, 1),
             std_macro('usepackage', True, 1),
```

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/_get_defaultspecs.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/_get_defaultspecs.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/_helpers.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/_helpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/_legacy_py1x.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/_legacy_py1x.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/latexwalker/_walker.py` & `pylatexenc-3.0a15/pylatexenc/latexwalker/_walker.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/__init__.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -44,18 +44,20 @@
 
 from ._latexcontextdb import (
     LatexContextDb,
     ParsingStateDeltaExtendLatexContextDb,
 )
 
 from ._argumentsparser import (
-    LatexArgumentsParser
+    LatexArgumentsParser,
+    LatexNoArgumentsParser,
 )
 
 from ._environmentbodyparser import (
+    LatexEnvironmentBodyContentsParserInfo,
     LatexEnvironmentBodyContentsParser
 )
 
 from ._macrocallparser import (
     LatexMacroCallParser,
     LatexEnvironmentCallParser,
     LatexSpecialsCallParser
```

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_argumentsparser.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_argumentsparser.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,18 @@
 ### BEGIN_PYLATEXENC2_LEGACY_SUPPORT_CODE
     @property
     def argspec(self):
         return ''
 ### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
     def parse(self, latex_walker, token_reader, parsing_state, **kwargs):
+        r"""
+        Returns an empty :py:class:`pylatexenc.latexnodes.ParsedArguments`
+        object instance, and no parsing state delta.
+        """
 
         parsed = ParsedArguments(
             arguments_spec_list=[],
             argnlist=[],
             # pos=token_reader.cur_pos(),
             # pos_end=token_reader.cur_pos()
         )
@@ -87,32 +91,35 @@
 
 
 class LatexArgumentsParser(LatexParserBase):
     r"""
     A parser class that handles the arguments of a callable (a macro, an
     environment, or specials).
 
-    ........................
+    Doc ........................
 
     The parser's main function (:py:meth:`parse()`) produces a
     :py:class:`~pylatexenc.latexnodes.ParsedArguments` instance.
 
     Any parser carry-over information generated by individual argument parsers
     is ignored (with a warning).
 
 
     .. py:attribute:: arguments_spec_list
 
-       A list of :py:class:`LatexArgumentSpec` instances describing a sequence
-       of arguments (along with suitable parsers) that a given callable accepts.
+       A list of :py:class:`pylatexenc.latexnodes.LatexArgumentSpec` instances
+       describing a sequence of arguments (along with suitable parsers) that a
+       given callable accepts.
 
        The constructor expects an iterable of elements that are either already
-       :py:class:`LatexArgumentSpec` instances, or that are a string
-       representing a standard argument type, in which case the string is used
-       to construct a :py:class:`LatexArgumentSpec` (see doc for that class).
+       :py:class:`~pylatexenc.latexnodes.LatexArgumentSpec` instances, or that
+       are a string representing a standard argument type, in which case the
+       string is used to construct a
+       :py:class:`~pylatexenc.latexnodes.LatexArgumentSpec` (see doc for that
+       class).
     """
 
     def __init__(self,
                  arguments_spec_list,
                  **kwargs
                  ):
         super(LatexArgumentsParser, self).__init__(**kwargs)
@@ -129,14 +136,17 @@
     @property
     def argspec(self):
         from ..latexnodes._parsedargs import _argspec_from_arguments_spec_list
         return _argspec_from_arguments_spec_list(self.arguments_spec_list)
 ### END_PYLATEXENC2_LEGACY_SUPPORT_CODE
 
     def parse(self, latex_walker, token_reader, parsing_state, **kwargs):
+        r"""
+        See class doc.
+        """
 
         argnlist = []
 
         # pos_start_default = token_reader.cur_pos()
         # pos_start = None
         # last_arg_node = None
```

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_environmentbodyparser.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_environmentbodyparser.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_latexcontextdb.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_latexcontextdb.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_macrocallparser.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_macrocallparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 
     def __init__(self, token_call, macrospec):
         macroname = token_call.arg
         macro_post_space = token_call.post_space
         super(LatexMacroCallParser, self).__init__(
             token_call=token_call,
             spec_object=macrospec,
-            what="macro call (\{})".format(macroname),
+            what=r"macro call (\{})".format(macroname),
             node_class=LatexMacroNode,
             node_extra_kwargs=dict(macroname=macroname,
                                    macro_post_space=macro_post_space),
         )
         self.macroname = macroname
         self.macro_post_space = macro_post_space
```

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,26 @@
 
 
 
 class MacroStandardArgsParser(object):
     r"""
     Parses the arguments to a LaTeX macro.
 
+    .. deprecated:: 3.0
+
+       This class is part of `pylatexenc 2.x`'s macro argument parsing API.
+       Starting with `pylatexenc 3.0`, each macro/environment/specials argument
+       is parsed with an individual macro parser.  See
+       :py:class:`pylatexenc.latexnodes.LatexArgumentSpec`,
+       :py:class:`pylatexenc.latexnodes.parsers.LatexStandardArgumentParser`.
+       (You can also check out the lower-level
+       :py:class:`pylatexenc.macrospec.LatexMacroCallParser`,
+       :py:class:`pylatexenc.macrospec.LatexEnvironmentCallParser`, and
+       :py:class:`pylatexenc.macrospec.LatexSpecialsCallParser`.)
+
     This class parses a simple macro argument specification with a specified
     arrangement of optional and mandatory arguments.
 
     This class also serves as base class for more advanced argument parsers
     (e.g. for a ``\verb+...+`` macro argument parser).  In such cases,
     subclasses should attempt to provide the most suitable `argspec` (and
     `argnlist` for the corresponding :py:class:`ParsedMacroArgs`) for their use,
```

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_pyltxenc2_argparsers/_verbatimargsparser.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,27 @@
 
 
 class VerbatimArgsParser(MacroStandardArgsParser):
     r"""
     Parses the arguments to various LaTeX verbatim constructs such as
     ``\begin{verbatim}...\end{verbatim}`` environment or ``\verb+...+``.
 
+    .. deprecated:: 3.0
+
+       This class is part of `pylatexenc 2.x`'s macro argument parsing API.
+       Starting with `pylatexenc 3.0`, each macro/environment/specials argument
+       is parsed with an individual macro parser.  (See
+       :py:class:`pylatexenc.latexnodes.LatexArgumentSpec`,
+       :py:class:`pylatexenc.macrospec.LatexStandardArgumentParser`.)  To parse
+       verbatim contents for macro arguments and body contents, see
+       :py:class:`pylatexenc.latexnodes.parsers.LatexDelimitedVerbatimParser`
+       and
+       :py:class:`pylatexenc.latexnodes.parsers.LatexVerbatimEnvironmentContentsParser`.
+
+
     This class also serves to illustrate how to write custom parsers for
     complicated macro arguments.  See also :py:class:`MacroStandardArgsParser`.
 
     Arguments:
 
     .. py:attribute:: verbatim_arg_type
```

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_specclasses.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_specclasses.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/macrospec/_spechelpers.py` & `pylatexenc-3.0a15/pylatexenc/macrospec/_spechelpers.py`

 * *Files identical despite different names*

### Comparing `pylatexenc-3.0a14/pylatexenc/version.py` & `pylatexenc-3.0a15/pylatexenc/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 #   7) on github.com, fill in release details with a summary of changes etc.
 #
 #   8) create the source package for PyPI (" python3 setup.py sdist ")
 #   
 #   8) upload package to PyPI (twine upload dist/pylatexenc-X.X.tar.gz -r realpypi)
 #
 
-version_str = "3.0alpha000014"
+version_str = "3.0alpha000015"
```

### Comparing `pylatexenc-3.0a14/pyproject.toml` & `pylatexenc-3.0a15/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylatexenc"
-version = "3.0alpha000014" # ALSO BUMP IN pylatexenc/version.py
+version = "3.0alpha000015" # ALSO BUMP IN pylatexenc/version.py
 description = "Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion"
 authors = ["Philippe Faist <philippe.faist@bluewin.ch>"]
 license = "MIT"
 readme = "README.rst"
 
 [tool.poetry.scripts]
 latexwalker = 'pylatexenc.latexwalker.__main__:main'
```

### Comparing `pylatexenc-3.0a14/PKG-INFO` & `pylatexenc-3.0a15/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pylatexenc
-Version: 3.0a14
+Version: 3.0a15
 Summary: Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 License: MIT
 Author: Philippe Faist
 Author-email: philippe.faist@bluewin.ch
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 
 pylatexenc
 ==========
 
 Simple LaTeX parser providing latex-to-unicode and unicode-to-latex conversion
 
@@ -26,14 +27,21 @@
    :target: https://pypi.org/project/pylatexenc/
 
 Python: ≥ 3.4 or ≥ 2.7. The library is designed to be as backwards-compatible as
 reasonably possible and is able to run on old python verisons should it be
 necessary. (Use the setup.py script directly if you have python<3.7, poetry
 doesn't seem to work with old python versions.)
 
+**NEW (4/2023)**: *PYLATEXENC 3.0alpha* is in pre-release on PyPI.  See `new features
+and major changes <https://pylatexenc.readthedocs.io/en/latest/new-in-pylatexenc-3/>`_.
+The `documentation <https://pylatexenc.readthedocs.io/en/latest/>`_ is still
+incomplete, and the new APIs are still subject to changes.  The code is meant
+to be as backwards compatible as is reasonably possible.  Feel free to try it
+out & submit feedback!
+
 
 Unicode Text to LaTeX code
 --------------------------
 
 The ``pylatexenc.latexencode`` module provides a function ``unicode_to_latex()``
 which converts a unicode string into LaTeX text and escape sequences. It should
 recognize accented characters and most math symbols. A couple of switches allow
@@ -86,7 +94,16 @@
 
 NOTE: See copyright notice and license information for file
 ``tools/unicode.xml`` provided in ``tools/unicode.xml.LICENSE``.  (The file
 ``tools/unicode.xml`` was downloaded from
 https://www.w3.org/2003/entities/2007xml/unicode.xml as linked from
 https://www.w3.org/TR/xml-entity-names/#source.)
 
+
+Javascript Library
+------------------
+
+Some core parts of this library can be transcribed to JavaScript.  This feature
+is used (and was developed for) my `Flexible Latex-like Markup
+project <https://github.com/phfaist/flm>`_.  See the *js-transcrypt/* folder and
+its `README file <js-transcrypt/README.md>`_.
+
```

