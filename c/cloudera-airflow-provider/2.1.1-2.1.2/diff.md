# Comparing `tmp/cloudera-airflow-provider-2.1.1.tar.gz` & `tmp/cloudera-airflow-provider-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudera-airflow-provider-2.1.1.tar", last modified: Wed Feb 22 12:59:04 2023, max compression
+gzip compressed data, was "cloudera-airflow-provider-2.1.2.tar", last modified: Tue Apr 25 16:56:18 2023, max compression
```

## Comparing `cloudera-airflow-provider-2.1.1.tar` & `cloudera-airflow-provider-2.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/
--rw-r--r--   0 jenkins   (1001) users      (100)    11358 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/LICENSE
--rw-r--r--   0 jenkins   (1001) users      (100)      222 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     9141 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/README.md
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/airflow/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/
--rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/__init__.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/
--rw-r--r--   0 jenkins   (1001) users      (100)     2336 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)    20327 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cde.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2275 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cde_hook.py
--rw-r--r--   0 jenkins   (1001) users      (100)    16751 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cdw.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2309 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cdw_hook.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/model/
--rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/model/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     7578 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/model/connection.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/
--rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)    14817 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cde.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2275 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cde_operator.py
--rw-r--r--   0 jenkins   (1001) users      (100)     4713 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cdw.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2281 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cdw_operator.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/
--rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     3448 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/cdw.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2274 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/cdw_sensor.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.650642 cloudera-airflow-provider-2.1.1/cloudera/cdp/
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/
--rw-r--r--   0 jenkins   (1001) users      (100)     3071 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/__init__.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/
--rw-r--r--   0 jenkins   (1001) users      (100)     2270 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2320 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/cde_hook.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2344 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/cdw_hook.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/model/
--rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/model/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2293 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/model/connection.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/
--rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2296 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/cde_operator.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2295 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/cdw_operator.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/sensors/
--rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/sensors/__init__.py
--rw-r--r--   0 jenkins   (1001) users      (100)     2300 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/sensors/cdw_sensor.py
-drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/
--rw-r--r--   0 jenkins   (1001) users      (100)      222 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) users      (100)     1510 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) users      (100)       82 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/entry_points.txt
--rw-r--r--   0 jenkins   (1001) users      (100)      114 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) users      (100)        9 2023-02-22 12:59:04.000000 cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) users      (100)      669 2023-02-22 12:59:04.654642 cloudera-airflow-provider-2.1.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) users      (100)       62 2023-02-22 12:59:03.000000 cloudera-airflow-provider-2.1.1/setup.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/
+-rw-r--r--   0 jenkins   (1001) users      (100)    11358 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/LICENSE
+-rw-r--r--   0 jenkins   (1001) users      (100)      222 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     9141 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/README.md
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.923493 cloudera-airflow-provider-2.1.2/cloudera/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.923493 cloudera-airflow-provider-2.1.2/cloudera/airflow/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.923493 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/
+-rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/__init__.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/
+-rw-r--r--   0 jenkins   (1001) users      (100)     2336 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    27995 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cde.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2275 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cde_hook.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    16751 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cdw.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2309 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cdw_hook.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/model/
+-rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/model/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     7578 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/model/connection.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/
+-rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)    14817 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cde.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2275 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cde_operator.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     4713 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cdw.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2281 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cdw_operator.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/
+-rw-r--r--   0 jenkins   (1001) users      (100)     1886 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     3448 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/cdw.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2274 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/cdw_sensor.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.923493 cloudera-airflow-provider-2.1.2/cloudera/cdp/
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/
+-rw-r--r--   0 jenkins   (1001) users      (100)     3071 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/__init__.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/
+-rw-r--r--   0 jenkins   (1001) users      (100)     2270 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2320 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/cde_hook.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2344 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/cdw_hook.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/model/
+-rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/model/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2293 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/model/connection.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/
+-rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2296 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/cde_operator.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2295 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/cdw_operator.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/sensors/
+-rw-r--r--   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/sensors/__init__.py
+-rw-r--r--   0 jenkins   (1001) users      (100)     2300 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/sensors/cdw_sensor.py
+drwxr-sr-x   0 jenkins   (1001) users      (100)        0 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/
+-rw-r--r--   0 jenkins   (1001) users      (100)      222 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) users      (100)     1510 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        1 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)       82 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)      114 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)        9 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) users      (100)      669 2023-04-25 16:56:18.927492 cloudera-airflow-provider-2.1.2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) users      (100)       62 2023-04-25 16:56:18.000000 cloudera-airflow-provider-2.1.2/setup.py
```

### Comparing `cloudera-airflow-provider-2.1.1/LICENSE` & `cloudera-airflow-provider-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/README.md` & `cloudera-airflow-provider-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cde.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cde.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,36 +35,182 @@
 """
 Holds airflow hook functionalities for CDE clusters like submitting a CDE job,
 checking its status or killing it.
 """
 
 from __future__ import annotations
 
+import datetime
 import logging
 import os
-from typing import Any
+import typing
+from datetime import timedelta
+from typing import Any, Callable, Tuple, Type
 
 import requests
 import tenacity  # type: ignore
 from cloudera.cdp.model.cde import VirtualCluster
 from cloudera.cdp.security import SecurityError
 from cloudera.cdp.security.cde_security import BearerAuth, CdeApiTokenAuth, CdeTokenAuthResponse
 from cloudera.cdp.security.cdp_security import CdpAccessKeyCredentials, CdpAccessKeyV2TokenAuth
 from cloudera.cdp.security.token_cache import EncryptedFileTokenCacheStrategy
 
 from airflow.configuration import conf
-from airflow.exceptions import AirflowException, AirflowConfigException  # type: ignore
+from airflow.exceptions import AirflowConfigException, AirflowException  # type: ignore
 from airflow.hooks.base import BaseHook  # type: ignore
 from airflow.providers.http.hooks.http import HttpHook  # type: ignore
 from cloudera.airflow.providers.hooks import CdpHookException
 from cloudera.airflow.providers.model.connection import CdeConnection
+from tenacity.stop import stop_base
+from tenacity.wait import wait_base
+
+DEFAULT_RETRY_INTERVAL = 4
+RETRY_AFTER_HEADER = "Retry-After"
+time_unit_type = typing.Union[int, float, timedelta]
 
 HTTP_EMPTY_BODY_RESPONSES = [b'', None]
 
 
+class CustomWait(wait_base):
+    """Custom wait class to handle Rate-limited retries (HTTP 429 + Retry-After header) separately.
+    Under normal circumstances, we use tenacity's exponential retry.
+    If the server's HTTP response code is 429, we use the fixed retry.
+    If the server has sent the 'Retry-After' header, the wait time between retries will be that value,
+    otherwise 4 seconds as a default.
+    """
+
+    def __init__(self, logger) -> None:
+        self.log = logger
+        self.wait_fixed_cls: Type[tenacity.wait_base] = tenacity.wait_fixed
+        self.wait_exponential_obj: Type[tenacity.wait_base] = tenacity.wait_exponential()
+        self.start_of_retries_logged = False
+
+    def __call__(self, retry_state: "RetryCallState") -> float:
+        if isinstance(retry_state.outcome, tenacity.Future):
+            future_outcome: tenacity.Future = retry_state.outcome
+            if not future_outcome.failed and isinstance(future_outcome.result(), requests.Response):
+                response: requests.Response = future_outcome.result()
+                if response.status_code == 429:
+                    # We wait a fixed interval for HTTP 429
+                    retry_after = self._get_retry_after_value(response)
+                    return self._wait_fixed(retry_state, retry_after)
+        return self._wait_exponential(retry_state)
+
+    def _wait_exponential(self, retry_state: "RetryCallState"):
+        self.log.debug("Waiting exponentially between requests")
+        return self.wait_exponential_obj(retry_state=retry_state)
+
+    def _wait_fixed(self, retry_state: "RetryCallState", retry_after: int):
+        if not self.start_of_retries_logged:
+            self.log.info("The server is overloaded and this request has been rejected due to server-side throttling. "
+                          "The request will be retried regularly until it gets accepted or typically fails after 2 hours of retry.")
+            self.start_of_retries_logged = True
+
+        # Since the value of retry after second can change from response to response,
+        # we need to instantiate tenacity.wait_fixed class here to have the correct value on each retry
+        self.log.debug("The server is overloaded and this request has been rejected due to server-side throttling (HTTP 429). "
+                       "Waiting fixed interval of %d seconds between requests", retry_after)
+        return self.wait_fixed_cls(retry_after)(retry_state=retry_state)
+
+    def _get_retry_after_value(self, response: requests.Response) -> int:
+        if RETRY_AFTER_HEADER in response.headers:
+            return self._parse_retry_after_as_int(response, DEFAULT_RETRY_INTERVAL)
+        else:
+            self.log.warning(
+                "Cannot find '%s' header in response, using default wait interval of %d seconds",
+                RETRY_AFTER_HEADER,
+                DEFAULT_RETRY_INTERVAL)
+            return DEFAULT_RETRY_INTERVAL
+
+    def _parse_retry_after_as_int(self, response: requests.Response, default_value: int) -> int:
+        header_value = response.headers[RETRY_AFTER_HEADER]
+        try:
+            int_value = int(header_value)
+            return int_value
+        except ValueError:
+            self.log.warning("Failed to parse '%s' as int, value of header was: %s. "
+                             "Using default wait interval of %d seconds",
+                             RETRY_AFTER_HEADER, header_value,
+                             DEFAULT_RETRY_INTERVAL)
+            return default_value
+
+
+class RateLimitedStop(stop_base):
+    TEN_MINUTES = 10 * 60
+
+    @staticmethod
+    def _to_seconds(time_unit: time_unit_type) -> float:
+        return float(time_unit.total_seconds() if isinstance(time_unit, timedelta) else time_unit)
+
+    def __init__(self, logger,
+                 num_retries: int,
+                 time_unit: time_unit_type) -> None:
+        self.log = logger
+        self.num_retries = num_retries
+        self.max_seconds_of_retries = self._to_seconds(time_unit)
+        self.stop_after_attempt: Type[tenacity.stop_base] = tenacity.stop_after_attempt(num_retries)
+        self.stop_after_delay: Type[tenacity.stop_base] = tenacity.stop_after_delay(self.max_seconds_of_retries)
+        self.log_start = datetime.datetime.now()
+
+    def __call__(self, retry_state: "RetryCallState") -> float:
+        seconds_since_start = retry_state.seconds_since_start
+        seconds_left = self.max_seconds_of_retries - seconds_since_start
+
+        self.log.debug("Request throttling (Rate limiting) retry progress: "
+                       "Number of retries: %s, "
+                       "Maximum time span of retries (in seconds): %d, "
+                       "Seconds left: %s", self.num_retries, self.max_seconds_of_retries, seconds_left)
+
+        stop_after_attempt_res = self.stop_after_attempt(retry_state)
+        stop_after_delay_res = self.stop_after_delay(retry_state)
+
+        if stop_after_attempt_res:
+            self.log.info("Stopping Rate-Limited retries as maximum number of retries exceeded. "
+                          "Please note that the server might still be overloaded.")
+        if stop_after_delay_res:
+            self.log.info("Stopping Rate-limited retries as maximum time span exceeded. "
+                          "Please note that the server might still be overloaded.")
+        else:
+            now = datetime.datetime.now()
+            seconds_elapsed = (now - self.log_start).total_seconds()
+            if seconds_elapsed >= RateLimitedStop.TEN_MINUTES:
+                self.log.info("Still retrying, as the server is overloaded. "
+                              "Please note that this message is printed every 10 minutes to indicate progress.")
+                self.log_start = now
+        return any([stop_after_attempt_res, stop_after_delay_res])
+
+
+class CustomStop(stop_base):
+    """
+    Custom stop class to handle Rate-limited retries (HTTP 429 + Retry-After) in a special way.
+    Under normal circumstances, we use tenacity's stop_after_attempt method.
+    If the server's HTTP response code is 429, we retry with fixed delays between retries, please refer to RateLimitedStop for more details.
+    Otherwise, with the normal wait, we stop after default_num_retries.
+    """
+
+    def __init__(self, logger,
+                 default_num_retries: int,
+                 rate_limited_num_retries: int,
+                 retry_time_span: time_unit_type) -> None:
+        self.log = logger
+        self.default_num_retries = default_num_retries
+        self.normal_stop = tenacity.stop_after_attempt(self.default_num_retries)
+        self.rate_limited_stop = RateLimitedStop(logger, rate_limited_num_retries, retry_time_span)
+
+    def __call__(self, retry_state: "RetryCallState") -> float:
+        if isinstance(retry_state.outcome, tenacity.Future):
+            future_outcome: tenacity.Future = retry_state.outcome
+            if not future_outcome.failed and isinstance(future_outcome.result(), requests.Response):
+                response: requests.Response = future_outcome.result()
+                if response.status_code == 429:
+                    return self.rate_limited_stop(retry_state)
+        self.log.debug("Using normal Tenacity stop object, number of retries: %s", self.default_num_retries)
+        return self.normal_stop(retry_state)
+
+
 class CdeHookException(CdpHookException):
     """Root exception for the CdeHook which is used to handle any known exceptions"""
 
 
 class CdeHook(BaseHook):  # type: ignore
     """A wrapper around the CDE Virtual Cluster REST API."""
 
@@ -83,21 +229,23 @@
                 "password": "CDP Private Key",
             },
         }
 
     DEFAULT_CONN_ID = "cde_runtime_api"
     # Gives a total of at least 2^8+2^7+...2=510 seconds of retry with exponential backoff
     DEFAULT_NUM_RETRIES = 9
+    DEFAULT_NUM_RETRIES_RATE_LIMITED = 1800  # 4 seconds * 1800 --> 2 hours worth of retries
+    RETRY_TIME_SPAN_FOR_RATE_LIMIT = datetime.timedelta(hours=2)
     DEFAULT_API_TIMEOUT = 300
 
     def __init__(
         self,
         connection_id: str = DEFAULT_CONN_ID,
         num_retries: int | None = None,
-        api_timeout: int | None = None,
+        api_timeout: int | None = None
     ) -> None:
         """
         Create a new CdeHook. The connection parameters are eagerly validated to highlight
         any problems early.
 
         :param connection_id: The connection name for the target virtual cluster API
             (default: {CdeHook.DEFAULT_CONN_ID}).
@@ -157,15 +305,14 @@
         self.api_timeout = api_timeout_val
 
     def _do_api_call(
         self,
         method: str,
         endpoint: str,
         timeout: int,
-        retries: int,
         params: dict[str, Any] | None = None
     ) -> dict[str, Any] | None:
         """
         Execute the API call. Requests are retried for connection errors and server-side errors
         using an exponential backoff.
 
         :param method: HTTP method
@@ -192,15 +339,15 @@
 
         self.log.debug(
             "Executing API call: (Method: %s, Endpoint: %s, Parameters: %s, Timeout: %s, Retries: %s)",
             method,
             endpoint,
             params,
             timeout,
-            retries,
+            self.num_retries,
         )
         http = HttpHook(method.upper(), http_conn_id=self.cde_conn_id)
         retry_handler = RetryHandler()
 
         try:
             extra_options: dict[str, Any] = dict(
                 timeout=timeout,
@@ -224,16 +371,19 @@
             # Small hack to override the insecure header property passed from the
             # extra in HTTPHook, which is a boolean but must be a string to be part
             # of the headers
             request_extra_headers = {"insecure": str(self.connection.insecure)}
 
             common_kwargs: dict[str, Any] = dict(
                 _retry_args=dict(
-                    wait=tenacity.wait_exponential(),
-                    stop=tenacity.stop_after_attempt(retries),
+                    wait=CustomWait(self.log),
+                    stop=CustomStop(self.log,
+                                    self.num_retries,
+                                    CdeHook.DEFAULT_NUM_RETRIES_RATE_LIMITED,
+                                    CdeHook.RETRY_TIME_SPAN_FOR_RATE_LIMIT),
                     retry=retry_handler,
                 ),
                 endpoint=endpoint,
                 extra_options=extra_options,
                 headers=request_extra_headers,
             )
 
@@ -350,15 +500,15 @@
         body = dict(
             variables=variables,
             overrides=overrides,
             # Shall be updated to proxy_user when we support this feature
             user=None,
             requestID=request_id,
         )
-        response = self._do_api_call("POST", f"/jobs/{job_name}/run", self.api_timeout, self.num_retries, body)
+        response = self._do_api_call("POST", f"/jobs/{job_name}/run", self.api_timeout, body)
         if response is None:
             msg = f"Unexpected 'None' response for '{job_name}' job."
             self.log.error(msg)
             raise CdeHookException(msg=msg)
         try:
             job_run_id: int = response["id"]
         except KeyError as err:
@@ -368,28 +518,28 @@
 
     def kill_job_run(self, run_id: int) -> None:
         """
         Kill a running job
 
         :param run_id: the run ID of the job run
         """
-        self._do_api_call("POST", f"/job-runs/{run_id}/kill", self.api_timeout, self.num_retries)
+        self._do_api_call("POST", f"/job-runs/{run_id}/kill", self.api_timeout)
 
     def check_job_run_status(self, run_id: int) -> str:
         """
         Check and return the status of a job run
 
         :param run_id: the run ID of the job run
         :return: the job run status
         :rtype: str
         """
         default_status_check_timeout = CdeHook.DEFAULT_API_TIMEOUT // 10
         timeout = self.api_timeout // 10 if self.api_timeout // 10 >= default_status_check_timeout else default_status_check_timeout
 
-        response = self._do_api_call("GET", f"/job-runs/{run_id}", timeout, self.num_retries)
+        response = self._do_api_call("GET", f"/job-runs/{run_id}", timeout)
         if response is None:
             msg = f"Unexpected 'None' response for '{run_id}' job run."
             self.log.error(msg)
             raise CdeHookException(msg=msg)
 
         try:
             response_status: str = response["status"]
@@ -458,17 +608,13 @@
                 elif response.status_code == 409:
                     self.log.warning(
                         f"Job run has been already triggered,"
                         f" waiting for run {response.text.rstrip()} to finish"
                     )
                     return self.EXIT_RETRIES
                 elif response.status_code == 429:
-                    self.log.info(
-                        f"Request could not be processed, "
-                        + "reached rate limit of CDE API: {error_msg}. Retrying"
-                    )
                     return self.CONTINUE_RETRIES
                 elif 500 <= response.status_code < 600:
                     return self.CONTINUE_RETRIES
                 else:
                     raise AirflowException(error_msg)
             return self.EXIT_RETRIES  # pragma: no cover , cannot think about a use case now.
```

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cde_hook.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cde_hook.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cdw.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cdw.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/hooks/cdw_hook.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/hooks/cdw_hook.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/model/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/model/connection.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/model/connection.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cde.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cde.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 from __future__ import annotations
 
 import time
 from typing import Any
 
 from airflow.configuration import conf
-from airflow.exceptions import AirflowException, AirflowConfigException
+from airflow.exceptions import AirflowConfigException, AirflowException
 from airflow.models import BaseOperator
 from cloudera.airflow.providers.hooks.cde import CdeHook, CdeHookException
 
 FORMAT_DATE_TIME = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 class CdeRunJobOperator(BaseOperator):
```

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cde_operator.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cde_operator.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cdw.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cdw.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/operators/cdw_operator.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/operators/cdw_operator.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/cdw.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/cdw.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/airflow/providers/sensors/cdw_sensor.py` & `cloudera-airflow-provider-2.1.2/cloudera/airflow/providers/sensors/cdw_sensor.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/__init__.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/cde_hook.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/cde_hook.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/hooks/cdw_hook.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/hooks/cdw_hook.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/model/connection.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/model/connection.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/cde_operator.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/cde_operator.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/operators/cdw_operator.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/operators/cdw_operator.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera/cdp/airflow/sensors/cdw_sensor.py` & `cloudera-airflow-provider-2.1.2/cloudera/cdp/airflow/sensors/cdw_sensor.py`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/cloudera_airflow_provider.egg-info/SOURCES.txt` & `cloudera-airflow-provider-2.1.2/cloudera_airflow_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudera-airflow-provider-2.1.1/setup.cfg` & `cloudera-airflow-provider-2.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cloudera-airflow-provider
-version = 2.1.1
+version = 2.1.2
 author = Cloudera
 description = Cloudera CDP Airflow Plugins
 
 [options]
 packages = find_namespace:
 python_requires = >=3.7
 install_requires =
```

