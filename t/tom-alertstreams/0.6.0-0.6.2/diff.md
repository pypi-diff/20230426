# Comparing `tmp/tom_alertstreams-0.6.0.tar.gz` & `tmp/tom_alertstreams-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_alertstreams-0.6.0.tar", max compression
+gzip compressed data, was "tom_alertstreams-0.6.2.tar", max compression
```

## Comparing `tom_alertstreams-0.6.0.tar` & `tom_alertstreams-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     8544 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/README.md
--rw-r--r--   0        0        0     1555 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/__init__.py
--rw-r--r--   0        0        0       63 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/admin.py
--rw-r--r--   0        0        0        0 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/__init__.py
--rw-r--r--   0        0        0     4430 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/alertstream.py
--rw-r--r--   0        0        0     2674 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/gcn.py
--rw-r--r--   0        0        0     8439 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/hopskotch.py
--rw-r--r--   0        0        0      163 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/apps.py
--rw-r--r--   0        0        0        0 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/management/commands/__init__.py
--rw-r--r--   0        0        0     1577 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/management/commands/hoptestpub.py
--rw-r--r--   0        0        0     1508 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/management/commands/readstreams.py
--rw-r--r--   0        0        0        0 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/migrations/__init__.py
--rw-r--r--   0        0        0       57 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/models.py
--rw-r--r--   0        0        0       60 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/tests.py
--rw-r--r--   0        0        0       63 2023-01-24 23:53:43.902204 tom_alertstreams-0.6.0/tom_alertstreams/views.py
--rw-r--r--   0        0        0     9696 1970-01-01 00:00:00.000000 tom_alertstreams-0.6.0/setup.py
--rw-r--r--   0        0        0    10258 1970-01-01 00:00:00.000000 tom_alertstreams-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     8684 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/README.md
+-rw-r--r--   0        0        0     1556 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/__init__.py
+-rw-r--r--   0        0        0       63 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/admin.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/__init__.py
+-rw-r--r--   0        0        0     4430 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/alertstream.py
+-rw-r--r--   0        0        0     2674 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/gcn.py
+-rw-r--r--   0        0        0     8569 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/hopskotch.py
+-rw-r--r--   0        0        0      163 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/apps.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/management/commands/__init__.py
+-rw-r--r--   0        0        0     1577 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/management/commands/hoptestpub.py
+-rw-r--r--   0        0        0     1508 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/management/commands/readstreams.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/models.py
+-rw-r--r--   0        0        0       60 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/tests.py
+-rw-r--r--   0        0        0       63 2023-04-26 21:54:46.465575 tom_alertstreams-0.6.2/tom_alertstreams/views.py
+-rw-r--r--   0        0        0    10398 1970-01-01 00:00:00.000000 tom_alertstreams-0.6.2/PKG-INFO
```

### Comparing `tom_alertstreams-0.6.0/README.md` & `tom_alertstreams-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,16 @@
 ```python
 ALERT_STREAMS = [
     {
         'ACTIVE': True,
         'NAME': 'tom_alertstreams.alertstreams.hopskotch.HopskotchAlertStream',
         'OPTIONS': {
             'URL': 'kafka://kafka.scimma.org/',
-            'GROUP_ID': 'uniqueidforyourapp12345',
+            # The hop-client requires that the GROUP_ID prefix match the SCIMMA_AUTH_USERNAME
+            'GROUP_ID': os.getenv('SCIMMA_AUTH_USERNAME', "") + '-' + 'uniqueidforyourapp12345',
             'USERNAME': os.getenv('SCIMMA_AUTH_USERNAME', None),
             'PASSWORD': os.getenv('SCIMMA_AUTH_PASSWORD', None),
             'TOPIC_HANDLERS': {
                 'sys.heartbeat': 'tom_alertstreams.alertstreams.hopskotch.heartbeat_handler',
                 'tomtoolkit.test': 'tom_alertstreams.alertstreams.hopskotch.alert_logger',
                 'hermes.test': 'tom_alertstreams.alertstreams.hopskotch.alert_logger',
                 'hermes.*': 'regex match public topics here, requires * handler to be defined'
```

### Comparing `tom_alertstreams-0.6.0/pyproject.toml` & `tom_alertstreams-0.6.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tom-alertstreams"
-version = "0.6.0"
+version = "0.6.2"
 description = "Reusable TOMToolkit app for listening to kafka streams."
 authors = ["TOM Toolkit Project <tomtoolkit@lco.global>", "Lindy Lindstrom <llindstrom@lco.global>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/TOMToolkit/tom-alertstreams"
 keywords = ["tomtoolkit", "astronomy", "astrophysics", "cosmology", "science"]
 classifiers = [
@@ -41,8 +41,8 @@
 [tool.poetry.dev-dependencies]
 coverage = "^6.3.2"
 factory_boy = "^3.1.0"
 pytest = "^3.0.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/alertstream.py` & `tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/alertstream.py`

 * *Files identical despite different names*

### Comparing `tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/gcn.py` & `tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/gcn.py`

 * *Files identical despite different names*

### Comparing `tom_alertstreams-0.6.0/tom_alertstreams/alertstreams/hopskotch.py` & `tom_alertstreams-0.6.2/tom_alertstreams/alertstreams/hopskotch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from datetime import datetime, timezone
 import logging
 import re
 import uuid
+import traceback
 
 from django.utils import timezone as tz
 from django.core.exceptions import ImproperlyConfigured
 
 from hop import Stream
 from hop.auth import Auth
 from hop.models import JSONBlob
 from hop.io import Metadata, StartPosition, list_topics
 
 from tom_alertstreams.alertstreams.alertstream import AlertStream
 
 logger = logging.getLogger(__name__)
-#logger.setLevel(logging.DEBUG)
 
 
 class HopskotchAlertStream(AlertStream):
     """
     """
     required_keys = ['URL', 'GROUP_ID', 'USERNAME', 'PASSWORD', 'TOPIC_HANDLERS']
     allowed_keys = ['URL', 'GROUP_ID', 'USERNAME', 'PASSWORD', 'TOPIC_HANDLERS']
@@ -110,15 +110,15 @@
                         if metadata.topic in self.alert_handler:
                             # TODO: should probably use *args, **kwargs to pass unknow number of arguments
                             self.alert_handler[metadata.topic](alert, metadata)
                         elif '*' in self.alert_handler:
                             # First check all wildcard topics to see if they will match this topic
                             matched_handler = False
                             for topic in self.alert_handler.keys():
-                                if '*' in topic and re.match(topic, metadata.topic):
+                                if topic != '*' and '*' in topic and re.match(topic, metadata.topic):
                                     self.alert_handler[topic](alert, metadata)
                                     matched_handler = True
                                     break
                             # If nothing matched, fall back to default public topic handler
                             if not matched_handler:
                                 self.alert_handler['*'](alert, metadata)
                         else:
@@ -130,14 +130,15 @@
                             if set(public_topics) != set(self.public_topics):
                                 logger.info(f"New public topics found, restarting hop stream")
                                 self.public_topics = public_topics
                                 self.stream_url = self.get_stream_url()
                                 break
             except Exception as ex:
                 logger.error(f'HopskotchAlertStream.listen: {ex}')
+                logger.error(traceback.format_exc())  # Show the traceback so we have a chance of figuring out what is breaking
 
 def heartbeat_handler(heartbeat: JSONBlob, metadata: Metadata):
     """Example alert handler for HopskotchAlertStream sys.heartbeat topic.
 
     Note that HopskotchAlertStream.listen() method knows that Hopskotch alerts come with
     both alert and metadata. So, the alert_handler methods have a signiture (taking both
     as arguments) specific to this stream.
```

### Comparing `tom_alertstreams-0.6.0/tom_alertstreams/management/commands/hoptestpub.py` & `tom_alertstreams-0.6.2/tom_alertstreams/management/commands/hoptestpub.py`

 * *Files identical despite different names*

### Comparing `tom_alertstreams-0.6.0/tom_alertstreams/management/commands/readstreams.py` & `tom_alertstreams-0.6.2/tom_alertstreams/management/commands/readstreams.py`

 * *Files identical despite different names*

### Comparing `tom_alertstreams-0.6.0/setup.py` & `tom_alertstreams-0.6.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,192 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tom-alertstreams
+Version: 0.6.2
+Summary: Reusable TOMToolkit app for listening to kafka streams.
+Home-page: https://github.com/TOMToolkit/tom-alertstreams
+License: GPL-3.0-only
+Keywords: tomtoolkit,astronomy,astrophysics,cosmology,science
+Author: TOM Toolkit Project
+Author-email: tomtoolkit@lco.global
+Requires-Python: >=3.8,<3.12
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.1
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Dist: gcn-kafka (>=0.2,<0.3)
+Requires-Dist: hop-client (>=0.8,<0.9)
+Requires-Dist: psycopg2-binary (>=2.9,<3.0)
+Requires-Dist: tomtoolkit (>=2.10,<3.0)
+Project-URL: Repository, https://github.com/TOMToolkit/tom-alertstreams
+Description-Content-Type: text/markdown
+
+# tom-alertstreams
+
+`tom-alertstreams` is a reusable TOM Toolkit app for listening to kafka streams.
+
+`tom-alertstreams` provides a management command, `readstreams`. There are no `urlpatterns`,
+no Views, and no templates. The `readstreams` management command reads the `settings.py` `ALERT_STREAMS`
+configuration and starts listening to each configured Kafka stream. It is not expected
+to return, and is intended to run along side your TOM's server component. The `ALERT_STREAMS`
+configuration (see below) tells `readstreams` what streams to access, how to access them,
+what topics to listen to, and what to do with messages that arrive on a given topic.
+
+## Installation
+
+1. Install the package into your TOM environment:
+    ```bash
+    pip install tom-alertstreams
+   ```
+
+2. In your project `settings.py`, add `tom_alertstreams` to your `INSTALLED_APPS` setting:
+
+    ```python
+    INSTALLED_APPS = [
+        ...
+        'tom_alertstreams',
+    ]
+    ```
+
+At this point you can verify the installation by running `./manage.py` to list the available
+management commands and see
+
+   ```bash
+   [tom_alertstreams]
+       readstreams
+   ```
+in the output.
+
+## Configuration
+
+Each Kafka stream that your TOM listens to (via `readstreams`) will have a configuration dictionary
+in your `settings.py` `ALERT_STREAMS`. `ALERT_STREAMS` is a list of configuration dictionaries, one
+dictionary for each Kafka stream. Here's an example `ALERT_STREAMS` configuration for two Kafka streams:
+[SCiMMA Hopskotch](https://scimma.org/hopskotch.html) and
+[GCN Classic over Kafka](https://gcn.nasa.gov/quickstart).
+
+```python
+ALERT_STREAMS = [
+    {
+        'ACTIVE': True,
+        'NAME': 'tom_alertstreams.alertstreams.hopskotch.HopskotchAlertStream',
+        'OPTIONS': {
+            'URL': 'kafka://kafka.scimma.org/',
+            # The hop-client requires that the GROUP_ID prefix match the SCIMMA_AUTH_USERNAME
+            'GROUP_ID': os.getenv('SCIMMA_AUTH_USERNAME', "") + '-' + 'uniqueidforyourapp12345',
+            'USERNAME': os.getenv('SCIMMA_AUTH_USERNAME', None),
+            'PASSWORD': os.getenv('SCIMMA_AUTH_PASSWORD', None),
+            'TOPIC_HANDLERS': {
+                'sys.heartbeat': 'tom_alertstreams.alertstreams.hopskotch.heartbeat_handler',
+                'tomtoolkit.test': 'tom_alertstreams.alertstreams.hopskotch.alert_logger',
+                'hermes.test': 'tom_alertstreams.alertstreams.hopskotch.alert_logger',
+                'hermes.*': 'regex match public topics here, requires * handler to be defined'
+                '*': 'default_handler_here'
+            },
+        },
+    },
+    {
+        'ACTIVE': True,
+        'NAME': 'tom_alertstreams.alertstreams.gcn.GCNClassicAlertStream',
+        # The keys of the OPTIONS dictionary become (lower-case) properties of the AlertStream instance.
+        'OPTIONS': {
+            # see https://github.com/nasa-gcn/gcn-kafka-python#to-use for configuration details.
+            'GCN_CLASSIC_CLIENT_ID': os.getenv('GCN_CLASSIC_CLIENT_ID', None),
+            'GCN_CLASSIC_CLIENT_SECRET': os.getenv('GCN_CLASSIC_CLIENT_SECRET', None),
+            'DOMAIN': 'gcn.nasa.gov',  # optional, defaults to 'gcn.nasa.gov'
+            'CONFIG': {  # optional
+                # 'group.id': 'tom_alertstreams-my-custom-group-id',
+                # 'auto.offset.reset': 'earliest',
+                # 'enable.auto.commit': False
+            },
+            'TOPIC_HANDLERS': {
+                'gcn.classic.text.LVC_INITIAL': 'tom_alertstreams.alertstreams.alertstream.alert_logger',
+                'gcn.classic.text.LVC_PRELIMINARY': 'tom_alertstreams.alertstreams.alertstream.alert_logger',
+                'gcn.classic.text.LVC_RETRACTION': 'tom_alertstreams.alertstreams.alertstream.alert_logger',
+            },
+        },
+    }
+]
+```
+
+The configuration dictionary for each `AlertStream` subclass will contain these key-value pairs:
+* `ACTIVE`: Boolean which tells `readstreams` to access this stream. Should be `True`, unless you want to
+keep a configuration dictionary, but ignore the stream.
+* `NAME`: The name of the `AlertStream` subclass that implements the interface to this Kafka stream. `tom_alertstreams`
+will provide `AlertStream` subclasses for major astromical Kafka streams. See below for instructions on Subclassing
+the `AlertStream` base class.
+* `OPTIONS`: A dictionary of key-value pairs specific to the`AlertStream` subclass given by `NAME`. The doc string for
+the `AlertStream` subclass should document what is expected. Typically, a URL, authentication information, and a
+dictionary, `TOPIC_HANDLERS`, will be required. See "Subclassing `AlertStream`" below. The `AlertStream` subclass will
+convert the key-value pairs of the `OPTIONS` dictionary into properties (and values) of the `AlertStream` subclass
+instance.
+  * The hopskotch alert stream supports a wildcard of `*` for an alert handler topic name. If specified, ALL public topics will be subscribed and use that handler function. A directly specified topic handler will always be used before the `*` handler for any topic that is covered twice. 
+
+### Getting Kafka Stream Credentials
+As part of your `OPTIONS` for each Kafka stream, you need to configure access credentials. Visit these links
+to get credentials for [Hopskotch](https://hop.scimma.org/) and [GCN Classic over Kafka](https://gcn.nasa.gov/quickstart).
+Set the environment variables with the username and passwords obtained. Do not check them in to your code repository.
+
+
+## Alert Handling
+
+Assuming that an `AlertStream` subclass exists for the Kafka stream of interest,
+the keys of the `TOPIC_HANDLERS` dictionary are the topics that will be subscribed to. The values
+of the `TOPIC_HANDLERS` dictionary specify alert handling methods that will be imported and called
+for each alert recieved on that topic. An example is provided,
+`tom_alerts.alertstreams.alertstream.alert_logger`, which simply logs the alert.
+
+To customize this behaviour according to the needs of your TOM, define an alert handling function for each
+topic that you wish to subscribe to. Your `TOPIC_HANDLERS` dictionary will have a an entry for each topic
+whose key is the topic name and whose value is a string indicating the dot-path to the alert handling function.
+When the `AlertStream` subclass is instanciated, the `OPTIONS` dictionary is read and an `alert_handler`
+dictionary is created. It is keyed by topic name and it's values are the imported callable functions specified by the
+dot-path strings. `readstreams` will call the alert handler for each alert that comes in on the topic. The signiture
+of the alert handling function is specific to the `AlertStream` subclasss.
+
+## Subclassing `AlertStream`
+
+Ideally, As a TOM developer, there is already an `AlertStream`-subclass for the alert stream that you
+want your TOM to listen to. If so, you need only to configure your TOM to use it in  `settings.py`
+`ALERT_STREAMS`. If you must implement your own `AlertStream` subclass, please get in touch. In the meantime, here's a brief outline:
+
+1. Create subclass of `AlertStream`.
+
+2. Create `required_keys` and `allowed_keys` class variables in your `AlertStream`-subclass.
+
+   These are lists of strings refering to the keys of the `OPTIONS` dictionary. The purpose of these is to
+   help TOM developers using your `AlertStream`-subclass with the key-value pairs in their `ALERT_STREAMS`
+  `OPTIONS` configuration dictionary.
+
+3. Implement the `listen()` method.
+
+   This method will be called by the `readstreams` management command and is not expected to return. It
+   should instanciate your consumer, subscribe to the topics configured in `ALERT_STREAMS`, and start
+   consuming. The detail of this will depend on the kafka-client used. See `alertstreams.gcn.listen()`
+   and `alertstreams.hopskotch.listen()` for examples to follow.
+   
+   The loop which consumes messages in your `listen()` method should extract the topic from each message
+   and call `self.alert_handler[topic]()` with the message or message-derived arguments specific to your
+   kafka client. Users of your `AlertStream`-subclass will write these topic-specific alert handling methods
+   and configure them in the `TOPIC_HANLDERS` dictionary of their `ALERT_STREAMS` configuration.
+   The `AlertStream` base class will set up the `alert_handler` dictionary according to your users'
+   configuration. It helps your users to provide an example `alert_hander()` function in your module as
+   an example. (Again, see `alertstreams.gcn.listen()` and `alertstreams.hopskotch.listen()`, their
+   configurations in `settings.py`, and the `alertstreams.gcn.alert_logger()` and
+   `alertstreams.hopskotch.alert_logger() methods, for example).
 
-packages = \
-['tom_alertstreams',
- 'tom_alertstreams.alertstreams',
- 'tom_alertstreams.management.commands',
- 'tom_alertstreams.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['gcn-kafka>=0.2,<0.3',
- 'hop-client>=0.8,<0.9',
- 'psycopg2-binary>=2.9,<3.0',
- 'tomtoolkit>=2.10,<3.0']
-
-setup_kwargs = {
-    'name': 'tom-alertstreams',
-    'version': '0.6.0',
-    'description': 'Reusable TOMToolkit app for listening to kafka streams.',
-    'long_description': '# tom-alertstreams\n\n`tom-alertstreams` is a reusable TOM Toolkit app for listening to kafka streams.\n\n`tom-alertstreams` provides a management command, `readstreams`. There are no `urlpatterns`,\nno Views, and no templates. The `readstreams` management command reads the `settings.py` `ALERT_STREAMS`\nconfiguration and starts listening to each configured Kafka stream. It is not expected\nto return, and is intended to run along side your TOM\'s server component. The `ALERT_STREAMS`\nconfiguration (see below) tells `readstreams` what streams to access, how to access them,\nwhat topics to listen to, and what to do with messages that arrive on a given topic.\n\n## Installation\n\n1. Install the package into your TOM environment:\n    ```bash\n    pip install tom-alertstreams\n   ```\n\n2. In your project `settings.py`, add `tom_alertstreams` to your `INSTALLED_APPS` setting:\n\n    ```python\n    INSTALLED_APPS = [\n        ...\n        \'tom_alertstreams\',\n    ]\n    ```\n\nAt this point you can verify the installation by running `./manage.py` to list the available\nmanagement commands and see\n\n   ```bash\n   [tom_alertstreams]\n       readstreams\n   ```\nin the output.\n\n## Configuration\n\nEach Kafka stream that your TOM listens to (via `readstreams`) will have a configuration dictionary\nin your `settings.py` `ALERT_STREAMS`. `ALERT_STREAMS` is a list of configuration dictionaries, one\ndictionary for each Kafka stream. Here\'s an example `ALERT_STREAMS` configuration for two Kafka streams:\n[SCiMMA Hopskotch](https://scimma.org/hopskotch.html) and\n[GCN Classic over Kafka](https://gcn.nasa.gov/quickstart).\n\n```python\nALERT_STREAMS = [\n    {\n        \'ACTIVE\': True,\n        \'NAME\': \'tom_alertstreams.alertstreams.hopskotch.HopskotchAlertStream\',\n        \'OPTIONS\': {\n            \'URL\': \'kafka://kafka.scimma.org/\',\n            \'GROUP_ID\': \'uniqueidforyourapp12345\',\n            \'USERNAME\': os.getenv(\'SCIMMA_AUTH_USERNAME\', None),\n            \'PASSWORD\': os.getenv(\'SCIMMA_AUTH_PASSWORD\', None),\n            \'TOPIC_HANDLERS\': {\n                \'sys.heartbeat\': \'tom_alertstreams.alertstreams.hopskotch.heartbeat_handler\',\n                \'tomtoolkit.test\': \'tom_alertstreams.alertstreams.hopskotch.alert_logger\',\n                \'hermes.test\': \'tom_alertstreams.alertstreams.hopskotch.alert_logger\',\n                \'hermes.*\': \'regex match public topics here, requires * handler to be defined\'\n                \'*\': \'default_handler_here\'\n            },\n        },\n    },\n    {\n        \'ACTIVE\': True,\n        \'NAME\': \'tom_alertstreams.alertstreams.gcn.GCNClassicAlertStream\',\n        # The keys of the OPTIONS dictionary become (lower-case) properties of the AlertStream instance.\n        \'OPTIONS\': {\n            # see https://github.com/nasa-gcn/gcn-kafka-python#to-use for configuration details.\n            \'GCN_CLASSIC_CLIENT_ID\': os.getenv(\'GCN_CLASSIC_CLIENT_ID\', None),\n            \'GCN_CLASSIC_CLIENT_SECRET\': os.getenv(\'GCN_CLASSIC_CLIENT_SECRET\', None),\n            \'DOMAIN\': \'gcn.nasa.gov\',  # optional, defaults to \'gcn.nasa.gov\'\n            \'CONFIG\': {  # optional\n                # \'group.id\': \'tom_alertstreams-my-custom-group-id\',\n                # \'auto.offset.reset\': \'earliest\',\n                # \'enable.auto.commit\': False\n            },\n            \'TOPIC_HANDLERS\': {\n                \'gcn.classic.text.LVC_INITIAL\': \'tom_alertstreams.alertstreams.alertstream.alert_logger\',\n                \'gcn.classic.text.LVC_PRELIMINARY\': \'tom_alertstreams.alertstreams.alertstream.alert_logger\',\n                \'gcn.classic.text.LVC_RETRACTION\': \'tom_alertstreams.alertstreams.alertstream.alert_logger\',\n            },\n        },\n    }\n]\n```\n\nThe configuration dictionary for each `AlertStream` subclass will contain these key-value pairs:\n* `ACTIVE`: Boolean which tells `readstreams` to access this stream. Should be `True`, unless you want to\nkeep a configuration dictionary, but ignore the stream.\n* `NAME`: The name of the `AlertStream` subclass that implements the interface to this Kafka stream. `tom_alertstreams`\nwill provide `AlertStream` subclasses for major astromical Kafka streams. See below for instructions on Subclassing\nthe `AlertStream` base class.\n* `OPTIONS`: A dictionary of key-value pairs specific to the`AlertStream` subclass given by `NAME`. The doc string for\nthe `AlertStream` subclass should document what is expected. Typically, a URL, authentication information, and a\ndictionary, `TOPIC_HANDLERS`, will be required. See "Subclassing `AlertStream`" below. The `AlertStream` subclass will\nconvert the key-value pairs of the `OPTIONS` dictionary into properties (and values) of the `AlertStream` subclass\ninstance.\n  * The hopskotch alert stream supports a wildcard of `*` for an alert handler topic name. If specified, ALL public topics will be subscribed and use that handler function. A directly specified topic handler will always be used before the `*` handler for any topic that is covered twice. \n\n### Getting Kafka Stream Credentials\nAs part of your `OPTIONS` for each Kafka stream, you need to configure access credentials. Visit these links\nto get credentials for [Hopskotch](https://hop.scimma.org/) and [GCN Classic over Kafka](https://gcn.nasa.gov/quickstart).\nSet the environment variables with the username and passwords obtained. Do not check them in to your code repository.\n\n\n## Alert Handling\n\nAssuming that an `AlertStream` subclass exists for the Kafka stream of interest,\nthe keys of the `TOPIC_HANDLERS` dictionary are the topics that will be subscribed to. The values\nof the `TOPIC_HANDLERS` dictionary specify alert handling methods that will be imported and called\nfor each alert recieved on that topic. An example is provided,\n`tom_alerts.alertstreams.alertstream.alert_logger`, which simply logs the alert.\n\nTo customize this behaviour according to the needs of your TOM, define an alert handling function for each\ntopic that you wish to subscribe to. Your `TOPIC_HANDLERS` dictionary will have a an entry for each topic\nwhose key is the topic name and whose value is a string indicating the dot-path to the alert handling function.\nWhen the `AlertStream` subclass is instanciated, the `OPTIONS` dictionary is read and an `alert_handler`\ndictionary is created. It is keyed by topic name and it\'s values are the imported callable functions specified by the\ndot-path strings. `readstreams` will call the alert handler for each alert that comes in on the topic. The signiture\nof the alert handling function is specific to the `AlertStream` subclasss.\n\n## Subclassing `AlertStream`\n\nIdeally, As a TOM developer, there is already an `AlertStream`-subclass for the alert stream that you\nwant your TOM to listen to. If so, you need only to configure your TOM to use it in  `settings.py`\n`ALERT_STREAMS`. If you must implement your own `AlertStream` subclass, please get in touch. In the meantime, here\'s a brief outline:\n\n1. Create subclass of `AlertStream`.\n\n2. Create `required_keys` and `allowed_keys` class variables in your `AlertStream`-subclass.\n\n   These are lists of strings refering to the keys of the `OPTIONS` dictionary. The purpose of these is to\n   help TOM developers using your `AlertStream`-subclass with the key-value pairs in their `ALERT_STREAMS`\n  `OPTIONS` configuration dictionary.\n\n3. Implement the `listen()` method.\n\n   This method will be called by the `readstreams` management command and is not expected to return. It\n   should instanciate your consumer, subscribe to the topics configured in `ALERT_STREAMS`, and start\n   consuming. The detail of this will depend on the kafka-client used. See `alertstreams.gcn.listen()`\n   and `alertstreams.hopskotch.listen()` for examples to follow.\n   \n   The loop which consumes messages in your `listen()` method should extract the topic from each message\n   and call `self.alert_handler[topic]()` with the message or message-derived arguments specific to your\n   kafka client. Users of your `AlertStream`-subclass will write these topic-specific alert handling methods\n   and configure them in the `TOPIC_HANLDERS` dictionary of their `ALERT_STREAMS` configuration.\n   The `AlertStream` base class will set up the `alert_handler` dictionary according to your users\'\n   configuration. It helps your users to provide an example `alert_hander()` function in your module as\n   an example. (Again, see `alertstreams.gcn.listen()` and `alertstreams.hopskotch.listen()`, their\n   configurations in `settings.py`, and the `alertstreams.gcn.alert_logger()` and\n   `alertstreams.hopskotch.alert_logger() methods, for example).\n',
-    'author': 'TOM Toolkit Project',
-    'author_email': 'tomtoolkit@lco.global',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/TOMToolkit/tom-alertstreams',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.12',
-}
-
-
-setup(**setup_kwargs)
```

