# Comparing `tmp/geocalc-0.0.2.tar.gz` & `tmp/geocalc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocalc-0.0.2.tar", last modified: Wed Apr 26 15:15:53 2023, max compression
+gzip compressed data, was "geocalc-0.0.3.tar", last modified: Wed Apr 26 16:05:46 2023, max compression
```

## Comparing `geocalc-0.0.2.tar` & `geocalc-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:15:53.365402 geocalc-0.0.2/
--rw-r--r--   0 mac        (501) admin       (80)     1071 2023-04-25 19:55:11.000000 geocalc-0.0.2/LICENSE.txt
--rw-r--r--   0 mac        (501) admin       (80)    12465 2023-04-26 15:15:53.365241 geocalc-0.0.2/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)    10080 2023-04-26 15:15:02.000000 geocalc-0.0.2/README.md
-drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 15:15:53.365056 geocalc-0.0.2/geocalc.egg-info/
--rw-r--r--   0 mac        (501) admin       (80)    12465 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) admin       (80)      199 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) admin       (80)       24 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/requires.txt
--rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 15:15:53.000000 geocalc-0.0.2/geocalc.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) admin       (80)     1373 2023-04-26 15:15:28.000000 geocalc-0.0.2/pyproject.toml
--rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-26 15:15:53.365442 geocalc-0.0.2/setup.cfg
--rw-r--r--   0 mac        (501) admin       (80)     1998 2023-04-26 15:10:52.000000 geocalc-0.0.2/setup.py
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 16:05:46.659172 geocalc-0.0.3/
+-rw-r--r--   0 mac        (501) admin       (80)     1071 2023-04-25 19:55:11.000000 geocalc-0.0.3/LICENSE.txt
+-rw-r--r--   0 mac        (501) admin       (80)    12370 2023-04-26 16:05:46.659001 geocalc-0.0.3/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)    10080 2023-04-26 15:15:02.000000 geocalc-0.0.3/README.md
+drwxr-xr-x   0 mac        (501) admin       (80)        0 2023-04-26 16:05:46.658790 geocalc-0.0.3/geocalc.egg-info/
+-rw-r--r--   0 mac        (501) admin       (80)    12370 2023-04-26 16:05:46.000000 geocalc-0.0.3/geocalc.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) admin       (80)      199 2023-04-26 16:05:46.000000 geocalc-0.0.3/geocalc.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 16:05:46.000000 geocalc-0.0.3/geocalc.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) admin       (80)       24 2023-04-26 16:05:46.000000 geocalc-0.0.3/geocalc.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) admin       (80)        1 2023-04-26 16:05:46.000000 geocalc-0.0.3/geocalc.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) admin       (80)     1294 2023-04-26 16:03:08.000000 geocalc-0.0.3/pyproject.toml
+-rw-r--r--   0 mac        (501) admin       (80)       38 2023-04-26 16:05:46.659227 geocalc-0.0.3/setup.cfg
+-rw-r--r--   0 mac        (501) admin       (80)     1998 2023-04-26 15:10:52.000000 geocalc-0.0.3/setup.py
```

### Comparing `geocalc-0.0.2/LICENSE.txt` & `geocalc-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geocalc-0.0.2/PKG-INFO` & `geocalc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocalc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for geometric calculations
 Author: Charles Gameti
 Author-email: Charles Gameti <gameticharles@gmail.com>
 Maintainer-email: Charles Gameti <gameticharles@gmail.com>, "Fiifi O. Turkson" <fiiturkson@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Charles Gameti
@@ -23,19 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
+Project-URL: Homepage, https://github.com/gameticharles/geocalc
+Project-URL: Bug Reports, https://github.com/gameticharles/geocalc/issues
+Project-URL: Source, https://github.com/gameticharles/geocalc
 Keywords: python,geomatic,levelling,curves,geodesy,polygon,triangle,horizontal,vertical
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `geocalc-0.0.2/README.md` & `geocalc-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `geocalc-0.0.2/geocalc.egg-info/PKG-INFO` & `geocalc-0.0.3/geocalc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocalc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library for geometric calculations
 Author: Charles Gameti
 Author-email: Charles Gameti <gameticharles@gmail.com>
 Maintainer-email: Charles Gameti <gameticharles@gmail.com>, "Fiifi O. Turkson" <fiiturkson@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Charles Gameti
@@ -23,19 +23,17 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Reports, https://github.com/pypa/sampleproject/issues
-Project-URL: Funding, https://donate.pypi.org
-Project-URL: Say Thanks!, http://saythanks.io/to/example
-Project-URL: Source, https://github.com/pypa/sampleproject/
+Project-URL: Homepage, https://github.com/gameticharles/geocalc
+Project-URL: Bug Reports, https://github.com/gameticharles/geocalc/issues
+Project-URL: Source, https://github.com/gameticharles/geocalc
 Keywords: python,geomatic,levelling,curves,geodesy,polygon,triangle,horizontal,vertical
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
```

### Comparing `geocalc-0.0.2/pyproject.toml` & `geocalc-0.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geocalc"
-version = "0.0.2"
+version = "0.0.3"
 license = {file = "LICENSE.txt"}
 keywords = ["python", "geomatic", "levelling", "curves", "geodesy", "polygon", "triangle", "horizontal", "vertical"]
 authors = [
   { name="Charles Gameti", email="gameticharles@gmail.com" },
 ]
 description = "A library for geometric calculations"
 readme = "README.md"
@@ -31,12 +31,10 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-data = {"sample" = ["*.dat"]}
 
 [project.urls]  # Optional
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Reports" = "https://github.com/pypa/sampleproject/issues"
-"Funding" = "https://donate.pypi.org"
-"Say Thanks!" = "http://saythanks.io/to/example"
-"Source" = "https://github.com/pypa/sampleproject/"
+"Homepage" = "https://github.com/gameticharles/geocalc"
+"Bug Reports" = "https://github.com/gameticharles/geocalc/issues"
+"Source" = "https://github.com/gameticharles/geocalc"
```

### Comparing `geocalc-0.0.2/setup.py` & `geocalc-0.0.3/setup.py`

 * *Files identical despite different names*

