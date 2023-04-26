# Comparing `tmp/crc-event-schemas-0.1.1.tar.gz` & `tmp/crc-event-schemas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-event-schemas-0.1.1.tar", last modified: Thu Apr 20 17:53:39 2023, max compression
+gzip compressed data, was "crc-event-schemas-0.1.2.tar", last modified: Tue Apr 25 16:02:13 2023, max compression
```

## Comparing `crc-event-schemas-0.1.1.tar` & `crc-event-schemas-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)    11358 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/LICENSE.txt
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      354 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/PKG-INFO
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      105 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/README.md
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      354 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/PKG-INFO
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      888 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        1 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)       14 2023-04-20 17:53:39.000000 crc-event-schemas-0.1.1/crc_event_schemas.egg-info/top_level.txt
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/advisor/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/__init__.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     6908 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/advisor_recommendations.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/policies/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.685796 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/__init__.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     5652 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/policy_triggered.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/apps/repositories/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/__init__.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     7133 2023-04-20 17:08:50.000000 crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/repository_events.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/core/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/core/__init__.py
-drwxr-xr-x   0 josejulio  (1000) josejulio  (1000)        0 2023-04-20 17:53:39.686796 crc-event-schemas-0.1.1/event_schemas/core/v1/
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)        0 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/__init__.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      125 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/common.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     2687 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/error.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     3829 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/notification.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)     4669 2023-04-20 12:44:44.000000 crc-event-schemas-0.1.1/event_schemas/core/v1/rhel_system.py
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)       87 2023-04-19 19:06:18.000000 crc-event-schemas-0.1.1/pyproject.toml
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)       38 2023-04-20 17:53:39.687796 crc-event-schemas-0.1.1/setup.cfg
--rw-r--r--   0 josejulio  (1000) josejulio  (1000)      364 2023-04-20 17:53:16.000000 crc-event-schemas-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.825531 crc-event-schemas-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 16:02:13.825531 crc-event-schemas-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/crc_event_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 16:02:13.000000 crc-event-schemas-0.1.2/crc_event_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-04-25 16:02:13.000000 crc-event-schemas-0.1.2/crc_event_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 16:02:13.000000 crc-event-schemas-0.1.2/crc_event_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 16:02:13.000000 crc-event-schemas-0.1.2/crc_event_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/advisor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/advisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/advisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/advisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/advisor/v1/advisor_recommendations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/policies/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/policies/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/policies/v1/policy_triggered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/repositories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/apps/repositories/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/repositories/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/apps/repositories/v1/repository_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.821531 crc-event-schemas-0.1.2/event_schemas/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:13.825531 crc-event-schemas-0.1.2/event_schemas/core/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/v1/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/v1/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3830 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/v1/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/event_schemas/core/v1/rhel_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 16:02:13.825531 crc-event-schemas-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-25 16:02:01.000000 crc-event-schemas-0.1.2/setup.py
```

### Comparing `crc-event-schemas-0.1.1/LICENSE.txt` & `crc-event-schemas-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/crc_event_schemas.egg-info/SOURCES.txt` & `crc-event-schemas-0.1.2/crc_event_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/event_schemas/apps/advisor/v1/advisor_recommendations.py` & `crc-event-schemas-0.1.2/event_schemas/apps/advisor/v1/advisor_recommendations.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/event_schemas/apps/policies/v1/policy_triggered.py` & `crc-event-schemas-0.1.2/event_schemas/apps/policies/v1/policy_triggered.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/event_schemas/apps/repositories/v1/repository_events.py` & `crc-event-schemas-0.1.2/event_schemas/apps/repositories/v1/repository_events.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/event_schemas/core/v1/error.py` & `crc-event-schemas-0.1.2/event_schemas/core/v1/error.py`

 * *Files identical despite different names*

### Comparing `crc-event-schemas-0.1.1/event_schemas/core/v1/notification.py` & `crc-event-schemas-0.1.2/event_schemas/core/v1/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 def to_class(c: Type[T], x: Any) -> dict:
     assert isinstance(x, c)
     return cast(Any, x).to_dict()
 
 
 class Recipients:
-    """Notification recipients. Should be in a top-level field named "notification_recipients""""
+    """Notification recipients. Should be in a top-level field named "notification_recipients\""""
     """Setting to true ignores all the user preferences on this Recipient setting (It doesn’t
     affect other configuration that an Administrator sets on their Notification settings).
     Setting to false honors the user preferences.
     """
     ignore_user_preferences: Optional[bool]
     """Setting to true sends an email to the administrators of the account. Setting to false
     sends an email to all users of the account.
```

### Comparing `crc-event-schemas-0.1.1/event_schemas/core/v1/rhel_system.py` & `crc-event-schemas-0.1.2/event_schemas/core/v1/rhel_system.py`

 * *Files identical despite different names*

