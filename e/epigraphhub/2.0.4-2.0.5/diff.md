# Comparing `tmp/epigraphhub-2.0.4.tar.gz` & `tmp/epigraphhub-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epigraphhub-2.0.4.tar", max compression
+gzip compressed data, was "epigraphhub-2.0.5.tar", max compression
```

## Comparing `epigraphhub-2.0.4.tar` & `epigraphhub-2.0.5.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    32471 2023-03-14 22:10:29.449278 epigraphhub-2.0.4/LICENSE
--rw-r--r--   0        0        0     4048 2023-03-14 22:10:29.449278 epigraphhub-2.0.4/README.md
--rw-r--r--   0        0        0      400 2023-03-14 22:12:54.295102 epigraphhub-2.0.4/epigraphhub/__init__.py
--rw-r--r--   0        0        0     1504 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/__main__.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/__init__.py
--rw-r--r--   0        0        0     9890 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/clustering.py
--rw-r--r--   0        0        0     2935 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/epistats.py
--rw-r--r--   0        0        0    27199 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/lstm_models.py
--rw-r--r--   0        0        0     2476 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/metrics.py
--rw-r--r--   0        0        0    13119 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/ngboost_models.py
--rw-r--r--   0        0        0     3350 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/plots.py
--rw-r--r--   0        0        0     7195 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/sklearn_models.py
--rw-r--r--   0        0        0     6939 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/preprocessing.py
--rw-r--r--   0        0        0       57 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/analysis/rtestim.py
--rw-r--r--   0        0        0     1927 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/connection.py
--rw-r--r--   0        0        0      137 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/.env
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/__init__.py
--rw-r--r--   0        0        0     1041 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/_config.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/brasil/__init__.py
--rw-r--r--   0        0        0      372 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/__init__.py
--rw-r--r--   0        0        0     1032 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/extract.py
--rw-r--r--   0        0        0     1802 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/loading.py
--rw-r--r--   0        0        0     1488 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/viz.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/colombia/__init__.py
--rw-r--r--   0        0        0     2619 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/colombia/extract.py
--rw-r--r--   0        0        0     4432 2023-03-14 22:10:29.777282 epigraphhub-2.0.4/epigraphhub/data/colombia/loading.py
--rw-r--r--   0        0        0     4378 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/epigraphhub_db.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/foph/__init__.py
--rw-r--r--   0        0        0     3281 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/foph/extract.py
--rw-r--r--   0        0        0     3888 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/foph/loading.py
--rw-r--r--   0        0        0     1513 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/foph/transform.py
--rw-r--r--   0        0        0     6680 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/foph/viz.py
--rw-r--r--   0        0        0      981 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/geoupload.py
--rw-r--r--   0        0        0     3026 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/ggtrends.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/owid/__init__.py
--rw-r--r--   0        0        0     3194 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/owid/extract.py
--rw-r--r--   0        0        0     2415 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/owid/loading.py
--rw-r--r--   0        0        0     2212 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/owid/transform.py
--rw-r--r--   0        0        0     4162 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/sinan_fetch.py
--rw-r--r--   0        0        0     7924 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/worldbank.py
--rw-r--r--   0        0        0     2346 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/data/worldpop.py
--rw-r--r--   0        0        0     1377 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/settings.py
--rw-r--r--   0        0        0        0 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/utils/__init__.py
--rw-r--r--   0        0        0     2287 2023-03-14 22:10:29.781282 epigraphhub-2.0.4/epigraphhub/utils/_config.py
--rw-r--r--   0        0        0     4621 2023-03-14 22:12:54.299103 epigraphhub-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 epigraphhub-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0    32471 2023-04-26 14:02:54.817961 epigraphhub-2.0.5/LICENSE
+-rw-r--r--   0        0        0     4048 2023-04-26 14:02:54.817961 epigraphhub-2.0.5/README.md
+-rw-r--r--   0        0        0      400 2023-04-26 14:05:17.298549 epigraphhub-2.0.5/epigraphhub/__init__.py
+-rw-r--r--   0        0        0     1504 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/__init__.py
+-rw-r--r--   0        0        0     9890 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/clustering.py
+-rw-r--r--   0        0        0     2935 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/epistats.py
+-rw-r--r--   0        0        0    27199 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/lstm_models.py
+-rw-r--r--   0        0        0     2476 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/metrics.py
+-rw-r--r--   0        0        0    13119 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/ngboost_models.py
+-rw-r--r--   0        0        0     3350 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/plots.py
+-rw-r--r--   0        0        0     7195 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/sklearn_models.py
+-rw-r--r--   0        0        0     6939 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/preprocessing.py
+-rw-r--r--   0        0        0       57 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/analysis/rtestim.py
+-rw-r--r--   0        0        0     1927 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/connection.py
+-rw-r--r--   0        0        0      137 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/.env
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/__init__.py
+-rw-r--r--   0        0        0     1115 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/_config.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/brasil/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/__init__.py
+-rw-r--r--   0        0        0     1032 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/extract.py
+-rw-r--r--   0        0        0     1802 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/loading.py
+-rw-r--r--   0        0        0     1488 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/viz.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/colombia/__init__.py
+-rw-r--r--   0        0        0     2619 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/colombia/extract.py
+-rw-r--r--   0        0        0     4432 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/colombia/loading.py
+-rw-r--r--   0        0        0     4378 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/epigraphhub_db.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/__init__.py
+-rw-r--r--   0        0        0     5945 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/extract.py
+-rw-r--r--   0        0        0     3904 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/loading.py
+-rw-r--r--   0        0        0   332068 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/schema.json
+-rw-r--r--   0        0        0     1503 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/transform.py
+-rw-r--r--   0        0        0     6680 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/foph/viz.py
+-rw-r--r--   0        0        0      981 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/geoupload.py
+-rw-r--r--   0        0        0     3026 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/ggtrends.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/owid/__init__.py
+-rw-r--r--   0        0        0     3194 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/owid/extract.py
+-rw-r--r--   0        0        0     2415 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/owid/loading.py
+-rw-r--r--   0        0        0     2212 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/owid/transform.py
+-rw-r--r--   0        0        0     4162 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/sinan_fetch.py
+-rw-r--r--   0        0        0     7924 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/worldbank.py
+-rw-r--r--   0        0        0     2346 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/data/worldpop.py
+-rw-r--r--   0        0        0     1377 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/settings.py
+-rw-r--r--   0        0        0        0 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/utils/__init__.py
+-rw-r--r--   0        0        0     2287 2023-04-26 14:02:55.145962 epigraphhub-2.0.5/epigraphhub/utils/_config.py
+-rw-r--r--   0        0        0     4719 2023-04-26 14:05:17.302549 epigraphhub-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     6290 1970-01-01 00:00:00.000000 epigraphhub-2.0.5/PKG-INFO
```

### Comparing `epigraphhub-2.0.4/LICENSE` & `epigraphhub-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/README.md` & `epigraphhub-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/__main__.py` & `epigraphhub-2.0.5/epigraphhub/__main__.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/clustering.py` & `epigraphhub-2.0.5/epigraphhub/analysis/clustering.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/epistats.py` & `epigraphhub-2.0.5/epigraphhub/analysis/epistats.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/lstm_models.py` & `epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/lstm_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/metrics.py` & `epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/metrics.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/ngboost_models.py` & `epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/ngboost_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/plots.py` & `epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/plots.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/forecast_models/sklearn_models.py` & `epigraphhub-2.0.5/epigraphhub/analysis/forecast_models/sklearn_models.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/analysis/preprocessing.py` & `epigraphhub-2.0.5/epigraphhub/analysis/preprocessing.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/connection.py` & `epigraphhub-2.0.5/epigraphhub/connection.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/_config.py` & `epigraphhub-2.0.5/epigraphhub/data/_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 COLOMBIA_CLIENT = Socrata("www.datos.gov.co", "078u4PCGpnDfH157kAkVFoWea")
 
 
 # Federal Office of Public Health (FOPH) COVID data config:
 FOPH_LOG_PATH = "/tmp/foph_fetch.log"
 FOPH_URL = "https://www.covid19.admin.ch/api/data/context"
 FOPH_CSV_PATH = "/tmp/foph/releases"
+FOPH_METADATA_URL = "https://www.covid19.admin.ch/api/data/documentation"
 
 
 # Our World in Data (OWID) COVID data config:
 OWID_LOG_PATH = "/tmp/owid_fetch.log"
 OWID_CSV_URL = "https://covid.ourworldindata.org/data/owid-covid-data.csv"
 OWID_CSV_PATH = "/tmp/owid/releases"
 OWID_FILENAME = OWID_CSV_URL.split("/")[-1]
```

### Comparing `epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/extract.py` & `epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/loading.py` & `epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/brasil/sinan/viz.py` & `epigraphhub-2.0.5/epigraphhub/data/brasil/sinan/viz.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/colombia/extract.py` & `epigraphhub-2.0.5/epigraphhub/data/colombia/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/colombia/loading.py` & `epigraphhub-2.0.5/epigraphhub/data/colombia/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/epigraphhub_db.py` & `epigraphhub-2.0.5/epigraphhub/data/epigraphhub_db.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/foph/loading.py` & `epigraphhub-2.0.5/epigraphhub/data/foph/loading.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,53 +18,53 @@
 from loguru import logger
 from pangres import upsert
 
 from epigraphhub.connection import get_engine
 from epigraphhub.data._config import FOPH_CSV_PATH, FOPH_LOG_PATH
 from epigraphhub.settings import env
 
-logger.add(FOPH_LOG_PATH, retention="7 days")
+logger.add(FOPH_LOG_PATH, retention='7 days')
 
 
 def upload(table, filename):
     """
     A generator responsible connecting and loading data
     retrieved from a CSV file into its respective table in
     the SQL Database, as defined in the connection configuration.
     @see epigraphhub.connection
 
     Args:
         table (str)    : Raw table name. Later parsed to SQL format.
         filename (str) : File name as defined in the CSV URL.
                          @see .download as above.
     """
-    new_df = pd.read_csv(f"{FOPH_CSV_PATH}/{filename}")
-    logger.info(f"Reading {filename}")
+    new_df = pd.read_csv(f'{FOPH_CSV_PATH}/{filename}')
+    logger.info(f'Reading {filename}')
 
     new_df = new_df.rename(columns=str.lower)
-    new_df.index.name = "id_"
-    if "date" not in new_df.columns:
-        new_df["date"] = pd.to_datetime(new_df.datum)
+    new_df.index.name = 'id_'
+    if 'date' not in new_df.columns:
+        new_df['date'] = pd.to_datetime(new_df.datum)
     else:
-        new_df["date"] = pd.to_datetime(new_df.date)
-    logger.info(f"Table {table} passed to DataFrame")
+        new_df['date'] = pd.to_datetime(new_df.date)
+    logger.info(f'Table {table} passed to DataFrame')
 
     engine = get_engine(env.db.default_credential)
     with engine.connect() as conn:
         upsert(
             con=conn,
             df=new_df,
-            table_name=f"foph_{table.lower()}_d",
-            schema="switzerland",
-            if_row_exists="update",
+            table_name=f'foph_{table.lower()}',
+            schema='switzerland',
+            if_row_exists='update',
             chunksize=1000,
             add_new_columns=True,
             create_table=True,
         )
-    logger.info(f"Table foph_{table.lower()}_d updated")
+    logger.info(f'Table foph_{table.lower()} updated')
 
 
 def compare(filename, table) -> bool:
     csv_date = _csv_last_update(filename)
     table_date = _table_last_update(table)
     return csv_date == table_date
 
@@ -78,22 +78,22 @@
 
     Returns:
         last_update (datetime) : Datetime with the max date in the CSV.
 
     Raises:
         Exception (Exception)  : Empty dataframe from CSV.
     """
-    df = pd.read_csv(f"{FOPH_CSV_PATH}/{filename}")
-    if "date" not in df:
+    df = pd.read_csv(f'{FOPH_CSV_PATH}/{filename}')
+    if 'date' not in df:
         last_update = df.datum.max()
     else:
         last_update = df.date.max()
     if df.empty:
-        raise Exception("Empty file.")
-    return datetime.strptime(str(last_update), "%Y-%m-%d")
+        raise Exception('Empty file.')
+    return datetime.strptime(str(last_update), '%Y-%m-%d')
 
 
 def _table_last_update(table) -> datetime:
     """
     Method responsible for connecting and retrieving the maximum date
     of a table in the SQL Database.
     @see epigraphhub.connection : Where the connection is configured.
@@ -107,17 +107,19 @@
 
     Raises:
         Exception (Exception)   : Connection with the database could not be
                                   stablished.
     """
     engine = get_engine(env.db.default_credential)
     try:
-        df = pd.read_sql(f"select * from switzerland.foph_{table.lower()}_d;", engine)
-        if "date" not in df:
+        df = pd.read_sql(
+            f'select * from switzerland.foph_{table.lower()};', engine
+        )
+        if 'date' not in df:
             df = df.datum.dropna()
             last_update = df.max()
         df = df.date.dropna()
         last_update = df.max()
-        return datetime.strptime(str(last_update), "%Y-%m-%d %H:%M:%S")
+        return datetime.strptime(str(last_update), '%Y-%m-%d %H:%M:%S')
     except Exception as e:
-        logger.error(f"Could not access {table} table\n{e}")
+        logger.error(f'Could not access {table} table\n{e}')
         raise (e)
```

### Comparing `epigraphhub-2.0.4/epigraphhub/data/foph/transform.py` & `epigraphhub-2.0.5/epigraphhub/data/foph/transform.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     engine = get_engine(env.db.default_credential)
 
     with engine.connect() as connection:
         try:
             connection.execute(
                 f"""
                 CREATE INDEX IF NOT EXISTS region_idx
-                ON switzerland.foph_{table.lower()}_d ('geoRegion');
+                ON switzerland.foph_{table.lower()} (geoRegion);
                 """
             )
-            logger.info(f"geoRegion index updated on foph_{table.lower()}_d")
+            logger.info(f'geoRegion index updated on foph_{table.lower()}')
         except Exception as e:
-            logger.error(f"Could not create region index: {e}")
+            logger.error(f'Could not create region index: {e}')
         try:
             connection.execute(
                 f"""
                 CREATE INDEX IF NOT EXISTS date_idx
-                ON switzerland.foph_{table.lower()}_d (date);
+                ON switzerland.foph_{table.lower()} (date);
                 """
             )
-            logger.info(f"date index updated on foph_{table.lower()}_d")
+            logger.info(f'date index updated on foph_{table.lower()}')
         except Exception as e:
-            logger.info(f"Could not create date index: {e}")
+            logger.info(f'Could not create date index: {e}')
```

### Comparing `epigraphhub-2.0.4/epigraphhub/data/foph/viz.py` & `epigraphhub-2.0.5/epigraphhub/data/foph/viz.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/geoupload.py` & `epigraphhub-2.0.5/epigraphhub/data/geoupload.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/ggtrends.py` & `epigraphhub-2.0.5/epigraphhub/data/ggtrends.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/owid/extract.py` & `epigraphhub-2.0.5/epigraphhub/data/owid/extract.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/owid/loading.py` & `epigraphhub-2.0.5/epigraphhub/data/owid/loading.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/owid/transform.py` & `epigraphhub-2.0.5/epigraphhub/data/owid/transform.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/sinan_fetch.py` & `epigraphhub-2.0.5/epigraphhub/data/sinan_fetch.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/worldbank.py` & `epigraphhub-2.0.5/epigraphhub/data/worldbank.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/data/worldpop.py` & `epigraphhub-2.0.5/epigraphhub/data/worldpop.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/settings.py` & `epigraphhub-2.0.5/epigraphhub/settings.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/epigraphhub/utils/_config.py` & `epigraphhub-2.0.5/epigraphhub/utils/_config.py`

 * *Files identical despite different names*

### Comparing `epigraphhub-2.0.4/pyproject.toml` & `epigraphhub-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "epigraphhub"
-version = "2.0.4"  # changed by semantic-release
+version = "2.0.5"  # changed by semantic-release
 description = "Epigraphhub Python package"
 readme = "README.md"
 authors = ["thegraphnetwork <fccoelho@gmail.com>"]
 license = "GNU GPL v3.0"
 repository = "https://github.com/thegraphnetwork/epigraphhub_py"
 homepage = "https://github.com/thegraphnetwork/epigraphhub_py"
 
@@ -55,15 +55,15 @@
 scikit-learn = "^1.0.2"
 wbgapi = "^1.0.7"
 rioxarray = "^0.10.2"
 wget = "^3.2"
 requests = "^2.27.1"
 tabulate = "^0.8.9"
 click = "^8.1.0"
-PyYAML = "^6.0"
+PyYAML = "^5.0"
 pymc = "^4.2.0"
 loguru = "^0.6.0"
 sodapy = "^2.2.0"
 pangres = "^4.1.2"
 ngboost = "^0.3.13"
 ibis-framework = "^3.2.0"
 
@@ -85,14 +85,19 @@
 pytest-html = "^3.1.1"
 pytest-cov = "^3.0.0"
 Sphinx = "^4.4.0"
 myst-parser = "^0.17.0"
 sphinx-pyproject = "^0.1.0"
 nbsphinx = "^0.8.8"
 
+[tool.poetry.group.dev.dependencies]
+makim = "1.6.4"
+containers-sugar = "1.4.2"
+pysus = "^0.8.0"
+
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py39"]
 line-length = 88
 color = true
 exclude = '''
 /(
```

### Comparing `epigraphhub-2.0.4/PKG-INFO` & `epigraphhub-2.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epigraphhub
-Version: 2.0.4
+Version: 2.0.5
 Summary: Epigraphhub Python package
 Home-page: https://github.com/thegraphnetwork/epigraphhub_py
 License: GNU GPL v3.0
 Keywords: epidemiology
 Author: thegraphnetwork
 Author-email: fccoelho@gmail.com
 Requires-Python: >=3.9,<3.11
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: GeoAlchemy2 (>=0.10.0,<0.11.0)
-Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: PyYAML (>=5.0,<6.0)
 Requires-Dist: SQLAlchemy (>=1.4.29,<2.0.0)
 Requires-Dist: arviz (>=0.12.0,<0.13.0)
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: geopandas (>=0.10.2,<0.11.0)
 Requires-Dist: ibis-framework (>=3.2.0,<4.0.0)
 Requires-Dist: joblib (>=1.1.0,<2.0.0)
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
```

