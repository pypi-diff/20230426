# Comparing `tmp/up_purple-0.1.1-py3-none-any.whl.zip` & `tmp/up_purple-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5116 bytes, number of entries: 6
--rw-r--r--  2.0 unx    10357 b- defN 23-Apr-26 15:53 up_purple.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Apr-26 16:19 up_purple-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      439 b- defN 23-Apr-26 16:19 up_purple-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 16:19 up_purple-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-26 16:19 up_purple-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      469 b- defN 23-Apr-26 16:19 up_purple-0.1.1.dist-info/RECORD
-6 files, 12469 bytes uncompressed, 4268 bytes compressed:  65.8%
+Zip file size: 5118 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    10360 b- defN 23-Apr-26 16:39 up_purple.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-Apr-26 16:39 up_purple-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      439 b- defN 23-Apr-26 16:39 up_purple-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 16:39 up_purple-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-26 16:39 up_purple-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      469 b- defN 23-Apr-26 16:39 up_purple-0.1.2.dist-info/RECORD
+6 files, 12472 bytes uncompressed, 4270 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: up_purple.py
 Comment: 
 
-Filename: up_purple-0.1.1.dist-info/LICENSE.txt
+Filename: up_purple-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: up_purple-0.1.1.dist-info/METADATA
+Filename: up_purple-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: up_purple-0.1.1.dist-info/WHEEL
+Filename: up_purple-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: up_purple-0.1.1.dist-info/top_level.txt
+Filename: up_purple-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: up_purple-0.1.1.dist-info/RECORD
+Filename: up_purple-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## up_purple.py

```diff
@@ -21,15 +21,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import typing
 import warnings
 import unified_planning as up
 
-import pypurple as purple
+import purple_plan as purple
 import black_sat as black
 
 
 credits = up.engines.Credits('PURPLE',
                   'Nicola Gigante',
                   'nicola.gigante@unibz.it',
                   'https://www.black-sat.org',
```

## Comparing `up_purple-0.1.1.dist-info/LICENSE.txt` & `up_purple-0.1.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

