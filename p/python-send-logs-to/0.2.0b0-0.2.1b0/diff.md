# Comparing `tmp/python-send-logs-to-0.2.0b0.tar.gz` & `tmp/python-send-logs-to-0.2.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-send-logs-to-0.2.0b0.tar", last modified: Tue Apr 18 10:51:00 2023, max compression
+gzip compressed data, was "python-send-logs-to-0.2.1b0.tar", last modified: Wed Apr 26 13:47:00 2023, max compression
```

## Comparing `python-send-logs-to-0.2.0b0.tar` & `python-send-logs-to-0.2.1b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.2.0b0/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1417 2023-01-09 11:59:08.000000 python-send-logs-to-0.2.0b0/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/log_to/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       27 2023-04-18 10:46:22.000000 python-send-logs-to-0.2.0b0/log_to/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5706 2023-04-18 10:47:06.000000 python-send-logs-to-0.2.0b0/log_to/redis.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      275 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        7 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.2.0b0/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.2.1b0/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3331 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2557 2023-04-26 13:31:01.000000 python-send-logs-to-0.2.1b0/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/log_to/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       27 2023-04-26 13:32:14.000000 python-send-logs-to-0.2.1b0/log_to/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5706 2023-04-18 10:47:06.000000 python-send-logs-to-0.2.1b0/log_to/redis.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     3331 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      275 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        7 2023-04-26 13:47:00.000000 python-send-logs-to-0.2.1b0/python_send_logs_to.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-26 13:47:00.221894 python-send-logs-to-0.2.1b0/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.2.1b0/setup.py
```

### Comparing `python-send-logs-to-0.2.0b0/LICENSE` & `python-send-logs-to-0.2.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.2.0b0/README.md` & `python-send-logs-to-0.2.1b0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 python-send-logs-to
 ===================
 A Python logging handler that sends logs to Redis; later to be a collection
-of logging handlers. 
+of logging handlers.
 
 
 
 
 Quickstart
 ----------
 
@@ -43,14 +43,70 @@
        )
        handler.setFormatter(formatter)
        logger.addHandler(handler)
        return logger
    ```
 
 
+Django logging example
+----------------------
+
+```python
+# In your project's settings.py file
+# Logging
+# https://docs.djangoproject.com/en/4.2/topics/logging/
+
+default_handlers = []
+if DEBUG:
+    default_handlers += ['console', 'redis']
+    log_level = 'DEBUG'
+
+else:
+    default_handlers += ['redis']
+    log_level = 'WARNING'
+
+default_logger_config = {
+    'handlers': default_handlers,
+    'level': log_level,
+}
+
+LOGGING = {
+    'version': 1,
+    'disable_existing_loggers': False,
+    'handlers': {
+        'console': {
+            'class': 'logging.StreamHandler',
+        },
+        'redis': {
+            'class': 'log_to.redis.RedisLogHandler',
+            'key': 'logging:myapp',
+            'host': REDIS_HOST,
+            'port': REDIS_PORT,
+            'password': REDIS_PASSWORD,
+        },
+    },
+    'loggers': {
+        'myapp': default_logger_config,
+        'specific_logger': default_logger_config,
+    },
+}
+```
+
+And then in some module where you want to use the logging:
+
+```python
+import logging
+
+logger = logging.getLogger('myapp')
+# OR
+# logger = logging.getLogger('specific_logger')
+
+logger.info('Testing 123')
+```
+
 
 Compatiblity
 ------------
 - Compatible with Python 3.8 and above.
 
 
 Versioning
```

### Comparing `python-send-logs-to-0.2.0b0/log_to/redis.py` & `python-send-logs-to-0.2.1b0/log_to/redis.py`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.2.0b0/setup.py` & `python-send-logs-to-0.2.1b0/setup.py`

 * *Files identical despite different names*

