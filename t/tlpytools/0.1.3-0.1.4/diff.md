# Comparing `tmp/tlpytools-0.1.3.tar.gz` & `tmp/tlpytools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlpytools-0.1.3.tar", last modified: Thu Nov 10 17:53:02 2022, max compression
+gzip compressed data, was "tlpytools-0.1.4.tar", last modified: Wed Apr 26 18:37:24 2023, max compression
```

## Comparing `tlpytools-0.1.3.tar` & `tlpytools-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 17:53:02.920595 tlpytools-0.1.3/
--rw-rw-rw-   0        0        0     3082 2022-11-10 17:53:02.922604 tlpytools-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2022-11-10 17:35:17.000000 tlpytools-0.1.3/README.md
--rw-rw-rw-   0        0        0      293 2022-11-09 23:54:35.000000 tlpytools-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      730 2022-11-10 17:53:02.931157 tlpytools-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-10 17:53:02.388080 tlpytools-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2022-11-10 17:53:02.843566 tlpytools-0.1.3/src/tlpytools/
--rw-rw-rw-   0        0        0        0 2021-09-24 22:31:24.000000 tlpytools-0.1.3/src/tlpytools/__init__.py
--rw-rw-rw-   0        0        0     3895 2022-11-10 17:34:41.000000 tlpytools-0.1.3/src/tlpytools/config.py
--rw-rw-rw-   0        0        0    19352 2022-02-07 22:05:26.000000 tlpytools-0.1.3/src/tlpytools/data.py
--rw-rw-rw-   0        0        0     2128 2021-09-27 22:47:24.000000 tlpytools-0.1.3/src/tlpytools/log.py
-drwxrwxrwx   0        0        0        0 2022-11-10 17:53:02.890392 tlpytools-0.1.3/src/tlpytools.egg-info/
--rw-rw-rw-   0        0        0     3082 2022-11-10 17:53:01.000000 tlpytools-0.1.3/src/tlpytools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2022-11-10 17:53:01.000000 tlpytools-0.1.3/src/tlpytools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 17:53:01.000000 tlpytools-0.1.3/src/tlpytools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2022-11-10 17:53:01.000000 tlpytools-0.1.3/src/tlpytools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-26 18:37:24.815843 tlpytools-0.1.4/
+-rw-rw-rw-   0        0        0     3082 2023-04-26 18:37:24.815843 tlpytools-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-04-26 09:40:17.000000 tlpytools-0.1.4/README.md
+-rw-rw-rw-   0        0        0      293 2023-04-26 16:38:48.000000 tlpytools-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      730 2023-04-26 18:37:24.818361 tlpytools-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-26 18:37:24.772652 tlpytools-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-26 18:37:24.799223 tlpytools-0.1.4/src/tlpytools/
+-rw-rw-rw-   0        0        0        0 2023-04-26 00:27:33.000000 tlpytools-0.1.4/src/tlpytools/__init__.py
+-rw-rw-rw-   0        0        0     3895 2023-04-26 09:34:12.000000 tlpytools-0.1.4/src/tlpytools/config.py
+-rw-rw-rw-   0        0        0    19436 2023-04-26 09:48:13.000000 tlpytools-0.1.4/src/tlpytools/data.py
+-rw-rw-rw-   0        0        0     2128 2023-04-26 00:27:33.000000 tlpytools-0.1.4/src/tlpytools/log.py
+drwxrwxrwx   0        0        0        0 2023-04-26 18:37:24.813372 tlpytools-0.1.4/src/tlpytools.egg-info/
+-rw-rw-rw-   0        0        0     3082 2023-04-26 18:37:24.000000 tlpytools-0.1.4/src/tlpytools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-04-26 18:37:24.000000 tlpytools-0.1.4/src/tlpytools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 18:37:24.000000 tlpytools-0.1.4/src/tlpytools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 18:37:24.000000 tlpytools-0.1.4/src/tlpytools.egg-info/top_level.txt
```

### Comparing `tlpytools-0.1.3/PKG-INFO` & `tlpytools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlpytools
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of tools for building models at the TransLink Forecasting Team
 Home-page: https://github.com/TransLinkForecasting/tlpytools
 Author: Forecasting TransLink
 Author-email: forecasting@translink.ca
 Project-URL: Bug Tracker, https://github.com/TransLinkForecasting/tlpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 Build and install from source allow you to access the latest version or a specific version without any available precompiled wheels:
 
 ```bash
 git clone https://github.com/TransLinkForecasting/tlpytools.git --depth=1
 cd tlpytools
 python -m pip install --upgrade build
 python -m build
-pip install dist/tlpytools-0.1.3-py3-none-any.whl --upgrade --force-reinstall
+pip install dist/tlpytools-0.1.4-py3-none-any.whl --upgrade --force-reinstall
 ```
 
 ### Method 3: editable install for development
 
 If you are developing and testing tlpytools to work with downstream code, you may install the package as an [editable install](https://pip.pypa.io/en/stable/cli/pip_install/?highlight=edit%20mode#editable-installs). This allows you to continuously make changes to the `tlpytools` package in your local development folder, while integrating these changes in real time with your downstream code.
 
 ```bash
```

### Comparing `tlpytools-0.1.3/README.md` & `tlpytools-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 Build and install from source allow you to access the latest version or a specific version without any available precompiled wheels:
 
 ```bash
 git clone https://github.com/TransLinkForecasting/tlpytools.git --depth=1
 cd tlpytools
 python -m pip install --upgrade build
 python -m build
-pip install dist/tlpytools-0.1.3-py3-none-any.whl --upgrade --force-reinstall
+pip install dist/tlpytools-0.1.4-py3-none-any.whl --upgrade --force-reinstall
 ```
 
 ### Method 3: editable install for development
 
 If you are developing and testing tlpytools to work with downstream code, you may install the package as an [editable install](https://pip.pypa.io/en/stable/cli/pip_install/?highlight=edit%20mode#editable-installs). This allows you to continuously make changes to the `tlpytools` package in your local development folder, while integrating these changes in real time with your downstream code.
 
 ```bash
```

### Comparing `tlpytools-0.1.3/setup.cfg` & `tlpytools-0.1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6c70 7974 6f6f 6c73 0d0a 7665   = tlpytools..ve
-00000020: 7273 696f 6e20 3d20 302e 312e 330d 0a61  rsion = 0.1.3..a
+00000020: 7273 696f 6e20 3d20 302e 312e 340d 0a61  rsion = 0.1.4..a
 00000030: 7574 686f 7220 3d20 466f 7265 6361 7374  uthor = Forecast
 00000040: 696e 6720 5472 616e 734c 696e 6b0d 0a61  ing TransLink..a
 00000050: 7574 686f 725f 656d 6169 6c20 3d20 666f  uthor_email = fo
 00000060: 7265 6361 7374 696e 6740 7472 616e 736c  recasting@transl
 00000070: 696e 6b2e 6361 0d0a 6465 7363 7269 7074  ink.ca..descript
 00000080: 696f 6e20 3d20 4120 7365 7420 6f66 2074  ion = A set of t
 00000090: 6f6f 6c73 2066 6f72 2062 7569 6c64 696e  ools for buildin
```

### Comparing `tlpytools-0.1.3/src/tlpytools/config.py` & `tlpytools-0.1.4/src/tlpytools/config.py`

 * *Files identical despite different names*

### Comparing `tlpytools-0.1.3/src/tlpytools/data.py` & `tlpytools-0.1.4/src/tlpytools/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,15 @@
                                                              salt=salt)
         elif source == 'server':
             engine = sql.create_engine(
                 "mssql+pyodbc://SAVONA/TL_RESEARCH_ANALYTICS_DEV?driver=SQL Server")
 
             # build reference of db tables
             query = 'SELECT SCHEMA_NAME(schema_id) AS schema_name,* FROM sys.tables ;'
-            ref_tables = pd.read_sql_query(query, engine)
+            ref_tables = pd.read_sql_query(con=engine.connect(), sql=sql.text(query))
             ref_tables = ref_tables.sort_values(by=["schema_id", "schema_name", "name"])
 
             # filter selected schema and table
             if schema != '':
                 ref_tables = ref_tables[ref_tables['schema_name'] == schema]
             if table != None:
                 ref_tables = ref_tables[ref_tables['name'] == table]
@@ -325,15 +325,15 @@
             # query data into df dict
             for index, data in ref_tables.iterrows():
                 db_table = "[{schema}].[{table}]".format(schema=data['schema_name'],
                                                          table=data['name'])
                 table_name = "{}.{}".format(data['schema_name'], data['name'])
                 print("Reading table from sql server " + db_table + 20 * " ", end="\r")
                 query = 'SELECT * FROM {db_tbl};'.format(db_tbl=db_table)
-                db_table_df = pd.read_sql_query(query, engine)
+                db_table_df = pd.read_sql_query(con=engine.connect(), sql=sql.text(query))
                 df_dict[table_name] = db_table_df
 
         else:
             raise ValueError('source must be either local or server')
         print('\n')  # make a new line for future print
         return (df_dict)
 
@@ -407,11 +407,11 @@
     @staticmethod
     def export_tbl_list(csv_file="savona.sys.tables.csv"):
         # engine = sql.create_engine(
         #     "mssql+pyodbc://SAVONA/TL_RESEARCH_ANALYTICS_DEV?driver=SQL+Server+Native+Client+11.0")
         engine = sql.create_engine(
             "mssql+pyodbc://SAVONA/TL_RESEARCH_ANALYTICS_DEV?driver=SQL Server")
         query = 'SELECT SCHEMA_NAME(schema_id) AS schema_name,* FROM sys.tables ;'
-        all_tables = pd.read_sql_query(query, engine)
+        all_tables = pd.read_sql_query(con=engine.connect(), sql=sql.text(query))
         all_tables = all_tables.sort_values(by=["schema_id", "schema_name", "name"])
         all_tables.insert(loc=0, column='extract', value=0)
         all_tables.to_csv(csv_file, index=False)
```

### Comparing `tlpytools-0.1.3/src/tlpytools/log.py` & `tlpytools-0.1.4/src/tlpytools/log.py`

 * *Files identical despite different names*

### Comparing `tlpytools-0.1.3/src/tlpytools.egg-info/PKG-INFO` & `tlpytools-0.1.4/src/tlpytools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tlpytools
-Version: 0.1.3
+Version: 0.1.4
 Summary: A set of tools for building models at the TransLink Forecasting Team
 Home-page: https://github.com/TransLinkForecasting/tlpytools
 Author: Forecasting TransLink
 Author-email: forecasting@translink.ca
 Project-URL: Bug Tracker, https://github.com/TransLinkForecasting/tlpytools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,15 +33,15 @@
 Build and install from source allow you to access the latest version or a specific version without any available precompiled wheels:
 
 ```bash
 git clone https://github.com/TransLinkForecasting/tlpytools.git --depth=1
 cd tlpytools
 python -m pip install --upgrade build
 python -m build
-pip install dist/tlpytools-0.1.3-py3-none-any.whl --upgrade --force-reinstall
+pip install dist/tlpytools-0.1.4-py3-none-any.whl --upgrade --force-reinstall
 ```
 
 ### Method 3: editable install for development
 
 If you are developing and testing tlpytools to work with downstream code, you may install the package as an [editable install](https://pip.pypa.io/en/stable/cli/pip_install/?highlight=edit%20mode#editable-installs). This allows you to continuously make changes to the `tlpytools` package in your local development folder, while integrating these changes in real time with your downstream code.
 
 ```bash
```

