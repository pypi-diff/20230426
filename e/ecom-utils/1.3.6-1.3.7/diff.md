# Comparing `tmp/ecom-utils-1.3.6.tar.gz` & `tmp/ecom-utils-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecom-utils-1.3.6.tar", last modified: Mon Mar  6 14:52:39 2023, max compression
+gzip compressed data, was "ecom-utils-1.3.7.tar", last modified: Wed Apr 26 14:57:24 2023, max compression
```

## Comparing `ecom-utils-1.3.6.tar` & `ecom-utils-1.3.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)      810 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/PKG-INFO
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)      314 2023-03-06 14:52:36.000000 ecom-utils-1.3.6/README.md
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.175923 ecom-utils-1.3.6/ecom_utils/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)        0 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/__init__.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/pon/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)        0 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/pon/__init__.py
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     2630 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/pon/core.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.175923 ecom-utils-1.3.6/ecom_utils/scient/
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/core/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)      183 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/core/__init__.py
--rwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)     6618 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/functions.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/core/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     4345 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/core/base.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/mssql/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     2520 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/mssql/functions.py
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     2038 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/mssql/operators.py
--rwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)     5803 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/operators.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/postgres/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     1057 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/postgres/functions.py
--rwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)     1566 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/postgres/operators.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/ecom_utils/tgd/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)        0 2023-02-28 14:36:58.000000 ecom-utils-1.3.6/ecom_utils/tgd/__init__.py
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     2414 2023-03-06 14:15:47.000000 ecom-utils-1.3.6/ecom_utils/tgd/base.py
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     9090 2023-03-06 14:52:36.000000 ecom-utils-1.3.6/ecom_utils/tgd/core.py
-drwxrwxr-x   0 ecom18250  (1000) ecom18250  (1000)        0 2023-03-06 14:52:39.175923 ecom-utils-1.3.6/ecom_utils.egg-info/
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)      810 2023-03-06 14:52:39.000000 ecom-utils-1.3.6/ecom_utils.egg-info/PKG-INFO
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)      703 2023-03-06 14:52:39.000000 ecom-utils-1.3.6/ecom_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)        1 2023-03-06 14:52:39.000000 ecom-utils-1.3.6/ecom_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)        9 2023-03-06 14:52:39.000000 ecom-utils-1.3.6/ecom_utils.egg-info/requires.txt
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)       11 2023-03-06 14:52:39.000000 ecom-utils-1.3.6/ecom_utils.egg-info/top_level.txt
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)       38 2023-03-06 14:52:39.179923 ecom-utils-1.3.6/setup.cfg
--rw-rw-r--   0 ecom18250  (1000) ecom18250  (1000)     1302 2023-03-06 14:52:36.000000 ecom-utils-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.431413 ecom-utils-1.3.7/
+-rw-rw-rw-   0        0        0     1069 2023-04-26 14:57:24.430409 ecom-utils-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-04-26 14:57:08.000000 ecom-utils-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.380409 ecom-utils-1.3.7/ecom_utils/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.414412 ecom-utils-1.3.7/ecom_utils/pon/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/pon/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-04-26 14:53:26.000000 ecom-utils-1.3.7/ecom_utils/pon/core.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.374410 ecom-utils-1.3.7/ecom_utils/scient/
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.416413 ecom-utils-1.3.7/ecom_utils/scient/airflow/
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.417421 ecom-utils-1.3.7/ecom_utils/scient/airflow/core/
+-rw-rw-rw-   0        0        0      190 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/core/__init__.py
+-rw-rw-rw-   0        0        0     6833 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/functions.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.418410 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.420411 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/core/
+-rw-rw-rw-   0        0        0     4503 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/core/base.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.422412 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/mssql/
+-rw-rw-rw-   0        0        0     2583 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/mssql/functions.py
+-rw-rw-rw-   0        0        0     2098 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/mssql/operators.py
+-rw-rw-rw-   0        0        0     5951 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/operators.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.425411 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/postgres/
+-rw-rw-rw-   0        0        0     1083 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/postgres/functions.py
+-rw-rw-rw-   0        0        0     1622 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/postgres/operators.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.429412 ecom-utils-1.3.7/ecom_utils/tgd/
+-rw-rw-rw-   0        0        0        0 2023-02-28 14:35:48.000000 ecom-utils-1.3.7/ecom_utils/tgd/__init__.py
+-rw-rw-rw-   0        0        0     2462 2023-03-16 11:25:12.000000 ecom-utils-1.3.7/ecom_utils/tgd/base.py
+-rw-rw-rw-   0        0        0     9285 2023-03-16 11:25:12.000000 ecom-utils-1.3.7/ecom_utils/tgd/core.py
+drwxrwxrwx   0        0        0        0 2023-04-26 14:57:24.410410 ecom-utils-1.3.7/ecom_utils.egg-info/
+-rw-rw-rw-   0        0        0     1069 2023-04-26 14:57:24.000000 ecom-utils-1.3.7/ecom_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-04-26 14:57:24.000000 ecom-utils-1.3.7/ecom_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 14:57:24.000000 ecom-utils-1.3.7/ecom_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 14:57:24.000000 ecom-utils-1.3.7/ecom_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-26 14:57:24.000000 ecom-utils-1.3.7/ecom_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 14:57:24.431413 ecom-utils-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1339 2023-04-26 14:56:33.000000 ecom-utils-1.3.7/setup.py
```

### Comparing `ecom-utils-1.3.6/ecom_utils/pon/core.py` & `ecom-utils-1.3.7/ecom_utils/pon/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,95 @@
-import json
-import requests
-
-ENDPOINT_STAGE = 'https://devapp8.ecomchaco.com.ar'
-ENDPOINT_PROD = 'https://devapp8.ecomchaco.com.ar'
-
-API_ENDPOINTS = {
-	'get_token_application': '_endpointbase_/ponapitest/oauth/access_token',
-	'obtener_jurisdicciones': '_endpointbase_/ponapitest/rest/ConsultaJurisdicciones',
-	'obtener_oficinas': '_endpointbase_/ponapitest/rest/ConsultaOficinas'
-}
-
-class Pon():
-	def __init__(self, username, password, client_id, mode_stage=True):
-		self.username = username
-		self.password = password
-		self.client_id = client_id
-		self.mode_stage = mode_stage
-
-		self.access_token = None
-		self.scope = None
-		self.refresh_token = None
-		self.user_guid = None
-
-	def get_endpoint_base(self):
-		if self.mode_stage:
-			return ENDPOINT_STAGE
-		return ENDPOINT_PROD
-
-	def get_token_application(self):
-		url = API_ENDPOINTS['get_token_application'].replace("_endpointbase_", self.get_endpoint_base())
-		headers = {
-			"client_id": self.client_id,
-			"grant_type": "password",
-			"scope": "FullControl",
-			'username': self.username,
-			'password': self.password,
-		}
-
-		response = requests.post(url, headers=headers)
-		if response.status_code == 200:
-			data = response.json()
-			self.access_token = data.get("access_token", None)
-			self.scope = data.get("scope", None) 
-			self.refresh_token = data.get("refresh_token", None)
-			self.user_guid = data.get("user_guid", None)
-	
-	def obtener_jurisdicciones(self):
-		if self.access_token is None:
-			self.get_token_application()
-			if self.access_token is None:
-				return None
-		jurisdicciones = []
-
-		url = API_ENDPOINTS['obtener_jurisdicciones'].replace("_endpointbase_", self.get_endpoint_base())
-
-		headers = {
-			"Authorization": self.access_token,
-			"Content-Type": "application/json"
-		}
-
-		data = json.dumps({
-			"Orden": 0,
-		    "Id": 0,
-		    "Nombre": ""
-		})
-		response = requests.post(url, headers=headers, data=data)
-		if response.status_code == 200:
-			data = response.json()
-			jurisdicciones = data["SDTJurisdicciones"]["Jurisdicciones"]
-		return jurisdicciones
-
-	def obtener_oficinas(self, jurId):
-		if self.access_token is None:
-			self.get_token_application()
-			if self.access_token is None:
-				return None
-		oficinas = []
-
-		url = API_ENDPOINTS['obtener_oficinas'].replace("_endpointbase_", self.get_endpoint_base())
-
-		headers = {
-			"Authorization": self.access_token,
-			"Content-Type": "application/json"
-		}
-
-		data = json.dumps({
-			"JurId": jurId
-		})
-		response = requests.post(url, headers=headers, data=data)
-
-		if response.status_code == 200:
-			data = response.json()
-			oficinas = data["SDTOficinas"]["Oficinas"]
+import json
+import requests
+
+ENDPOINT_STAGE = 'https://devapp8.ecomchaco.com.ar'
+ENDPOINT_PROD = 'https://apps8.chaco.gob.ar/ponapi'
+
+API_ENDPOINTS = {
+	'get_token_application': '_endpointbase_/ponapitest/oauth/access_token',
+	'obtener_jurisdicciones': '_endpointbase_/ponapitest/rest/ConsultaJurisdicciones',
+	'obtener_oficinas': '_endpointbase_/ponapitest/rest/ConsultaOficinas'
+}
+
+class Pon():
+	def __init__(self, username, password, client_id, mode_stage=True):
+		self.username = username
+		self.password = password
+		self.client_id = client_id
+		self.mode_stage = mode_stage
+
+		self.access_token = None
+		self.scope = None
+		self.refresh_token = None
+		self.user_guid = None
+
+	def get_endpoint_base(self):
+		if self.mode_stage:
+			return ENDPOINT_STAGE
+		return ENDPOINT_PROD
+
+	def get_token_application(self):
+		url = API_ENDPOINTS['get_token_application'].replace("_endpointbase_", self.get_endpoint_base())
+		headers = {
+			"client_id": self.client_id,
+			"grant_type": "password",
+			"scope": "FullControl",
+			'username': self.username,
+			'password': self.password,
+		}
+
+		response = requests.post(url, headers=headers)
+		if response.status_code == 200:
+			data = response.json()
+			self.access_token = data.get("access_token", None)
+			self.scope = data.get("scope", None) 
+			self.refresh_token = data.get("refresh_token", None)
+			self.user_guid = data.get("user_guid", None)
+	
+	def obtener_jurisdicciones(self):
+		if self.access_token is None:
+			self.get_token_application()
+			if self.access_token is None:
+				return None
+		jurisdicciones = []
+
+		url = API_ENDPOINTS['obtener_jurisdicciones'].replace("_endpointbase_", self.get_endpoint_base())
+
+		headers = {
+			"Authorization": self.access_token,
+			"Content-Type": "application/json"
+		}
+
+		data = json.dumps({
+			"Orden": 0,
+		    "Id": 0,
+		    "Nombre": ""
+		})
+		response = requests.post(url, headers=headers, data=data)
+		if response.status_code == 200:
+			data = response.json()
+			jurisdicciones = data["SDTJurisdicciones"]["Jurisdicciones"]
+		return jurisdicciones
+
+	def obtener_oficinas(self, jurId):
+		if self.access_token is None:
+			self.get_token_application()
+			if self.access_token is None:
+				return None
+		oficinas = []
+
+		url = API_ENDPOINTS['obtener_oficinas'].replace("_endpointbase_", self.get_endpoint_base())
+
+		headers = {
+			"Authorization": self.access_token,
+			"Content-Type": "application/json"
+		}
+
+		data = json.dumps({
+			"JurId": jurId
+		})
+		response = requests.post(url, headers=headers, data=data)
+
+		if response.status_code == 200:
+			data = response.json()
+			oficinas = data["SDTOficinas"]["Oficinas"]
 		return oficinas
```

### Comparing `ecom-utils-1.3.6/ecom_utils/scient/airflow/functions.py` & `ecom-utils-1.3.7/ecom_utils/scient/airflow/functions.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,216 +1,216 @@
-import importlib
-import logging
-import base64
-
-import pandas as pd
-import os
-
-from airflow.hooks.postgres_hook import PostgresHook
-
-from contextlib import contextmanager
-
-# ===========================================
-def get_dict_connection(name, settings_modulo):
-    x = importlib.import_module(settings_modulo.SETTINGS_MODULE)
-    return getattr(x, "DATABASES")[name]
-
-def get_conexion(name, settings_modulo):
-    return get_dict_connection(name, settings_modulo)["AIRFLOW_PARAMETERS"]["AIRFLOW_NAME"]
-
-def get_str_conexion_mssql(name, settings_modulo):
-	dict_conexion = get_dict_connection(name, settings_modulo)
-	driver = dict_conexion["OPTIONS"]["driver"]
-	return f'DRIVER={driver};SERVER={dict_conexion["HOST"]};DATABASE={dict_conexion["NAME"]};UID={dict_conexion["USER"]};PWD={dict_conexion["PASSWORD"]}'
-# ===========================================
-
-def get_query_from_sql(path_sql):
-    f = open(path_sql, "r")
-    return f.read().replace('\n', ' ')
-
-
-@contextmanager
-def get_dbconnection(strconn, engine):
-    conn = engine.connect(strconn)
-    try:
-        conn.cursor()
-        yield conn
-    except Exception as e:
-        logging.error(f"{e}")
-        return e
-    finally:
-        conn.commit()
-        conn.close()
-
-
-def to_base_64_logo(path_image):
-    with open(path_image, "rb") as image_file:
-        encoded_string = base64.b64encode(image_file.read())
-        return "data:image/png;base64," + encoded_string.decode('utf-8')
-
-# ================================================================
-# Funciones para poblar dimensiones temporales
-def _insert_dim_nivel_superior(**context):
-	dtypes = context.get("dtypes", None)
-	if dtypes is None:
-		df = pd.read_csv(context['file_input'])
-	else:
-		df = pd.read_csv(context['file_input'], dtype=dtypes)
-	
-	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
-	conn = pg_hook.get_conn()
-	cur = conn.cursor()
-	for index, row in df.iterrows():
-		mes = row[context['campo_mes']] 
-		anio = row[context['campo_anio']] 
-		cur.execute(f"select inserta_tiemponivelsuperior('{anio}', '{mes}')")
-		conn.commit()
-
-	# Eliminamos Archivo de entrada
-	os.remove(context['file_input'])
-
-def _insert_fechas_dim_temporal(**context):
-	"""Inserta fechas en tabla
-	"""
-	
-	df = pd.read_csv(context['file_input'])
-	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
-	conn = pg_hook.get_conn()
-	cur = conn.cursor()
-	for index, row in df.iterrows():
-		cur.execute(f"select inserta_tiemponiveldia('{row['fechas']}')")
-		conn.commit()
-
-	# Eliminamos Archivo de entrada
-	os.remove(context['file_input'])
-
-def _get_fechas_to_create_dim_temporal(**context):
-
-	"""Obtiene las fechas a crear"""
-
-	
-	data = pd.read_csv(context['data_input'])
-	dim_tiemponiveldia = pd.read_csv(context['dim_tiemponiveldia'])
-	fechas = set(data.TabAuxiliarFechaLiq.unique()).difference(set(dim_tiemponiveldia.fecha.unique()))
-	fechas_df = pd.DataFrame({'fechas' : list(fechas)})
-	fechas_df.to_csv(context['file_output'], index=False)
-	
-	# Eliminamos Archivos de entrada
-	os.remove(context['tabaux'])
-	os.remove(context['dim_tiemponiveldia'])
-
-# ================================================================
-def _insert_dim_planta(**context):
-	dtypes = context.get("dtypes", None)
-	if dtypes is None:
-		df = pd.read_csv(context['file_input'])
-	else:
-		df = pd.read_csv(context['file_input'], dtype=dtypes)
-	
-	# df = df.fillna('None')
-	
-	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
-	conn = pg_hook.get_conn()
-	cur = conn.cursor()
-	
-	errors_count = 0
-	success_count = 0
-	
-	for index, row in df.iterrows():
-		aptaid=f"{row['ptaid']}::integer"
-		asrevid=f"{row['srevid']}::smallint"
-		aescid=f"{row['escid']}::smallint"
-		acarid=f"{row['carid']}::smallint"
-		ajurid=f"{row['jurid']}::smallint"
-		aptamarcaba= "true::boolean" if row['ptamarcaba'] == 1 else "false::boolean"
-		
-		abajfch = "NULL" if row["bajfch"] == "None" else f"'{row['bajfch'].split(' ')[0]}'::timestamp"
-		
-		amotbajid=f"{row['motbajid']}::smallint"
-		
-		aptahscat="NULL" if pd.isna(row['ptahscat']) else f"{row['ptahscat']}::integer"
-		
-		asipnumempl="NULL" if pd.isna(row['sipnumempl']) else f"{row['sipnumempl']}::integer"
-		
-		aptaultperl=f"{row['ptaultperl']}::integer"
-		apptcarid=f"{row['pptcarid']}::integer"
-		
-		apptafchdesd="NULL" if row["ptafchdesd"] == "None" else f"'{row['ptafchdesd'].split(' ')[0]}'::timestamp"
-		apptafchhast="NULL" if row["ptafchhast"] == "None" else f"'{row['ptafchhast'].split(' ')[0]}'::timestamp"
-
-		aptatipo=f"{row['ptatipo']}::smallint"
-		
-		acant_horas_contrato="NULL" if pd.isna(row['ctocanths']) else f"{row['ctocanths']}::decimal(10,2)"
-		
-		acuit=f"'{row['cuit']}'::text"
-
-		query = f"select id, message from inserta_dimplanta({aptaid}, {asrevid}, {aescid}, {acarid}, {ajurid}, {aptamarcaba}, {abajfch}, {amotbajid}, {aptahscat}, {asipnumempl}, {aptaultperl}, {apptcarid}, {apptafchdesd}, {apptafchhast}, {aptatipo}, {acant_horas_contrato}, {acuit})" 
-		
-		
-		try:
-			cur.execute(query)
-			success_count+=1
-		except Exception as e:
-			errors_count+=1
-			logging.error(f"Error ejecutando consulta: {query}")
-			logging.error(f"Se ha generado el siguiente mensaje de error: {e}")
-
-		conn.commit()
-
-	logging.info(f"Success query: {success_count}")
-	logging.info(f"Errors query: {errors_count}")
-
-	# Eliminamos Archivo de entrada
-	os.remove(context['file_input'])
-
-if __name__ == '__main__':
-	
-	LIQ_CARGO_DATA_COLS = {
-		"liqanio": "Int64",
-		"liqmes": "Int64",
-		"liqtipo": "Int64",
-		"liqnro": "Int64", 
-		"ptaid": "Int64", 
-		"liqrbo": "Int64",
-		"liqdiast": "Int64",
-		"liqsrip": "Int64", 
-		"liqpuroca": "float",
-		"liqpurosa": "float",
-		"liqajusca": "float",
-		"liqajussa": "float",
-		"liqasfapur": "float",
-		"liqasfaaju": "float",
-		"liqdtosley": "float",
-		"liqotros": "float",
-		"liqliqpuro": "float",
-		"liqdedaut": "float",
-		"liqapatos": "float",
-		"liqapatjub": "float",
-		"ptaid": "Int64",
-		"perpref": "Int64",
-		"perdocid": "Int64",
-		"perdigito": "Int64",
-		"srevid": "Int64",
-		"escid": "Int64",
-		"carid": "Int64",
-		"jurid": "Int64",
-		"ptamarcaba": "Int64",
-		"bajfch": "str",
-		"motbajid":"Int64",
-		"ctocanths":"float",
-		"ptahscat":"Int64",
-		"sipnumempl":"Int64",
-		"ptaultperl":"Int64",
-		"pptcarid":"Int64",
-		"ptafchdesd":"str",
-		"ptafchhast": "str",
-		"ptatipo": "Int64",
-		"planta_fk": "Int64", 
-		"dim_planta_ptaid": "Int64"
-	}
-	
-	context={
-		"dtypes":LIQ_CARGO_DATA_COLS,
-		"file_input":'/home/lucas/work/projects/airflow/dags/dw_chaco_etl/etl_pon_activos/temp/manual__2022-03-29T20:37:26.997765+00:00_plantaoc_inserts.csv',
-		"POSTGRES_CONN_ID":'dw_provincial_local'
-	}
+import importlib
+import logging
+import base64
+
+import pandas as pd
+import os
+
+from airflow.hooks.postgres_hook import PostgresHook
+
+from contextlib import contextmanager
+
+# ===========================================
+def get_dict_connection(name, settings_modulo):
+    x = importlib.import_module(settings_modulo.SETTINGS_MODULE)
+    return getattr(x, "DATABASES")[name]
+
+def get_conexion(name, settings_modulo):
+    return get_dict_connection(name, settings_modulo)["AIRFLOW_PARAMETERS"]["AIRFLOW_NAME"]
+
+def get_str_conexion_mssql(name, settings_modulo):
+	dict_conexion = get_dict_connection(name, settings_modulo)
+	driver = dict_conexion["OPTIONS"]["driver"]
+	return f'DRIVER={driver};SERVER={dict_conexion["HOST"]};DATABASE={dict_conexion["NAME"]};UID={dict_conexion["USER"]};PWD={dict_conexion["PASSWORD"]}'
+# ===========================================
+
+def get_query_from_sql(path_sql):
+    f = open(path_sql, "r")
+    return f.read().replace('\n', ' ')
+
+
+@contextmanager
+def get_dbconnection(strconn, engine):
+    conn = engine.connect(strconn)
+    try:
+        conn.cursor()
+        yield conn
+    except Exception as e:
+        logging.error(f"{e}")
+        return e
+    finally:
+        conn.commit()
+        conn.close()
+
+
+def to_base_64_logo(path_image):
+    with open(path_image, "rb") as image_file:
+        encoded_string = base64.b64encode(image_file.read())
+        return "data:image/png;base64," + encoded_string.decode('utf-8')
+
+# ================================================================
+# Funciones para poblar dimensiones temporales
+def _insert_dim_nivel_superior(**context):
+	dtypes = context.get("dtypes", None)
+	if dtypes is None:
+		df = pd.read_csv(context['file_input'])
+	else:
+		df = pd.read_csv(context['file_input'], dtype=dtypes)
+	
+	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
+	conn = pg_hook.get_conn()
+	cur = conn.cursor()
+	for index, row in df.iterrows():
+		mes = row[context['campo_mes']] 
+		anio = row[context['campo_anio']] 
+		cur.execute(f"select inserta_tiemponivelsuperior('{anio}', '{mes}')")
+		conn.commit()
+
+	# Eliminamos Archivo de entrada
+	os.remove(context['file_input'])
+
+def _insert_fechas_dim_temporal(**context):
+	"""Inserta fechas en tabla
+	"""
+	
+	df = pd.read_csv(context['file_input'])
+	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
+	conn = pg_hook.get_conn()
+	cur = conn.cursor()
+	for index, row in df.iterrows():
+		cur.execute(f"select inserta_tiemponiveldia('{row['fechas']}')")
+		conn.commit()
+
+	# Eliminamos Archivo de entrada
+	os.remove(context['file_input'])
+
+def _get_fechas_to_create_dim_temporal(**context):
+
+	"""Obtiene las fechas a crear"""
+
+	
+	data = pd.read_csv(context['data_input'])
+	dim_tiemponiveldia = pd.read_csv(context['dim_tiemponiveldia'])
+	fechas = set(data.TabAuxiliarFechaLiq.unique()).difference(set(dim_tiemponiveldia.fecha.unique()))
+	fechas_df = pd.DataFrame({'fechas' : list(fechas)})
+	fechas_df.to_csv(context['file_output'], index=False)
+	
+	# Eliminamos Archivos de entrada
+	os.remove(context['tabaux'])
+	os.remove(context['dim_tiemponiveldia'])
+
+# ================================================================
+def _insert_dim_planta(**context):
+	dtypes = context.get("dtypes", None)
+	if dtypes is None:
+		df = pd.read_csv(context['file_input'])
+	else:
+		df = pd.read_csv(context['file_input'], dtype=dtypes)
+	
+	# df = df.fillna('None')
+	
+	pg_hook = PostgresHook(postgres_conn_id=context["POSTGRES_CONN_ID"])
+	conn = pg_hook.get_conn()
+	cur = conn.cursor()
+	
+	errors_count = 0
+	success_count = 0
+	
+	for index, row in df.iterrows():
+		aptaid=f"{row['ptaid']}::integer"
+		asrevid=f"{row['srevid']}::smallint"
+		aescid=f"{row['escid']}::smallint"
+		acarid=f"{row['carid']}::smallint"
+		ajurid=f"{row['jurid']}::smallint"
+		aptamarcaba= "true::boolean" if row['ptamarcaba'] == 1 else "false::boolean"
+		
+		abajfch = "NULL" if row["bajfch"] == "None" else f"'{row['bajfch'].split(' ')[0]}'::timestamp"
+		
+		amotbajid=f"{row['motbajid']}::smallint"
+		
+		aptahscat="NULL" if pd.isna(row['ptahscat']) else f"{row['ptahscat']}::integer"
+		
+		asipnumempl="NULL" if pd.isna(row['sipnumempl']) else f"{row['sipnumempl']}::integer"
+		
+		aptaultperl=f"{row['ptaultperl']}::integer"
+		apptcarid=f"{row['pptcarid']}::integer"
+		
+		apptafchdesd="NULL" if row["ptafchdesd"] == "None" else f"'{row['ptafchdesd'].split(' ')[0]}'::timestamp"
+		apptafchhast="NULL" if row["ptafchhast"] == "None" else f"'{row['ptafchhast'].split(' ')[0]}'::timestamp"
+
+		aptatipo=f"{row['ptatipo']}::smallint"
+		
+		acant_horas_contrato="NULL" if pd.isna(row['ctocanths']) else f"{row['ctocanths']}::decimal(10,2)"
+		
+		acuit=f"'{row['cuit']}'::text"
+
+		query = f"select id, message from inserta_dimplanta({aptaid}, {asrevid}, {aescid}, {acarid}, {ajurid}, {aptamarcaba}, {abajfch}, {amotbajid}, {aptahscat}, {asipnumempl}, {aptaultperl}, {apptcarid}, {apptafchdesd}, {apptafchhast}, {aptatipo}, {acant_horas_contrato}, {acuit})" 
+		
+		
+		try:
+			cur.execute(query)
+			success_count+=1
+		except Exception as e:
+			errors_count+=1
+			logging.error(f"Error ejecutando consulta: {query}")
+			logging.error(f"Se ha generado el siguiente mensaje de error: {e}")
+
+		conn.commit()
+
+	logging.info(f"Success query: {success_count}")
+	logging.info(f"Errors query: {errors_count}")
+
+	# Eliminamos Archivo de entrada
+	os.remove(context['file_input'])
+
+if __name__ == '__main__':
+	
+	LIQ_CARGO_DATA_COLS = {
+		"liqanio": "Int64",
+		"liqmes": "Int64",
+		"liqtipo": "Int64",
+		"liqnro": "Int64", 
+		"ptaid": "Int64", 
+		"liqrbo": "Int64",
+		"liqdiast": "Int64",
+		"liqsrip": "Int64", 
+		"liqpuroca": "float",
+		"liqpurosa": "float",
+		"liqajusca": "float",
+		"liqajussa": "float",
+		"liqasfapur": "float",
+		"liqasfaaju": "float",
+		"liqdtosley": "float",
+		"liqotros": "float",
+		"liqliqpuro": "float",
+		"liqdedaut": "float",
+		"liqapatos": "float",
+		"liqapatjub": "float",
+		"ptaid": "Int64",
+		"perpref": "Int64",
+		"perdocid": "Int64",
+		"perdigito": "Int64",
+		"srevid": "Int64",
+		"escid": "Int64",
+		"carid": "Int64",
+		"jurid": "Int64",
+		"ptamarcaba": "Int64",
+		"bajfch": "str",
+		"motbajid":"Int64",
+		"ctocanths":"float",
+		"ptahscat":"Int64",
+		"sipnumempl":"Int64",
+		"ptaultperl":"Int64",
+		"pptcarid":"Int64",
+		"ptafchdesd":"str",
+		"ptafchhast": "str",
+		"ptatipo": "Int64",
+		"planta_fk": "Int64", 
+		"dim_planta_ptaid": "Int64"
+	}
+	
+	context={
+		"dtypes":LIQ_CARGO_DATA_COLS,
+		"file_input":'/home/lucas/work/projects/airflow/dags/dw_chaco_etl/etl_pon_activos/temp/manual__2022-03-29T20:37:26.997765+00:00_plantaoc_inserts.csv',
+		"POSTGRES_CONN_ID":'dw_provincial_local'
+	}
 	_insert_dim_planta(**context)
```

### Comparing `ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/mssql/functions.py` & `ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/mssql/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,158 +1,162 @@
-00000000: 0a66 726f 6d20 6169 7266 6c6f 772e 7574  .from airflow.ut
-00000010: 696c 732e 7461 736b 5f67 726f 7570 2069  ils.task_group i
-00000020: 6d70 6f72 7420 5461 736b 4772 6f75 700a  mport TaskGroup.
-00000030: 0a66 726f 6d20 6563 6f6d 5f75 7469 6c73  .from ecom_utils
-00000040: 2e73 6369 656e 742e 6169 7266 6c6f 772e  .scient.airflow.
-00000050: 7371 6c2e 6d73 7371 6c2e 6f70 6572 6174  sql.mssql.operat
-00000060: 6f72 7320 696d 706f 7274 2047 656e 6572  ors import Gener
-00000070: 6174 6549 6e73 6572 744d 7373 716c 4f70  ateInsertMssqlOp
-00000080: 6572 6174 6f72 2c20 506f 7075 6c61 7465  erator, Populate
-00000090: 4d73 7371 6c4f 7065 7261 746f 720a 6672  MssqlOperator.fr
-000000a0: 6f6d 2065 636f 6d5f 7574 696c 732e 7363  om ecom_utils.sc
-000000b0: 6965 6e74 2e61 6972 666c 6f77 2e73 716c  ient.airflow.sql
-000000c0: 2e6f 7065 7261 746f 7273 2020 2020 2020  .operators      
-000000d0: 2069 6d70 6f72 7420 4466 5472 616e 7366   import DfTransf
-000000e0: 6f72 6d4f 7065 7261 746f 720a 6672 6f6d  ormOperator.from
-000000f0: 2061 6972 666c 6f77 2e6f 7065 7261 746f   airflow.operato
-00000100: 7273 2e70 7974 686f 6e20 696d 706f 7274  rs.python import
-00000110: 2042 7261 6e63 6850 7974 686f 6e4f 7065   BranchPythonOpe
-00000120: 7261 746f 720a 6672 6f6d 2061 6972 666c  rator.from airfl
-00000130: 6f77 2e6f 7065 7261 746f 7273 2e64 756d  ow.operators.dum
-00000140: 6d79 2069 6d70 6f72 7420 4475 6d6d 794f  my import DummyO
-00000150: 7065 7261 746f 720a 0a64 6566 2073 6967  perator..def sig
-00000160: 7569 656e 7465 5f74 6172 6561 282a 2a6b  uiente_tarea(**k
-00000170: 7761 7267 7329 3a0a 2020 2020 696d 706f  wargs):.    impo
-00000180: 7274 206f 730a 2020 2020 6966 206f 732e  rt os.    if os.
-00000190: 7061 7468 2e65 7869 7374 7328 6b77 6172  path.exists(kwar
-000001a0: 6773 5b27 6669 6c65 5f69 6e70 7574 275d  gs['file_input']
-000001b0: 293a 0a20 2020 2020 2020 2074 6173 6b5f  ):.        task_
-000001c0: 696e 5f67 726f 7570 203d 206b 7761 7267  in_group = kwarg
-000001d0: 735b 2767 7275 706f 5f69 6427 5d2b 272e  s['grupo_id']+'.
-000001e0: 272b 6b77 6172 6773 5b27 7461 736b 5f70  '+kwargs['task_p
-000001f0: 726f 6365 7373 5f65 7272 6f72 5f69 6427  rocess_error_id'
-00000200: 5d0a 2020 2020 2020 2020 7265 7475 726e  ].        return
-00000210: 2074 6173 6b5f 696e 5f67 726f 7570 0a20   task_in_group. 
-00000220: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00000230: 2074 6173 6b5f 696e 5f67 726f 7570 203d   task_in_group =
-00000240: 206b 7761 7267 735b 2767 7275 706f 5f69   kwargs['grupo_i
-00000250: 6427 5d2b 272e 272b 6b77 6172 6773 5b27  d']+'.'+kwargs['
-00000260: 6475 6d6d 795f 6964 275d 0a20 2020 2020  dummy_id'].     
-00000270: 2020 2072 6574 7572 6e20 7461 736b 5f69     return task_i
-00000280: 6e5f 6772 6f75 700a 0a64 6566 206d 7373  n_group..def mss
-00000290: 716c 5f70 6f70 756c 6174 655f 6572 726f  ql_populate_erro
-000002a0: 7273 2867 726f 7570 5f69 642c 2074 6173  rs(group_id, tas
-000002b0: 6b5f 6964 5f62 7261 6e63 682c 2074 6173  k_id_branch, tas
-000002c0: 6b5f 6964 5f64 756d 6d79 2c74 6173 6b5f  k_id_dummy,task_
-000002d0: 6964 5f74 7261 6e73 666f 726d 5f65 7272  id_transform_err
-000002e0: 6f72 2c65 7272 6f72 735f 6669 6c65 2c20  or,errors_file, 
-000002f0: 636f 6c5f 6373 765f 6572 726f 7265 732c  col_csv_errores,
-00000300: 2064 6167 5f69 642c 2074 6173 6b5f 6964   dag_id, task_id
-00000310: 5f67 656e 6572 6174 655f 696e 7365 7274  _generate_insert
-00000320: 5f65 7272 6f72 2c6f 7574 7075 745f 6669  _error,output_fi
-00000330: 6c65 5f73 716c 2c74 6162 6c65 5f6e 616d  le_sql,table_nam
-00000340: 655f 6572 726f 722c 636f 6c5f 7461 626c  e_error,col_tabl
-00000350: 655f 6572 726f 722c 7365 702c 7461 736b  e_error,sep,task
-00000360: 5f69 645f 706f 7075 6c61 7465 5f74 6162  _id_populate_tab
-00000370: 6c61 5f65 7272 6f72 2c63 6f6e 6e5f 6964  la_error,conn_id
-00000380: 2c73 6368 656d 6129 3a0a 2020 2020 7769  ,schema):.    wi
-00000390: 7468 2054 6173 6b47 726f 7570 2867 726f  th TaskGroup(gro
-000003a0: 7570 5f69 642c 2074 6f6f 6c74 6970 3d66  up_id, tooltip=f
-000003b0: 2254 6173 6b73 2066 6f72 207b 6772 6f75  "Tasks for {grou
-000003c0: 705f 6964 7d22 2920 6173 2078 7878 3a0a  p_id}") as xxx:.
-000003d0: 0a20 2020 2020 2020 2062 7261 6e63 685f  .        branch_
-000003e0: 7461 736b 203d 2042 7261 6e63 6850 7974  task = BranchPyt
-000003f0: 686f 6e4f 7065 7261 746f 7228 0a20 2020  honOperator(.   
-00000400: 2020 2020 2020 2020 2074 6173 6b5f 6964           task_id
-00000410: 3d74 6173 6b5f 6964 5f62 7261 6e63 682c  =task_id_branch,
-00000420: 0a20 2020 2020 2020 2020 2020 2070 7974  .            pyt
-00000430: 686f 6e5f 6361 6c6c 6162 6c65 3d73 6967  hon_callable=sig
-00000440: 7569 656e 7465 5f74 6172 6561 2c0a 2020  uiente_tarea,.  
-00000450: 2020 2020 2020 2020 2020 6f70 5f6b 7761            op_kwa
-00000460: 7267 733d 7b0a 2020 2020 2020 2020 2020  rgs={.          
-00000470: 2020 2020 2020 2266 696c 655f 696e 7075        "file_inpu
-00000480: 7422 3a20 6572 726f 7273 5f66 696c 652c  t": errors_file,
-00000490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000004a0: 2022 7461 736b 5f70 726f 6365 7373 5f65   "task_process_e
-000004b0: 7272 6f72 5f69 6422 3a20 7461 736b 5f69  rror_id": task_i
-000004c0: 645f 7472 616e 7366 6f72 6d5f 6572 726f  d_transform_erro
-000004d0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-000004e0: 2020 2022 6475 6d6d 795f 6964 223a 2074     "dummy_id": t
-000004f0: 6173 6b5f 6964 5f64 756d 6d79 2c0a 2020  ask_id_dummy,.  
-00000500: 2020 2020 2020 2020 2020 2020 2020 2267                "g
-00000510: 7275 706f 5f69 6422 3a20 6772 6f75 705f  rupo_id": group_
-00000520: 6964 0a20 2020 2020 2020 2020 2020 207d  id.            }
-00000530: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00000540: 2020 2020 6475 6d6d 795f 7461 736b 203d      dummy_task =
-00000550: 2044 756d 6d79 4f70 6572 6174 6f72 280a   DummyOperator(.
-00000560: 2020 2020 2020 2020 2020 2020 7461 736b              task
-00000570: 5f69 6420 3d20 7461 736b 5f69 645f 6475  _id = task_id_du
-00000580: 6d6d 790a 2020 2020 2020 2020 290a 0a20  mmy.        ).. 
-00000590: 2020 2020 2020 2074 6173 6b5f 7472 616e         task_tran
-000005a0: 7366 6f72 6d5f 6572 726f 7220 3d20 4466  sform_error = Df
-000005b0: 5472 616e 7366 6f72 6d4f 7065 7261 746f  TransformOperato
-000005c0: 7228 0a20 2020 2020 2020 2020 2020 2074  r(.            t
-000005d0: 6173 6b5f 6964 3d74 6173 6b5f 6964 5f74  ask_id=task_id_t
-000005e0: 7261 6e73 666f 726d 5f65 7272 6f72 2c0a  ransform_error,.
-000005f0: 2020 2020 2020 2020 2020 2020 6474 7970              dtyp
-00000600: 653d 636f 6c5f 6373 765f 6572 726f 7265  e=col_csv_errore
-00000610: 732c 0a20 2020 2020 2020 2020 2020 2069  s,.            i
-00000620: 6e70 7574 5f66 696c 653d 6572 726f 7273  nput_file=errors
-00000630: 5f66 696c 652c 0a20 2020 2020 2020 2020  _file,.         
-00000640: 2020 206f 7065 7261 7469 6f6e 733d 5b0a     operations=[.
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 7b22 7479 7065 223a 2022 7265 6d6f 7665  {"type": "remove
-00000670: 222c 2022 636f 6c75 6d6e 5f6e 616d 6522  ", "column_name"
-00000680: 3a20 2265 7272 6f72 5f70 6f70 756c 6174  : "error_populat
-00000690: 696f 6e5f 696e 7374 616e 7422 2c20 226f  ion_instant", "o
-000006a0: 7065 7261 7469 6f6e 223a 2022 6465 6c22  peration": "del"
-000006b0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000006c0: 2020 207b 2274 7970 6522 3a20 2261 6464     {"type": "add
-000006d0: 222c 2022 636f 6c75 6d6e 5f6e 616d 6522  ", "column_name"
-000006e0: 3a20 2264 6167 5f69 6422 2c20 226f 7065  : "dag_id", "ope
-000006f0: 7261 7469 6f6e 223a 2022 6669 7865 6422  ration": "fixed"
-00000700: 2c20 2276 616c 7565 223a 6461 675f 6964  , "value":dag_id
-00000710: 2c22 7365 7061 7261 746f 7222 3a27 2c27  ,"separator":','
-00000720: 7d0a 2020 2020 2020 2020 2020 2020 5d0a  }.            ].
-00000730: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00000740: 2020 2074 6173 6b5f 6765 6e65 7261 7465     task_generate
-00000750: 5f69 6e73 6572 745f 6572 726f 723d 4765  _insert_error=Ge
-00000760: 6e65 7261 7465 496e 7365 7274 4d73 7371  nerateInsertMssq
-00000770: 6c4f 7065 7261 746f 7228 0a20 2020 2020  lOperator(.     
-00000780: 2020 2020 2020 2074 6173 6b5f 6964 3d74         task_id=t
-00000790: 6173 6b5f 6964 5f67 656e 6572 6174 655f  ask_id_generate_
-000007a0: 696e 7365 7274 5f65 7272 6f72 2c0a 2020  insert_error,.  
-000007b0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-000007c0: 6669 6c65 3d65 7272 6f72 735f 6669 6c65  file=errors_file
-000007d0: 2c0a 2020 2020 2020 2020 2020 2020 6f75  ,.            ou
-000007e0: 7470 7574 5f66 696c 653d 6f75 7470 7574  tput_file=output
-000007f0: 5f66 696c 655f 7371 6c2c 0a20 2020 2020  _file_sql,.     
-00000800: 2020 2020 2020 2074 6162 6c65 5f6e 616d         table_nam
-00000810: 653d 7461 626c 655f 6e61 6d65 5f65 7272  e=table_name_err
-00000820: 6f72 2c20 0a20 2020 2020 2020 2020 2020  or, .           
-00000830: 2064 6174 615f 636f 6c73 3d63 6f6c 5f74   data_cols=col_t
-00000840: 6162 6c65 5f65 7272 6f72 2c0a 2020 2020  able_error,.    
-00000850: 2020 2020 2020 2020 7365 703d 7365 700a          sep=sep.
-00000860: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00000870: 2020 2074 6173 6b5f 706f 7075 6c61 7465     task_populate
-00000880: 5f74 6162 6c61 5f65 7272 6f72 203d 2050  _tabla_error = P
-00000890: 6f70 756c 6174 654d 7373 716c 4f70 6572  opulateMssqlOper
-000008a0: 6174 6f72 280a 2020 2020 2020 2020 2020  ator(.          
-000008b0: 2020 7461 736b 5f69 643d 7461 736b 5f69    task_id=task_i
-000008c0: 645f 706f 7075 6c61 7465 5f74 6162 6c61  d_populate_tabla
-000008d0: 5f65 7272 6f72 2c0a 2020 2020 2020 2020  _error,.        
-000008e0: 2020 2020 7175 6572 795f 6669 6c65 3d6f      query_file=o
-000008f0: 7574 7075 745f 6669 6c65 5f73 716c 2c0a  utput_file_sql,.
-00000900: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
-00000910: 5f69 643d 636f 6e6e 5f69 642c 200a 2020  _id=conn_id, .  
-00000920: 2020 2020 2020 2020 2020 7363 6865 6d61            schema
-00000930: 3d73 6368 656d 612c 0a09 2020 2020 290a  =schema,..    ).
-00000940: 0a20 2020 2020 2020 2062 7261 6e63 685f  .        branch_
-00000950: 7461 736b 203e 3e20 7461 736b 5f74 7261  task >> task_tra
-00000960: 6e73 666f 726d 5f65 7272 6f72 203e 3e20  nsform_error >> 
-00000970: 7461 736b 5f67 656e 6572 6174 655f 696e  task_generate_in
-00000980: 7365 7274 5f65 7272 6f72 203e 3e20 7461  sert_error >> ta
-00000990: 736b 5f70 6f70 756c 6174 655f 7461 626c  sk_populate_tabl
-000009a0: 615f 6572 726f 720a 2020 2020 2020 2020  a_error.        
-000009b0: 6272 616e 6368 5f74 6173 6b20 3e3e 2064  branch_task >> d
-000009c0: 756d 6d79 5f74 6173 6b0a 2020 2020 7265  ummy_task.    re
-000009d0: 7475 726e 2078 7878                      turn xxx
+00000000: 0d0a 6672 6f6d 2061 6972 666c 6f77 2e75  ..from airflow.u
+00000010: 7469 6c73 2e74 6173 6b5f 6772 6f75 7020  tils.task_group 
+00000020: 696d 706f 7274 2054 6173 6b47 726f 7570  import TaskGroup
+00000030: 0d0a 0d0a 6672 6f6d 2065 636f 6d5f 7574  ....from ecom_ut
+00000040: 696c 732e 7363 6965 6e74 2e61 6972 666c  ils.scient.airfl
+00000050: 6f77 2e73 716c 2e6d 7373 716c 2e6f 7065  ow.sql.mssql.ope
+00000060: 7261 746f 7273 2069 6d70 6f72 7420 4765  rators import Ge
+00000070: 6e65 7261 7465 496e 7365 7274 4d73 7371  nerateInsertMssq
+00000080: 6c4f 7065 7261 746f 722c 2050 6f70 756c  lOperator, Popul
+00000090: 6174 654d 7373 716c 4f70 6572 6174 6f72  ateMssqlOperator
+000000a0: 0d0a 6672 6f6d 2065 636f 6d5f 7574 696c  ..from ecom_util
+000000b0: 732e 7363 6965 6e74 2e61 6972 666c 6f77  s.scient.airflow
+000000c0: 2e73 716c 2e6f 7065 7261 746f 7273 2020  .sql.operators  
+000000d0: 2020 2020 2069 6d70 6f72 7420 4466 5472       import DfTr
+000000e0: 616e 7366 6f72 6d4f 7065 7261 746f 720d  ansformOperator.
+000000f0: 0a66 726f 6d20 6169 7266 6c6f 772e 6f70  .from airflow.op
+00000100: 6572 6174 6f72 732e 7079 7468 6f6e 2069  erators.python i
+00000110: 6d70 6f72 7420 4272 616e 6368 5079 7468  mport BranchPyth
+00000120: 6f6e 4f70 6572 6174 6f72 0d0a 6672 6f6d  onOperator..from
+00000130: 2061 6972 666c 6f77 2e6f 7065 7261 746f   airflow.operato
+00000140: 7273 2e64 756d 6d79 2069 6d70 6f72 7420  rs.dummy import 
+00000150: 4475 6d6d 794f 7065 7261 746f 720d 0a0d  DummyOperator...
+00000160: 0a64 6566 2073 6967 7569 656e 7465 5f74  .def siguiente_t
+00000170: 6172 6561 282a 2a6b 7761 7267 7329 3a0d  area(**kwargs):.
+00000180: 0a20 2020 2069 6d70 6f72 7420 6f73 0d0a  .    import os..
+00000190: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
+000001a0: 7869 7374 7328 6b77 6172 6773 5b27 6669  xists(kwargs['fi
+000001b0: 6c65 5f69 6e70 7574 275d 293a 0d0a 2020  le_input']):..  
+000001c0: 2020 2020 2020 7461 736b 5f69 6e5f 6772        task_in_gr
+000001d0: 6f75 7020 3d20 6b77 6172 6773 5b27 6772  oup = kwargs['gr
+000001e0: 7570 6f5f 6964 275d 2b27 2e27 2b6b 7761  upo_id']+'.'+kwa
+000001f0: 7267 735b 2774 6173 6b5f 7072 6f63 6573  rgs['task_proces
+00000200: 735f 6572 726f 725f 6964 275d 0d0a 2020  s_error_id']..  
+00000210: 2020 2020 2020 7265 7475 726e 2074 6173        return tas
+00000220: 6b5f 696e 5f67 726f 7570 0d0a 2020 2020  k_in_group..    
+00000230: 656c 7365 3a0d 0a20 2020 2020 2020 2074  else:..        t
+00000240: 6173 6b5f 696e 5f67 726f 7570 203d 206b  ask_in_group = k
+00000250: 7761 7267 735b 2767 7275 706f 5f69 6427  wargs['grupo_id'
+00000260: 5d2b 272e 272b 6b77 6172 6773 5b27 6475  ]+'.'+kwargs['du
+00000270: 6d6d 795f 6964 275d 0d0a 2020 2020 2020  mmy_id']..      
+00000280: 2020 7265 7475 726e 2074 6173 6b5f 696e    return task_in
+00000290: 5f67 726f 7570 0d0a 0d0a 6465 6620 6d73  _group....def ms
+000002a0: 7371 6c5f 706f 7075 6c61 7465 5f65 7272  sql_populate_err
+000002b0: 6f72 7328 6772 6f75 705f 6964 2c20 7461  ors(group_id, ta
+000002c0: 736b 5f69 645f 6272 616e 6368 2c20 7461  sk_id_branch, ta
+000002d0: 736b 5f69 645f 6475 6d6d 792c 7461 736b  sk_id_dummy,task
+000002e0: 5f69 645f 7472 616e 7366 6f72 6d5f 6572  _id_transform_er
+000002f0: 726f 722c 6572 726f 7273 5f66 696c 652c  ror,errors_file,
+00000300: 2063 6f6c 5f63 7376 5f65 7272 6f72 6573   col_csv_errores
+00000310: 2c20 6461 675f 6964 2c20 7461 736b 5f69  , dag_id, task_i
+00000320: 645f 6765 6e65 7261 7465 5f69 6e73 6572  d_generate_inser
+00000330: 745f 6572 726f 722c 6f75 7470 7574 5f66  t_error,output_f
+00000340: 696c 655f 7371 6c2c 7461 626c 655f 6e61  ile_sql,table_na
+00000350: 6d65 5f65 7272 6f72 2c63 6f6c 5f74 6162  me_error,col_tab
+00000360: 6c65 5f65 7272 6f72 2c73 6570 2c74 6173  le_error,sep,tas
+00000370: 6b5f 6964 5f70 6f70 756c 6174 655f 7461  k_id_populate_ta
+00000380: 626c 615f 6572 726f 722c 636f 6e6e 5f69  bla_error,conn_i
+00000390: 642c 7363 6865 6d61 293a 0d0a 2020 2020  d,schema):..    
+000003a0: 7769 7468 2054 6173 6b47 726f 7570 2867  with TaskGroup(g
+000003b0: 726f 7570 5f69 642c 2074 6f6f 6c74 6970  roup_id, tooltip
+000003c0: 3d66 2254 6173 6b73 2066 6f72 207b 6772  =f"Tasks for {gr
+000003d0: 6f75 705f 6964 7d22 2920 6173 2078 7878  oup_id}") as xxx
+000003e0: 3a0d 0a0d 0a20 2020 2020 2020 2062 7261  :....        bra
+000003f0: 6e63 685f 7461 736b 203d 2042 7261 6e63  nch_task = Branc
+00000400: 6850 7974 686f 6e4f 7065 7261 746f 7228  hPythonOperator(
+00000410: 0d0a 2020 2020 2020 2020 2020 2020 7461  ..            ta
+00000420: 736b 5f69 643d 7461 736b 5f69 645f 6272  sk_id=task_id_br
+00000430: 616e 6368 2c0d 0a20 2020 2020 2020 2020  anch,..         
+00000440: 2020 2070 7974 686f 6e5f 6361 6c6c 6162     python_callab
+00000450: 6c65 3d73 6967 7569 656e 7465 5f74 6172  le=siguiente_tar
+00000460: 6561 2c0d 0a20 2020 2020 2020 2020 2020  ea,..           
+00000470: 206f 705f 6b77 6172 6773 3d7b 0d0a 2020   op_kwargs={..  
+00000480: 2020 2020 2020 2020 2020 2020 2020 2266                "f
+00000490: 696c 655f 696e 7075 7422 3a20 6572 726f  ile_input": erro
+000004a0: 7273 5f66 696c 652c 0d0a 2020 2020 2020  rs_file,..      
+000004b0: 2020 2020 2020 2020 2020 2274 6173 6b5f            "task_
+000004c0: 7072 6f63 6573 735f 6572 726f 725f 6964  process_error_id
+000004d0: 223a 2074 6173 6b5f 6964 5f74 7261 6e73  ": task_id_trans
+000004e0: 666f 726d 5f65 7272 6f72 2c0d 0a20 2020  form_error,..   
+000004f0: 2020 2020 2020 2020 2020 2020 2022 6475               "du
+00000500: 6d6d 795f 6964 223a 2074 6173 6b5f 6964  mmy_id": task_id
+00000510: 5f64 756d 6d79 2c0d 0a20 2020 2020 2020  _dummy,..       
+00000520: 2020 2020 2020 2020 2022 6772 7570 6f5f           "grupo_
+00000530: 6964 223a 2067 726f 7570 5f69 640d 0a20  id": group_id.. 
+00000540: 2020 2020 2020 2020 2020 207d 0d0a 2020             }..  
+00000550: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+00000560: 2020 2064 756d 6d79 5f74 6173 6b20 3d20     dummy_task = 
+00000570: 4475 6d6d 794f 7065 7261 746f 7228 0d0a  DummyOperator(..
+00000580: 2020 2020 2020 2020 2020 2020 7461 736b              task
+00000590: 5f69 6420 3d20 7461 736b 5f69 645f 6475  _id = task_id_du
+000005a0: 6d6d 790d 0a20 2020 2020 2020 2029 0d0a  mmy..        )..
+000005b0: 0d0a 2020 2020 2020 2020 7461 736b 5f74  ..        task_t
+000005c0: 7261 6e73 666f 726d 5f65 7272 6f72 203d  ransform_error =
+000005d0: 2044 6654 7261 6e73 666f 726d 4f70 6572   DfTransformOper
+000005e0: 6174 6f72 280d 0a20 2020 2020 2020 2020  ator(..         
+000005f0: 2020 2074 6173 6b5f 6964 3d74 6173 6b5f     task_id=task_
+00000600: 6964 5f74 7261 6e73 666f 726d 5f65 7272  id_transform_err
+00000610: 6f72 2c0d 0a20 2020 2020 2020 2020 2020  or,..           
+00000620: 2064 7479 7065 3d63 6f6c 5f63 7376 5f65   dtype=col_csv_e
+00000630: 7272 6f72 6573 2c0d 0a20 2020 2020 2020  rrores,..       
+00000640: 2020 2020 2069 6e70 7574 5f66 696c 653d       input_file=
+00000650: 6572 726f 7273 5f66 696c 652c 0d0a 2020  errors_file,..  
+00000660: 2020 2020 2020 2020 2020 6f70 6572 6174            operat
+00000670: 696f 6e73 3d5b 0d0a 2020 2020 2020 2020  ions=[..        
+00000680: 2020 2020 2020 2020 7b22 7479 7065 223a          {"type":
+00000690: 2022 7265 6d6f 7665 222c 2022 636f 6c75   "remove", "colu
+000006a0: 6d6e 5f6e 616d 6522 3a20 2265 7272 6f72  mn_name": "error
+000006b0: 5f70 6f70 756c 6174 696f 6e5f 696e 7374  _population_inst
+000006c0: 616e 7422 2c20 226f 7065 7261 7469 6f6e  ant", "operation
+000006d0: 223a 2022 6465 6c22 7d2c 0d0a 2020 2020  ": "del"},..    
+000006e0: 2020 2020 2020 2020 2020 2020 7b22 7479              {"ty
+000006f0: 7065 223a 2022 6164 6422 2c20 2263 6f6c  pe": "add", "col
+00000700: 756d 6e5f 6e61 6d65 223a 2022 6461 675f  umn_name": "dag_
+00000710: 6964 222c 2022 6f70 6572 6174 696f 6e22  id", "operation"
+00000720: 3a20 2266 6978 6564 222c 2022 7661 6c75  : "fixed", "valu
+00000730: 6522 3a64 6167 5f69 642c 2273 6570 6172  e":dag_id,"separ
+00000740: 6174 6f72 223a 272c 277d 0d0a 2020 2020  ator":','}..    
+00000750: 2020 2020 2020 2020 5d0d 0a20 2020 2020          ]..     
+00000760: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+00000770: 7461 736b 5f67 656e 6572 6174 655f 696e  task_generate_in
+00000780: 7365 7274 5f65 7272 6f72 3d47 656e 6572  sert_error=Gener
+00000790: 6174 6549 6e73 6572 744d 7373 716c 4f70  ateInsertMssqlOp
+000007a0: 6572 6174 6f72 280d 0a20 2020 2020 2020  erator(..       
+000007b0: 2020 2020 2074 6173 6b5f 6964 3d74 6173       task_id=tas
+000007c0: 6b5f 6964 5f67 656e 6572 6174 655f 696e  k_id_generate_in
+000007d0: 7365 7274 5f65 7272 6f72 2c0d 0a20 2020  sert_error,..   
+000007e0: 2020 2020 2020 2020 2069 6e70 7574 5f66           input_f
+000007f0: 696c 653d 6572 726f 7273 5f66 696c 652c  ile=errors_file,
+00000800: 0d0a 2020 2020 2020 2020 2020 2020 6f75  ..            ou
+00000810: 7470 7574 5f66 696c 653d 6f75 7470 7574  tput_file=output
+00000820: 5f66 696c 655f 7371 6c2c 0d0a 2020 2020  _file_sql,..    
+00000830: 2020 2020 2020 2020 7461 626c 655f 6e61          table_na
+00000840: 6d65 3d74 6162 6c65 5f6e 616d 655f 6572  me=table_name_er
+00000850: 726f 722c 200d 0a20 2020 2020 2020 2020  ror, ..         
+00000860: 2020 2064 6174 615f 636f 6c73 3d63 6f6c     data_cols=col
+00000870: 5f74 6162 6c65 5f65 7272 6f72 2c0d 0a20  _table_error,.. 
+00000880: 2020 2020 2020 2020 2020 2073 6570 3d73             sep=s
+00000890: 6570 0d0a 2020 2020 2020 2020 290d 0a0d  ep..        )...
+000008a0: 0a20 2020 2020 2020 2074 6173 6b5f 706f  .        task_po
+000008b0: 7075 6c61 7465 5f74 6162 6c61 5f65 7272  pulate_tabla_err
+000008c0: 6f72 203d 2050 6f70 756c 6174 654d 7373  or = PopulateMss
+000008d0: 716c 4f70 6572 6174 6f72 280d 0a20 2020  qlOperator(..   
+000008e0: 2020 2020 2020 2020 2074 6173 6b5f 6964           task_id
+000008f0: 3d74 6173 6b5f 6964 5f70 6f70 756c 6174  =task_id_populat
+00000900: 655f 7461 626c 615f 6572 726f 722c 0d0a  e_tabla_error,..
+00000910: 2020 2020 2020 2020 2020 2020 7175 6572              quer
+00000920: 795f 6669 6c65 3d6f 7574 7075 745f 6669  y_file=output_fi
+00000930: 6c65 5f73 716c 2c0d 0a20 2020 2020 2020  le_sql,..       
+00000940: 2020 2020 2063 6f6e 6e5f 6964 3d63 6f6e       conn_id=con
+00000950: 6e5f 6964 2c20 0d0a 2020 2020 2020 2020  n_id, ..        
+00000960: 2020 2020 7363 6865 6d61 3d73 6368 656d      schema=schem
+00000970: 612c 0d0a 0920 2020 2029 0d0a 0d0a 2020  a,...    )....  
+00000980: 2020 2020 2020 6272 616e 6368 5f74 6173        branch_tas
+00000990: 6b20 3e3e 2074 6173 6b5f 7472 616e 7366  k >> task_transf
+000009a0: 6f72 6d5f 6572 726f 7220 3e3e 2074 6173  orm_error >> tas
+000009b0: 6b5f 6765 6e65 7261 7465 5f69 6e73 6572  k_generate_inser
+000009c0: 745f 6572 726f 7220 3e3e 2074 6173 6b5f  t_error >> task_
+000009d0: 706f 7075 6c61 7465 5f74 6162 6c61 5f65  populate_tabla_e
+000009e0: 7272 6f72 0d0a 2020 2020 2020 2020 6272  rror..        br
+000009f0: 616e 6368 5f74 6173 6b20 3e3e 2064 756d  anch_task >> dum
+00000a00: 6d79 5f74 6173 6b0d 0a20 2020 2072 6574  my_task..    ret
+00000a10: 7572 6e20 7878 78                        urn xxx
```

### Comparing `ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/mssql/operators.py` & `ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/mssql/operators.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-import jinja2
-import logging
-import os
-import pandas as pd
-import pyodbc
-
-from airflow.models import BaseOperator
-from airflow.providers.microsoft.mssql.hooks.mssql import MsSqlHook
-
-from ecom_utils.scient.airflow.functions import get_dbconnection
-from ecom_utils.scient.airflow.sql.core.base import GenerateInsertOperator, PopulateOperator
-
-class MSSQLQueryToCSV(BaseOperator):
-	template_fields = ["output_file", "render_sql"]
-
-	def __init__(self, query, strconn, output_file, dtypes=None, render_sql=None,*args, **kwargs):
-		"""Ejecuta una consulta sobre una base de datos SQL SERVER, devolviendo el resultado en un archivo csv.
-
-		Args:
-			query (str): consulta en SQL
-			strconn (str): String de Conexion a la BD
-			output_file (str): Nombre del arhivo de salida
-			dtypes (duct, optional): Tipo de datos de entrada. Defaults to None.
-			render_sql (dict, optional): Indica si el archivo SQL necesita ser renderizado con el diccionario que se recibe como parametro. Defaults to None.
-		"""
-		super(MSSQLQueryToCSV, self).__init__(*args, **kwargs)
-		self.query=query
-		self.strconn=strconn
-		self.output_file=output_file
-		self.dtypes=dtypes
-		self.render_sql=render_sql
-
-	def execute(self, context):
-		if self.render_sql is not None:
-			t = jinja2.Template(self.query)
-			logging.info("Renderizando consulta...")
-			self.query=t.render(self.render_sql)
-			
-		with get_dbconnection(self.strconn, pyodbc) as conn:
-			logging.info(f"Running query: {self.query}")
-			
-			if self.dtypes is None:
-				df = pd.read_sql_query(self.query, conn)
-			else:
-				df = pd.read_sql_query(self.query, conn, dtype=self.dtypes)
-
-			df.to_csv(self.output_file, index=False)
-
-			logging.info(f"Archivo {self.output_file} creado exitosamente!")
-
-class GenerateInsertMssqlOperator(GenerateInsertOperator):
-	pass
-
-# ============================================================
-
-
-class PopulateMssqlOperator(PopulateOperator):
-	def get_conn(self):
-		pg_hook = MsSqlHook(mssql_conn_id=self.conn_id, schema=self.schema)
-		conn = pg_hook.get_conn()
+import jinja2
+import logging
+import os
+import pandas as pd
+import pyodbc
+
+from airflow.models import BaseOperator
+from airflow.providers.microsoft.mssql.hooks.mssql import MsSqlHook
+
+from ecom_utils.scient.airflow.functions import get_dbconnection
+from ecom_utils.scient.airflow.sql.core.base import GenerateInsertOperator, PopulateOperator
+
+class MSSQLQueryToCSV(BaseOperator):
+	template_fields = ["output_file", "render_sql"]
+
+	def __init__(self, query, strconn, output_file, dtypes=None, render_sql=None,*args, **kwargs):
+		"""Ejecuta una consulta sobre una base de datos SQL SERVER, devolviendo el resultado en un archivo csv.
+
+		Args:
+			query (str): consulta en SQL
+			strconn (str): String de Conexion a la BD
+			output_file (str): Nombre del arhivo de salida
+			dtypes (duct, optional): Tipo de datos de entrada. Defaults to None.
+			render_sql (dict, optional): Indica si el archivo SQL necesita ser renderizado con el diccionario que se recibe como parametro. Defaults to None.
+		"""
+		super(MSSQLQueryToCSV, self).__init__(*args, **kwargs)
+		self.query=query
+		self.strconn=strconn
+		self.output_file=output_file
+		self.dtypes=dtypes
+		self.render_sql=render_sql
+
+	def execute(self, context):
+		if self.render_sql is not None:
+			t = jinja2.Template(self.query)
+			logging.info("Renderizando consulta...")
+			self.query=t.render(self.render_sql)
+			
+		with get_dbconnection(self.strconn, pyodbc) as conn:
+			logging.info(f"Running query: {self.query}")
+			
+			if self.dtypes is None:
+				df = pd.read_sql_query(self.query, conn)
+			else:
+				df = pd.read_sql_query(self.query, conn, dtype=self.dtypes)
+
+			df.to_csv(self.output_file, index=False)
+
+			logging.info(f"Archivo {self.output_file} creado exitosamente!")
+
+class GenerateInsertMssqlOperator(GenerateInsertOperator):
+	pass
+
+# ============================================================
+
+
+class PopulateMssqlOperator(PopulateOperator):
+	def get_conn(self):
+		pg_hook = MsSqlHook(mssql_conn_id=self.conn_id, schema=self.schema)
+		conn = pg_hook.get_conn()
 		return conn
```

### Comparing `ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/postgres/functions.py` & `ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/postgres/functions.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from airflow.utils.task_group import TaskGroup
-
-from ecom_utils.scient.airflow.sql.postgres.operators import PopulatePostgresOperator, GenerateInsertPostgresOperator
-
-def postgres_populate(group_id, insert_task_id, insert_input_file, insert_input_output_file, insert_table_name, insert_data_cols, populate_task_id, populate_conn_id, encoding = "utf-8", sep=",", remove_input=True, populate_errors_file=None, insert_extras_args=[]):
-	with TaskGroup(group_id, tooltip=f"Tasks for {group_id}") as xxx:
-		task_1 = GenerateInsertPostgresOperator(
-			task_id=insert_task_id,
-			input_file=insert_input_file,
-			output_file=insert_input_output_file, 
-			table_name=insert_table_name, 
-			data_cols=insert_data_cols,
-			extras_args=insert_extras_args,
-			remove_input=remove_input,
-			sep=sep, 
-			encoding=encoding
-		)
-		task_2 = PopulatePostgresOperator(
-			task_id=populate_task_id,
-			POSTGRES_CONN_ID=populate_conn_id,
-			query_file=insert_input_output_file,
-			errors_file=populate_errors_file,
-			remove_input=remove_input
-		)
-
-		task_1 >> task_2
+from airflow.utils.task_group import TaskGroup
+
+from ecom_utils.scient.airflow.sql.postgres.operators import PopulatePostgresOperator, GenerateInsertPostgresOperator
+
+def postgres_populate(group_id, insert_task_id, insert_input_file, insert_input_output_file, insert_table_name, insert_data_cols, populate_task_id, populate_conn_id, encoding = "utf-8", sep=",", remove_input=True, populate_errors_file=None, insert_extras_args=[]):
+	with TaskGroup(group_id, tooltip=f"Tasks for {group_id}") as xxx:
+		task_1 = GenerateInsertPostgresOperator(
+			task_id=insert_task_id,
+			input_file=insert_input_file,
+			output_file=insert_input_output_file, 
+			table_name=insert_table_name, 
+			data_cols=insert_data_cols,
+			extras_args=insert_extras_args,
+			remove_input=remove_input,
+			sep=sep, 
+			encoding=encoding
+		)
+		task_2 = PopulatePostgresOperator(
+			task_id=populate_task_id,
+			POSTGRES_CONN_ID=populate_conn_id,
+			query_file=insert_input_output_file,
+			errors_file=populate_errors_file,
+			remove_input=remove_input
+		)
+
+		task_1 >> task_2
 	return xxx
```

### Comparing `ecom-utils-1.3.6/ecom_utils/scient/airflow/sql/postgres/operators.py` & `ecom-utils-1.3.7/ecom_utils/scient/airflow/sql/postgres/operators.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import logging
-import pandas as pd
-
-from airflow.hooks.postgres_hook import PostgresHook
-from airflow.models              import BaseOperator
-
-from ecom_utils.scient.airflow.sql.core.base import GenerateInsertOperator, PopulateOperator
-
-def execute_pg(query, conn_id):
-	status, message = False, ""
-	try:
-		pg_hook = PostgresHook(postgres_conn_id=conn_id)
-		conn = pg_hook.get_conn()
-		cur = conn.cursor()
-		cur.execute(query)
-		conn.commit()
-		status=True
-		message="Ok"
-	except Exception as e:
-		logging.error(f"Error ejecutando: {query} - {e}")
-		message=str(e)
-	finally:
-		cur.close()
-		conn.close()
-	return status, message
-
-class PopulatePostgresOperator(PopulateOperator):
-	def get_conn(conn_id):
-		pg_hook = PostgresHook(postgres_conn_id=conn_id)
-		conn = pg_hook.get_conn()
-		return conn
-
-class GenerateInsertPostgresOperator(GenerateInsertOperator):
-	pass
-
-class PgQueryToCSV(BaseOperator):
-	template_fields = ["output_file"]
-
-	def __init__(self, query, postgres_conn_id, output_file, dtypes=None, *args, **kwargs):
-		super(PgQueryToCSV, self).__init__(*args, **kwargs)
-		self.query=query
-		self.postgres_conn_id=postgres_conn_id
-		self.output_file=output_file
-		self.dtypes=dtypes
-
-	def execute(self, context):
-		pg_hook = PostgresHook(postgres_conn_id=self.postgres_conn_id)
-		conn = pg_hook.get_conn()
-
-		if self.dtypes is None:
-			df = pd.read_sql_query(self.query, conn)
-		else:
-			df = pd.read_sql_query(self.query, conn, dtype=self.dtypes)
-
-
-		df.to_csv(self.output_file, index=False)
+import logging
+import pandas as pd
+
+from airflow.hooks.postgres_hook import PostgresHook
+from airflow.models              import BaseOperator
+
+from ecom_utils.scient.airflow.sql.core.base import GenerateInsertOperator, PopulateOperator
+
+def execute_pg(query, conn_id):
+	status, message = False, ""
+	try:
+		pg_hook = PostgresHook(postgres_conn_id=conn_id)
+		conn = pg_hook.get_conn()
+		cur = conn.cursor()
+		cur.execute(query)
+		conn.commit()
+		status=True
+		message="Ok"
+	except Exception as e:
+		logging.error(f"Error ejecutando: {query} - {e}")
+		message=str(e)
+	finally:
+		cur.close()
+		conn.close()
+	return status, message
+
+class PopulatePostgresOperator(PopulateOperator):
+	def get_conn(conn_id):
+		pg_hook = PostgresHook(postgres_conn_id=conn_id)
+		conn = pg_hook.get_conn()
+		return conn
+
+class GenerateInsertPostgresOperator(GenerateInsertOperator):
+	pass
+
+class PgQueryToCSV(BaseOperator):
+	template_fields = ["output_file"]
+
+	def __init__(self, query, postgres_conn_id, output_file, dtypes=None, *args, **kwargs):
+		super(PgQueryToCSV, self).__init__(*args, **kwargs)
+		self.query=query
+		self.postgres_conn_id=postgres_conn_id
+		self.output_file=output_file
+		self.dtypes=dtypes
+
+	def execute(self, context):
+		pg_hook = PostgresHook(postgres_conn_id=self.postgres_conn_id)
+		conn = pg_hook.get_conn()
+
+		if self.dtypes is None:
+			df = pd.read_sql_query(self.query, conn)
+		else:
+			df = pd.read_sql_query(self.query, conn, dtype=self.dtypes)
+
+
+		df.to_csv(self.output_file, index=False)
 		logging.info(f"Archivo {self.output_file} creado exitosamente!")
```

### Comparing `ecom-utils-1.3.6/ecom_utils/tgd/base.py` & `ecom-utils-1.3.7/ecom_utils/tgd/base.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# ENDPOINT_STAGE = 'http://stage.ventanillaunica.chaco.gov.ar'
-# ENDPOINT_PROD = 'https://gobiernodigital.chaco.gob.ar'
-#
-# API_ENDPOINTS = {
-#     'oauth_base_uri': '_endpointbase_/oauth/v2/',
-#     'get_token_via_authorization_code': '_endpointbase_/oauth/v2/token',
-#     'get_token_application': '_endpointbase_/oauth/v2/token',
-#     'get_persona_via_cuil': '_endpointbase_/api/v1/persona/cuil/_cuil_',
-#     'get_persona_via_token': '_endpointbase_/api/v1/persona'
-# }
-#
-# # VERSION 2: Nueva llamada 2023
-#
-# ENDPOINT_STAGE_NEW = ' https://core.tgdpruebas.chaco.gob.ar'
-# ENDPOINT_PROD_NEW = 'https://gobiernodigital.chaco.gob.ar'
-#
-# API_ENDPOINTS_NEW = {
-#     'oauth_base_uri': '_endpointbase_',
-#     'get_token_via_authorization_code': '_endpointbase_/token',
-#     'get_token_application': '_endpointbase_/token',
-#     'get_persona_via_cuil': '_endpointbase_/api/v2/persona/cuil/_cuil_',
-#     'get_persona_via_token': '_endpointbase_/api/v2/persona'
-# }
-
-SETTINGS = {"V1": {"ENDPOINT_STAGE": 'http://stage.ventanillaunica.chaco.gov.ar',
-                   "ENDPOINT_PROD": 'https://gobiernodigital.chaco.gob.ar',
-                   "API_ENDPOINTS": {
-                       'oauth_base_uri': '_endpointbase_/oauth/v2/',
-                       'get_token_via_authorization_code': '_endpointbase_/oauth/v2/token',
-                       'get_token_application': '_endpointbase_/oauth/v2/token',
-                       'get_persona_via_cuil': '_endpointbase_/api/v1/persona/cuil/_cuil_',
-                       'get_persona_via_token': '_endpointbase_/api/v1/persona',
-                       'Content-Type': 'application/json'
-                   }
-                   },
-
-            "V1.1": {"ENDPOINT_STAGE": 'https://core.tgdpruebas.chaco.gob.ar',
-                     "ENDPOINT_PROD": 'https://gobiernodigital.chaco.gob.ar',
-                     "API_ENDPOINTS": {
-                         'oauth_base_uri': '_endpointbase_',
-                         'get_token_via_authorization_code': '_endpointbase_/token',
-                         'get_token_application': '_endpointbase_/token',
-                         'get_persona_via_cuil': '_endpointbase_/api/v2/persona/cuil/_cuil_',
-                         'get_persona_via_token': '_endpointbase_/api/v2/persona',
-                         'Content-Type': 'application/x-www-form-urlencoded'
-                     }
-                     },
-            }
+# ENDPOINT_STAGE = 'http://stage.ventanillaunica.chaco.gov.ar'
+# ENDPOINT_PROD = 'https://gobiernodigital.chaco.gob.ar'
+#
+# API_ENDPOINTS = {
+#     'oauth_base_uri': '_endpointbase_/oauth/v2/',
+#     'get_token_via_authorization_code': '_endpointbase_/oauth/v2/token',
+#     'get_token_application': '_endpointbase_/oauth/v2/token',
+#     'get_persona_via_cuil': '_endpointbase_/api/v1/persona/cuil/_cuil_',
+#     'get_persona_via_token': '_endpointbase_/api/v1/persona'
+# }
+#
+# # VERSION 2: Nueva llamada 2023
+#
+# ENDPOINT_STAGE_NEW = ' https://core.tgdpruebas.chaco.gob.ar'
+# ENDPOINT_PROD_NEW = 'https://gobiernodigital.chaco.gob.ar'
+#
+# API_ENDPOINTS_NEW = {
+#     'oauth_base_uri': '_endpointbase_',
+#     'get_token_via_authorization_code': '_endpointbase_/token',
+#     'get_token_application': '_endpointbase_/token',
+#     'get_persona_via_cuil': '_endpointbase_/api/v2/persona/cuil/_cuil_',
+#     'get_persona_via_token': '_endpointbase_/api/v2/persona'
+# }
+
+SETTINGS = {"V1": {"ENDPOINT_STAGE": 'http://stage.ventanillaunica.chaco.gov.ar',
+                   "ENDPOINT_PROD": 'https://gobiernodigital.chaco.gob.ar',
+                   "API_ENDPOINTS": {
+                       'oauth_base_uri': '_endpointbase_/oauth/v2/',
+                       'get_token_via_authorization_code': '_endpointbase_/oauth/v2/token',
+                       'get_token_application': '_endpointbase_/oauth/v2/token',
+                       'get_persona_via_cuil': '_endpointbase_/api/v1/persona/cuil/_cuil_',
+                       'get_persona_via_token': '_endpointbase_/api/v1/persona',
+                       'Content-Type': 'application/json'
+                   }
+                   },
+
+            "V1.1": {"ENDPOINT_STAGE": 'https://core.tgdpruebas.chaco.gob.ar',
+                     "ENDPOINT_PROD": 'https://gobiernodigital.chaco.gob.ar',
+                     "API_ENDPOINTS": {
+                         'oauth_base_uri': '_endpointbase_',
+                         'get_token_via_authorization_code': '_endpointbase_/token',
+                         'get_token_application': '_endpointbase_/token',
+                         'get_persona_via_cuil': '_endpointbase_/api/v2/persona/cuil/_cuil_',
+                         'get_persona_via_token': '_endpointbase_/api/v2/persona',
+                         'Content-Type': 'application/x-www-form-urlencoded'
+                     }
+                     },
+            }
```

### Comparing `ecom-utils-1.3.6/ecom_utils/tgd/core.py` & `ecom-utils-1.3.7/ecom_utils/tgd/core.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-import requests
-import json
-
-from datetime import datetime
-from .base import SETTINGS
-
-
-def get_endpoint_base(mode_stage, version):
-    """
-    Obtiene endpoint base acorde a el modo y su version. Ver el archivo de configuracion para los tipos de versiones permitidos.
-    """
-    if mode_stage:
-        return SETTINGS[version]["API_ENDPOINTS"]["oauth_base_uri"].replace("_endpointbase_",
-                                                                            SETTINGS[version]["ENDPOINT_STAGE"])
-    return SETTINGS[version]["API_ENDPOINTS"]["oauth_base_uri"].replace("_endpointbase_",
-                                                                        SETTINGS[version]["ENDPOINT_PROD"])
-
-
-class TGD():
-    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="v1"):
-        self.client_id = client_id
-        self.client_secret = client_secret
-        self.url_base = url_base
-        self.redirect_url = redirect_url
-        self.mode_stage = mode_stage
-        self.version = version
-
-    def get_endpoint_base(self):
-        """
-        Obtiene endpoint base acorde a el modo y su version. Ver el archivo de configuracion para los tipos de versiones permitidos.
-        """
-        if self.mode_stage:
-            # print(f'GEB1- stage')
-            return SETTINGS[self.version]["ENDPOINT_STAGE"]
-        return SETTINGS[self.version]["ENDPOINT_PROD"]
-
-    def get_token_application(self):
-        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_token_application'].replace("_endpointbase_",
-                                                                                       self.get_endpoint_base())
-        # print(f'GTA1-{url}')
-        payload = (
-        ("grant_type", "client_credentials"), ("client_id", self.client_id), ('client_secret', self.client_secret))
-        # print(f'GTA2-{payload}')
-        response = requests.get(url, headers={'Content-Type': 'application/json'}, params=payload)
-        access_token, expires_in = None, None
-        # print(f'GTA3-{response}')
-        if response.status_code == 200:
-            data = response.json()
-            access_token = data['access_token']
-            expires_in = data['expires_in']
-        # print(f'GTA4-{access_token} {expires_in}')
-        return access_token, expires_in
-
-
-class TGD_OAUTH(TGD):
-    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="V1"):
-        super().__init__(mode_stage=mode_stage, client_id=client_id, client_secret=client_secret, url_base=url_base,
-                         redirect_url=redirect_url, version=version)
-
-    def get_user_by_cuil(self, cuil):
-        # print(f'GUBC1-{cuil}')
-        access_token, expires_in = self.get_token_application()
-        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_persona_via_cuil'].replace('_cuil_', cuil)
-        # print(f'GUBC2-{access_token} {url}')
-        user = None
-        message = None
-        if access_token and expires_in:
-            # print(f'GUBC3-dentro')
-            response = requests.get(url, headers={'Content-Type': 'application/json',
-                                                  'Authorization': 'Bearer %s' % access_token})
-            # print(f'GUBC4-{response}')
-            if response.status_code == 200:
-                data = response.json()
-                # print(f'GUBC5-{data}')
-                user = {'cuil': data['cuitCuil'], 'apellidos': data['apellidos'], 'nombres': data['nombres'],
-                        'id': data['id']}
-            elif response.status_code == 403:
-                data = response.json()
-                # print(f'GUBC6-{data}')
-                message = data["message"]
-            else:
-                # print(f'GUBC7-error')
-                message = "Ha ocurrido un inconveniente, contáctese con el Adminstrador (CODE_ERROR: 10-01-01 L45[%s])" % response.status_code
-
-        # message = "Usuario obtenido corectamente"
-        # user = {'cuil': '20362069247', 'apellidos': 'IBANEZ', 'nombres': 'Lucas Sebastian', 'id': 123456}
-        # print(f'GUBC8-{user}')
-        return user, message
-
-    def get_token_via_authorization_code(self, code):
-        # print(f'GTVAC1-{code}')
-        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_token_via_authorization_code'].replace("_endpointbase_",
-                                                                                                  self.get_endpoint_base())
-        # print(f'GTVAC2-{url}')
-        payload = (
-            ("code", code),
-            ("grant_type", "authorization_code"),
-            ("client_id", self.client_id),
-            ('client_secret', self.client_secret),
-            ("redirect_uri", self.redirect_url)
-        )
-        # print(f'GTVAC3-{payload}')
-        if SETTINGS[self.version] == "V1":
-            # print("1 ",SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type'])
-            response = requests.get(url, headers={'Content-Type': SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type']}, params=payload)
-        else:
-            # print("2 ",SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type'])
-            response = requests.post(url,
-                                    headers={'Content-Type': SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type']},
-                                    data=payload)
-        access_token, expires_in, refresh_token = None, None, None
-        # print(f'GTVAC4-{response}')
-        if response.status_code == 200:
-            data = response.json()
-            access_token = data['access_token']
-            expires_in = data['expires_in']
-            refresh_token = data['refresh_token']
-            # print(f'GTVAC5-{data}')
-        return access_token, expires_in, refresh_token
-
-    def get_persona_via_token(self, access_token):
-        # print(f'GPVT1-{access_token}')
-        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_persona_via_token'].replace("_endpointbase_",
-                                                                                       self.get_endpoint_base())
-        # print(f'GPVT2-{url}')
-        response = requests.get(url, headers={'Content-Type': 'application/json',
-                                              'Authorization': 'Bearer %s' % (access_token)})
-        # print(f'GPVT3-{response}')
-        user, message = None, None
-        if response.status_code == 200:
-            data = response.json()
-            email = None
-            # print(f'GPVT1-{data}')
-            try:
-                email = data['emails'][0]['email']
-            except Exception as e:
-                print("ERROR - " + str(e))
-                pass
-
-            dni = None
-            for documento in data.get("tiposDocumentoPersona", []):
-                if documento["tipoDocumento"]["tipoDocumento"] == "DNI":
-                    dni = documento["numeroDocumento"]
-                    break
-            fecha_nacimiento = None
-            if data['fechaNacimiento']:  # FORMATO: 2020-06-26T10:24:13-0300
-                fecha_nacimiento = datetime.strptime(data['fechaNacimiento'], '%Y-%m-%dT%H:%M:%S%z')
-            user = {'cuil': data['cuitCuil'],
-                    'apellidos': data['apellidos'],
-                    'nombres': data['nombres'],
-                    'id': data['id'],
-                    'email': email,
-                    'sexo': data['sexo'],
-                    'fecha_nacimiento': fecha_nacimiento,
-                    'dni': dni}
-        # print(f'GPVT2-{user}')
-        return user, message
-
-
-class ApiComunicaciones(TGD_OAUTH):
-    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="v1"):
-        super().__init__(mode_stage=mode_stage, client_id=client_id, client_secret=client_secret, url_base=url_base,
-                         redirect_url=redirect_url, version=version)
-
-    def enviar_notificacion(self, asunto, plazo_dias, contenido, persona_envia, cuils=[], cuof="6-283-0",
-                            lectura_obligatoria=False):
-        access_token, expires_in = self.get_token_application()
-        url = SETTINGS[self.version]["API_ENDPOINTS"]['comunicaciones'].replace("_endpointbase_", self.get_endpoint_base())
-
-        data = None
-        status = False
-
-        x = {
-            "cuof": cuof,
-            "asunto": asunto,
-            "contenido": contenido,
-            "plazoDias": plazo_dias,
-            "cuils": cuils,
-            "lecturaObligatoria": lectura_obligatoria,
-            "personaEnvia": persona_envia
-        }
-        if access_token and expires_in:
-            response = requests.post(url, headers={'Content-Type': 'application/json',
-                                                   'Authorization': 'Bearer %s' % access_token}, data=json.dumps(x))
-
-            if response.status_code in [200, 201]:
-                data = response.json()
-                status = True
-            else:
-                try:
-                    data = response.json()
-                except Exception as e:
-                    data = {"error": str(e)}
-
-        return data, status
+import requests
+import json
+
+from datetime import datetime
+from .base import SETTINGS
+
+
+def get_endpoint_base(mode_stage, version):
+    """
+    Obtiene endpoint base acorde a el modo y su version. Ver el archivo de configuracion para los tipos de versiones permitidos.
+    """
+    if mode_stage:
+        return SETTINGS[version]["API_ENDPOINTS"]["oauth_base_uri"].replace("_endpointbase_",
+                                                                            SETTINGS[version]["ENDPOINT_STAGE"])
+    return SETTINGS[version]["API_ENDPOINTS"]["oauth_base_uri"].replace("_endpointbase_",
+                                                                        SETTINGS[version]["ENDPOINT_PROD"])
+
+
+class TGD():
+    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="v1"):
+        self.client_id = client_id
+        self.client_secret = client_secret
+        self.url_base = url_base
+        self.redirect_url = redirect_url
+        self.mode_stage = mode_stage
+        self.version = version
+
+    def get_endpoint_base(self):
+        """
+        Obtiene endpoint base acorde a el modo y su version. Ver el archivo de configuracion para los tipos de versiones permitidos.
+        """
+        if self.mode_stage:
+            # print(f'GEB1- stage')
+            return SETTINGS[self.version]["ENDPOINT_STAGE"]
+        return SETTINGS[self.version]["ENDPOINT_PROD"]
+
+    def get_token_application(self):
+        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_token_application'].replace("_endpointbase_",
+                                                                                       self.get_endpoint_base())
+        # print(f'GTA1-{url}')
+        payload = (
+        ("grant_type", "client_credentials"), ("client_id", self.client_id), ('client_secret', self.client_secret))
+        # print(f'GTA2-{payload}')
+        response = requests.get(url, headers={'Content-Type': 'application/json'}, params=payload)
+        access_token, expires_in = None, None
+        # print(f'GTA3-{response}')
+        if response.status_code == 200:
+            data = response.json()
+            access_token = data['access_token']
+            expires_in = data['expires_in']
+        # print(f'GTA4-{access_token} {expires_in}')
+        return access_token, expires_in
+
+
+class TGD_OAUTH(TGD):
+    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="V1"):
+        super().__init__(mode_stage=mode_stage, client_id=client_id, client_secret=client_secret, url_base=url_base,
+                         redirect_url=redirect_url, version=version)
+
+    def get_user_by_cuil(self, cuil):
+        # print(f'GUBC1-{cuil}')
+        access_token, expires_in = self.get_token_application()
+        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_persona_via_cuil'].replace('_cuil_', cuil)
+        # print(f'GUBC2-{access_token} {url}')
+        user = None
+        message = None
+        if access_token and expires_in:
+            # print(f'GUBC3-dentro')
+            response = requests.get(url, headers={'Content-Type': 'application/json',
+                                                  'Authorization': 'Bearer %s' % access_token})
+            # print(f'GUBC4-{response}')
+            if response.status_code == 200:
+                data = response.json()
+                # print(f'GUBC5-{data}')
+                user = {'cuil': data['cuitCuil'], 'apellidos': data['apellidos'], 'nombres': data['nombres'],
+                        'id': data['id']}
+            elif response.status_code == 403:
+                data = response.json()
+                # print(f'GUBC6-{data}')
+                message = data["message"]
+            else:
+                # print(f'GUBC7-error')
+                message = "Ha ocurrido un inconveniente, contáctese con el Adminstrador (CODE_ERROR: 10-01-01 L45[%s])" % response.status_code
+
+        # message = "Usuario obtenido corectamente"
+        # user = {'cuil': '20362069247', 'apellidos': 'IBANEZ', 'nombres': 'Lucas Sebastian', 'id': 123456}
+        # print(f'GUBC8-{user}')
+        return user, message
+
+    def get_token_via_authorization_code(self, code):
+        # print(f'GTVAC1-{code}')
+        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_token_via_authorization_code'].replace("_endpointbase_",
+                                                                                                  self.get_endpoint_base())
+        # print(f'GTVAC2-{url}')
+        payload = (
+            ("code", code),
+            ("grant_type", "authorization_code"),
+            ("client_id", self.client_id),
+            ('client_secret', self.client_secret),
+            ("redirect_uri", self.redirect_url)
+        )
+        # print(f'GTVAC3-{payload}')
+        if SETTINGS[self.version] == "V1":
+            # print("1 ",SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type'])
+            response = requests.get(url, headers={'Content-Type': SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type']}, params=payload)
+        else:
+            # print("2 ",SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type'])
+            response = requests.post(url,
+                                    headers={'Content-Type': SETTINGS[self.version]["API_ENDPOINTS"]['Content-Type']},
+                                    data=payload)
+        access_token, expires_in, refresh_token = None, None, None
+        # print(f'GTVAC4-{response}')
+        if response.status_code == 200:
+            data = response.json()
+            access_token = data['access_token']
+            expires_in = data['expires_in']
+            refresh_token = data['refresh_token']
+            # print(f'GTVAC5-{data}')
+        return access_token, expires_in, refresh_token
+
+    def get_persona_via_token(self, access_token):
+        # print(f'GPVT1-{access_token}')
+        url = SETTINGS[self.version]["API_ENDPOINTS"]['get_persona_via_token'].replace("_endpointbase_",
+                                                                                       self.get_endpoint_base())
+        # print(f'GPVT2-{url}')
+        response = requests.get(url, headers={'Content-Type': 'application/json',
+                                              'Authorization': 'Bearer %s' % (access_token)})
+        # print(f'GPVT3-{response}')
+        user, message = None, None
+        if response.status_code == 200:
+            data = response.json()
+            email = None
+            # print(f'GPVT1-{data}')
+            try:
+                email = data['emails'][0]['email']
+            except Exception as e:
+                print("ERROR - " + str(e))
+                pass
+
+            dni = None
+            for documento in data.get("tiposDocumentoPersona", []):
+                if documento["tipoDocumento"]["tipoDocumento"] == "DNI":
+                    dni = documento["numeroDocumento"]
+                    break
+            fecha_nacimiento = None
+            if data['fechaNacimiento']:  # FORMATO: 2020-06-26T10:24:13-0300
+                fecha_nacimiento = datetime.strptime(data['fechaNacimiento'], '%Y-%m-%dT%H:%M:%S%z')
+            user = {'cuil': data['cuitCuil'],
+                    'apellidos': data['apellidos'],
+                    'nombres': data['nombres'],
+                    'id': data['id'],
+                    'email': email,
+                    'sexo': data['sexo'],
+                    'fecha_nacimiento': fecha_nacimiento,
+                    'dni': dni}
+        # print(f'GPVT2-{user}')
+        return user, message
+
+
+class ApiComunicaciones(TGD_OAUTH):
+    def __init__(self, client_id, client_secret, url_base, redirect_url, mode_stage=True, version="v1"):
+        super().__init__(mode_stage=mode_stage, client_id=client_id, client_secret=client_secret, url_base=url_base,
+                         redirect_url=redirect_url, version=version)
+
+    def enviar_notificacion(self, asunto, plazo_dias, contenido, persona_envia, cuils=[], cuof="6-283-0",
+                            lectura_obligatoria=False):
+        access_token, expires_in = self.get_token_application()
+        url = SETTINGS[self.version]["API_ENDPOINTS"]['comunicaciones'].replace("_endpointbase_", self.get_endpoint_base())
+
+        data = None
+        status = False
+
+        x = {
+            "cuof": cuof,
+            "asunto": asunto,
+            "contenido": contenido,
+            "plazoDias": plazo_dias,
+            "cuils": cuils,
+            "lecturaObligatoria": lectura_obligatoria,
+            "personaEnvia": persona_envia
+        }
+        if access_token and expires_in:
+            response = requests.post(url, headers={'Content-Type': 'application/json',
+                                                   'Authorization': 'Bearer %s' % access_token}, data=json.dumps(x))
+
+            if response.status_code in [200, 201]:
+                data = response.json()
+                status = True
+            else:
+                try:
+                    data = response.json()
+                except Exception as e:
+                    data = {"error": str(e)}
+
+        return data, status
```

### Comparing `ecom-utils-1.3.6/ecom_utils.egg-info/SOURCES.txt` & `ecom-utils-1.3.7/ecom_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

