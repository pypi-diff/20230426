# Comparing `tmp/coredb_pgmq_python-0.1.1.tar.gz` & `tmp/coredb_pgmq_python-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredb_pgmq_python-0.1.1.tar", max compression
+gzip compressed data, was "coredb_pgmq_python-0.2.0.tar", max compression
```

## Comparing `coredb_pgmq_python-0.1.1.tar` & `coredb_pgmq_python-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1465 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/README.md
--rw-r--r--   0        0        0      106 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/coredb_pgmq_python/__init__.py
--rw-r--r--   0        0        0     3485 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/coredb_pgmq_python/queue.py
--rw-r--r--   0        0        0     1015 2023-04-14 18:23:56.964191 coredb_pgmq_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.1/setup.py
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/README.md
+-rw-r--r--   0        0        0      106 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/coredb_pgmq_python/__init__.py
+-rw-r--r--   0        0        0     3532 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/coredb_pgmq_python/queue.py
+-rw-r--r--   0        0        0     1015 2023-04-25 14:35:45.630453 coredb_pgmq_python-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2301 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.0/setup.py
+-rw-r--r--   0        0        0     2425 1970-01-01 00:00:00.000000 coredb_pgmq_python-0.2.0/PKG-INFO
```

### Comparing `coredb_pgmq_python-0.1.1/README.md` & `coredb_pgmq_python-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 Install with `pip` from pypi.org
 
 ```bash
 pip install coredb-pgmq-python
 ```
 
-Dependencies
+Dependencies:
 
 Postgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).
 
 ## Usage
 
 ## Start a Postgres Instance with the CoreDB extension installed
 
 ```bash
-docker run -d -p 5432:5432 quay.io/coredb/coredb-pg:latest
+docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest
 ```
 
 Initialize a connection to Postgres
 
 ```python
 
 from coredb_pgmq_python import PGMQueue, Message
```

### Comparing `coredb_pgmq_python-0.1.1/coredb_pgmq_python/queue.py` & `coredb_pgmq_python-0.2.0/coredb_pgmq_python/queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """Base class for interacting with a queue"""
 
     host: str = "localhost"
     port: str = "5432"
     database: str = "postgres"
     delay: int = 0
     vt: int = 30
-    partition_size: int = 5000
 
     username: str = "postgres"
     password: str = "postgres"
 
     pool_size: int = 10
 
     kwargs: dict = field(default_factory=dict)
@@ -49,18 +48,20 @@
             conn.execute("create extension if not exists pgmq cascade;")
 
     def create_queue(self, queue: str) -> None:
         """Create a queue"""
         with self.pool.connection() as conn:
             conn.execute("select pgmq_create(%s);", [queue])
 
-    def create_partitioned_queue(self, queue: str, partition_size: Optional[int] = None) -> None:
+    def create_(
+        self, queue: str, partition_interval: Optional[str] = "daily", retention_interval: Optional[str] = "5 days"
+    ) -> None:
         """Create a partitioned queue"""
         with self.pool.connection() as conn:
-            conn.execute("select pgmq_create_partitioned(%s, %s);", [queue, partition_size])
+            conn.execute("select pgmq_create_non_partitioned(%s, %s);", [queue, partition_interval, retention_interval])
 
     def send(self, queue: str, message: dict, delay: Optional[int] = None) -> int:
         """Send a message to a queue"""
 
         with self.pool.connection() as conn:
             if delay is not None:
                 # TODO(chuckend): implement send_delay in pgmq
```

### Comparing `coredb_pgmq_python-0.1.1/pyproject.toml` & `coredb_pgmq_python-0.2.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coredb-pgmq-python"
-version = "0.1.1"
+version = "0.2.0"
 description = "Python client for the PGMQ Postgres extension."
 authors = ["Adam Hendel <adam@coredb.io>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "coredb_pgmq_python"}]
 
 [tool.poetry.urls]
```

### Comparing `coredb_pgmq_python-0.1.1/setup.py` & `coredb_pgmq_python-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 install_requires = \
 ['orjson>=3.8.10,<4.0.0',
  'psycopg[binary,pool]>=3.1.8,<4.0.0',
  'pydantic>=1.10.7,<2.0.0']
 
 setup_kwargs = {
     'name': 'coredb-pgmq-python',
-    'version': '0.1.1',
+    'version': '0.2.0',
     'description': 'Python client for the PGMQ Postgres extension.',
-    'long_description': '# Coredb\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install coredb-pgmq-python\n```\n\nDependencies\n\nPostgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the CoreDB extension installed\n\n```bash\ndocker run -d -p 5432:5432 quay.io/coredb/coredb-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\n\nfrom coredb_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
+    'long_description': '# Coredb\'s Python Client for PGMQ\n\n## Installation\n\nInstall with `pip` from pypi.org\n\n```bash\npip install coredb-pgmq-python\n```\n\nDependencies:\n\nPostgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).\n\n## Usage\n\n## Start a Postgres Instance with the CoreDB extension installed\n\n```bash\ndocker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest\n```\n\nInitialize a connection to Postgres\n\n```python\n\nfrom coredb_pgmq_python import PGMQueue, Message\n\nqueue = PGMQueue(host="0.0.0.0")\n```\n\nCreate a queue (or a partitioned queue)\n\n```python\nqueue.create_queue("my_queue")\n# queue.create_partitioned_queue("my_partitioned_queue", partition_size=10000)\n```\n\n\nSend a message\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\n```\n\nRead a message, set it invisible for 30 seconds.\n\n```python\nread_message: Message = queue.read("my_queue", vt=10)\nprint(read_message)\n```\n\nArchive the message after we\'re done with it. Archived messages are moved to an archive table.\n\n```python\narchived: bool = queue.archive("my_queue", read_message.msg_id)\n```\n\nDelete a message completely.\n\n```python\nmsg_id: int = queue.send("my_queue", {"hello": "world"})\nread_message: Message = queue.read("my_queue")\ndeleted: bool = queue.delete("my_queue", read_message.msg_id)\n```\n\nPop a message, deleting it and reading it in one transaction.\n\n```python\npopped_message: Message = queue.pop("my_queue")\nprint(popped_message)\n```\n',
     'author': 'Adam Hendel',
     'author_email': 'adam@coredb.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `coredb_pgmq_python-0.1.1/PKG-INFO` & `coredb_pgmq_python-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coredb-pgmq-python
-Version: 0.1.1
+Version: 0.2.0
 Summary: Python client for the PGMQ Postgres extension.
 License: Apache 2.0
 Author: Adam Hendel
 Author-email: adam@coredb.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -25,24 +25,24 @@
 
 Install with `pip` from pypi.org
 
 ```bash
 pip install coredb-pgmq-python
 ```
 
-Dependencies
+Dependencies:
 
 Postgres running the [CoreDB PGMQ extension](https://github.com/CoreDB-io/coredb/tree/main/extensions/pgmq).
 
 ## Usage
 
 ## Start a Postgres Instance with the CoreDB extension installed
 
 ```bash
-docker run -d -p 5432:5432 quay.io/coredb/coredb-pg:latest
+docker run -d --name postgres -e POSTGRES_PASSWORD=postgres -p 5432:5432 quay.io/coredb/pgmq-pg:latest
 ```
 
 Initialize a connection to Postgres
 
 ```python
 
 from coredb_pgmq_python import PGMQueue, Message
```

