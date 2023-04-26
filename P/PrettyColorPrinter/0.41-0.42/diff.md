# Comparing `tmp/PrettyColorPrinter-0.41.tar.gz` & `tmp/PrettyColorPrinter-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrettyColorPrinter-0.41.tar", last modified: Sat Apr 15 15:46:48 2023, max compression
+gzip compressed data, was "PrettyColorPrinter-0.42.tar", last modified: Wed Apr 26 01:44:07 2023, max compression
```

## Comparing `PrettyColorPrinter-0.41.tar` & `PrettyColorPrinter-0.42.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.269403 PrettyColorPrinter-0.41/
--rw-rw-rw-   0        0        0     1148 2023-04-15 15:46:39.000000 PrettyColorPrinter-0.41/LICENSE.rst
--rw-rw-rw-   0        0        0      161 2023-04-15 15:46:38.000000 PrettyColorPrinter-0.41/MANIFEST.in
--rw-rw-rw-   0        0        0     5450 2023-04-15 15:46:48.269403 PrettyColorPrinter-0.41/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.264418 PrettyColorPrinter-0.41/PrettyColorPrinter/
--rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/LICENSE
--rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/README.MD
--rw-rw-rw-   0        0        0    53608 2023-04-15 15:34:24.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/__init__.py
--rw-rw-rw-   0        0        0       45 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/requirements.txt
--rw-rw-rw-   0        0        0    64025 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/PrettyColorPrinter/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-15 15:46:48.268413 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/
--rw-rw-rw-   0        0        0     5450 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-15 15:46:48.000000 PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PrettyColorPrinter-0.41/README.md
--rw-rw-rw-   0        0        0       85 2023-04-15 15:46:48.270428 PrettyColorPrinter-0.41/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-04-15 15:46:47.000000 PrettyColorPrinter-0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 01:44:07.951245 PrettyColorPrinter-0.42/
+-rw-rw-rw-   0        0        0     1148 2023-04-26 01:43:59.000000 PrettyColorPrinter-0.42/LICENSE.rst
+-rw-rw-rw-   0        0        0      161 2023-04-26 01:43:58.000000 PrettyColorPrinter-0.42/MANIFEST.in
+-rw-rw-rw-   0        0        0     5450 2023-04-26 01:44:07.951245 PrettyColorPrinter-0.42/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 01:44:07.944264 PrettyColorPrinter-0.42/PrettyColorPrinter/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 15:47:55.000000 PrettyColorPrinter-0.42/PrettyColorPrinter/LICENSE
+-rw-rw-rw-   0        0        0     4579 2023-04-15 15:47:55.000000 PrettyColorPrinter-0.42/PrettyColorPrinter/README.MD
+-rw-rw-rw-   0        0        0    53806 2023-04-26 01:42:12.000000 PrettyColorPrinter-0.42/PrettyColorPrinter/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-04-26 01:44:06.000000 PrettyColorPrinter-0.42/PrettyColorPrinter/requirements.txt
+-rw-rw-rw-   0        0        0    64025 2023-04-26 01:44:06.000000 PrettyColorPrinter-0.42/PrettyColorPrinter/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-26 01:44:07.950248 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/
+-rw-rw-rw-   0        0        0     5450 2023-04-26 01:44:07.000000 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-26 01:44:07.000000 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 01:44:07.000000 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 01:44:07.000000 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-26 01:44:07.000000 PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4579 2023-04-15 15:47:55.000000 PrettyColorPrinter-0.42/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-26 01:44:07.951245 PrettyColorPrinter-0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-04-26 01:44:06.000000 PrettyColorPrinter-0.42/setup.py
```

### Comparing `PrettyColorPrinter-0.41/LICENSE.rst` & `PrettyColorPrinter-0.42/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.41/PKG-INFO` & `PrettyColorPrinter-0.42/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrettyColorPrinter
-Version: 0.41
+Version: 0.42
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PrettyColorPrinter
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PrettyColorPrinter-0.41/PrettyColorPrinter/LICENSE` & `PrettyColorPrinter-0.42/PrettyColorPrinter/LICENSE`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.41/PrettyColorPrinter/README.MD` & `PrettyColorPrinter-0.42/PrettyColorPrinter/README.MD`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.41/PrettyColorPrinter/__init__.py` & `PrettyColorPrinter-0.42/PrettyColorPrinter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -532,26 +532,34 @@
             dataf.index = [columnname]
             dataf = dataf.T
         isseries = True
 
     return dataf, isseries
 
 
+def _conv_col(column):
+    try:
+        return column.astype("string")
+    except Exception:
+        return column.apply(lambda x: x.decode('utf-8', 'replace') if isinstance(x, bytes) else str(x)).astype(
+        "string")
+
+
 def print_df_with_multiindex(df, max_colwidth=300):
     gruppiert, isser = series_to_dataframe(df)
 
     # das = lambda x: choice(['q23', '5235234534534534634643563543', 'dddddddd'])
     # gruppiert['vbasaxa'] = gruppiert['vbasa'].apply(das)
     allindexlen = []
     for __x in range(len(gruppiert.index[0])):
         allindexlen.append(
             len(sorted([str(x[__x]) for x in gruppiert.index], key=len)[-1])
         )
     valuelen = [
-        gruppiert[x].astype("string").__array__().astype("U").itemsize // 4
+        _conv_col(gruppiert[x])  .__array__().astype("U").itemsize // 4
         for x in gruppiert.columns
     ]
     valuelen = [
         len(str(x)) if len(str(x)) > y else y
         for x, y in zip(gruppiert.columns, valuelen)
     ]
     valuelen = [
@@ -764,21 +772,21 @@
                 print(TC(f"{labels}  ").bg_red.fg_black, end="")
                 print(TC("█").fg_yellow.bg_black, end="")
             if indiprint + 1 == len(columnsprint):
                 pass
                 print("", end="\n")
 
     maxsize = (
-        df[x].astype("string").__array__().astype("U").dtype.itemsize //4 for x in df.columns
+        _conv_col(df[x]).__array__().astype("U").dtype.itemsize //4 for x in df.columns
     )
     maxsize_cols = [len(str(x)) for x in df.columns]
     maxsize = [x if x >= y else y for x, y in zip(maxsize, maxsize_cols)]
 
     maxsize_ = [x + 2 if x < max_column_size else max_column_size for x in maxsize]
-    maxindexsize = 4 + (df.index.astype("string").__array__().astype("U").dtype.itemsize // 4)
+    maxindexsize = 4 + (_conv_col(df.index).__array__().astype("U").dtype.itemsize // 4)
     if maxindexsize < 8:
         maxindexsize = 9
 
     columnsprint = [
         str(f"{col}").replace("\n", "\\n").replace("\r", "\\r")[:size].rjust(size + 1)
         for col, size in zip(df.columns, maxsize_)
     ]
@@ -1365,26 +1373,26 @@
 
 
 
 def stringprint(dframe, max_colwidth=50, repeatcols=70,*args,**kwargs):
     try:
         df, isseries = series_to_dataframe(dframe)
         valuelen = [
-            g if (g := df[x].astype("string").__array__().astype("U").itemsize // 4) < max_colwidth else max_colwidth
+            g if (g := _conv_col(df[x]).__array__().astype("U").itemsize // 4) < max_colwidth else max_colwidth
             for x in df.columns]
-        indi = (df.index.astype("string").__array__().astype("U").itemsize // 4)
+        indi = (_conv_col(df.index).__array__().astype("U").itemsize // 4)
         valuelen.insert(0, indi if indi < max_colwidth else max_colwidth)
         valuelen = [len(str(x)) if len(str(x)) > y else y for x, y in
                     zip(['i n d e x'] + df.columns.to_list(), valuelen)]
         for l1, l2 in zip(range(len(df)), range(1, len(df) + 1)):
             df2 = df.iloc[l1:l2].copy()
             df2.insert(0, 'i n d e x', df2.index.__array__().copy())
 
             for a, b in zip(valuelen, ['i n d e x'] + df.columns.to_list()):
-                df2[b] = df2[b].astype(str).str.ljust(a).str.rjust(a).apply(
+                df2[b] = _conv_col(df2[b]).str.ljust(a).str.rjust(a).apply(
                     lambda ax: ax[:a] + ' █')  # df2[b]['i n d e x'] =df2.index.__array__().copy()
 
 
             if l1 == 0 or l1 % repeatcols == 0:
                 collis = [' ' + str(b).ljust(a).rjust(a)[:a] + c * '' + ' █' for a, b, c in
                           zip(valuelen, ['i n d e x'] + df.columns.to_list(), range(len(valuelen)))]
 
@@ -1418,15 +1426,15 @@
 
     allindexlen = []
     for __x in range(len(gruppiert.index[0])):
         allindexlen.append(
             len(sorted([str(x[__x]) for x in gruppiert.index], key=len)[-1])
         )
     valuelen = [
-        gruppiert[x].astype("string").__array__().astype("U").itemsize // 4
+        _conv_col(gruppiert[x]).__array__().astype("U").itemsize // 4
         for x in gruppiert.columns
     ]
     valuelen = [
         len(str(x)) if len(str(x)) > y else y
         for x, y in zip(gruppiert.columns, valuelen)
     ]
     valuelen = [
```

### Comparing `PrettyColorPrinter-0.41/PrettyColorPrinter/thirdparty.json` & `PrettyColorPrinter-0.42/PrettyColorPrinter/thirdparty.json`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.41/PrettyColorPrinter.egg-info/PKG-INFO` & `PrettyColorPrinter-0.42/PrettyColorPrinter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrettyColorPrinter
-Version: 0.41
+Version: 0.42
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PrettyColorPrinter
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PrettyColorPrinter-0.41/README.md` & `PrettyColorPrinter-0.42/README.md`

 * *Files identical despite different names*

### Comparing `PrettyColorPrinter-0.41/setup.py` & `PrettyColorPrinter-0.42/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.41'''
+VERSION = '''0.42'''
 DESCRIPTION = '''Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!'''
 
 # Setting up
 setup(
     name="PrettyColorPrinter",
     version=VERSION,
     license='MIT',
```

