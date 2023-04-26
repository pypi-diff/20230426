# Comparing `tmp/rabbitmq_pika_flask-1.2.8.tar.gz` & `tmp/rabbitmq_pika_flask-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitmq_pika_flask-1.2.8.tar", last modified: Mon Dec  6 18:37:10 2021, max compression
+gzip compressed data, was "rabbitmq_pika_flask-1.2.9.tar", last modified: Thu Dec  9 18:19:28 2021, max compression
```

## Comparing `rabbitmq_pika_flask-1.2.8.tar` & `rabbitmq_pika_flask-1.2.9.tar`

### file list

```diff
@@ -1,7 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 18:37:10.039262 rabbitmq_pika_flask-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      856 2021-12-06 18:37:10.039262 rabbitmq_pika_flask-1.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-06 18:37:10.039262 rabbitmq_pika_flask-1.2.8/rabbitmq_pika_flask/
--rw-r--r--   0 runner    (1001) docker     (121)    12724 2021-12-06 18:36:56.727098 rabbitmq_pika_flask-1.2.8/rabbitmq_pika_flask/RabbitMQ.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-06 18:36:56.727098 rabbitmq_pika_flask-1.2.8/rabbitmq_pika_flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-06 18:36:56.727098 rabbitmq_pika_flask-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-12-06 18:36:56.727098 rabbitmq_pika_flask-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 18:19:28.775629 rabbitmq_pika_flask-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      856 2021-12-09 18:19:28.775629 rabbitmq_pika_flask-1.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-09 18:19:28.775629 rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/ExchangeType.py
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/QueueParams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12574 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/RabbitMQ.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1842 2021-12-09 18:19:19.163315 rabbitmq_pika_flask-1.2.9/setup.py
```

### Comparing `rabbitmq_pika_flask-1.2.8/PKG-INFO` & `rabbitmq_pika_flask-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rabbitmq_pika_flask
-Version: 1.2.8
+Version: 1.2.9
 Summary: Adapter for RabbitMQs pika and flask
 Home-page: https://github.com/aylton-almeida/rabbitmq-pika-flask
 Author: Aylton Almeida
 Author-email: almeida@aylton.dev
 License: MIT
 Download-URL: https://github.com/aylton-almeida/rabbitmq-pika-flask/archive/0.1.tar.gz
 Description: UNKNOWN
```

### Comparing `rabbitmq_pika_flask-1.2.8/rabbitmq_pika_flask/RabbitMQ.py` & `rabbitmq_pika_flask-1.2.9/rabbitmq_pika_flask/RabbitMQ.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,25 @@
 import json
 import os
-from enum import Enum
 from functools import wraps
 from hashlib import sha256
 from threading import Thread
 from typing import Callable
 from uuid import uuid4
 
 from flask.app import Flask
 from flask.config import Config
 from pika import BlockingConnection, URLParameters, spec
 from pika.adapters.blocking_connection import BlockingChannel
 from pika.exceptions import AMQPConnectionError
 from retry import retry
 from retry.api import retry_call
 
-
-class QueueParams:
-    """ Default parameters for queues
-    """
-
-    durable: bool
-    auto_delete: bool
-    exclusive: bool
-
-    def __init__(self, durable=True, auto_delete=False,  exclusive=False) -> None:
-        self.durable = durable
-        self.auto_delete = auto_delete
-        self.exclusive = exclusive
-
-
-class ExchangeType(Enum):
-    """The type of exchange to be used
-    """
-
-    DEFAULT = 'topic'
-    DIRECT = 'direct'
-    FANOUT = 'fanout'
-    TOPIC = 'topic'
-    HEADER = 'header'
+from rabbitmq_pika_flask.ExchangeType import ExchangeType
+from rabbitmq_pika_flask.QueueParams import QueueParams
 
 
 class RabbitMQ():
     """ Main class containing queue and message sending methods
     """
 
     app: Flask
@@ -68,34 +45,41 @@
         development: bool = False
     ) -> None:
         self.app = None
         self.consumers = set()
         self.queue_params = queue_params
 
         if app is not None:
-            self.init_app(app, queue_prefix, body_parser,
-                          msg_parser, development)
+            self.init_app(
+                app,
+                queue_prefix,
+                body_parser,
+                msg_parser,
+                development
+            )
 
     # Inits class from flask app
     def init_app(
         self,
         app: Flask,
         queue_prefix: str,
-        body_parser: Callable = None,
-        msg_parser: Callable = None,
+        body_parser: Callable = lambda body: body,
+        msg_parser: Callable = lambda msg: msg,
         development: bool = False
     ):
         """This callback can be used to initialize an application for the use with this RabbitMQ setup.
 
         Args:
             app (Flask): Flask app
+            queue_prefix (str): Prefix for queue names
             body_parser (Callable, optional): A parser function to
                 parse received messages. Defaults to None.
             msg_parser (Callable, optional): A parser function to
                 parse messages to be sent. Defaults to None.
+            development (bool, optional): If the app is in development mode. Defaults to False.
         """
 
         self.app = app
         self.queue_prefix = queue_prefix
         self.config = app.config
 
         self._check_env()
@@ -103,14 +87,15 @@
         self.body_parser = body_parser
         self.msg_parser = msg_parser
         self.development = development
         self.exchange_name = self.config['MQ_EXCHANGE']
         params = URLParameters(self.config['MQ_URL'])
         self.get_connection = lambda: BlockingConnection(params)
 
+        # Avoiding running twice when flask in debug mode
         if os.getenv('FLASK_ENV') == 'production' or os.getenv('WERKZEUG_RUN_MAIN') == 'true':
             self._validate_connection()
 
         if development:
             self.queue_prefix = 'dev.' + str(uuid4()) + queue_prefix
             self.queue_params = QueueParams(False, True, True)
 
@@ -266,29 +251,28 @@
         def callback(_: BlockingChannel, method: spec.Basic.Deliver, props: spec.BasicProperties, body: bytes):
             with self.app.app_context():
                 decoded_body = body.decode()
 
                 try:
                     func(
                         routing_key=method.routing_key,
-                        body=self.body_parser(
-                            decoded_body) if self.body_parser is not None else decoded_body,
+                        body=self.body_parser(decoded_body),
                         message_id=props.message_id
                     )
 
                     if not auto_ack:
                         # ack message after fn was ran
                         channel.basic_ack(method.delivery_tag)
                 except Exception as err:
+                    self.app.logger.error(f'ERROR IN {queue_name}: {err}')
+
                     if not auto_ack:
                         channel.basic_reject(
                             method.delivery_tag, requeue=(not method.redelivered))
 
-                    raise err from err
-
         channel.basic_consume(
             queue=queue_name, on_message_callback=callback, auto_ack=auto_ack)
 
         try:
             channel.start_consuming()
         except Exception as err:
             self.app.logger.error(err)
```

### Comparing `rabbitmq_pika_flask-1.2.8/setup.py` & `rabbitmq_pika_flask-1.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 
 setup(
     # How you named your package folder (MyLib)
     name='rabbitmq_pika_flask',
     packages=['rabbitmq_pika_flask'],   # Chose the same as "name"
     # Start with a small number and increase it with every change you make
-    version='1.2.8',
+    version='1.2.9',
     # Chose a license from here: https://help.github.com/articles/licensing-a-repository
     license='MIT',
     # Give a short description about your library
     description='Adapter for RabbitMQs pika and flask',
     author='Aylton Almeida',                   # Type in your name
     author_email='almeida@aylton.dev',      # Type in your E-Mail
     # Provide either the link to your github or to your website
```

