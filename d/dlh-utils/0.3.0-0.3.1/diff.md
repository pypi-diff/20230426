# Comparing `tmp/dlh_utils-0.3.0.tar.gz` & `tmp/dlh_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlh_utils-0.3.0.tar", max compression
+gzip compressed data, was "dlh_utils-0.3.1.tar", max compression
```

## Comparing `dlh_utils-0.3.0.tar` & `dlh_utils-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0     2743 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0     2917 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/README.md
--rw-r--r--   0        0        0      341 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/__init__.py
--rw-r--r--   0        0        0       93 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/_version.py
--rwxr-xr-x   0        0        0    73861 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/dataframes.py
--rw-r--r--   0        0        0    22516 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/dataframes_testing.py
--rw-r--r--   0        0        0    15604 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/flags.py
--rw-r--r--   0        0        0     7719 2023-03-08 11:17:07.797760 dlh_utils-0.3.0/dlh_utils/flags_testing.py
--rwxr-xr-x   0        0        0    40581 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/linkage.py
--rw-r--r--   0        0        0    15855 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/linkage_testing.py
--rw-r--r--   0        0        0    15289 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/profiling.py
--rw-r--r--   0        0        0     9398 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/sessions.py
--rw-r--r--   0        0        0    48363 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/standardisation.py
--rw-r--r--   0        0        0    23255 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/standardisation_testing.py
--rw-r--r--   0        0        0    31334 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/dlh_utils/utilities.py
--rw-r--r--   0        0        0      829 2023-03-08 11:17:07.801760 dlh_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3880 1970-01-01 00:00:00.000000 dlh_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2743 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3220 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/README.md
+-rw-r--r--   0        0        0      378 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/__init__.py
+-rw-r--r--   0        0        0      141 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/_version.py
+-rwxr-xr-x   0        0        0    74673 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/dataframes.py
+-rw-r--r--   0        0        0    15780 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/flags.py
+-rwxr-xr-x   0        0        0    41020 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/linkage.py
+-rw-r--r--   0        0        0    15273 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/profiling.py
+-rw-r--r--   0        0        0     6442 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/sessions.py
+-rw-r--r--   0        0        0    47883 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/standardisation.py
+-rwxr-xr-x   0        0        0        0 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/__init__.py
+-rwxr-xr-x   0        0        0      904 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/conftest.py
+-rw-r--r--   0        0        0    27443 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_dataframes.py
+-rw-r--r--   0        0        0    21704 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_flags.py
+-rw-r--r--   0        0        0    22391 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_linkage.py
+-rw-r--r--   0        0        0    31733 2023-04-26 10:09:02.628761 dlh_utils-0.3.1/dlh_utils/tests/test_standardisation.py
+-rw-r--r--   0        0        0    30872 2023-04-26 10:09:02.632761 dlh_utils-0.3.1/dlh_utils/utilities.py
+-rw-r--r--   0        0        0      829 2023-04-26 10:09:02.632761 dlh_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 dlh_utils-0.3.1/PKG-INFO
```

### Comparing `dlh_utils-0.3.0/LICENSE` & `dlh_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlh_utils-0.3.0/README.md` & `dlh_utils-0.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 ```sh
 pip install dlh_utils
 ```
 Or, if using CDSW, in a terminal session run:
 ```sh
 pip3 install dlh_utils
 ```
+The -U argument can be used to upgrade the package to its newest version:
+```sh
+pip3 install -U dlh_utils
+```
 
 ## Demo
 For a worked demonstration notebook of these functions being applied within a data linkage context, head over to our [separate demo repository](https://github.com/anthonye93/dlh_utils_demo)
 
 ## Common issues
 
 ### When using the jaro/jaro_winkler functions the error "no module called Jellyfish found" is thrown
@@ -53,7 +57,11 @@
 ```sh
 spark.conf.set('spark.jars', path_to_jar_file)
 ```
 
 ## Thanks
 
 Thanks to all those in the Data Linkage Hub, Data Engineering and Methodology at ONS that have contributed towards this repository.
+
+## Any questions?
+
+If you need any additional help, or have any feedback on the package, please contact Jenna Hart (Jenna.Hart@ons.gov.uk) or the Data Linkage Hub at Linkage.Hub@ons.gov.uk .
```

### Comparing `dlh_utils-0.3.0/dlh_utils/dataframes.py` & `dlh_utils-0.3.1/dlh_utils/dataframes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+'''
+Functions used to modify aspects of a dataframe prior to linkage.
+'''
 import re
 import pyspark.sql.functions as F
 from pyspark.sql import Window
 from dlh_utils import standardisation as st
 
 ##################################################################################
 
@@ -56,21 +59,22 @@
     Raises
     ------
     None at present.
 
     Example
     -------
 
-    data = [("1","6","1","Simpson","1983-05-12","M","ET74 2SP"),
-            ("2","8","2","Simpson","1983-03-19","F","ET74 2SP"),
-            ("3","7","3","Simpson","2012-04-01","M","ET74 2SP"),
-            ("3","9","3","Simpson","2012-04-01","M","ET74 2SP"),
-            ("4","9","4","Simpson","2014-05-09","F","ET74 2SP"),
-            ("5","6","4","Simpson","2021-01-12","F","ET74 2SP")]
-    df=spark.createDataFrame(data=data,schema=["ID","ID2","clust","ROWNUM","DoB","Sex","Postcode"])
+  data = [("1","Homer","Jay","Simpson","1983-05-12","M","ET74 2SP"),
+          ("2","Marge","Juliet","Simpson","1983-03-19","F","ET74 2SP"),
+          ("3","Bart","Jo-Jo","Simpson","2012-04-01","M","ET74 2SP"),
+          ("3","Bart","Jo-Jo","Simpson","2012-04-01","M","ET74 2SP"),
+          ("4","Lisa","Marie","Simpson","2014-05-09","F","ET74 2SP"),
+          ("5","Maggie",None,"Simpson","2021-01-12","F","ET74 2SP")]
+  df = spark.createDataFrame(data=data,schema=["ID","Forename","Middlename",\
+                                              "Surname","DoB","Sex","Postcode"])
 
     > df.show()
     +---+--------+----------+-------+----------+---+--------+
     | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
     +---+--------+----------+-------+----------+---+--------+
     |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|
     |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|
@@ -154,15 +158,15 @@
 
     return df
 
 ###############################################################################
 
 
 def drop_columns(df, subset=None, startswith=None, endswith=None, contains=None,
-                regex=None, drop_duplicates=True):
+                 regex=None, drop_duplicates=True):
     """
     drop_columns allows user to specify one or more columns
     to be dropped from the dataframe.
 
     Parameters
     ----------
     df : dataframe
@@ -285,16 +289,16 @@
                      )
 
     if regex is not None:
         df = df.drop(*
                      [x for x in df.columns if re.search(regex, x)]
                      )
 
-    if subset != None:
-        if type(subset) != list:
+    if subset is not None:
+        if not isinstance(subset, list):
             subset = [subset]
         df = df.drop(*subset)
 
     if drop_duplicates:
         df = df.dropDuplicates()
 
     return df
@@ -430,14 +434,15 @@
     |3  |Bart    |Jo-Jo     |Simpson|2012-04-01|M  |ET74 2SP|Spikey-hair Rebellious|
     |3  |Bart    |Jo-Jo     |Simpson|2012-04-01|M  |ET74 2SP|Spikey-hair Rebellious|
     |4  |Lisa    |Marie     |Simpson|2014-05-09|F  |ET74 2SP|Red-dress Smart       |
     |5  |Maggie  |null      |Simpson|2021-01-12|F  |ET74 2SP|Star-hair Mute        |
     +---+--------+----------+-------+----------+---+--------+----------------------+
 
     e.g, if you wanted to separate the record's appearance from their personality description:
+
     > explode(df,column ='Description',on = ' ',retain =False,drop_duplicates=True,flag=None).show()
     +---+--------+----------+-------+----------+---+--------+------------+
     | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode| Description|
     +---+--------+----------+-------+----------+---+--------+------------+
     |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP| Spikey-hair|
     |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|     Balding|
     |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|       Smart|
@@ -447,14 +452,15 @@
     |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|   Blue-hair|
     |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|Kind-hearted|
     |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|        Mute|
     |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|        Lazy|
     +---+--------+----------+-------+----------+---+--------+------------+
 
     if you wanted to also keep the original overall description:
+
     > explode(df,column='Description',on=' ',retain=True,drop_duplicates=True,flag=None).show()
     +---+--------+----------+-------+----------+---+--------+----------------------+
     |ID |Forename|Middlename|Surname|DoB       |Sex|Postcode|Description           |
     +---+--------+----------+-------+----------+---+--------+----------------------+
     |3  |Bart    |Jo-Jo     |Simpson|2012-04-01|M  |ET74 2SP|Spikey-hair           |
     |1  |Homer   |Jay       |Simpson|1983-05-12|M  |ET74 2SP|Balding               |
     |4  |Lisa    |Marie     |Simpson|2014-05-09|F  |ET74 2SP|Smart                 |
@@ -469,27 +475,27 @@
     |5  |Maggie  |null      |Simpson|2021-01-12|F  |ET74 2SP|Mute                  |
     |1  |Homer   |Jay       |Simpson|1983-05-12|M  |ET74 2SP|Lazy                  |
     |2  |Marge   |Juliet    |Simpson|1983-03-19|F  |ET74 2SP|Blue-hair Kind-hearted|
     |4  |Lisa    |Marie     |Simpson|2014-05-09|F  |ET74 2SP|Red-dress Smart       |
     +---+--------+----------+-------+----------+---+--------+----------------------+
     """
 
-    if retain == False:
+    if retain is False:
 
         df = (df
               .where(F.col(column).rlike(on))
               .select(*[x for x in df.columns if x != column],
                       F.explode(F.split(F.col(column), on))
                       .alias(column))
               .unionByName((df
                            .where((F.col(column).rlike(on) == False)
                                   | (F.col(column).rlike(on).isNull()))))
               )
 
-    if retain == True:
+    if retain is True:
 
         if flag is None:
 
             df = (df
                   .where(F.col(column).rlike(on))
                   .select(*[x for x in df.columns if x != column],
                           F.explode(F.split(F.col(column), on))
@@ -504,23 +510,23 @@
                   .withColumn(flag, F.lit(True))
                   .select(*[x for x in df.columns+[flag] if x != column],
                           F.explode(F.split(F.col(column), on))
                           .alias(column))
                   .unionByName(df.withColumn(flag, F.lit(False)))
                   )
 
-    if drop_duplicates == True:
+    if drop_duplicates is True:
         df = df.dropDuplicates()
 
     return df
 
 
 #############################################################################
 
-def rename_columns(df, rename_dict={}):
+def rename_columns(df, rename_dict):
     """
     Allows multiple columns to be renamed in one command from {before:after}
     replacement dictionary
 
     Parameters
     ----------
     df : dataframe
@@ -571,15 +577,15 @@
         df = df.withColumnRenamed(before, after)
 
     return df
 
 #############################################################################
 
 
-def prefix_columns(df, prefix, exclude=[]):
+def prefix_columns(df, prefix, exclude=None):
     """
     Renames columns with specified prefix string.
 
     Parameters
     ----------
     df: dataframe
     prefix : string
@@ -640,15 +646,15 @@
     |          3|             Bart|              Jo-Jo|Simpson|  2012-04-01|           M|
     |          4|             Lisa|              Marie|Simpson|  2014-05-09|           F|
     |          5|           Maggie|               null|Simpson|  2021-01-12|           F|
     +-----------+-----------------+-------------------+-------+------------+------------+
 
     """
 
-    if type(exclude) != list:
+    if not isinstance(exclude, list):
         exclude = [exclude]
 
     old = [x for x in df.columns if x not in exclude]
     new = [prefix + x for x in old]
 
     rename = dict(zip(old, new))
 
@@ -656,15 +662,15 @@
         df = df.withColumnRenamed(old, new)
 
     return df
 
 #############################################################################
 
 
-def suffix_columns(df, suffix, exclude=[]):
+def suffix_columns(df, suffix, exclude):
     """
     Renames columns with specified suffix string.
 
     Parameters
     ----------
     df: dataframe
     suffix : string
@@ -722,15 +728,15 @@
     |          3|             Bart|              Jo-Jo|Simpson|  2012-04-01|           M|
     |          4|             Lisa|              Marie|Simpson|  2014-05-09|           F|
     |          5|           Maggie|               null|Simpson|  2021-01-12|           F|
     +-----------+-----------------+-------------------+-------+------------+------------+
 
     """
 
-    if type(exclude) != list:
+    if not isinstance(exclude, list):
         exclude = [exclude]
 
     old = [x for x in df.columns if x not in exclude]
     new = [x+suffix for x in old]
 
     rename = dict(zip(old, new))
 
@@ -811,17 +817,17 @@
     +---+--------+----------+-------+----------+---+------------------------+
 
     """
 
     if len(dfs) == 1:
         return dfs[0]
 
-    columns = list(set([x for y in
-                        [df.columns for df in dfs]
-                        for x in y]))
+    columns = list({x for y in
+                    [df.columns for df in dfs]
+                    for x in y})
 
     out = dfs[0]
 
     add_columns = [x for x in columns
                    if x not in out.columns]
 
     for col in add_columns:
@@ -892,18 +898,18 @@
     |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
 
     """
 
     if subset is not None:
 
-        if type(subset) != list:
+        if not isinstance(subset, list):
             subset = [subset]
 
-    if val != None:
+    if val is not None:
         df = df.replace(val, value=None, subset=subset)
 
     df = df.dropna(how='any', subset=subset)
 
     return df
 
 ###############################################################################
@@ -1052,102 +1058,101 @@
     +---+----------------+---+--------+----------+-------+----------+-----------------+
 
     See Also
     --------
     standardisation.standardise_null()
     """
 
-    if type(window) != list:
+    if not isinstance(window, list):
         window = [window]
 
-    w = Window.partitionBy(window)
+    window_spec = Window.partitionBy(window)
 
     if mode == 'count':
 
         if alias is not None:
 
             df = (df
                   .select(*df.columns,
                           F.count(target)
-                          .over(w)
+                          .over(window_spec)
                           .alias(alias))
                   )
 
         else:
             df = (df
                   .select(*df.columns,
                           F.count(target)
-                          .over(w))
+                          .over(window_spec))
                   )
 
     if mode == 'countDistinct':
 
         df = df.fillna("<<<>>>", subset=window)
 
         if alias is not None:
-            if drop_na == True:
+            if drop_na is True:
                 df = (df
                       .dropDuplicates(subset=window+[target])
                       .dropna(subset=[target])
                       .select(*window+[target],
                               F.count(target)
-                              .over(w)
+                              .over(window_spec)
                               .alias(alias))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
             else:
                 df = (df
                       .dropDuplicates(subset=window+[target])
                       .select(*window+[target],
                               F.count(target)
-                              .over(w)
+                              .over(window_spec)
                               .alias(alias))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
 
         else:
-            if drop_na == True:
+            if drop_na is True:
                 df = (df
                       .dropDuplicates(subset=window+[target])
                       .dropna(subset=[target])
                       .select(*window+[target],
                               F.count(target)
-                              .over(w))
+                              .over(window_spec))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
             else:
                 df = (df
                       .dropDuplicates(subset=window+[target])
                       .select(*window+[target],
                               F.count(target)
-                              .over(w))
+                              .over(window_spec))
                       .drop(target)
                       .dropDuplicates()
                       ).join(df,
                              on=window,
                              how='right')
 
-
     if mode == 'min':
         if alias is not None:
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.min(target)
-                            .over(w)
+                            .over(window_spec)
                             .alias(alias))
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
@@ -1164,15 +1169,15 @@
                   )
 
         else:
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.min(target)
-                            .over(w))
+                            .over(window_spec))
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
                           on=window,
@@ -1191,29 +1196,29 @@
     if mode == 'max':
         if alias is not None:
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.max(target)
-                            .over(w)
+                            .over(window_spec)
                             .alias(alias))
                     .select(window+[alias])
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
                           on=window,
                           how='left_anti')
                     .select(window)
                     )
 
-            df = (union_all(df_1,df_2)
+            df = (union_all(df_1, df_2)
                   .select(window+[alias])
                   .dropDuplicates()
                   .join(df,
                         on=window,
                         how='right')
                   )
 
@@ -1224,15 +1229,15 @@
             drop = [x for x in df.columns
                     if x not in window]
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.max(target)
-                            .over(w))
+                            .over(window_spec))
                     .drop(*drop)
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
@@ -1253,15 +1258,15 @@
     if mode == 'sum':
         if alias is not None:
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.sum(target)
-                            .over(w)
+                            .over(window_spec)
                             .alias(alias))
                     .select(window+[alias])
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
@@ -1286,15 +1291,15 @@
             drop = [x for x in df.columns
                     if x not in window]
 
             df_1 = (df
                     .dropna(subset=target)
                     .select(*df.columns,
                             F.sum(target)
-                            .over(w))
+                            .over(window_spec))
                     .drop(*drop)
                     )
 
             df_2 = (df
                     .where((F.col(target).isNull())
                            | F.isnan(F.col(target)))
                     .join(df_1.select(window),
@@ -1429,15 +1434,15 @@
 
 
     See Also
     --------
     standardisation.fill_nulls()
     """
 
-    if type(filter_window) != list:
+    if not isinstance(filter_window, list):
         filter_window = [filter_window]
 
     w = Window.partitionBy(filter_window)
 
     if mode in ['count', 'countDistinct']:
 
         if condition:
@@ -1450,47 +1455,47 @@
         else:
 
             df = (window(df, filter_window, target, mode, alias='count')
                   .where(F.col('count') != value)
                   .drop('count')
                   )
 
-    if mode in ['min','max']:
+    if mode in ['min', 'max']:
 
         if condition:
 
-            df = window(df,filter_window,target,mode,alias='value')
+            df = window(df, filter_window, target, mode, alias='value')
 
-            df = st.fill_nulls(df,fill='<<<>>>',subset=['value']+[target])
+            df = st.fill_nulls(df, fill='<<<>>>', subset=['value']+[target])
 
             df = (df
-                  .where(F.col(target)==F.col('value'))
+                  .where(F.col(target) == F.col('value'))
                   .drop('value')
-                 )
+                  )
 
-            df = (st.standardise_null(df = df,
-                                      replace = "^<<<>>>$",
-                                      subset = target)
-                 )
+            df = (st.standardise_null(df=df,
+                                      replace="^<<<>>>$",
+                                      subset=target)
+                  )
 
         else:
 
-            df = window(df,filter_window,target,mode,alias='value')
+            df = window(df, filter_window, target, mode, alias='value')
 
-            df = st.fill_nulls(df,fill='<<<>>>',subset=['value']+[target])
+            df = st.fill_nulls(df, fill='<<<>>>', subset=['value']+[target])
 
             df = (df
-                  .where(F.col(target)!=F.col('value'))
+                  .where(F.col(target) != F.col('value'))
                   .drop('value')
-                 )
+                  )
 
-            df = (st.standardise_null(df = df,
-                                      replace = "^<<<>>>$",
-                                      subset = target)
-                 )
+            df = (st.standardise_null(df=df,
+                                      replace="^<<<>>>$",
+                                      subset=target)
+                  )
 
     return df
 
 ###############################################################################
 
 
 def literal_column(df, col_name, literal):
@@ -1501,15 +1506,15 @@
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
     col_name : string
       New column title.
     literal :data-type
-      Values populating the colName column.
+      Values populating the col_name column.
 
     Returns
     -------
     dataframe
       Dataframe with new literal column.
 
     Raises
@@ -1546,15 +1551,15 @@
 
     df = df.withColumn(col_name, F.lit(literal))
     return df
 
 ###########################################################################
 
 
-def coalesced(df, subset=None, output_col="coalesced_col"):
+def coalesced(df, subset=None, output_col="coalesced_col", drop=False):
     """
     Produces a new column from a supplied dataframe, that contains the first
     non-null value from each row.
 
     Parameters:
     ----------
     df : dataframe
@@ -1562,14 +1567,17 @@
     subset : list of strings, default = None
       Subset of columns being coalesced together
       into a single column, if subset = None then
       subset = all columns in dataframe.
     output_col : string, default = 'coalesced_col'
       Name of the output column for results of
       the coalesced columns.
+    drop : boolean, default = False
+      If drop = True, the columns that were coalesced 
+      will be dropped from the dataframe.
 
     Returns
     -------
     dataframe
       Dataframe with coalesced columns results
       appended to original dataframe in the
       output_col arg column.
@@ -1595,21 +1603,35 @@
     +----+----+-------------+
     |   a|   b|coalesced_col|
     +----+----+-------------+
     |null|null|        null |
     |   1|null|           1 |
     |null|   2|           2 |
     +----+----+-------------+
+
+    > dataframes.coalesced(df3,subset = None, output_col="coalesced_col", drop=True).show()
+
+    +-------------+
+    |coalesced_col|
+    +-------------+
+    |        null |
+    |           1 |
+    |           2 |
+    +-------------+
     """
 
-    if subset == None:
+    if subset is None:
         subset = df.columns
 
     df = df.withColumn(output_col,
                        F.coalesce(*[F.col(x) for x in subset]))
+
+    if drop:
+        df = drop_columns(df, subset=subset, drop_duplicates=False)
+
     return df
 
 ##############################################################################
 
 
 def split(df, col_in, col_out=None, split_on=' '):
     """
@@ -1704,15 +1726,15 @@
     +------+----+---------+
     |[1, 2]|null|        1|
     |[4, 5]|null|        4|
     |[7, 8]|   2|        7|
     +------+----+---------+
     """
 
-    if type(index) == tuple:
+    if isinstance(index, tuple):
 
         for i in range(index[1])[index[0]:]:
 
             df = df.withColumn(f'index_select_{i}', F.col(split_col)
                                .getItem(i))
 
         df = concat(df, out_col, sep,
@@ -1874,23 +1896,23 @@
     +--------+---+---------+
     |tomatoes|  b|      toe|
     |potatoes|  c|      toe|
     +--------+---+---------+
 
     """
 
-    if from_end == False:
+    if from_end is False:
 
         df = (df
               .withColumn(out_col,
                           F.substring(F.col(target_col),
                                       start, length))
               )
 
-    if from_end == True:
+    if from_end is True:
 
         df = (df
               .withColumn(target_col,
                           F.reverse(F.col(target_col)))
               .withColumn(out_col,
                           F.reverse(F.substring(F.col(target_col),
                                                 start, length)))
@@ -1965,15 +1987,15 @@
         df = df.where(F.col(threshold_column) <= val)
     return df
 
 ###############################################################################
 
 
 def date_diff(df, col_name1, col_name2, diff='Difference',
-             in_date_format='dd-mm-yyyy', units='days', absolute=True):
+              in_date_format='dd-mm-yyyy', units='days', absolute=True):
     """
     date_diff finds the number of days/months/years between two date columns
     by subtracting the dates in the second column from the dates in the first.
     Note, using just months is currently inaccurate as all months are assumed
     to have 31 days.
 
     Parameters
@@ -2057,10 +2079,10 @@
     elif units == 'months':
         # months value is slightly inaccurate as it assumes every month is a 31 day month
         df = df.withColumn(diff, F.col(diff)/(31*86400))
         df = df.withColumn(diff, F.round(diff, 2))
     elif units == 'years':
         df = df.withColumn(diff, F.col(diff)/(86400*365))
         df = df.withColumn(diff, F.round(diff, 2))
-    if absolute == True:
+    if absolute is True:
         df = df.withColumn(diff, F.abs((F.col(diff))))
     return df
```

### Comparing `dlh_utils-0.3.0/dlh_utils/flags.py` & `dlh_utils-0.3.1/dlh_utils/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 '''
 Flag functions, used to quickly highlight anomalous values within data
 '''
 from operator import add
+from functools import reduce
 from pyspark.sql import SparkSession
 from pyspark.sql.types import IntegerType
 import pyspark.sql.functions as F
 import pandas as pd
-from functools import reduce
 
 ###############################################################################
 
 
-def flag(df, ref_col, condition, condition_value=None, condition_col=None,
+def flag(df, ref_col, condition = None, condition_value=None, condition_col=None,
          alias=None, prefix='FLAG', fill_null=None):
     """
     Adds True or False flags to supplied dataframe that can then be used for
     quality checks.
 
     Conditions can be set in comparison to columns or specific values
     (e.g. == column, ==1).  Conditions covered are equals, not equals,
-    greater/less than, is/is not null. Optional TRUE/FALSE
+    greater/less than, is/is not null, and regex. Optional TRUE/FALSE
     fill for null outputs of comparision. Designed for use in conjunction with
     flag_summary() and flag_check() functions.
 
     This function creates a column filled with TRUE or FALSE values
     based on whether a condition has been met.
 
     NOTE: If an alias is not specified, a Flag column name is automatically
@@ -32,15 +32,15 @@
     Parameters
     ----------
     df : dataframe
       The dataframe the function is applied to.
     ref_col : string
       The column title that the conditions are
       performing checks upon.
-    condition : {'==','!=','>','>=',<=','<','isNull','isNotNull'}
+    condition : {'==','!=','>','>=',<=','<','isNull','isNotNull','regex'}
       Conditional statements used to compare values to the
       ref_col.
     condition_value : data-types, default = None
       The value the ref_col is being compared against.
     condition_col : data-types, default = None
       Comparison column for flag condition
     alias : string, default = None
@@ -179,14 +179,19 @@
                            )
 
     if condition == 'isNotNull':
         df = df.withColumn(alias,
                            (F.col(ref_col).isNotNull()) & (
                                F.isnan(F.col(ref_col)) == False)
                            )
+   
+    if condition == 'regex':
+        df = df.withColumn(alias,
+                          (F.col(ref_col).rlike(condition_value)
+                          ))
 
     if fill_null is not None:
         df = (df
               .withColumn(alias,
                           F.when(F.col(alias).isNull(),
                                  fill_null)
                           .otherwise(F.col(alias)))
@@ -253,15 +258,15 @@
     """
     spark = SparkSession.builder.getOrCreate()
 
     if flags is None:
         flags = [
             column for column in df.columns if column.startswith('FLAG_')]
 
-    if type(flags) != list:
+    if not isinstance(flags, list):
         flags = [flags]
 
     rows = df.count()
 
     flags_out = []
 
     for col in flags:
@@ -287,15 +292,15 @@
         'true',
         'false',
         'rows',
         'percent_true',
         'percent_false'
     ]]
 
-    if pandas == False:
+    if pandas is False:
 
         out = (spark
                .createDataFrame(out)
                .coalesce(1))
 
     return out
 
@@ -379,20 +384,21 @@
     flag_summary()
 
     Notes
     -----
     In all instances summary will be the last component returned e.g. master,summary
     """
     if flags is None:
-        try:
-            flags = [
-                column for column in df.columns if column.startswith(prefix)]
-        except:
-            print("No flag columns found! Please specify which flag column to summarise\
-            with the flags = argument, or specify the correct prefix")
+
+        flags = [
+            column for column in df.columns if column.startswith(prefix)]
+
+    if len(flags) == 0:
+        print("No flag columns found! Please specify which flag column to summarise\
+        with the flags = argument, or specify the correct prefix")
 
     df = df.withColumn('flag_count', F.lit(0))
 
     for flag in flags:
 
         df = (df
               .withColumn('flag_count',
@@ -402,15 +408,15 @@
               )
 
     df = df.withColumn("FAIL",
                        reduce(add, [F.col(flag).cast(IntegerType())
                                     for flag in flags]))
     df = df.withColumn('FAIL', F.col('FAIL') > 0)
 
-    if summary == True:
+    if summary is True:
 
         summary_df = flag_summary(df, flags+['FAIL'], pandas=False)
 
         if mode == 'master':
             return (df,
                     summary_df)
```

### Comparing `dlh_utils-0.3.0/dlh_utils/linkage.py` & `dlh_utils-0.3.1/dlh_utils/linkage.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 '''
 Functions used within the linkage phase of data linkage projects
 '''
 import os
+import re
 import pandas as pd
 import jellyfish
-from copy import deepcopy
-import re
 import py4j
 from pyspark.sql import SparkSession, Window
 import pyspark.sql.functions as F
 from pyspark.sql.types import StringType, FloatType
-from graphframes import *
+from graphframes import GraphFrame
 from dlh_utils import dataframes as da
 from dlh_utils import utilities as ut
 
+###############################################################################
+
 # phonetic encoders
 
+
 def alpha_name(df, input_col, output_col):
     """
     Orders string columns alphabetically, also setting them to UPPER CASE.
 
     Parameters
     ----------
     df: dataframe
@@ -95,16 +97,16 @@
     |  3|   Edward|             ETWRT|
     |  4|   Gordon|              KRTN|
     |  5|     Emma|                EM|
     +---+---------+------------------+
 
     """
     @F.udf(returnType=StringType())
-    def meta(s):
-        return None if s == None else jellyfish.metaphone(s)
+    def meta(_string):
+        return None if _string is None else jellyfish.metaphone(_string)
 
     df = df.withColumn(output_col, meta(F.col(input_col)))
 
     return df
 
 ###############################################################################
 
@@ -213,16 +215,16 @@
 
     MK = [linkage.std_lev_score(F.col('First_Name_cen'), F.col('First_Name_ccs')) > 0.7,
         CEN.Last_Name_cen == CCS.Last_Name_ccs,
         CEN.Sex_cen == CCS.Sex_ccs,
         CEN.Resident_Age_cen == CCS.Resident_Age_ccs,
         CEN.Postcode_cen == CCS.Postcode_ccs]
 
-    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS, id_l = 'Resident_ID_cen',
-                                          id_r = 'Resident_ID_ccs',
+    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS,
+                                          id_l = 'Resident_ID_cen', id_r = 'Resident_ID_ccs',
                                           matchkeys = MK, out_dir = '/some_path/links')
     """
 
     return (1 - ((F.levenshtein(string1, string2)) /
                  F.greatest(F.length(string1), F.length(string2))))
 
 ###############################################################################
@@ -285,16 +287,16 @@
 
     MK = [linkage.jaro(F.col('First_Name_cen'), F.col('First_Name_ccs')) > 0.7,
         CEN.Last_Name_cen == CCS.Last_Name_ccs,
         CEN.Sex_cen == CCS.Sex_ccs,
         CEN.Resident_Age_cen == CCS.Resident_Age_ccs,
         CEN.Postcode_cen == CCS.Postcode_ccs]
 
-    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS, id_l = 'Resident_ID_cen',
-                                          id_r = 'Resident_ID_ccs',
+    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS,
+                                          id_l = 'Resident_ID_cen', id_r = 'Resident_ID_ccs',
                                           matchkeys = MK, out_dir = '/some_path/links')
     """
 
     return jellyfish.jaro_similarity(
         string1, string2) if string1 is not None and string2 is not None else None
 
 ###############################################################################
@@ -352,18 +354,17 @@
 
     MK = [linkage.jaro_winkler(F.col('First_Name_cen'), F.col('First_Name_ccs')) > 0.7,
         CEN.Last_Name_cen == CCS.Last_Name_ccs,
         CEN.Sex_cen == CCS.Sex_ccs,
         CEN.Resident_Age_cen == CCS.Resident_Age_ccs,
         CEN.Postcode_cen == CCS.Postcode_ccs]
 
-    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS, id_l = 'Resident_ID_cen',
-                                          id_r = 'Resident_ID_ccs',
-                                          matchkeys = MK, 
-                                          out_dir = '/user/username/cen_ccs_links')
+    links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS,
+                                          id_l = 'Resident_ID_cen', id_r = 'Resident_ID_ccs',
+                                          matchkeys = MK, out_dir = '/user/username/cen_ccs_links')
 
     """
 
     return jellyfish.jaro_winkler_similarity(
         string1, string2) if string1 is not None and string2 is not None else None
 
 ###############################################################################
@@ -507,15 +508,16 @@
     | 1a| 2b|             2|
     | 1a| 8b|             2|
     | 3a| 7b|             3|
     | 3a| 3b|             3|
     +---+---+--------------+
     """
     # Check variable types
-    if not ((isinstance(df.schema[id_1].dataType, StringType)) and (isinstance(df.schema[id_2].dataType, StringType))):
+    if not ((isinstance(df.schema[id_1].dataType, StringType))
+            and (isinstance(df.schema[id_2].dataType, StringType))):
         raise TypeError('ID variables must be strings')
 
     # Set up spark checkpoint settings
     spark = SparkSession.builder.getOrCreate()
     username = os.getenv("HADOOP_USER_NAME")
     checkpoint_path = f"/user/{username}/checkpoints"
     spark.sparkContext.setCheckpointDir(checkpoint_path)
@@ -527,85 +529,90 @@
     # Rename matched data columns ready for clustering
     matches = df.select(id_1, id_2).withColumnRenamed(
         id_1, 'src').withColumnRenamed(id_2, 'dst')
 
     # Create graph & get connected components / clusters
     try:
         graph = GraphFrame(ids, matches)
-      
+
         cluster = graph.connectedComponents()
 
-      # Update cluster numbers to be consecutive (1,2,3,4,... instead of 1,2,3,1000,1001...)
+        # Update cluster numbers to be consecutive (1,2,3,4,... instead of 1,2,3,1000,1001...)
         lookup = cluster.select('component').dropDuplicates(['component']).withColumn(
             'Cluster_Number', F.rank().over(Window.orderBy("component"))).sort('component')
         cluster = cluster.join(lookup, on='component',
-                             how='left').withColumnRenamed('id', id_1)
+                               how='left').withColumnRenamed('id', id_1)
 
         # Join new cluster number onto matched pairs
         df = df.join(cluster, on=id_1, how='left').sort(
             'Cluster_Number').drop('component')
 
         return df
-  
+
     except py4j.protocol.Py4JJavaError:
-      print("""WARNING: A graphframes wrapper package installation has not been found! If you have not already done so,
-      you will need to submit graphframes' JAR file dependency to your spark context. This can be found here:
-      \nhttps://repos.spark-packages.org/graphframes/graphframes/0.6.0-spark2.3-s_2.11/graphframes-0.6.0-spark2.3-s_2.11.jar
-      \nOnce downloaded, this can be submitted to your spark context via: spark.conf.set('spark.jars', path_to_jar_file)
-      """)
+        print("""WARNING: A graphframes wrapper package installation has not been found!
+        If you have not already done so, you will need to submit graphframes' JAR file 
+        dependency to your spark context. This can be found here:
+        \nhttps://repos.spark-packages.org/graphframes/graphframes/0.6.0-spark2.3-s_2.11/
+        graphframes-0.6.0-spark2.3-s_2.11.jar\nOnce downloaded, 
+        this can be submitted to your spark context via:
+        spark.conf.set('spark.jars', path_to_jar_file) or by starting a sparksession from the
+        sessions module of dlh_utils
+        """)
+
 ###############################################################################
 
 
-def extract_mk_variables(df, mk):
+def extract_mk_variables(df, match_key):
     '''
     Extracts variables from matchkey join condition
 
-    For example, would return ['first_name','last_name',date_of_birth'] for a 
-    matchkey using these components. Used in mk_drop(na) to exclude instances 
+    For example, would return ['first_name','last_name',date_of_birth'] for a
+    matchkey using these components. Used in mk_drop(na) to exclude instances
     of null in any matchkey component columns.
 
     Parameters
-    ---------- 
+    ----------
     df : dataframe
       Dataframe the to which matchkeys will be applied.
-    mk : list
+    match_key : list
       The join conditions as specified in matchkey
 
     Returns
     -------
     list
       list of components included in matchkey
 
     Raises
     -------
-      None at present.  
+      None at present.
     '''
 
-    mk_variables = re.split("[^a-zA-Z0-9_]", str(mk))
+    mk_variables = re.split("[^a-zA-Z0-9_]", str(match_key))
     mk_variables = [x for x in mk_variables if x in df.columns]
     mk_variables = list(set(mk_variables))
 
     return mk_variables
 
 ###############################################################################
 
 
-def mk_dropna(df, mk):
+def mk_dropna(df, match_key):
     """
     Drops null values in variables included in matchkeys join conditions
 
-    Improves efficiency of join by excluding records containing nulls in matchkey 
+    Improves efficiency of join by excluding records containing nulls in matchkey
     component columns as these records would not match. Also avoids skew resulting
     from nulls. Used in order_matchkeys() and matchkey_join()
 
     Parameters
-    ---------- 
+    ----------
     df : dataframe
       Dataframe the to which matchkeys will be applied.
-    mk : list
+    match_key : list
       A list of join conditions (as specified in a matchkey(s)).
 
     Returns
     -------
     dataframe
       Dataframe with null values dropped from matchkey component variables.
 
@@ -613,34 +620,38 @@
     -------
       None at present.
 
     See Also
     --------
     extract_mk_variables()
     """
-    variables = extract_mk_variables(df, mk)
+    variables = extract_mk_variables(df, match_key)
 
     df = df.dropna(subset=variables)
 
     return df
 
 ###############################################################################
 
 
 def order_matchkeys(df_l, df_r, mks, chunk=10):
     '''
     Orders matchkey components based on the number of matches made by each matchkey
     in ascending order
 
     Parameters
-    ---------- 
-    df : dataframe
-      Dataframe the to which matchkeys will be applied.
-    mk : list
-      A list of join conditions (as specified in a matchkey(s)).
+    ----------
+    df_l : dataframe
+      Left dataframe to which matchkeys will be applied.
+    df_r : dataframe
+      Right dataframe to which matchkeys will be applied.
+    mks : list
+      A list of join conditions (as specified in a matchkey(s))
+    chunk, int
+      default = 10
 
     Returns
     -------
     dataframe
       Dataframe with null values dropped from matchkey component variables.
 
     Raises
@@ -695,104 +706,105 @@
     mk_order = list(mk_order['mks'])
 
     return mk_order
 
 ###############################################################################
 
 
-def matchkey_join(df_l, df_r, id_l, id_r, mk, mk_n=0):
+def matchkey_join(df_l, df_r, id_l, id_r, match_key, mk_n=0):
     """
     Joins dataframes on matchkey retaining only 1:1 matches
 
     Joins left and right dataframes on specified matchkey. Retains only instances
-    of 1:1 matches between left and right identifiers (i.e. where matches are 
+    of 1:1 matches between left and right identifiers (i.e. where matches are
     unique and there is only one match candidate for each left and right identifier).
     Adds 'matchkey' column to record matchkey number.
 
     Parameters
-    ---------- 
+    ----------
     df_l : dataframe
       left dataframe to be joined.
     df_r : dataframe
       right dataframe to be joined.
     id_l : string
       variable name of column containing left unique identifier
     id_r : string
       variable name of column containing right unique identifier
-    mk : list
+    match_key : list
       matchkey join conditions
     mk_n : int
       matchkey number (order of application)
 
     Returns
     -------
     dataframe
       dataframe of unique 1:1 joins on left and right dataframe. Retaining
       only left and right identifiers and matchkey number.
 
     Raises
     -------
-      None at present. 
+      None at present.
 
     See Also
     --------
     mk_dropna()
     """
-    #variables_l = extract_mk_variables(df_l,mk)
-    #variables_r = extract_mk_variables(df_r,mk)
+    # variables_l = extract_mk_variables(df_l,match_key)
+    # variables_r = extract_mk_variables(df_r,match_key)
 
-    #df_l = df_l.dropna(subset=variables_l)
-    #df_r = df_r.dropna(subset=variables_r)
+    # df_l = df_l.dropna(subset=variables_l)
+    # df_r = df_r.dropna(subset=variables_r)
 
-    df_l = mk_dropna(df_l, mk)
-    df_r = mk_dropna(df_r, mk)
+    df_l = mk_dropna(df_l, match_key)
+    df_r = mk_dropna(df_r, match_key)
 
     df = (df_l
-          .join(df_r, mk, 'inner')
+          .join(df_r, match_key, 'inner')
           .select(id_l, id_r)
           .dropDuplicates()
           .withColumn('matchkey', F.lit(mk_n))
           )
 
     df = da.filter_window(df, id_r, id_l, 'count', 1)
     df = da.filter_window(df, id_l, id_r, 'count', 1)
 
     return df
 
 ###############################################################################
 
 
-def chunk_list(l, n):
-    return [l[i * n:(i + 1) * n]
-            for i in range((len(l) + n - 1) // n)]
+def chunk_list(_list, _num):
+    '''splits a list into a specified number of chunks'''
+    return [_list[i * _num:(i + 1) * _num]
+            for i in range((len(_list) + _num - 1) // _num)]
 
 ###############################################################################
 
 
 def matchkey_dataframe(mks):
     """
-    Creates dataframe of matchkeys and descriptions 
+    Creates dataframe of matchkeys and descriptions
 
-    Takes a list of matchkeys. Assigns numbers to matchkeys based on order in list 
+    Takes a list of matchkeys. Assigns numbers to matchkeys based on order in list
     provided. Adds description of each matchkey from string manipulation of join
     condition.
 
     Parameters
-    ---------- 
+    ----------
     mks : list
       list of matchkeys
 
     Returns
     -------
     dataframe
       Dataframe of matchkeys and descriptions.
 
     Raises
     -------
-      None at present.  
+      None at present.
     """
     spark = SparkSession.builder.getOrCreate()
 
     mk_df = (spark.createDataFrame(
         pd.DataFrame(
             {
                 'matchkey': [x for x, y in enumerate(mks, 1)],
@@ -811,21 +823,21 @@
 
 
 ###############################################################################
 
 
 def assert_unique_matches(linked_ids, *identifier_col):
     """
-    Asserts that all linkage results are unique (i.e. that there is 1:1 relationship 
+    Asserts that all linkage results are unique (i.e. that there is 1:1 relationship
     between matched records).
 
     Note: This will return an AssertError if linkage results are not unique.
 
     Parameters
-    ---------- 
+    ----------
     linked_ids : dataframe
       linked dataframe that includes unique identifier columns
     identifier_col: string or multiple strings
       column name(s) of unique identifiers in linked data
 
     """
 
@@ -838,44 +850,48 @@
                 .collect()[0][0]
                 ) == 1
 
 ###############################################################################
 
 
 def assert_unique(df, column):
+    '''
+    Asserts whether a dataframe contains only one instance of each
+    unique identifier, specified by the col argument.
+    '''
 
-    if type(column) != list:
-        column = [column]
+    if not isinstance(column, list):
+        col = [col]
 
     assert df.count() == df.dropDuplicates(subset=column).count()
 
 ###############################################################################
 
 
 def matchkey_counts(linked_df):
     """
     Counts number of links made on each matchkey
 
     Returns dataframe of matchkey number and the number of matches made on
     each matchkey.
 
     Parameters
-    ---------- 
+    ----------
     linked_df : dataframe
       dataframe returned by deterministic_linkage(). This will include variables:
       left identifier; right identifier and matchkey number
 
     Returns
     -------
     dataframe
       Dataframe of counts of matches achieved by matchkey number.
 
     Raises
     -------
-      None at present.    
+      None at present.
     """
 
     return (linked_df
             .groupBy('matchkey')
             .count()
             .sort('count', ascending=False)
             )
@@ -885,15 +901,15 @@
 
 def clerical_sample(linked_ids, mk_df, df_l, df_r, id_l, id_r, n_ids=100):
     """
     Suffixes left and right dataframes with specified suffix. Joins raw data
     to linked identifier output of deterministic linkage. Returns a number of
     examples for each matchkey as specified.
     Parameters
-    ---------- 
+    ----------
     linked_ids : dataframe
       dataframe returned by deterministic_linkage(). This will include variables:
       left identifier; right identifier and matchkey number.
     mk_df : dataframe
       dataframe returned by matchkey_dataframe(). This will include matchkey
       number and description
     df_l : dataframe
@@ -912,15 +928,16 @@
       The number of identifier pairs sampled for each matchkey
     Returns
     -------
     dataframe
       Dataframe of deterministic linkage samples by matchkey.
     Raises
     -------
-      None at present.    
+    None at present. 
+
     See Also
     --------
     dataframes.union_all()
     """
 
     mks = sorted([x[0] for x in
                   linked_ids.select('matchkey').dropDuplicates().collect()])
@@ -936,16 +953,16 @@
                    .dropDuplicates()
                    .limit(n_ids))
                   for mk in mks]
 
     linked_ids = da.union_all(*linked_ids)
 
     review_df = (linked_ids
-                 .join(df_l, id_l , 'inner')
-                 .join(df_r, id_r , 'inner')
+                 .join(df_l, id_l, 'inner')
+                 .join(df_r, id_r, 'inner')
                  .join(mk_df, on='matchkey')
                  .sort('matchkey', id_l)
                  )
 
     lead_columns = ['matchkey', id_l, id_r]
     end_columns = ['description']
 
@@ -962,20 +979,20 @@
 ###################################################################
 
 
 def demographics(*args, df, identifier,):
     """
     Produces demographics count of dataframe for groups specified.
 
-    Used to get counts of, for example number of persons in age 
+    Used to get counts of, for example number of persons in age
     groups, to allow comparison of counts in raw data to counts in
     linked data. Produces output used in demographics_compare()
 
     Parameters
-    ---------- 
+    ----------
     *args : str or list of str
       Variable column titles to be included in group counts
     df : dataframe
       the dataframe for which demographics are calculated
       number and description
     identifier : string
       Reference to column containing unique identifier
@@ -1031,15 +1048,15 @@
     Determines the expected counts in linked data per demographic
     group, from match rates and counts in raw data. Produces positive
     or negative discrepency metric, highlighting under or
     over-representation of each group in the linked data, versus the
     raw data.
 
     Parameters
-    ---------- 
+    ----------
     df_raw : dataframe
       output of demographics() for raw data
     df_linked : dataframe
       output of demographics() for linked data
 
     Returns
     -------
@@ -1113,33 +1130,34 @@
 
     return df
 
 ###############################################################################
 
 
 def matchkeys_drop_duplicates(mks):
-    ''' 
+    '''
     Removes duplicates from generated matchkeys
     '''
     out = pd.DataFrame({'mks': mks})
     out['mks_str'] = [str(x) for x in out['mks']]
     out = out.drop_duplicates(subset=['mks_str'])
     out = list(out['mks'])
 
     return out
-      
+
 ############################################################################
 
-def deduplicate(df, record_id, mks, checkpoint = False):
+
+def deduplicate(df, record_id, mks, checkpoint=False):
     """
     Matches a dataframe to itself on a specified set of matchkeys. Returns
     either the unique records in your data, or the identified duplicates.
 
     Parameters
-    ---------- 
+    ----------
     df : dataframe
     record_id : string
       name of unique identifier column in data
     mks : list
       either a single list of variables to match on, or a list of matchkeys
     checkpoint: boolean, default = False
       option to checkpoint the outputs (checkpointing will break up
@@ -1171,91 +1189,92 @@
     10487
     """
 
     # get active spark session
     spark = SparkSession.builder.getOrCreate()
 
     # check to see if matchkeys are passed as a list of lists
-    if any(isinstance(MK, list) for MK in mks) == False:
+    if any(isinstance(matchkey, list) for matchkey in mks) is False:
         mks = [mks]
-        
-    df2 = da.suffix_columns(df, suffix = '_2')
 
-    for count, MK in enumerate(mks, 1):
+    df2 = da.suffix_columns(df, suffix='_2')
+
+    for count, matchkey in enumerate(mks, 1):
 
         print(f"\nLinking on matchkey number {count}")
-        
+
         mk_df2 = [x + "_2" for x in MK]
-        
-        duplicates = df.join(df2, on = [df[x] == df2[y] for x, y in zip(MK, mk_df2)],
-                            how = 'inner')
-        
+
+        duplicates = df.join(df2, on=[df[x] == df2[y] for x, y in zip(MK, mk_df2)],
+                             how='inner')
+
         duplicates = duplicates.withColumn('matchkey', F.lit(count))
-        
-        
+
         if count == 1:
+
             matches = duplicates
 
         else:
-          matches = matches.union(duplicates)
-          
+            matches = matches.union(duplicates)
+
         if checkpoint:
-          if (count % 20) == 0:
-            matches = matches.checkpoint
-    
+            if (count % 20) == 0:
+                matches = matches.checkpoint
+
     duplicates = matches.filter(f"{record_id} != {record_id}_2")
-    
+
     duplicates = duplicates.withColumn(f"{record_id}_min",
                                        F.least(*[f"{record_id}", f"{record_id}_2"]))\
-                           .withColumn(f"{record_id}_max",
-                                       F.greatest(*[f"{record_id}", f"{record_id}_2"]))
-      
+        .withColumn(f"{record_id}_max",
+                    F.greatest(*[f"{record_id}", f"{record_id}_2"]))
+
     duplicates = duplicates.selectExpr(f"{record_id}_min AS {record_id}",
                                        f"{record_id}_max AS {record_id}_2",
                                        "matchkey")
-    
+
     duplicates = duplicates.drop_duplicates([f"{record_id}", f"{record_id}_2"])
-      
-    unique = df.join(duplicates, how = "left_anti",
-                     on = (df[f"{record_id}"] == duplicates[f"{record_id}"]) | \
-                          (df[f"{record_id}"] == duplicates[f"{record_id}_2"]))
+
+    unique = df.join(duplicates, how="left_anti",
+                     on=(df[f"{record_id}"] == duplicates[f"{record_id}"]) |
+                     (df[f"{record_id}"] == duplicates[f"{record_id}_2"]))
 
     return unique, duplicates
 
 ############################################################################
 
+
 def deterministic_linkage(df_l, df_r, id_l, id_r, matchkeys, out_dir):
     '''
     Performs determistic linkage of two dataframes given a list of matchkeys /
-    join conditions. Returns a dataframe of the linked identifers of left and 
-    right dataframes,together with the numeric identifier of the matchkey / join 
-    condition on which the link was achieved. Also saves a parquet of linked 
+    join conditions. Returns a dataframe of the linked identifers of left and
+    right dataframes,together with the numeric identifier of the matchkey / join
+    condition on which the link was achieved. Also saves a parquet of linked
     identifiers in specified directory.
 
     Parameters
-    ---------- 
+    ----------
     df_l : dataframe
       Left dtaframe to be linked
     df_r : dataframe
       Right dtaframe to be linked
     id_l : string
       Unique identifier in left dataframe
     id_r : string
       Unique identifier in right dataframe
     matchkeys : list
       A list of join conditions to be sequentially applied in linkage
     out_dir : string
       Specified file path for the directory in which parquet of linked identifiers
-      will be saved and which will be used in processing the linkage. 
+      will be saved and which will be used in processing the linkage.
 
     Returns
     -------
     list
-      a dataframe of the linked identifers of left and right dataframes,together with 
-      the numeric identifier of the matchkey / join condition on which the link was 
+      a dataframe of the linked identifers of left and right dataframes,together with
+      the numeric identifier of the matchkey / join condition on which the link was
       achieved. Also saves a parquet of linked identifiers in out_dir.
 
     Raises
     -------
       None at present.
 
     Example
@@ -1268,15 +1287,15 @@
     > MK2 = [CEN.First_Name_cen == CCS.First_Name_ccs,
              CEN.Last_Name_cen == CCS.Last_Name_ccs,
              CEN.Sex_cen == CCS.Sex_ccs,
              CEN.Postcode_cen == CCS.Postcode_ccs]
 
     > matchkeys = [MK1, MK2, MK3, MK4, MK5]
 
-    > links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS, 
+    > links = linkage.deterministic_linkage(df_l = CEN, df_r = CCS,
                                             id_l = 'Resident_ID_cen', id_r = 'Resident_ID_ccs',
                                             matchkeys = matchkeys, out_dir = '/path_to_file')
 
     MATCHKEY 1
     matches on matchkey:  2815
     total matches:  2815
     left residual:  997186
@@ -1326,15 +1345,15 @@
                 f"{out_dir}/linked_identifiers",
                 mode='overwrite')
 
         else:
             # reads previous matches
             # used in left anti join to ignore matched records
             matches = ut.read_format('parquet',
-                                    f"{out_dir}/linked_identifiers")
+                                     f"{out_dir}/linked_identifiers")
 
             last_count = count
             count = matches.count()
 
             print("\nMATCHKEY", index-1)
             print("matches on matchkey: ", count-last_count)
             print("total matches: ", count)
@@ -1348,15 +1367,15 @@
                 id_l, id_r, matchkey, index),
                 'parquet',
                 f"{out_dir}/linked_identifiers",
                 mode='append')
 
     # reads and returns final matches
     matches = ut.read_format('parquet',
-                            f"{out_dir}/linked_identifiers")
+                             f"{out_dir}/linked_identifiers")
 
     last_count = count
     count = matches.count()
 
     print("\nMATCHKEY", index)
     print("matches on matchkey: ", count-last_count)
     print("total matches: ", count)
```

### Comparing `dlh_utils-0.3.0/dlh_utils/profiling.py` & `dlh_utils-0.3.1/dlh_utils/profiling.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from pyspark.sql import Window
 from pyspark.sql.types import IntegerType, StringType
 from dlh_utils import utilities as ut
 from dlh_utils import dataframes as da
 
 ###############################################################################
 
+
 def create_table_statements(database, regex=None, output_mode='spark'):
     '''
     Returns a dataframe summarising the SQL CREATE TABLE statement that
     creates a named table within a Hive database. Can use regular expressions
     to filter for given tables.
 
     This gives detailed information on table creation parameters, including:
@@ -286,15 +287,15 @@
 
 ###############################################################################
 
 
 def value_counts(df, limit=20, output_mode='pandas'):
     '''
     Produces dataframes summarising the top and bottom distinct value counts within
-    a supplied spark dataframe,
+    a supplied spark dataframe.
 
     Parameters
     ----------
     df: dataframe
         data to be summarised
     limit: integer, default = 20
         the top n values to be summarised
@@ -455,18 +456,18 @@
     if regex is not None:
         tables = list(
             filter(re.compile(regex).match, tables))
 
     variable_types = [(table, hive_dtypes(database, table))
                       for table in tables]
 
-    all_variables = list(set([y[0] for y in
-                              [item for sublist in
-                               [x[1] for x in variable_types]
-                               for item in sublist]]))
+    all_variables = list({y[0] for y in
+                          [item for sublist in
+                           [x[1] for x in variable_types]
+                           for item in sublist]})
 
     out = pd.DataFrame({'variable': all_variables})
 
     for table, dtype in variable_types:
 
         df = pd.DataFrame({
             'variable': [x[0] for x in dtype],
```

### Comparing `dlh_utils-0.3.0/dlh_utils/sessions.py` & `dlh_utils-0.3.1/dlh_utils/sessions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,17 @@
+'''
+Function used to create and start different sized spark sessions, also
+generating a Spark UI link to monitor session progress.
+'''
 import os
 from IPython.core.display import display, HTML
 from pyspark.sql import SparkSession
 import graphframes_jars as graphframes
 
+
 def getOrCreateSparkSession(appName='DE_DL',
                             size='large',
                             showConsoleProgress='false',
                             shufflePartitions=200,
                             defaultParallelism=200,
                             memory='10g',
                             memoryOverhead='1g',
@@ -47,53 +52,34 @@
     Raises
     -------
       None at present.
     """
     # obtain spark UI url parameters
     url = 'spark-' + str(os.environ['CDSW_ENGINE_ID']) + \
         '.'+str(os.environ['CDSW_DOMAIN'])
-    spark_ui = display(HTML('<a href=http://%s>Spark UI</a>' % url))
+    spark_ui = display(HTML(f'<a href=http://{url}s>Spark UI</a>'))
 
     try:
 
       # get graphframes jar path to configure session with
         graphframes_path = graphframes.__file__
         graphframes_path = graphframes_path.rsplit('/', 1)[0]
 
         for file in os.listdir(graphframes_path):
             if file.endswith(".jar"):
                 # Get the latest jar file
                 jar_path = os.path.join(graphframes_path, file)
-       
+
     except FileNotFoundError:
-        print("graphframes wrapper package not found. Please install this to use the cluster_number function.")
+        print("graphframes wrapper package not found.\
+              Please install this to use the cluster_number() function.")
         jar_path = None
 
     if size == 'small':
 
-        """
-        Small Session
-
-        This session is similar to that used for DAPCATS training
-        It is the smallest session that is realistically used
-
-        Details:
-            Only 1g of memory and 3 executors
-            Only 1 core
-            Number of partitions are limited to 12, which can improve
-            performance with smaller data
-
-        Use case:
-            Simple data exploration of small survey data
-
-        Example of actual usage:
-            Used for DAPCATS PySpark training
-            Mostly simple calculations
-        """
-
         spark = (
             SparkSession.builder.appName(appName)
             .config("spark.executor.memory", "1g")
             .config("spark.executor.cores", 1)
             .config("spark.dynamicAllocation.enabled", "true")
             .config("spark.dynamicAllocation.maxExecutors", 3)
             .config("spark.sql.shuffle.partitions", 12)
@@ -103,38 +89,14 @@
             .config("spark.ui.showConsoleProgress", showConsoleProgress)
             .enableHiveSupport()
             .getOrCreate()
         )
 
     if size == 'medium':
 
-        """
-        Medium Session
-
-        A standard session used for analysing survey or synthetic
-        datasets. Also used for some Production pipelines based on
-        survey and/or smaller administrative data.
-
-        Details:
-            6g of memory and 3 executors
-            3 cores
-            Number of partitions are limited to 18, which can improve
-            performance with smaller data
-
-        Use case:
-            Developing code in Dev Test
-            Data exploration in Production
-            Developing Production pipelines on a sample of data
-            Running smaller Production pipelines on mostly survey data
-
-        Example of actual usage:
-            Complex calculations, but on smaller synthetic data in
-                Dev Test
-        """
-
         spark = (
             SparkSession.builder.appName(appName)
             .config("spark.executor.memory", "6g")
             .config("spark.executor.cores", 3)
             .config("spark.dynamicAllocation.enabled", "true")
             .config("spark.dynamicAllocation.maxExecutors", 3)
             .config("spark.sql.shuffle.partitions", 18)
@@ -144,36 +106,14 @@
             .config("spark.ui.showConsoleProgress", showConsoleProgress)
             .enableHiveSupport()
             .getOrCreate()
         )
 
     if size == 'large':
 
-        """
-        Large Session
-
-        Session designed for running Production pipelines on large
-        administrative data, rather than just survey data. Will often
-        develop using a smaller session then change to this once the
-        pipeline is complete.
-
-        Details:
-            10g of memory and 5 executors
-            1g of memory overhead
-            5 cores, which is generally optimal on larger sessions
-
-        Use case:
-            Production pipelines on administrative data
-            Cannot be used in Dev Test, as 9 GB limit per executor
-
-        Example of actual usage:
-            One administrative dataset of 100 million rows
-            Many calculations
-        """
-
         spark = (
             SparkSession.builder.appName(appName)
             .config("spark.executor.memory", "10g")
             .config("spark.yarn.executor.memoryOverhead", "1g")
             .config("spark.executor.cores", 5)
             .config("spark.dynamicAllocation.enabled", "true")
             .config("spark.dynamicAllocation.maxExecutors", 5)
@@ -183,40 +123,14 @@
             .config("spark.ui.showConsoleProgress", showConsoleProgress)
             .enableHiveSupport()
             .getOrCreate()
         )
 
     if size == 'extra_large':
 
-        """
-        Extra Large session
-
-        Used for the most complex pipelines, with huge administrative
-        data sources and complex calculations. Uses a large amount of
-        resource on the cluster, so only use when running Production
-        pipelines
-
-        Details:
-            20g of memory and 12 executors
-            2g of memory overhead
-            5 cores; using too many cores can actually cause worse
-                performance on larger sessions
-
-        Use case:
-            Running large, complex pipelines in Production on mostly
-                administrative data
-            Do not use for development purposes; use a smaller session
-                and work on a sample of data or synthetic data
-
-        Example of actual usage:
-            Three administrative datasets of around 300 million rows
-            Significant calculations, including joins and writing/reading
-                to many intermediate tables
-        """
-
         spark = (
             SparkSession.builder.appName(appName)
             .config("spark.executor.memory", "20g")
             .config("spark.yarn.executor.memoryOverhead", "2g")
             .config("spark.executor.cores", 5)
             .config("spark.dynamicAllocation.enabled", "true")
             .config("spark.dynamicAllocation.maxExecutors", 12)
@@ -226,18 +140,14 @@
             .config("spark.ui.showConsoleProgress", showConsoleProgress)
             .enableHiveSupport()
             .getOrCreate()
         )
 
     if size == 'custom':
 
-        """
-        Optional custom spark settings
-        """
-
         spark = (
             SparkSession.builder.appName(appName)
             .config('spark.executor.memory', memory)
             .config('spark.executor.memoryOverhead', memoryOverhead)
             .config('spark.executor.cores', cores)
             .config('spark.dynamicAllocation.maxExecutors', maxExecutors)
             .config("spark.sql.shuffle.partitions", shufflePartitions)
```

### Comparing `dlh_utils-0.3.0/dlh_utils/standardisation.py` & `dlh_utils-0.3.1/dlh_utils/standardisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+'''
+Functions used to standardise and clean data prior to linkage.
+'''
 import pyspark.sql.functions as F
-from pyspark.sql.types import *
+from pyspark.sql.types import IntegerType
 from dlh_utils import dataframes as da
 
 ###############################################################################
 
-
 def cast_type(df, subset=None, types='string'):
     """
     Casts specific dataframe columns to a specified type.
 
     The function can either take a subset of columns or if no subset is defined
     it takes all the columns and converts their datatypes into the datatype
     specified by the user.
@@ -68,15 +70,15 @@
      |-- Sex: string (nullable = true)
      |-- Postcode: string (nullable = true)
 
     """
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
         if df.select(col).dtypes[0][1] != types:
             df = df.withColumn(col, F.col(col).cast(types))
     return df
 
@@ -120,20 +122,19 @@
     -------
     None at present.
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
-        if fill != None:
-            wsl == None
+        if fill is not None:
             if df.select(col).dtypes[0][1] == 'string':
                 df = df.withColumn(col, F.trim(F.col(col)))
                 df = df.withColumn(col, F.regexp_replace(
                     F.col(col), "\\s+", fill))
 
         elif wsl == 'none':
             if df.select(col).dtypes[0][1] == 'string':
@@ -156,15 +157,15 @@
     Standardises misalignments of first and middle names by splitting
     the string in specified column(s) on a specified separator and appending
     new columns to the dataframe with each part of the split string.
 
     Data are then repartitioned on a specified unique identifier column for
     performance purposes.
 
-    Note - if either middle name or first_name column is not present in data set,
+    Note - if either middle_name or first_name column is not present in data set,
     this needs to be created as a null column before applying this function
 
     Parameters
     ----------
     df : dataframe
       The dataframe the function is applied to.
     first_name : string
@@ -188,16 +189,16 @@
     None at present.
 
     See Also
     --------
     dataframes.concat()
     """
 
-    out = (df.where((F.col(first_name).contains(sep) == False)
-                    | (F.col(first_name).isNull())))
+    out = df.where((F.col(first_name).contains(sep) == False)
+                   | (F.col(first_name).isNull()))
     df = df.where(F.col(first_name).contains(sep))
 
     df = da.concat(df, 'align_forenames', sep, [
         first_name,
         middle_name
     ])
 
@@ -213,15 +214,15 @@
     df = df.repartition(identifier)
 
     return df
 
 ##############################################################################
 
 
-def reg_replace(df, dic={}, subset=None):
+def reg_replace(df, replace_dict, subset=None):
     """
     Uses regular expressions to replace values within dataframe columns.
 
     Parameters
     ----------
     df : dataframe
       The dataframe to which the function is applied.
@@ -246,20 +247,20 @@
     Raises
     -------
     None at present.
     """
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
-    if subset != None:
+    if subset is not None:
         for col in subset:
-            for key, val in dic.items():
+            for key, val in replace_dict.items():
                 df = df.withColumn(col, F.regexp_replace(F.col(col), val, key))
 
     return df
 
 ##########################################################################
 
 
@@ -319,15 +320,15 @@
     ]
 
     surname_prefix_regex = "|".join([f"(?<=\\b{prefix})[ -]"
                                      for prefix in prefixes])
 
     surname_regex = surname_regex+"|"+surname_prefix_regex
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = df.withColumn(col, F.regexp_replace(F.col(col),
                                                  surname_regex,
                                                  ''))
@@ -335,15 +336,15 @@
     return df
 
 ############################################################################
 
 
 def clean_forename(df, subset):
     '''
-    Removes common invalid responses/forename prefixes from a specified column.
+    Removes common forename prefixes from a specified column.
 
     Parameters
     ----------
     df : dataframe
       The dataframe to which the function is applied.
     subset : str or list of str
       The columns on which this function will be applied.
@@ -374,29 +375,29 @@
         'SIR',
         'LADY'
     ]
 
     forename_regex = "|".join([f"\\b{component}\\b"
                                for component in components])
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = df.withColumn(col, F.regexp_replace(F.col(col),
                                                  forename_regex,
                                                  ''))
 
     return df
 
 ##########################################################################
 
 
-def group_single_characters(df, subset=None):
+def group_single_characters(df, subset=None, include_terminals=False):
     """
     Remove spaces between single characters
 
     The function takes a dataframe and specified columns.
     It then looks for single characters within the column
     values and groups them together by removing the whitespace
     around them.
@@ -408,14 +409,21 @@
       The dataframe to which the function is applied.
     subset : str or list of str, default = None
       Subset of columns on which the function is applied.
       If left as None, the function applies to all
       columns. If the user gives a string value it
       is converted to a list of one column.
       It can also take a list of strings.
+    include_terminals : boolean, default = False
+      If False, single characters in the first and last
+      positions will not be grouped; for example, "a bc d" will
+      be returned as "a bc d" without grouping the "a" and "d"
+      If True, single characters in the first and last
+      positions will be grouped; for example, "a bc d" will
+      be grouped as "abcd"
 
     Returns
     -------
     dataframe
       Dataframe with the same columns but with the
       group single characters function applied to
       the specified columns.
@@ -424,23 +432,27 @@
     ------
     None at present.
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
+    regex = r"(?<= \w|^\w|^)[ ]+(?=\w |\w$|$)"
+    if include_terminals:
+        regex += r"|(?<=^\w)[ ]+(?=\w)"   # Initial single letter
+        regex += r"|(?<=\w)[ ]+(?=\w$)"   # Final single letter
+
     for col in subset:
 
         df = (df
               .withColumn(col,
-                          F.regexp_replace(F.col(col),
-                                           "(?<= \\w|^\\w|^) (?=\\w |\\w$|$)", "")
+                          F.regexp_replace(F.col(col), regex, "")
                           )
               )
 
     return df
 
 ##########################################################################
 
@@ -474,15 +486,15 @@
     ------
     None at present.
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = df.withColumn(col, F.regexp_replace(F.col(col),
                                                  "[ ]+[-]+[ ]+|[-]+[ ]+|[ ]+[-]",
                                                  '-'))
@@ -506,15 +518,15 @@
     values. Otherwise, the exact values entered in replace are searched
     for and replaced in the data.
 
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
-    replace: data-type, default = None
+    replace: data-type
       These are the artificial null values
       that are being replaced.
     subset : str or list of str, default = None
       Subset of columns on which the function is applied.
       If left as None, the function applies to all
       columns. If the user gives a string value it
       is converted to a list of one column.
@@ -568,29 +580,29 @@
     |  5|  Maggie|      null| DONUTS|2021-01-12|DONUTS|ET74 2SP|
     +---+--------+----------+-------+----------+------+--------+
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
-    if regex == True:
+    if regex is True:
 
         for column in subset:
 
             df = (df
                   .withColumn(column,
                               F.when(F.col(column).rlike(
                                   replace), replace_with)
                               .otherwise(F.col(column)))
                   )
 
-    if regex == False:
+    if regex is False:
 
         for column in subset:
 
             df = (df
                   .withColumn(column,
                               F.when(F.col(column).like(replace), replace_with)
                               .otherwise(F.col(column)))
@@ -659,15 +671,15 @@
     |  5|  Maggie|      null|     -9|2021-01-12| -9|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = (df
               .withColumn('space_count',
                           F.length(
@@ -741,15 +753,15 @@
     +---+--------+----------+--------+----------+---+--------+
 
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     number_hyphens = "-"*limit
 
     for col in subset:
 
         df = (df
@@ -826,18 +838,18 @@
     +---+--------+----------+-------+--------+---+--------+
 
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
-    if keep != None:
+    if keep is not None:
         keep = "".join(keep)
         regex = f"[^A-Za-z0-9 {keep}]"
     else:
         regex = "[^A-Za-z0-9 ]"
 
     for x in subset:
         df = df.withColumn(x, F.regexp_replace(F.col(x), regex, ""))
@@ -858,15 +870,15 @@
     df : dataframe
       Dataframe to which the function is applied.
     subset :  str or list of str, default = None
       The subset is the column(s) on which the function is applied.
       If None the function applies to the whole dataframe.
     val: {'upper','lower','title'}, default = 'upper'
       Takes three types of string values
-      and changes the values in the subset columns to the 
+      and changes the values in the subset columns to the
       case type respectively.
 
     Returns
     -------
     dataframe
       Function returns dataframe with case conversions applied.
 
@@ -901,15 +913,15 @@
     +---+--------+----------+-------+----------+---+--------+
 
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
         if val == 'upper':
             if df.select(col).dtypes[0][1] == 'string':
                 df = df.withColumn(col, F.upper(F.col(col)))
         if val == 'lower':
@@ -974,15 +986,15 @@
     |  5|  MAGGie|      null|SiMpSoN|2021-01-12|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     types = [x for x in df.dtypes
              if x[0] in subset]
 
     types = dict(zip([x[0] for x in types],
                      [x[1] for x in types]))
@@ -1048,15 +1060,16 @@
     |002|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|
     |003|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |003|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |004|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
     |005|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
     """
-    if type(subset) != list:
+
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         df = (df
               .withColumn(col,
                           F.lpad(F.col(col), n, '0')
@@ -1117,15 +1130,15 @@
     |  3|Turbo man|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  3|Turbo man|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  4|     Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
     |  5|   Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
     +---+---------+----------+-------+----------+---+--------+
     """
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
 
         for before, after in replace_dict.items():
             df = (df
                   .withColumn(col, F.when(F.col(col).like(before), after)
@@ -1134,42 +1147,55 @@
 
     return df
 
 ##############################################################################
 
 
 def standardise_date(df, col_name, in_date_format='dd-MM-yyyy',
-                     out_date_format='yyyy-MM-dd'):
+                     out_date_format='yyyy-MM-dd',null_counts=False):
     """
     Changes the date format of a specified date column.
+    
+    Also has an optional argument null_counts. If set to False, the function
+    only returns the dataframe with specified date values altered. 
+    However, if set to True, will also return a tuple, displaying a count of 
+    nulls in the dataframe before and after the function has been applied.  
+    This is because the standardise_date function will make a date
+    value null if its format differs from the in_date_format. 
 
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
     col_name: string
       The column in the dataframe to which the function is being
       applied.
     in_date_format: default = 'dd-mm-yyyy', string
       This is the current date format of the the column.
-      It uses hyphens or forward slashes to split the date
-      up and dd,mm,yyyy to show date month and year respectively.
-      e.g. 'dd-mm-yyyy' , 'dd/mm/yyyy', 'yyyy-mm-dd'.
     out_date_format: default = 'yyyy-mm-dd', string
       This is the date format to which the column values will be
       changed.
-      It uses hyphens or forward slashes to split the date
-      up and dd,mm,yyyy to show date month and year respectively.
-      e.g. 'dd-mm-yyyy' , 'dd/mm/yyyy', 'yyyy-mm-dd'.
+    null_counts: default = False, bool
+      If set to True provides a tuple, where the first part displays
+      the df null count before the function has been applied, and the 
+      second part is the df null count after the function has been 
+      applied. 
 
     Returns
     -------
+    If null_counts = False:
     dataframe
       Dataframe with specified date column values altered
       to new specified format.
+    
+    If null_counts = True:
+    dataframe as described above,
+    Tuple
+      showing null counts before and after standardise_date
+      has been applied to df
 
     Raises
     -------
       None at present.
 
     Example
     -------
@@ -1195,18 +1221,58 @@
     |  1|   Homer|       Jay|Simpson|12/05/1983|  M|ET74 2SP|
     |  2|   Marge|    Juliet|Simpson|19/03/1983|  F|ET74 2SP|
     |  3|    Bart|     Jo-Jo|Simpson|01/04/2012|  M|ET74 2SP|
     |  3|    Bart|     Jo-Jo|Simpson|01/04/2012|  M|ET74 2SP|
     |  4|    Lisa|     Marie|Simpson|09/05/2014|  F|ET74 2SP|
     |  5|  Maggie|      null|Simpson|12/01/2021|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
+    
+    Example using null_counts:
+    > df.show()
+    
+    +----------+
+    |      date|
+    +----------+
+    |1990/07/19|
+    |2020/09/01|
+    |1998/03/21|
+    |1999/11/02|
+    |2005-12-24|
+    +----------+
+    
+    >df,nulls = standardise_date(df,'date','yyyy/MM/dd','yyyy.MM.dd',True)
+    
+    >df.show()
+    +----------+
+    |      date|
+    +----------+
+    |1990.07.19|
+    |2020.09.01|
+    |1998.03.21|
+    |1999.11.02|
+    |      null|
+    +----------+
+    
+    >nulls
+    (0, 1)
+     
     """
+    if null_counts:
+        null_before = df.where(F.col(col_name).isNull()).count()
+
     df = df.withColumn(col_name, F.unix_timestamp(F.col(col_name), in_date_format))
     df = df.withColumn(col_name, F.from_unixtime(F.col(col_name), out_date_format))
-    return df
+
+    if null_counts:
+        null_after = df.where(F.col(col_name).isNull()).count()
+
+        return df,(null_before,null_after)
+
+    else:
+      return df
 
 ##############################################################################
 
 
 def fill_nulls(df, fill, subset=None):
     """
     Fills null and NaN with specified value
@@ -1262,15 +1328,15 @@
     |  5|  Maggie|    donuts|Simpson|2021-01-12|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
     """
 
     if subset is None:
         subset = df.columns
 
-    if type(subset) != list:
+    if not isinstance(subset, list):
         subset = [subset]
 
     for col in subset:
         df = (df
               .withColumn(col, F.when(
                   (F.col(col).isNull())
                   | (F.isnan(F.col(col))), fill)
@@ -1278,115 +1344,28 @@
               )
 
     return df
 
 ################################################################################
 
 
-def cast_geography_null(df, target_col, regex, geo_cols=None):
+def age_at(df, reference_col, in_date_format='dd-MM-yyyy', *age_at_dates):
     """
-    Casts a target geography variable value, and if specified corresponding values in
-    additional geography variables, to null (None type) where target geography value
-    meets regex.
-
-    Parameters
-    ----------
-    df : dataframe
-      Dataframe to which the function is applied.
-    target_col : str
-      The target reference column
-   regex: str
-      The regex conditions defining null postcode (default postcodes beginning
-      zz999 case insensitive)
-    geo_cols: str or list of str, default = None
-      Additional geography variables to be cast to null.
-
-    Returns
-    -------
-    dataframe
-      Dataframe with null postcodes and respective geographies cast to true null
-      None type
-
-    Raises
-    -------
-    None at present.
+    Calculates individuals' ages at specified dates from a reference Date of Birth column
 
-    Example
-    -------
-
-    >df.show()
-
-    +---+--------+----------+-------+----------+---+--------+
-    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
-    +---+--------+----------+-------+----------+---+--------+
-    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ZZ99 9SZ|
-    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ZZ99 5GB|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ZZ99 2SP|
-    |  5|  Maggie|      null|Simpson|2021-01-12|  F|ZZ99 2FA|
-    +---+--------+----------+-------+----------+---+--------+
-
-    > cast_geography_null(df,target_col = 'Postcode',geo_cols = None,regex = "^ZZ99").show()
-
-    +---+--------+----------+-------+----------+---+--------+
-    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
-    +---+--------+----------+-------+----------+---+--------+
-    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|    null|
-    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|    null|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
-    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|    null|
-    |  5|  Maggie|      null|Simpson|2021-01-12|  F|    null|
-    +---+--------+----------+-------+----------+---+--------+
-
-    """
-    if geo_cols is not None:
-
-        if type(geo_cols) != list:
-            geo_cols = [geo_cols]
-
-        for col in geo_cols:
-
-            df = (df
-                  .withColumn(col,
-                              F.when(F.col(target_col).rlike(regex), None)
-                              .otherwise(F.col(col)))
-                  )
-
-    df = (df
-          .withColumn(target_col,
-                      F.when(F.col(target_col).rlike(regex), None)
-                      .otherwise(F.col(target_col)))
-          )
-
-    return df
-
-################################################################################
-
-
-def age_at(df, birth_date, in_date_format='yyyy-MM-dd', *age_at_dates):
-    """
-    Calculates individuals' ages at specified dates.
-
-
-    From a reference Date of Birth column, the function takes
-    a list of dates, and for each date creates a new column
+    The function takes a list of dates, and for each date creates a new column
     specifying an individual's age at that date.
 
-    Need to import the standardise_date function first.
-
-
     Parameters
     ----------
     df : dataframe
       Dataframe to which the function is applied.
-    birth_date: string
+    reference_column: string
       The original date of birth column needed to calculate age.
-    in_date_format: default = 'yyyy-MM-dd',string
+    in_date_format: default = 'dd-MM-yyyy',string
       The date format of the date of birth column.
       It uses hyphens or forward slashes to split the date
       up and dd,MM,yyyy to show date month and year respectively.
       e.g. 'dd-MM-yyyy' , 'dd/MM/yyyy', 'yyyy-MM-dd'.
     *age_at_dates: list of strings
       The list of dates at which the user wants to calculate ages. Any
       number of dates can be given. The dates need to be in the
@@ -1414,26 +1393,43 @@
     |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|
     |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|
     +---+--------+----------+-------+----------+---+--------+
 
     > dates = ['2022-11-03','2020-12-25']
     > age_at(df,'DoB','yyyy-MM-dd',*dates).show()
-    +---+--------+----------+-------+----------+---+--------+-----------------+-----------------+
-    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|age_at_2022-11-03|age_at_2020-12-25|
-    +---+--------+----------+-------+----------+---+--------+-----------------+-----------------+
-    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|               39|               37|
-    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|               39|               37|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|               10|                8|
-    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|               10|                8|
-    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|                8|                6|
-    |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|                1|                0|
-    +---+--------+----------+-------+----------+---+--------+-----------------+-----------------+
+    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
+    | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|DoB_age_at_2022-11-03|DoB_age_at_2020-12-25|
+    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
+    |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ET74 2SP|                   39|                   37|
+    |  2|   Marge|    Juliet|Simpson|1983-03-19|  F|ET74 2SP|                   39|                   37|
+    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|                   10|                    8|
+    |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|                   10|                    8|
+    |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ET74 2SP|                    8|                    6|
+    |  5|  Maggie|      null|Simpson|2021-01-12|  F|ET74 2SP|                    1|                    0|
+    +---+--------+----------+-------+----------+---+--------+---------------------+---------------------+
 
     """
 
-    df = standardise_date(df, birth_date, in_date_format,
-                          out_date_format='yyyy-MM-dd')
+    df = df.withColumn(
+        f"{reference_col}_fmt", F.unix_timestamp(F.col(reference_col), in_date_format)
+    ).withColumn(
+        f"{reference_col}_fmt",
+        F.from_unixtime(F.col(f"{reference_col}_fmt"), "yyyy-MM-dd"),
+    )
+
     for age_at_date in age_at_dates:
-        df = df.withColumn(f"age_at_{age_at_date}", (F.months_between(
-            F.lit(age_at_date), F.col(birth_date),)/F.lit(12)).cast(IntegerType()))
+
+        df = df.withColumn(
+            f"{reference_col}_age_at_{age_at_date}",
+            (
+                F.months_between(
+                    F.lit(age_at_date),
+                    F.col(f"{reference_col}_fmt"),
+                )
+                / F.lit(12)
+            ).cast(IntegerType()),
+        )
+        
+    df = df.drop(f"{reference_col}_fmt")
+        
     return df
```

### Comparing `dlh_utils-0.3.0/dlh_utils/utilities.py` & `dlh_utils-0.3.1/dlh_utils/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,104 +1,78 @@
 '''
 Utility functions used to ease difficulty in querying databases and produce descriptive
 metrics about a dataframe
 '''
 import subprocess
+import os
+import re
 from pyspark.sql import SparkSession
-from pyspark.sql.types import *
+from pyspark.sql.types import TimestampType, LongType, IntegerType, DoubleType,\
+    FloatType, StringType, StructType, StructField
 import pyspark.sql.functions as F
 from pyspark.context import SparkContext as sc
-import pandas as pd
-import os
-import errno
-import re
 from dlh_utils import dataframes as da
-from dlh_utils import utilities as ut
 
 ###############################################################################
 
 
-def list_files(directory, walk=False):
+def list_files(file_path, walk=False, regex=None, full_path=True):
     """
     Lists files in a given HDFS directory, and/or all of that directory's
     subfolders if specified
 
 
     Parameters
     ----------
-    directory : str
+    file_path : str
       String path of directory
     walk : boolean {True, False}
       Lists files only in immediate directory specified if walk = False.
       Lists all files in immediate directory and all subfolders if Walk = True
+    regex : str
+      use regex rexpression to find certain words within the listed files
+    full_path : boolean
+      show full file path is full_path = True
+      show just files if full_path = False
 
     Returns
     -------
     list
       List of files
 
-    Raises
-    -------
-      None at present.
-
-    Example
-    -------
-    > list_files(directory = '/dev/kicktyres/',walk=False)
-
-    ['hdfs://prod1/dev/kicktyres/hive_tables',
-     'hdfs://prod1/dev/kicktyres/shakes',
-     'hdfs://prod1/dev/kicktyres/shakes_count',
-     'hdfs://prod1/dev/kicktyres/timings_tables']
-
-    > list_files(directory = '/dev/kicktyres/',walk=True)
-
-    ['hdfs://prod1/dev/kicktyres/shakes_count/part-r-00111',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00164',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00190',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00039',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00202',
-     'hdfs://prod1/dev/kicktyres/shakes',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00036',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00183',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00193',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00128',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00005',
-     'hdfs://prod1/dev/kicktyres/shakes_count/part-r-00057',
-     ... and all other files contained within these sub-directories
 
     """
+    list_of_filenames = []
+    list_of_filename = []
 
-    URI = sc._gateway.jvm.java.net.URI
-    Path = sc._gateway.jvm.org.apache.hadoop.fs.Path
-    FileSystem = sc._gateway.jvm.org.apache.hadoop.fs.FileSystem
-    Configuration = sc._gateway.jvm.org.apache.hadoop.conf.Configuration
-
-    host = 'user'
-
-    fs = FileSystem.get(URI(host), Configuration())
-
-    status = fs.listStatus(Path(directory))
-
-    files = [str(fileStatus.getPath()) for fileStatus in status]
-
-    if walk == False:
-
-        return files
-
+    if walk == True:
+        process = subprocess.Popen(["hadoop","fs", "-ls", "-R", file_path]\
+                                   ,stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     else:
+        process = subprocess.Popen(["hadoop","fs", "-ls", "-C", file_path]\
+                                   ,stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
-        for file in files:
-            if len(files) == len(set(files)):
-                files.extend(list_files(file))
-            else:
-                break
+    std_out, std_error = process.communicate()
+    std_out = str(std_out).split("\\n")[:-1]
+    std_out[0] = std_out[0].strip("b'")
+
+    if full_path == True:
+        for i in std_out:
+            file_name = str(i).split(' ')[-1]
+            list_of_filenames.append(file_name)
+
+    elif full_path == False:
+        for i in std_out:
+            file_name = str(i).split('/')[-1]
+            list_of_filenames.append(file_name)  
 
-        files = list(set(files))
+    if regex != None:
+        list_of_filenames = list(filter(re.compile(regex).search, list_of_filenames))
 
-        return files
+    return list_of_filenames
 
 ###############################################################################
 
 
 def list_checkpoints(checkpoint):
     """
     Lists checkpoints in HDFS directory
@@ -118,15 +92,16 @@
       None at present.
 
     Example
     -------
 
     > list_checkpoints(checkpoint = '/user/edwara5/checkpoints')
 
-['hdfs://prod1/user/edwara5/checkpoints/0299d46e-96ad-4d3a-9908-c99b9c6a7509/connected-components-985ca288']
+    ['hdfs://prod1/user/checkpoints/0299d46e-96ad-4d3a-9908-\
+    c99b9c6a7509/connected-components-985ca288']
     """
 
     return list_files(
         list_files(checkpoint, walk=False)[0])
 
 ###############################################################################
 
@@ -211,15 +186,15 @@
 
     ('baby_names.bv_girl_names_std', 'hive')
     """
 
     # pass spark context to function
     spark = SparkSession.builder.getOrCreate()
 
-    if regex == None:
+    if regex is None:
 
         if filetype == 'hive':
 
             try:
 
                 # list all tables in directory
                 tables = spark.sql(
@@ -229,32 +204,32 @@
                 filepaths = tables.withColumn('path', F.concat(
                     F.lit(path), F.lit("."), F.col("tableName")))
 
                 # convert to list
                 filepaths = list(filepaths.select('path').toPandas()['path'])
 
                 # initialise empty dictionary
-                filepath_dict = dict()
+                filepath_dict = {}
 
                 # loop through paths, appending path and time to dictionary
-                for path in filepaths:
+                for filepath in filepaths:
 
                     time = spark.sql(
-                        f"SHOW tblproperties {path} ('transient_lastDdlTime')").collect()[0][0]
+                        f"SHOW tblproperties {filepath} ('transient_lastDdlTime')").collect()[0][0]
 
-                    filepath_dict.update({path: time})
+                    filepath_dict.update({filepath: time})
 
                 # sort by max time since epoch and return corresponding path
                 most_recent_filepath = max(
                     filepath_dict, key=filepath_dict.get)
 
-            except:
+            except Exception as exc:
 
                 raise FileNotFoundError(
-                    filetype + " file not found in this directory: " + path)
+                    filetype + " file not found in this directory: " + path) from exc
 
         # if filetype != hive
         else:
 
             # return all files in dir recursively, sorted by modification date (ascending),
             # decode from bytes-like to str
             files = subprocess.check_output(
@@ -269,33 +244,33 @@
 
                     # filter for .csv ext and take last element of list
                     result = [f for f in files if f.endswith('csv')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
-                except:
+                except Exception as exc:
 
                     raise FileNotFoundError(
-                        filetype + " file not found in this directory: " + path)
+                        filetype + " file not found in this directory: " + path) from exc
 
             elif filetype == 'parquet':
 
                 try:
 
                     # filter for .csv ext and take last element of list
                     result = [f for f in files if f.endswith('parquet')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
-                except:
+                except Exception as exc:
 
                     raise FileNotFoundError(
-                        filetype + " file not found in this directory: " + path)
+                        filetype + " file not found in this directory: " + path) from exc
 
     # if regex argument specified:
     else:
 
         if filetype == 'hive':
 
             try:
@@ -313,32 +288,32 @@
                     filepaths["path"].rlike(regex))
 
                 # convert to list
                 filtered_filepaths = list(
                     filtered_filepaths.select('path').toPandas()['path'])
 
                 # initialise empty dictionary
-                filepath_dict = dict()
+                filepath_dict = {}
 
                 # loop through paths, appending path and time to dict
-                for path in filtered_filepaths:
+                for filepath in filtered_filepaths:
 
                     time = spark.sql(
-                        f"SHOW tblproperties {path} ('transient_lastDdlTime')").collect()[0][0]
+                        f"SHOW tblproperties {filepath} ('transient_lastDdlTime')").collect()[0][0]
 
-                    filepath_dict.update({path: time})
+                    filepath_dict.update({filepath: time})
 
                 # sort by max time since epoch and return corresponding path
                 most_recent_filepath = max(
                     filepath_dict, key=filepath_dict.get)
 
-            except:
+            except Exception as exc:
 
-                raise FileNotFoundError(filetype + " file, matching this regular expression: " + 
-                                        regex + " not found in this directory: " + path)
+                raise FileNotFoundError(filetype + " file, matching this regular expression: " +
+                                        regex + " not found in this directory: " + path) from exc
 
         # if filetype != hive
         else:
 
             # return all files in dir recursively, sorted by modification date (ascending),
             # decode from bytes-like to str
             files = subprocess.check_output(
@@ -359,42 +334,46 @@
                     # filter for .csv ext and take last element of list
                     result = [
                         f for f in filtered_files if f.endswith('csv')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
-                except:
+                except Exception as exc:
 
-                    raise FileNotFoundError(filetype + " file, matching this regular expression: " 
-                                            + regex + " not found in this directory: " + path)
+                    raise FileNotFoundError(filetype +
+                                            " file, matching this regular expression: " +
+                                            regex + " not found in this directory: " +
+                                            path) from exc
 
             elif filetype == 'parquet':
 
                 try:
 
                     # filter for .csv ext and take last element of list
                     result = [
                         f for f in filtered_files if f.endswith('parquet')][-1]
 
                     # return path up until last '/'
                     most_recent_filepath = re.search('.*\/', result).group(0)
 
-                except:
+                except Exception as exc:
 
-                    raise FileNotFoundError(filetype + " file, matching this regular expression: " 
-                                            + regex + " not found in this directory: " + path)
+                    raise FileNotFoundError(filetype +
+                                            " file, matching this regular expression: " +
+                                            regex + " not found in this directory: " +
+                                            path) from exc
 
     return most_recent_filepath, filetype
 
 ###############################################################################
 
 
 def write_format(df, write, path,
-                file_name=None, sep=",", header="true", mode='overwrite'):
+                 file_name=None, sep=",", header="true", mode='overwrite'):
     """
     Writes dataframe in specified format
 
     Can write data to HDFS in csv or parquet format and to database in hive table
     format.
 
     Parameters
@@ -427,38 +406,39 @@
 
     Example
     -------
 
     > write_format(df = df, write = 'parquet', path = 'user/edwara5/simpsons.parquet',
                   mode = 'overwrite')
     """
+
     spark = SparkSession.builder.getOrCreate()
-    if file_name == None:
+    if file_name is None:
         if write == 'csv':
             df.write.format('csv').option('header', header).mode(
                 mode).option('sep', sep).save(f'{path}')
         if write == 'parquet':
-            df.write.parquet(path=f'{path}', mode=mode)    
+            df.write.parquet(path=f'{path}', mode=mode)
         if write == 'hive':
-          df.write.mode('overwrite').saveAsTable(f'{path}')
-        
+            df.write.mode('overwrite').saveAsTable(f'{path}')
+
     else:
         if write == 'csv':
             df.write.format('csv').option('header', header).mode(
                 mode).option('sep', sep).save(f'{path}/{file_name}')
         if write == 'parquet':
             df.write.parquet(path=f'{path}/{file_name}', mode=mode)
         if write == 'hive':
             df.write.mode("overwrite").saveAsTable(f'{path}.{file_name}')
 
 ###############################################################################
 
 
 def read_format(read, path=None, file_name=None,
-               sep=",", header="true", inferSchema="True"):
+                sep=",", header="true", infer_schema="True"):
     """
     Reads dataframe from specified format.
 
     Can read from HDFS in csv or parquet format and from database hive table
     format.
 
     Parameters
@@ -471,17 +451,15 @@
       The file or table name from which dataframe is to be read. Note that if
       None, function will read from HDFS path specified in case of csv
       or parquet
     sep : str
       specified separator for data in csv format
     header : {"true", "false"} (default = "true")
       Boolean indicating whether or not data will be read to include a header
-    mode : {overwrite, append}, default = overwrite
-      Choice to overwrite existing file or table or to append new data into it
-    inferSchema : {"true", "false"}:
+    infer_schema : {"true", "false"}:
       Boolean indicating whether data should be read with infered data types and
       schema. If false, all data will read as string format.
 
     Returns
     -------
     dataframe
       Dataframe of data read from specified path and format
@@ -490,15 +468,15 @@
     -------
       None at present.
 
     Example
     -------
 
     > df = read_format(read = 'parquet', path = '/user/edwara5/simpsons.parquet',
-                      file_name = None, header= "true", inferSchema = "True")
+                      file_name = None, header= "true", infer_schema = "True")
 
     > df.show()
 
     +---+--------+----------+-------+----------+---+--------+
     | ID|Forename|Middlename|Surname|       DoB|Sex|Postcode|
     +---+--------+----------+-------+----------+---+--------+
     |  1|   Homer|       Jay|Simpson|1983-05-12|  M|ZZ99 9SZ|
@@ -506,43 +484,43 @@
     |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  3|    Bart|     Jo-Jo|Simpson|2012-04-01|  M|ET74 2SP|
     |  4|    Lisa|     Marie|Simpson|2014-05-09|  F|ZZ99 2SP|
     |  5|  Maggie|      null|Simpson|2021-01-12|  F|ZZ99 2FA|
     +---+--------+----------+-------+----------+---+--------+
     """
     spark = SparkSession.builder.getOrCreate()
-    if file_name == None:
+    if file_name is None:
         if read == 'csv':
             df = (spark.read.format('csv')
                   .option('sep', sep)
                   .option('header', header)
-                  .option('inferSchema', inferSchema)
+                  .option('inferSchema', infer_schema)
                   .load(f"{path}")
                   )
         if read == 'parquet':
             df = (spark.read.format('parquet')
                   .option('header', header)
-                  .option('inferSchema', inferSchema)
+                  .option('inferSchema', infer_schema)
                   .load(f"{path}")
                   )
         if read == 'hive':
             df = spark.sql(f"SELECT * FROM {path}")
-        
+
     else:
         if read == 'csv':
             df = (spark.read.format('csv')
                   .option('sep', sep)
                   .option('header', header)
-                  .option('inferSchema', inferSchema)
+                  .option('inferSchema', infer_schema)
                   .load(f"{path}/{file_name}")
                   )
         if read == 'parquet':
             df = (spark.read.format('parquet')
                   .option('header', header)
-                  .option('inferSchema', inferSchema)
+                  .option('inferSchema', infer_schema)
                   .load(f"{path}/{file_name}")
                   )
         if read == 'hive':
             df = spark.sql(f"SELECT * FROM {path}.{file_name}")
 
     return df
 
@@ -580,29 +558,29 @@
 
     """
     files_in_dir = os.listdir(path)
     diction = {}  # try empty dictionary
 
     for file in files_in_dir:
         count = 0
-        countList = []
+        count_list = []
 
         try:
             with open(f'{path}/{file}') as f:
                 datafile = f.readlines()
 
             for line in datafile:
                 count = count + 1
 
                 if string in line:
-                    countList.append(count)
+                    count_list.append(count)
 
-            if len(countList) != 0:
-                diction[file] = countList
-        except:
+            if len(count_list) != 0:
+                diction[file] = count_list
+        except IsADirectoryError:
             continue
 
     return diction
 
 ###############################################################################
 
 
@@ -634,25 +612,25 @@
     ------
     None at present.
 
     Example
     -------
     > describe_metrics(df = df,output_mode='spark').show()
 
-    +----------+------+-----+--------+------------------+----+------------------+--------+-----------------+
-    |  variable|  type|count|distinct|  percent_distinct|null|      percent_null|not_null| percent_not_null|
-    +----------+------+-----+--------+------------------+----+------------------+--------+-----------------+
-    |        ID|string|    6|       5| 83.33333333333334|   0|               0.0|       6|            100.0|
-    |  Forename|string|    6|       5| 83.33333333333334|   0|               0.0|       6|            100.0|
-    |Middlename|string|    6|       4| 66.66666666666666|   1|16.666666666666664|       5|83.33333333333334|
-    |   Surname|string|    6|       1|16.666666666666664|   0|               0.0|       6|            100.0|
-    |       DoB|string|    6|       5| 83.33333333333334|   0|               0.0|       6|            100.0|
-    |       Sex|string|    6|       2| 33.33333333333333|   0|               0.0|       6|            100.0|
-    |  Postcode|string|    6|       1|16.666666666666664|   0|               0.0|       6|            100.0|
-    +----------+------+-----+--------+------------------+----+------------------+--------+-----------------+
+    +----------+------+-----+--------+----------------+----+------------+--------+----------------+
+    |  variable|  type|count|distinct|percent_distinct|null|percent_null|not_null|percent_not_null|
+    +----------+------+-----+--------+----------------+----+------------+--------+----------------+
+    |        ID|string|    6|       5| 83.333333333334|   0|         0.0|       6|           100.0|
+    |  Forename|string|    6|       5| 83.333333333334|   0|         0.0|       6|           100.0|
+    |Middlename|string|    6|       4| 66.666666666666|   1|16.666666664|       5| 83.333333333334|
+    |   Surname|string|    6|       1|16.6666666666664|   0|         0.0|       6|           100.0|
+    |       DoB|string|    6|       5| 83.333333333334|   0|         0.0|       6|           100.0|
+    |       Sex|string|    6|       2| 33.333333333333|   0|         0.0|       6|           100.0|
+    |  Postcode|string|    6|       1|16.6666666666664|   0|         0.0|       6|           100.0|
+    +----------+------+-----+--------+----------------+----+------------+--------+----------------+
     """
 
     spark = SparkSession.builder.getOrCreate()
 
     distinct_df = (df
                    .agg(*(F.countDistinct(F.col(c)).alias(c) for c in df.columns))
                    .withColumn('summary', F.lit('distinct')))
@@ -690,15 +668,15 @@
         'null',
         'percent_null',
         'not_null',
         'percent_not_null'
     ]]
 
     if output_mode == 'spark':
-        decribe_df = ut.pandas_to_spark(decribe_df)
+        decribe_df = pandas_to_spark(decribe_df)
 
     return decribe_df
 
 ###############################################################################
 
 
 def value_counts(df, limit=20, output_mode='pandas'):
@@ -1013,40 +991,39 @@
     df
       A spark dataframe
 
     Raises
     ------
     None at present.
     """
-    def equivalent_type(f):
+    def equivalent_type(_format):
 
-        if f == 'datetime64[ns]':
+        if _format == 'datetime64[ns]':
             return TimestampType()
 
-        elif f == 'int64':
+        if _format == 'int64':
             return LongType()
 
-        elif f == 'int32':
+        if _format == 'int32':
             return IntegerType()
 
-        elif f == 'float64':
+        if _format == 'float64':
             return DoubleType()
 
-        elif f == 'float32':
+        if _format == 'float32':
             return FloatType()
 
-        else:
-            return StringType()
+        return StringType()
 
     def define_structure(string, format_type):
 
         try:
             vartype = equivalent_type(format_type)
 
-        except:
+        except TypeError:
             vartype = StringType()
 
         return StructField(string, vartype)
 
     spark = SparkSession.builder.getOrCreate()
 
     columns = list(pandas_df.columns)
```

### Comparing `dlh_utils-0.3.0/pyproject.toml` & `dlh_utils-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlh_utils"
-version = "0.3.0"
+version = "0.3.1"
 description = "A PySpark package used to expedite and standardise the data linkage process"
 authors = ["Anthony Edwards <anthonygedwards93@gmail.com>", "Jenna Hart", "David Cobbledick", "Madalina Iova", "Dean Jathoonia"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "dlh_utils"}]
 homepage = "https://github.com/Data-Linkage/dlh_utils"
 repository = "https://github.com/Data-Linkage/dlh_utils"
```

### Comparing `dlh_utils-0.3.0/PKG-INFO` & `dlh_utils-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlh-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: A PySpark package used to expedite and standardise the data linkage process
 Home-page: https://github.com/Data-Linkage/dlh_utils
 License: MIT
 Author: Anthony Edwards
 Author-email: anthonygedwards93@gmail.com
 Requires-Python: >=3.6.8
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,18 @@
 ```sh
 pip install dlh_utils
 ```
 Or, if using CDSW, in a terminal session run:
 ```sh
 pip3 install dlh_utils
 ```
+The -U argument can be used to upgrade the package to its newest version:
+```sh
+pip3 install -U dlh_utils
+```
 
 ## Demo
 For a worked demonstration notebook of these functions being applied within a data linkage context, head over to our [separate demo repository](https://github.com/anthonye93/dlh_utils_demo)
 
 ## Common issues
 
 ### When using the jaro/jaro_winkler functions the error "no module called Jellyfish found" is thrown
@@ -78,7 +82,11 @@
 spark.conf.set('spark.jars', path_to_jar_file)
 ```
 
 ## Thanks
 
 Thanks to all those in the Data Linkage Hub, Data Engineering and Methodology at ONS that have contributed towards this repository.
 
+## Any questions?
+
+If you need any additional help, or have any feedback on the package, please contact Jenna Hart (Jenna.Hart@ons.gov.uk) or the Data Linkage Hub at Linkage.Hub@ons.gov.uk . 
+
```

