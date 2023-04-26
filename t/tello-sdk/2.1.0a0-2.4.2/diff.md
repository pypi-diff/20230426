# Comparing `tmp/tello-sdk-2.1.0a0.tar.gz` & `tmp/tello_sdk-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tello-sdk-2.1.0a0.tar", last modified: Fri Sep 16 14:17:11 2022, max compression
+gzip compressed data, was "tello_sdk-2.4.2.tar", last modified: Wed Apr 26 14:34:15 2023, max compression
```

## Comparing `tello-sdk-2.1.0a0.tar` & `tello_sdk-2.4.2.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-09-16 14:17:11.926534 tello-sdk-2.1.0a0/
--rw-rw-rw-   0        0        0     1085 2022-09-13 09:10:07.000000 tello-sdk-2.1.0a0/LICENSE.txt
--rw-rw-rw-   0        0        0     1034 2022-09-16 14:17:11.926534 tello-sdk-2.1.0a0/PKG-INFO
--rw-rw-rw-   0        0        0     6587 2022-09-15 14:58:58.000000 tello-sdk-2.1.0a0/README.md
--rw-rw-rw-   0        0        0       86 2022-09-16 14:17:11.926534 tello-sdk-2.1.0a0/setup.cfg
--rw-rw-rw-   0        0        0     1301 2022-09-15 15:06:10.000000 tello-sdk-2.1.0a0/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-16 14:17:11.926534 tello-sdk-2.1.0a0/tello_sdk.egg-info/
--rw-rw-rw-   0        0        0     1034 2022-09-16 14:17:11.000000 tello-sdk-2.1.0a0/tello_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2022-09-16 14:17:11.000000 tello-sdk-2.1.0a0/tello_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-16 14:17:11.000000 tello-sdk-2.1.0a0/tello_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-09-16 14:17:11.000000 tello-sdk-2.1.0a0/tello_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2022-09-16 14:17:11.000000 tello-sdk-2.1.0a0/tello_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 14:34:15.178025 tello_sdk-2.4.2/
+-rw-rw-rw-   0        0        0     1087 2023-04-26 07:18:49.000000 tello_sdk-2.4.2/LICENCE
+-rw-rw-rw-   0        0        0     2193 2023-04-26 14:34:15.177035 tello_sdk-2.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1528 2023-04-26 10:07:30.000000 tello_sdk-2.4.2/README.md
+-rw-rw-rw-   0        0        0      953 2023-04-26 14:23:36.000000 tello_sdk-2.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:34:15.178025 tello_sdk-2.4.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 14:34:15.171035 tello_sdk-2.4.2/tello_sdk/
+-rw-rw-rw-   0        0        0    34429 2023-04-26 14:11:41.000000 tello_sdk-2.4.2/tello_sdk/Tello.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 14:23:18.000000 tello_sdk-2.4.2/tello_sdk/__init__.py
+-rw-rw-rw-   0        0        0     9055 2023-04-26 07:18:49.000000 tello_sdk-2.4.2/tello_sdk/telloLive.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:34:15.176035 tello_sdk-2.4.2/tello_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2193 2023-04-26 14:34:15.000000 tello_sdk-2.4.2/tello_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-04-26 14:34:15.000000 tello_sdk-2.4.2/tello_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:34:15.000000 tello_sdk-2.4.2/tello_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 14:34:15.000000 tello_sdk-2.4.2/tello_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 14:34:15.000000 tello_sdk-2.4.2/tello_sdk.egg-info/top_level.txt
```

### Comparing `tello-sdk-2.1.0a0/LICENSE.txt` & `tello_sdk-2.4.2/LICENCE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
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

