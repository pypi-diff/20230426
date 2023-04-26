# Comparing `tmp/openbrokerapi-4.5.0.tar.gz` & `tmp/openbrokerapi-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbrokerapi-4.5.0.tar", max compression
+gzip compressed data, was "openbrokerapi-4.5.1.tar", max compression
```

## Comparing `openbrokerapi-4.5.0.tar` & `openbrokerapi-4.5.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0     1065 2023-02-16 12:22:26.460217 openbrokerapi-4.5.0/LICENSE
--rw-r--r--   0        0        0     6596 2023-02-16 12:22:26.460217 openbrokerapi-4.5.0/README.rst
--rw-r--r--   0        0        0     1375 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/__init__.py
--rw-r--r--   0        0        0    25386 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/api.py
--rw-r--r--   0        0        0     1830 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/auth.py
--rw-r--r--   0        0        0     2328 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/catalog.py
--rw-r--r--   0        0        0      333 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/constants.py
--rw-r--r--   0        0        0     2051 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/errors.py
--rw-r--r--   0        0        0     1009 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/helper.py
--rw-r--r--   0        0        0     1057 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/log_util.py
--rw-r--r--   0        0        0     2762 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/request_filter.py
--rw-r--r--   0        0        0     2641 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/response.py
--rw-r--r--   0        0        0     4148 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/router.py
--rw-r--r--   0        0        0    17197 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/service_broker.py
--rw-r--r--   0        0        0      400 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/openbrokerapi/settings.py
--rw-r--r--   0        0        0     2308 2023-02-16 12:22:26.464217 openbrokerapi-4.5.0/pyproject.toml
--rw-r--r--   0        0        0     7719 1970-01-01 00:00:00.000000 openbrokerapi-4.5.0/setup.py
--rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 openbrokerapi-4.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-26 09:13:32.818504 openbrokerapi-4.5.1/LICENSE
+-rw-r--r--   0        0        0     6596 2023-04-26 09:13:32.818504 openbrokerapi-4.5.1/README.rst
+-rw-r--r--   0        0        0     1375 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/__init__.py
+-rw-r--r--   0        0        0    25386 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/api.py
+-rw-r--r--   0        0        0     1830 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/auth.py
+-rw-r--r--   0        0        0     2328 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/catalog.py
+-rw-r--r--   0        0        0      333 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/constants.py
+-rw-r--r--   0        0        0     2051 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/errors.py
+-rw-r--r--   0        0        0     1009 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/helper.py
+-rw-r--r--   0        0        0     1057 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/log_util.py
+-rw-r--r--   0        0        0     2762 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/request_filter.py
+-rw-r--r--   0        0        0     2641 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/response.py
+-rw-r--r--   0        0        0     4148 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/router.py
+-rw-r--r--   0        0        0    17197 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/service_broker.py
+-rw-r--r--   0        0        0      400 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/openbrokerapi/settings.py
+-rw-r--r--   0        0        0     2358 2023-04-26 09:13:32.822504 openbrokerapi-4.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8267 1970-01-01 00:00:00.000000 openbrokerapi-4.5.1/PKG-INFO
```

### Comparing `openbrokerapi-4.5.0/LICENSE` & `openbrokerapi-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/README.rst` & `openbrokerapi-4.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/__init__.py` & `openbrokerapi-4.5.1/openbrokerapi/__init__.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/api.py` & `openbrokerapi-4.5.1/openbrokerapi/api.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/auth.py` & `openbrokerapi-4.5.1/openbrokerapi/auth.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/catalog.py` & `openbrokerapi-4.5.1/openbrokerapi/catalog.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/errors.py` & `openbrokerapi-4.5.1/openbrokerapi/errors.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/helper.py` & `openbrokerapi-4.5.1/openbrokerapi/helper.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/log_util.py` & `openbrokerapi-4.5.1/openbrokerapi/log_util.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/request_filter.py` & `openbrokerapi-4.5.1/openbrokerapi/request_filter.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/response.py` & `openbrokerapi-4.5.1/openbrokerapi/response.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/router.py` & `openbrokerapi-4.5.1/openbrokerapi/router.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/openbrokerapi/service_broker.py` & `openbrokerapi-4.5.1/openbrokerapi/service_broker.py`

 * *Files identical despite different names*

### Comparing `openbrokerapi-4.5.0/pyproject.toml` & `openbrokerapi-4.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openbrokerapi"
-version = "4.5.0"
+version = "4.5.1"
 description = "A python package for the V2 CF Service Broker API and Open Broker API (version 2.13+)"
 authors = ["Maic Siemering <maic@siemering.tech>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://openbrokerapi.readthedocs.io/"
 documentation = "https://openbrokerapi.readthedocs.io/"
 repository = "https://github.com/eruvanos/openbrokerapi"
@@ -37,14 +37,15 @@
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = "^2.2.3"
 Sphinx = {version = "^6.1.3", optional = true}
 sphinx-rtd-theme = {version = "^1.2.0", optional = true}
```

### Comparing `openbrokerapi-4.5.0/setup.py` & `openbrokerapi-4.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: openbrokerapi
+Version: 4.5.1
+Summary: A python package for the V2 CF Service Broker API and Open Broker API (version 2.13+)
+Home-page: https://openbrokerapi.readthedocs.io/
+License: MIT
+Keywords: cloudfoundry,cfbrokerapi,openbrokerapi,openservicebrokerapi,servicebroker,flask,kubernetes,k8s
+Author: Maic Siemering
+Author-email: maic@siemering.tech
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Flask
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: docs
+Provides-Extra: gevent
+Provides-Extra: gunicorn
+Requires-Dist: Flask (>=2.2.3,<3.0.0)
+Requires-Dist: Sphinx (>=6.1.3,<7.0.0) ; extra == "docs"
+Requires-Dist: gevent (>=22.10.2,<23.0.0) ; extra == "gevent"
+Requires-Dist: gunicorn (>=20.1.0,<21.0.0) ; extra == "gunicorn"
+Requires-Dist: sphinx-rtd-theme (>=1.2.0,<2.0.0) ; extra == "docs"
+Project-URL: Documentation, https://openbrokerapi.readthedocs.io/
+Project-URL: Repository, https://github.com/eruvanos/openbrokerapi
+Description-Content-Type: text/x-rst
+
+|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP|
+
+Open Broker API
+===============
+
+A Python package for building Service Brokers supporting API version 2.13+.
+
+Following `Open Service Broker
+API Spec <https://github.com/openservicebrokerapi/servicebroker/blob/master/spec.md>`__ and `Open
+Service Broker API <https://www.openservicebrokerapi.org/>`__
+
+Check out the documentation_.
+
+.. _documentation: http://openbrokerapi.readthedocs.io/en/latest/
+
+To find out more about Platform Compatibility for OSBAPI versions, check out
+`Platform Compatibility for OSBAPI <https://github.com/openservicebrokerapi/servicebroker/blob/master/compatibility.md>`__
+
+ Not all features are supported with this library due to conflicting features.
+
+Installation
+------------
+
+This package is available for Python 3.6+.
+
+.. code:: bash
+
+    pip3 install openbrokerapi
+
+    # including gevent as server
+    pip3 install openbrokerapi[gevent]
+    
+    # recommended production setup
+    pip3 install openbrokerapi[gunicorn]
+
+Or install the development version from github:
+
+.. code:: bash
+
+    pip3 install git+https://github.com/eruvanos/openbrokerapi.git
+
+Usage
+-----
+
+You can start with a `skeleton project <https://github.com/eruvanos/openbrokerapi-skeleton>`__ or just from scratch.
+
+.. code:: python
+
+    from typing import Union, List
+
+    import openbrokerapi
+    from openbrokerapi import api
+    from openbrokerapi.api import ServiceBroker
+    from openbrokerapi.catalog import ServicePlan
+    from openbrokerapi.service_broker import (
+        Service,
+        ProvisionDetails,
+        ProvisionedServiceSpec,
+        DeprovisionDetails,
+        DeprovisionServiceSpec
+    )
+
+
+    class MyServiceBroker(ServiceBroker):
+        def catalog(self) -> Union[Service, List[Service]]:
+            return Service(
+                id='service id',
+                name='service name',
+                description='service description',
+                bindable=False,
+                plans=[
+                    ServicePlan(
+                        id='plan id',
+                        name='plan name',
+                        description='plan description',
+                    )
+                ]
+            )
+
+        def provision(self,
+                      instance_id: str,
+                      details: ProvisionDetails,
+                      async_allowed: bool,
+                      **kwargs) -> ProvisionedServiceSpec:
+            # Create service instance
+            # ...
+
+            return ProvisionedServiceSpec()
+
+        def deprovision(self,
+                        instance_id: str,
+                        details: DeprovisionDetails,
+                        async_allowed: bool,
+                        **kwargs) -> DeprovisionServiceSpec:
+            # Delete service instance
+            # ...
+
+            return DeprovisionServiceSpec(is_async=False)
+
+    print('Start server on 127.0.0.1:5000')
+    print('Check the catalog at:')
+    print('> curl 127.0.0.1:5000/v2/catalog -H "X-Broker-API-Version: 2.14"')
+    api.serve(MyServiceBroker(), None)
+
+    # Simply start the server
+    # api.serve(ExampleServiceBroker(), api.BrokerCredentials("", ""))
+
+    # or start the server without authentication
+    # api.serve(ExampleServiceBroker(), None)
+
+    # or start the server with multiple authentication
+    # api.serve(ExampleServiceBroker(), [api.BrokerCredentials("", ""), api.BrokerCredentials("", "")])
+
+    # or with multiple service brokers and multiple credentials
+    # api.serve_multiple([ExampleServiceBroker(), ExampleServiceBroker()], [api.BrokerCredentials("", ""), api.BrokerCredentials("", "")])
+
+    # or register blueprint to your own FlaskApp instance
+    # app = Flask(__name__)
+    # logger = basic_config()  # Use root logger with a basic configuration provided by openbrokerapi.log_util
+    # openbroker_bp = api.get_blueprint(ExampleServiceBroker(), api.BrokerCredentials("", ""), logger)
+    # app.register_blueprint(openbroker_bp)
+    # app.run("0.0.0.0")
+
+Deployment
+----------
+The included :code:`api.serve` function provides a server setup for **local usage only**.
+
+For productive deployments use the blueprint from :code:`api.get_blueprint` to
+setup a production ready server like `Waitress <https://docs.pylonsproject.org/projects/waitress/en/latest/>`__
+or other mentioned in `Flask Deployment Docs <http://flask.pocoo.org/docs/dev/deploying/wsgi-standalone/>`__
+
+Error Types
+-----------
+
+Openbrokerapi defines a handful of error types in errors.py for some
+common error cases that your service broker may encounter. Raise these
+from your ServiceBroker methods where appropriate, and openbrokerapi
+will do the "right thing" (™), and give Cloud Foundry an appropriate
+status code, as per the Service Broker API specification.
+
+
+Bugs or Issues
+--------------
+
+Please report bugs, issues or feature requests to `Github
+Issues`_
+
+
+How to contribute
+-----------------
+
+You want to contribute, I really appreciate!
+
+So let us check how you can contribute:
+
+- Create an issue in the `Github Issues`_. Please provide all information that you think are usefull to solve it.
+- Use the `Github Issues`_ to create a feature request, so we can discuss and find a good interface for that feature.
+- Create a Pull Request. There are some things that will make it easier to review your Pull Request:
+
+    - Use a new branch for every Pull Request
+    - Include just related commits in this branch
+    - Less commits are better, one would be the best (You can squash them.)
+    - Always add tests for your feature, if you are not familiar with writing tests, ask for help.
+    - Hint: To update your fork with the newest changes, follow `these instructions <https://stackoverflow.com/a/7244456/2947505>`_.
+
+[ ~ Dependencies scanned by PyUp.io ~ ]
+
+.. _Github Issues: https://github.com/eruvanos/openbrokerapi/issues
+
+.. |Build Status| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml/badge.svg
+    :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml
+.. |Coverage Status| image:: https://coveralls.io/repos/github/eruvanos/openbrokerapi/badge.svg?branch=master
+   :target: https://coveralls.io/github/eruvanos/openbrokerapi?branch=main
+.. |Known Vulnerabilities| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml/badge.svg
+   :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml
+.. |PYUP| image:: https://pyup.io/repos/github/eruvanos/openbrokerapi/shield.svg
+     :target: https://pyup.io/repos/github/eruvanos/openbrokerapi/
 
-packages = \
-['openbrokerapi']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Flask>=2.2.3,<3.0.0']
-
-extras_require = \
-{'docs': ['Sphinx>=6.1.3,<7.0.0', 'sphinx-rtd-theme>=1.2.0,<2.0.0'],
- 'gevent': ['gevent>=22.10.2,<23.0.0'],
- 'gunicorn': ['gunicorn>=20.1.0,<21.0.0']}
-
-setup_kwargs = {
-    'name': 'openbrokerapi',
-    'version': '4.5.0',
-    'description': 'A python package for the V2 CF Service Broker API and Open Broker API (version 2.13+)',
-    'long_description': '|Build Status| |Coverage Status| |Known Vulnerabilities| |PYUP|\n\nOpen Broker API\n===============\n\nA Python package for building Service Brokers supporting API version 2.13+.\n\nFollowing `Open Service Broker\nAPI Spec <https://github.com/openservicebrokerapi/servicebroker/blob/master/spec.md>`__ and `Open\nService Broker API <https://www.openservicebrokerapi.org/>`__\n\nCheck out the documentation_.\n\n.. _documentation: http://openbrokerapi.readthedocs.io/en/latest/\n\nTo find out more about Platform Compatibility for OSBAPI versions, check out\n`Platform Compatibility for OSBAPI <https://github.com/openservicebrokerapi/servicebroker/blob/master/compatibility.md>`__\n\n Not all features are supported with this library due to conflicting features.\n\nInstallation\n------------\n\nThis package is available for Python 3.6+.\n\n.. code:: bash\n\n    pip3 install openbrokerapi\n\n    # including gevent as server\n    pip3 install openbrokerapi[gevent]\n    \n    # recommended production setup\n    pip3 install openbrokerapi[gunicorn]\n\nOr install the development version from github:\n\n.. code:: bash\n\n    pip3 install git+https://github.com/eruvanos/openbrokerapi.git\n\nUsage\n-----\n\nYou can start with a `skeleton project <https://github.com/eruvanos/openbrokerapi-skeleton>`__ or just from scratch.\n\n.. code:: python\n\n    from typing import Union, List\n\n    import openbrokerapi\n    from openbrokerapi import api\n    from openbrokerapi.api import ServiceBroker\n    from openbrokerapi.catalog import ServicePlan\n    from openbrokerapi.service_broker import (\n        Service,\n        ProvisionDetails,\n        ProvisionedServiceSpec,\n        DeprovisionDetails,\n        DeprovisionServiceSpec\n    )\n\n\n    class MyServiceBroker(ServiceBroker):\n        def catalog(self) -> Union[Service, List[Service]]:\n            return Service(\n                id=\'service id\',\n                name=\'service name\',\n                description=\'service description\',\n                bindable=False,\n                plans=[\n                    ServicePlan(\n                        id=\'plan id\',\n                        name=\'plan name\',\n                        description=\'plan description\',\n                    )\n                ]\n            )\n\n        def provision(self,\n                      instance_id: str,\n                      details: ProvisionDetails,\n                      async_allowed: bool,\n                      **kwargs) -> ProvisionedServiceSpec:\n            # Create service instance\n            # ...\n\n            return ProvisionedServiceSpec()\n\n        def deprovision(self,\n                        instance_id: str,\n                        details: DeprovisionDetails,\n                        async_allowed: bool,\n                        **kwargs) -> DeprovisionServiceSpec:\n            # Delete service instance\n            # ...\n\n            return DeprovisionServiceSpec(is_async=False)\n\n    print(\'Start server on 127.0.0.1:5000\')\n    print(\'Check the catalog at:\')\n    print(\'> curl 127.0.0.1:5000/v2/catalog -H "X-Broker-API-Version: 2.14"\')\n    api.serve(MyServiceBroker(), None)\n\n    # Simply start the server\n    # api.serve(ExampleServiceBroker(), api.BrokerCredentials("", ""))\n\n    # or start the server without authentication\n    # api.serve(ExampleServiceBroker(), None)\n\n    # or start the server with multiple authentication\n    # api.serve(ExampleServiceBroker(), [api.BrokerCredentials("", ""), api.BrokerCredentials("", "")])\n\n    # or with multiple service brokers and multiple credentials\n    # api.serve_multiple([ExampleServiceBroker(), ExampleServiceBroker()], [api.BrokerCredentials("", ""), api.BrokerCredentials("", "")])\n\n    # or register blueprint to your own FlaskApp instance\n    # app = Flask(__name__)\n    # logger = basic_config()  # Use root logger with a basic configuration provided by openbrokerapi.log_util\n    # openbroker_bp = api.get_blueprint(ExampleServiceBroker(), api.BrokerCredentials("", ""), logger)\n    # app.register_blueprint(openbroker_bp)\n    # app.run("0.0.0.0")\n\nDeployment\n----------\nThe included :code:`api.serve` function provides a server setup for **local usage only**.\n\nFor productive deployments use the blueprint from :code:`api.get_blueprint` to\nsetup a production ready server like `Waitress <https://docs.pylonsproject.org/projects/waitress/en/latest/>`__\nor other mentioned in `Flask Deployment Docs <http://flask.pocoo.org/docs/dev/deploying/wsgi-standalone/>`__\n\nError Types\n-----------\n\nOpenbrokerapi defines a handful of error types in errors.py for some\ncommon error cases that your service broker may encounter. Raise these\nfrom your ServiceBroker methods where appropriate, and openbrokerapi\nwill do the "right thing" (™), and give Cloud Foundry an appropriate\nstatus code, as per the Service Broker API specification.\n\n\nBugs or Issues\n--------------\n\nPlease report bugs, issues or feature requests to `Github\nIssues`_\n\n\nHow to contribute\n-----------------\n\nYou want to contribute, I really appreciate!\n\nSo let us check how you can contribute:\n\n- Create an issue in the `Github Issues`_. Please provide all information that you think are usefull to solve it.\n- Use the `Github Issues`_ to create a feature request, so we can discuss and find a good interface for that feature.\n- Create a Pull Request. There are some things that will make it easier to review your Pull Request:\n\n    - Use a new branch for every Pull Request\n    - Include just related commits in this branch\n    - Less commits are better, one would be the best (You can squash them.)\n    - Always add tests for your feature, if you are not familiar with writing tests, ask for help.\n    - Hint: To update your fork with the newest changes, follow `these instructions <https://stackoverflow.com/a/7244456/2947505>`_.\n\n[ ~ Dependencies scanned by PyUp.io ~ ]\n\n.. _Github Issues: https://github.com/eruvanos/openbrokerapi/issues\n\n.. |Build Status| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml/badge.svg\n    :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/python-test.yml\n.. |Coverage Status| image:: https://coveralls.io/repos/github/eruvanos/openbrokerapi/badge.svg?branch=master\n   :target: https://coveralls.io/github/eruvanos/openbrokerapi?branch=main\n.. |Known Vulnerabilities| image:: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml/badge.svg\n   :target: https://github.com/eruvanos/openbrokerapi/actions/workflows/codeql.yml\n.. |PYUP| image:: https://pyup.io/repos/github/eruvanos/openbrokerapi/shield.svg\n     :target: https://pyup.io/repos/github/eruvanos/openbrokerapi/\n',
-    'author': 'Maic Siemering',
-    'author_email': 'maic@siemering.tech',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://openbrokerapi.readthedocs.io/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

