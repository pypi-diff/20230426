# Comparing `tmp/HammerTime-http-0.9.0.tar.gz` & `tmp/HammerTime-http-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HammerTime-http-0.9.0.tar", last modified: Mon Apr 24 17:16:35 2023, max compression
+gzip compressed data, was "HammerTime-http-0.9.1.tar", last modified: Wed Apr 26 19:18:15 2023, max compression
```

## Comparing `HammerTime-http-0.9.0.tar` & `HammerTime-http-0.9.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/HammerTime_http.egg-info/
--rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)      936 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/SOURCES.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)        1 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/dependency_links.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)      140 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/requires.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)       11 2023-04-24 17:16:35.000000 HammerTime-http-0.9.0/HammerTime_http.egg-info/top_level.txt
--rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/LICENSE.md
--rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/PKG-INFO
--rw-rw-r--   0 lph       (1000) lph       (1000)     1753 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/README.md
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/
--rw-rw-r--   0 lph       (1000) lph       (1000)      929 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      778 2023-04-24 17:15:45.000000 HammerTime-http-0.9.0/hammertime/__version__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1308 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/config.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     5947 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/core.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/engine/
--rw-rw-r--   0 lph       (1000) lph       (1000)      916 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     7190 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/engine/aiohttp.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      897 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/interface.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2963 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/hammertime/engine/retry.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     7051 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/engine/scaling.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3201 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/http.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1214 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/kb.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2935 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/requestscheduler.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/rules/
--rw-rw-r--   0 lph       (1000) lph       (1000)     1630 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/__init__.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3332 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/behavior.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2992 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/body.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2191 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/deadhostdetection.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3560 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/filterrequestfromurl.py
--rw-rw-r--   0 lph       (1000) lph       (1000)      962 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/header.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     6765 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/redirects.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     4642 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/sampling.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2399 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/simhash.py
--rw-rw-r--   0 lph       (1000) lph       (1000)    13063 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/status.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     3656 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/timeout.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     1464 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/rules/waf.py
--rw-rw-r--   0 lph       (1000) lph       (1000)     2796 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/ruleset.py
-drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/hammertime/utils/
--rw-rw-r--   0 lph       (1000) lph       (1000)     2647 2023-04-20 19:54:14.000000 HammerTime-http-0.9.0/hammertime/utils/har.py
--rw-rw-r--   0 lph       (1000) lph       (1000)       97 2023-04-24 17:16:35.609327 HammerTime-http-0.9.0/setup.cfg
--rwxrwxr-x   0 lph       (1000) lph       (1000)     1270 2023-04-24 17:14:53.000000 HammerTime-http-0.9.0/setup.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.900100 HammerTime-http-0.9.1/
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.892100 HammerTime-http-0.9.1/HammerTime_http.egg-info/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-26 19:18:15.000000 HammerTime-http-0.9.1/HammerTime_http.egg-info/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)      936 2023-04-26 19:18:15.000000 HammerTime-http-0.9.1/HammerTime_http.egg-info/SOURCES.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)        1 2023-04-26 19:18:15.000000 HammerTime-http-0.9.1/HammerTime_http.egg-info/dependency_links.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)      154 2023-04-26 19:18:15.000000 HammerTime-http-0.9.1/HammerTime_http.egg-info/requires.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)       11 2023-04-26 19:18:15.000000 HammerTime-http-0.9.1/HammerTime_http.egg-info/top_level.txt
+-rw-rw-r--   0 lph       (1000) lph       (1000)    17893 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/LICENSE.md
+-rw-rw-r--   0 lph       (1000) lph       (1000)      449 2023-04-26 19:18:15.900100 HammerTime-http-0.9.1/PKG-INFO
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1753 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/README.md
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.896100 HammerTime-http-0.9.1/hammertime/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      929 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      778 2023-04-26 19:17:00.000000 HammerTime-http-0.9.1/hammertime/__version__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1308 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/config.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     5947 2023-04-24 17:14:53.000000 HammerTime-http-0.9.1/hammertime/core.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.896100 HammerTime-http-0.9.1/hammertime/engine/
+-rw-rw-r--   0 lph       (1000) lph       (1000)      916 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/engine/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     7190 2023-04-24 17:14:53.000000 HammerTime-http-0.9.1/hammertime/engine/aiohttp.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      897 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/engine/interface.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2963 2023-04-24 17:14:53.000000 HammerTime-http-0.9.1/hammertime/engine/retry.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     7051 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/engine/scaling.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3201 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/http.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1214 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/kb.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2935 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/requestscheduler.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.900100 HammerTime-http-0.9.1/hammertime/rules/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1630 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/__init__.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3332 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/behavior.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2992 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/body.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2191 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/deadhostdetection.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3560 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/filterrequestfromurl.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)      962 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/header.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     6765 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/redirects.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     4642 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/sampling.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2399 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/simhash.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)    13063 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/status.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     3656 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/timeout.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     1464 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/rules/waf.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2796 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/ruleset.py
+drwxrwxr-x   0 lph       (1000) lph       (1000)        0 2023-04-26 19:18:15.900100 HammerTime-http-0.9.1/hammertime/utils/
+-rw-rw-r--   0 lph       (1000) lph       (1000)     2647 2023-04-20 19:54:14.000000 HammerTime-http-0.9.1/hammertime/utils/har.py
+-rw-rw-r--   0 lph       (1000) lph       (1000)       97 2023-04-26 19:18:15.904101 HammerTime-http-0.9.1/setup.cfg
+-rwxrwxr-x   0 lph       (1000) lph       (1000)     1302 2023-04-26 19:13:58.000000 HammerTime-http-0.9.1/setup.py
```

### Comparing `HammerTime-http-0.9.0/HammerTime_http.egg-info/SOURCES.txt` & `HammerTime-http-0.9.1/HammerTime_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/LICENSE.md` & `HammerTime-http-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/README.md` & `HammerTime-http-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/__init__.py` & `HammerTime-http-0.9.1/hammertime/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/__version__.py` & `HammerTime-http-0.9.1/hammertime/__version__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
```

### Comparing `HammerTime-http-0.9.0/hammertime/config.py` & `HammerTime-http-0.9.1/hammertime/config.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/core.py` & `HammerTime-http-0.9.1/hammertime/core.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/engine/__init__.py` & `HammerTime-http-0.9.1/hammertime/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/engine/aiohttp.py` & `HammerTime-http-0.9.1/hammertime/engine/aiohttp.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/engine/interface.py` & `HammerTime-http-0.9.1/hammertime/engine/interface.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/engine/retry.py` & `HammerTime-http-0.9.1/hammertime/engine/retry.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/engine/scaling.py` & `HammerTime-http-0.9.1/hammertime/engine/scaling.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/http.py` & `HammerTime-http-0.9.1/hammertime/http.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/kb.py` & `HammerTime-http-0.9.1/hammertime/kb.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/requestscheduler.py` & `HammerTime-http-0.9.1/hammertime/requestscheduler.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/__init__.py` & `HammerTime-http-0.9.1/hammertime/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/behavior.py` & `HammerTime-http-0.9.1/hammertime/rules/behavior.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/body.py` & `HammerTime-http-0.9.1/hammertime/rules/body.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/deadhostdetection.py` & `HammerTime-http-0.9.1/hammertime/rules/deadhostdetection.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/filterrequestfromurl.py` & `HammerTime-http-0.9.1/hammertime/rules/filterrequestfromurl.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/header.py` & `HammerTime-http-0.9.1/hammertime/rules/header.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/redirects.py` & `HammerTime-http-0.9.1/hammertime/rules/redirects.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/sampling.py` & `HammerTime-http-0.9.1/hammertime/rules/sampling.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/simhash.py` & `HammerTime-http-0.9.1/hammertime/rules/simhash.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/status.py` & `HammerTime-http-0.9.1/hammertime/rules/status.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/timeout.py` & `HammerTime-http-0.9.1/hammertime/rules/timeout.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/rules/waf.py` & `HammerTime-http-0.9.1/hammertime/rules/waf.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/ruleset.py` & `HammerTime-http-0.9.1/hammertime/ruleset.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/hammertime/utils/har.py` & `HammerTime-http-0.9.1/hammertime/utils/har.py`

 * *Files identical despite different names*

### Comparing `HammerTime-http-0.9.0/setup.py` & `HammerTime-http-0.9.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,19 +22,19 @@
                 'hammertime.utils'],
       install_requires=[
         'aiodns>=1.1.1,<3.0.0',
         'aiohttp>=3.7.3,<4.0.0',
         'coverage==4.2',
         'easyinject==0.3',
         'flake8==3.8.4',
-        'marshmallow_autoschema==0.3.3',
-        'marshmallow_har==1.1.0',
+        'marshmallow-autoschema>=0.3.3,<0.4.0',
+        'marshmallow-har>=1.1.1,<1.2.0',
       ],
       setup_requires=["pytest-runner"],
       tests_require=[
-        'async_timeout==4.0.0a3',
-        'flake8==3.8.4',
+        'async_timeout>=4.0.2,<5.0.0',
+        'flake8>=3.8.4,<4.0.0',
         'pytest>=6.0,<7.0',
         'simhash==2.1.2',
       ],
       license="GPLv2",
-)
+      )
```

