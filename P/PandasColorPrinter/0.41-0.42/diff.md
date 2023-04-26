# Comparing `tmp/PandasColorPrinter-0.41.tar.gz` & `tmp/PandasColorPrinter-0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PandasColorPrinter-0.41.tar", last modified: Sat Apr 15 15:44:54 2023, max compression
+gzip compressed data, was "PandasColorPrinter-0.42.tar", last modified: Wed Apr 26 01:46:20 2023, max compression
```

## Comparing `PandasColorPrinter-0.41.tar` & `PandasColorPrinter-0.42.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 15:44:54.532073 PandasColorPrinter-0.41/
--rw-rw-rw-   0        0        0     1148 2023-04-15 15:44:48.000000 PandasColorPrinter-0.41/LICENSE.rst
--rw-rw-rw-   0        0        0      161 2023-04-15 15:44:44.000000 PandasColorPrinter-0.41/MANIFEST.in
--rw-rw-rw-   0        0        0     5450 2023-04-15 15:44:54.532073 PandasColorPrinter-0.41/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-15 15:44:54.527086 PandasColorPrinter-0.41/PandasColorPrinter/
--rw-rw-rw-   0        0        0     1069 2023-04-15 00:18:29.000000 PandasColorPrinter-0.41/PandasColorPrinter/LICENSE
--rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PandasColorPrinter-0.41/PandasColorPrinter/README.MD
--rw-rw-rw-   0        0        0    53608 2023-04-15 15:34:24.000000 PandasColorPrinter-0.41/PandasColorPrinter/__init__.py
--rw-rw-rw-   0        0        0       45 2023-04-15 15:44:53.000000 PandasColorPrinter-0.41/PandasColorPrinter/requirements.txt
--rw-rw-rw-   0        0        0    64025 2023-04-15 15:44:53.000000 PandasColorPrinter-0.41/PandasColorPrinter/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-04-15 15:44:54.531075 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/
--rw-rw-rw-   0        0        0     5450 2023-04-15 15:44:54.000000 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      419 2023-04-15 15:44:54.000000 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 15:44:54.000000 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 15:44:54.000000 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-15 15:44:54.000000 PandasColorPrinter-0.41/PandasColorPrinter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4579 2023-04-15 00:18:29.000000 PandasColorPrinter-0.41/README.md
--rw-rw-rw-   0        0        0       85 2023-04-15 15:44:54.533070 PandasColorPrinter-0.41/setup.cfg
--rw-rw-rw-   0        0        0     1507 2023-04-15 15:44:53.000000 PandasColorPrinter-0.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 01:46:20.839359 PandasColorPrinter-0.42/
+-rw-rw-rw-   0        0        0     1148 2023-04-26 01:46:08.000000 PandasColorPrinter-0.42/LICENSE.rst
+-rw-rw-rw-   0        0        0      161 2023-04-26 01:46:06.000000 PandasColorPrinter-0.42/MANIFEST.in
+-rw-rw-rw-   0        0        0     5450 2023-04-26 01:46:20.854319 PandasColorPrinter-0.42/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 01:46:20.833375 PandasColorPrinter-0.42/PandasColorPrinter/
+-rw-rw-rw-   0        0        0     1069 2023-04-15 15:47:55.000000 PandasColorPrinter-0.42/PandasColorPrinter/LICENSE
+-rw-rw-rw-   0        0        0     4579 2023-04-15 15:47:55.000000 PandasColorPrinter-0.42/PandasColorPrinter/README.MD
+-rw-rw-rw-   0        0        0    53806 2023-04-26 01:42:12.000000 PandasColorPrinter-0.42/PandasColorPrinter/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-04-26 01:46:18.000000 PandasColorPrinter-0.42/PandasColorPrinter/requirements.txt
+-rw-rw-rw-   0        0        0    64025 2023-04-26 01:46:18.000000 PandasColorPrinter-0.42/PandasColorPrinter/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-04-26 01:46:20.838361 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/
+-rw-rw-rw-   0        0        0     5450 2023-04-26 01:46:20.000000 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      419 2023-04-26 01:46:20.000000 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 01:46:20.000000 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 01:46:20.000000 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-26 01:46:20.000000 PandasColorPrinter-0.42/PandasColorPrinter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4579 2023-04-15 15:47:55.000000 PandasColorPrinter-0.42/README.md
+-rw-rw-rw-   0        0        0       85 2023-04-26 01:46:20.855316 PandasColorPrinter-0.42/setup.cfg
+-rw-rw-rw-   0        0        0     1507 2023-04-26 01:46:18.000000 PandasColorPrinter-0.42/setup.py
```

### Comparing `PandasColorPrinter-0.41/LICENSE.rst` & `PandasColorPrinter-0.42/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `PandasColorPrinter-0.41/PKG-INFO` & `PandasColorPrinter-0.42/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PandasColorPrinter
-Version: 0.41
+Version: 0.42
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PandasColorPrinter
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PandasColorPrinter-0.41/PandasColorPrinter/LICENSE` & `PandasColorPrinter-0.42/PandasColorPrinter/LICENSE`

 * *Files identical despite different names*

### Comparing `PandasColorPrinter-0.41/PandasColorPrinter/README.MD` & `PandasColorPrinter-0.42/PandasColorPrinter/README.MD`

 * *Files identical despite different names*

### Comparing `PandasColorPrinter-0.41/PandasColorPrinter/__init__.py` & `PandasColorPrinter-0.42/PandasColorPrinter/__init__.py`

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

### Comparing `PandasColorPrinter-0.41/PandasColorPrinter/thirdparty.json` & `PandasColorPrinter-0.42/PandasColorPrinter/thirdparty.json`

 * *Files identical despite different names*

### Comparing `PandasColorPrinter-0.41/PandasColorPrinter.egg-info/PKG-INFO` & `PandasColorPrinter-0.42/PandasColorPrinter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PandasColorPrinter
-Version: 0.41
+Version: 0.42
 Summary: Pandas DataFrames / Pandas Series / Print colored Numpy arrays / lists / dicts / tuples!
 Home-page: https://github.com/hansalemaos/PandasColorPrinter
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: pandas,numpy,dataframe,series,print,prettyprint,colored,coloured
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PandasColorPrinter-0.41/README.md` & `PandasColorPrinter-0.42/README.md`

 * *Files identical despite different names*

### Comparing `PandasColorPrinter-0.41/setup.py` & `PandasColorPrinter-0.42/setup.py`

 * *Files 1% similar despite different names*

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
     name="PandasColorPrinter",
     version=VERSION,
     license='MIT',
```

