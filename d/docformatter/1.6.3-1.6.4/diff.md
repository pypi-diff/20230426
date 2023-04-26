# Comparing `tmp/docformatter-1.6.3.tar.gz` & `tmp/docformatter-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.6.3.tar", max compression
+gzip compressed data, was "docformatter-1.6.4.tar", max compression
```

## Comparing `docformatter-1.6.3.tar` & `docformatter-1.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.3/LICENSE
--rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.3/README.rst
--rw-r--r--   0        0        0     5858 2023-04-23 23:47:52.454167 docformatter-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.3/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.3/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-04-23 23:47:52.454167 docformatter-1.6.3/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.3/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.3/src/docformatter/encode.py
--rw-r--r--   0        0        0    20665 2023-04-22 15:20:07.189864 docformatter-1.6.3/src/docformatter/format.py
--rw-r--r--   0        0        0     5603 2023-04-22 16:15:51.925969 docformatter-1.6.3/src/docformatter/strings.py
--rw-r--r--   0        0        0    14990 2023-04-23 23:41:32.417985 docformatter-1.6.3/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.3/src/docformatter/util.py
--rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.3/setup.py
--rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.4/LICENSE
+-rw-r--r--   0        0        0     6497 2023-04-04 01:14:10.762053 docformatter-1.6.4/README.rst
+-rw-r--r--   0        0        0     5881 2023-04-26 13:06:31.058027 docformatter-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.4/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     2555 2023-04-12 22:55:21.294454 docformatter-1.6.4/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-04-26 13:06:31.058027 docformatter-1.6.4/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    11411 2023-04-12 22:55:21.304454 docformatter-1.6.4/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.4/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20933 2023-04-25 02:19:20.744420 docformatter-1.6.4/src/docformatter/format.py
+-rw-r--r--   0        0        0     5967 2023-04-25 02:19:20.744420 docformatter-1.6.4/src/docformatter/strings.py
+-rw-r--r--   0        0        0    15048 2023-04-26 03:57:38.348349 docformatter-1.6.4/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4572 2023-04-12 22:55:21.329455 docformatter-1.6.4/src/docformatter/util.py
+-rw-r--r--   0        0        0     7714 1970-01-01 00:00:00.000000 docformatter-1.6.4/setup.py
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 docformatter-1.6.4/PKG-INFO
```

### Comparing `docformatter-1.6.3/LICENSE` & `docformatter-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/README.rst` & `docformatter-1.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/pyproject.toml` & `docformatter-1.6.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.6.3"
+version = "1.6.4"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -216,14 +216,15 @@
         {toxinidir}/tests/
     pytest -s -x -c {toxinidir}/pyproject.toml \
         -m system \
         --cache-clear \
         --cov=docformatter \
         --cov-config={toxinidir}/pyproject.toml \
         --cov-branch \
+        --cov-append \
         {toxinidir}/tests/
 
 [testenv:coverage]
 description = combine coverage data and create report
 setenv =
     COVERAGE_FILE = {toxworkdir}/.coverage
 skip_install = true
```

### Comparing `docformatter-1.6.3/src/docformatter/__init__.py` & `docformatter-1.6.4/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/src/docformatter/__main__.py` & `docformatter-1.6.4/src/docformatter/__main__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/src/docformatter/__pkginfo__.py` & `docformatter-1.6.4/src/docformatter/__pkginfo__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.6.3"
+__version__ = "1.6.4"
```

### Comparing `docformatter-1.6.3/src/docformatter/configuration.py` & `docformatter-1.6.4/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/src/docformatter/encode.py` & `docformatter-1.6.4/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/src/docformatter/format.py` & `docformatter-1.6.4/src/docformatter/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,22 +524,28 @@
         -------
         modified_tokens: list
             The list of tokens with any blank lines following a variable
             definition removed.
         """
         for _idx, _token in enumerate(modified_tokens):
             if _token[0] == 3:
-                # Remove newline between variable definition and docstring.
                 j = 1
-                while modified_tokens[_idx - j][
-                    4
-                ] == "\n" and not modified_tokens[_idx - j - 1][
-                    4
-                ].strip().endswith(
-                    '"""'
+
+                # Remove newline between variable definition and docstring
+                # unless is separating docstring from:
+                #     * A previous docstring.
+                #     * The file's shebang.
+                while (
+                    modified_tokens[_idx - j][4] == "\n"
+                    and not (
+                        modified_tokens[_idx - j - 1][4]
+                        .strip()
+                        .endswith('"""')
+                    )
+                    and not modified_tokens[_idx - j - 1][4].startswith("#!/")
                 ):
                     modified_tokens.pop(_idx - j)
                     j += 1
 
                 # Remove newline between class, method, and function
                 # definitions and docstring.
                 j = 2
```

### Comparing `docformatter-1.6.3/src/docformatter/strings.py` & `docformatter-1.6.4/src/docformatter/strings.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """This module provides docformatter string functions."""
 
+
+import contextlib
 # Standard Library Imports
 import re
 
 
 def find_shortest_indentation(lines):
     """Determine the shortest indentation in a list of lines.
 
@@ -98,23 +100,29 @@
 
 
 def normalize_summary(summary: str) -> str:
     """Return normalized docstring summary."""
     # Remove trailing whitespace
     summary = summary.rstrip()
 
-    # Add period at end of sentence and capitalize the first word of the
-    # summary.
+    # Add period at end of sentence.
     if (
         summary
         and (summary[-1].isalnum() or summary[-1] in ['"', "'"])
         and (not summary.startswith("#"))
     ):
         summary += "."
-        summary = summary[0].upper() + summary[1:]
+
+    with contextlib.suppress(IndexError):
+        # Look for underscores, periods in the first word, this would typically
+        # indicate the first word is a variable name, file name, or some other
+        # non-standard English word.  If none of these exist capitalize the
+        # first word of the summary.
+        if all(char not in summary.split(" ", 1)[0] for char in ["_", "."]):
+            summary = summary[0].upper() + summary[1:]
 
     return summary
 
 
 def split_first_sentence(text):
     """Split text into first sentence and the rest.
```

### Comparing `docformatter-1.6.3/src/docformatter/syntax.py` & `docformatter-1.6.4/src/docformatter/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,16 +334,17 @@
                 description_to_list(
                     text[_text_idx : _idx[0]],
                     indentation,
                     wrap_length,
                 )
             )
 
-            if _lines[-1] == "":
-                _lines.pop(-1)
+            with contextlib.suppress(IndexError):
+                if _lines[-1] == "":
+                    _lines.pop(-1)
 
             # Add the URL.
             _lines.append(
                 f"{do_clean_url(text[_idx[0] : _idx[1]], indentation)}"
             )
 
             _text_idx = _idx[1]
```

### Comparing `docformatter-1.6.3/src/docformatter/util.py` & `docformatter-1.6.4/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.3/setup.py` & `docformatter-1.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'tomli': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.6.3',
+    'version': '1.6.4',
     'description': 'Formats docstrings to follow PEP 257',
     'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT|                             +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
```

### Comparing `docformatter-1.6.3/PKG-INFO` & `docformatter-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.6.3
+Version: 1.6.4
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```

