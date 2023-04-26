# Comparing `tmp/SalesforceMinu-0.0.1.tar.gz` & `tmp/SalesforceMinu-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.1.tar", last modified: Tue Apr 25 17:54:16 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.2.tar", last modified: Tue Apr 25 20:15:38 2023, max compression
```

## Comparing `SalesforceMinu-0.0.1.tar` & `SalesforceMinu-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-25 17:54:16.266339 SalesforceMinu-0.0.1/
--rw-rw-rw-   0        0        0      419 2023-04-25 17:54:16.266339 SalesforceMinu-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      103 2023-04-25 17:20:16.000000 SalesforceMinu-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-25 17:54:16.251378 SalesforceMinu-0.0.1/SalesforceMinu/
--rw-rw-rw-   0        0        0     4082 2023-04-25 17:17:42.000000 SalesforceMinu-0.0.1/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.1/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-25 17:54:16.265343 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-25 17:54:15.000000 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-04-25 17:54:16.000000 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-25 17:54:15.000000 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 17:54:15.000000 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-25 17:54:15.000000 SalesforceMinu-0.0.1/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-25 17:54:16.267336 SalesforceMinu-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-04-25 17:53:10.000000 SalesforceMinu-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.332517 SalesforceMinu-0.0.2/
+-rw-rw-rw-   0        0        0      419 2023-04-25 20:15:38.331518 SalesforceMinu-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-04-25 17:20:16.000000 SalesforceMinu-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.316676 SalesforceMinu-0.0.2/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4100 2023-04-25 19:40:31.000000 SalesforceMinu-0.0.2/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.2/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 20:15:38.330520 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-25 20:15:38.000000 SalesforceMinu-0.0.2/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-25 20:15:38.332517 SalesforceMinu-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-04-25 20:14:24.000000 SalesforceMinu-0.0.2/setup.py
```

### Comparing `SalesforceMinu-0.0.1/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.2/SalesforceMinu/Funciones.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         names = ",".join(df[title])
     # Convertimos a lista
     names = names.split(',')
     return names
 
 # OBTENER LOS IDS DE ACCOUNT Y EL ORDEN DE SUS NOMBRE
 # Si no encuentra el nombre que mande mensaje de error o algo
-def get_account_id_names(names):
+def get_account_id_names(names,sf):
     # Puede ser un nombre o varios
     case = 0
     if type(names) == str:
         where = f"Name = '{str(names)[1:-1]}'"
     else:
         where = f"Name IN ({str(names)[1:-1]})"
         case = 1
@@ -40,15 +40,15 @@
     if case == 1 and len(names) != len(Names_order):
         raise ValueError("No se encontro una o más empresas")
     elif case == 0 and Names_order == []:
         raise ValueError("No se encontro el nombre de la empresa")
     return Names_order, IDs
 
 # OBTENER LOS SUSCRIPTORES DE EMPRESAS
-def get_subs(account_ids):
+def get_subs(account_ids,sf):
     # Puede ser un ID o varios
     razones = [sf.query_all(f"""SELECT Head_count__c
                       FROM Raz_n_Social__c
                       WHERE Cuenta__c = '{row}'""")['records'] for row in account_ids]
     # Puede haber más de una razón por empresa
     subs = []
     for i in range(len(razones)):
@@ -59,37 +59,37 @@
             for j in range(len(razones[i])):
                 lis.append(razones[i][j]['Head_count__c'])
             subs.append(sum(lis))
     
     return subs
     
 # OBTENEMOS FECHA CIERRE DE CONTRATO
-def get_contract_dates(account_ids):
+def get_contract_dates(account_ids,sf):
     contract_dates = [sf.query_all(f"""SELECT Fecha_cierre_en_el_contrato__c
                       FROM Opportunity
                       WHERE AccountId = '{row}'""")['records'][0]['Fecha_cierre_en_el_contrato__c'] for row in account_ids]
     return contract_dates
 
 # OBTENEMOS OPPORTUNITY IDS
-def get_opportunity_ids(account_ids):
+def get_opportunity_ids(account_ids,sf):
     opportunity_ids = [sf.query_all(f"""SELECT Id
                       FROM Opportunity
                       WHERE AccountId = '{row}'""")['records'][0]['Id'] for row in account_ids]
     return opportunity_ids
 
 # OBTENEMOS EL PRODUCTID
-def get_product_id(opportunity_ids):
+def get_product_id(opportunity_ids,sf):
     products_ids = [sf.query_all(f"""SELECT Product2Id
                       FROM OpportunityLineItem
                       WHERE OpportunityId = '{row}'""")['records'][0]['Product2Id'] for row in opportunity_ids]
     return products_ids
     
 
 # OBTENEMOS MODELO DE SUSCRIPCIÓN, EL CODIGO Y SU NOMBRE
-def get_model(products_ids):
+def get_model(products_ids,sf):
     
     dict_plan = {'005':'starter',
              '009':'starter',
              '011':'starter',
              '013':'starter',
              '006':'total',
              '008':'total',
```

### Comparing `SalesforceMinu-0.0.1/setup.py` & `SalesforceMinu-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

