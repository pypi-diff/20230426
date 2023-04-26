# Comparing `tmp/questdb-connect-0.0.21.tar.gz` & `tmp/questdb-connect-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "questdb-connect-0.0.21.tar", last modified: Wed Apr 26 18:12:05 2023, max compression
+gzip compressed data, was "questdb-connect-0.0.22.tar", last modified: Wed Apr 26 18:19:41 2023, max compression
```

## Comparing `questdb-connect-0.0.21.tar` & `questdb-connect-0.0.22.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:12:05.674612 questdb-connect-0.0.21/
--rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.21/LICENSE
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:12:05.674483 questdb-connect-0.0.21/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.21/README.md
--rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 18:11:43.000000 questdb-connect-0.0.21/pyproject.toml
--rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 18:12:05.674647 questdb-connect-0.0.21/setup.cfg
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:12:05.671162 questdb-connect-0.0.21/src/
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:12:05.672772 questdb-connect-0.0.21/src/questdb_connect/
--rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.21/src/questdb_connect/__init__.py
--rw-r--r--   0 marregui   (501) staff       (20)     9766 2023-04-26 18:11:51.000000 questdb-connect-0.0.21/src/questdb_connect/dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     8316 2023-04-26 17:38:03.000000 questdb-connect-0.0.21/src/questdb_connect/superset_engine.py
--rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.21/src/questdb_connect/types.py
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:12:05.673634 questdb-connect-0.0.21/src/questdb_connect.egg-info/
--rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/PKG-INFO
--rw-r--r--   0 marregui   (501) staff       (20)      488 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/SOURCES.txt
--rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/dependency_links.txt
--rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/entry_points.txt
--rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/requires.txt
--rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 18:12:05.000000 questdb-connect-0.0.21/src/questdb_connect.egg-info/top_level.txt
-drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:12:05.674205 questdb-connect-0.0.21/tests/
--rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.21/tests/test_dialect.py
--rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.21/tests/test_superset.py
--rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.21/tests/test_types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.824389 questdb-connect-0.0.22/
+-rw-r--r--   0 marregui   (501) staff       (20)    11357 2023-04-19 08:13:39.000000 questdb-connect-0.0.22/LICENSE
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:19:41.824229 questdb-connect-0.0.22/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)     3295 2023-04-24 12:57:30.000000 questdb-connect-0.0.22/README.md
+-rw-r--r--   0 marregui   (501) staff       (20)     2432 2023-04-26 18:19:28.000000 questdb-connect-0.0.22/pyproject.toml
+-rw-r--r--   0 marregui   (501) staff       (20)       38 2023-04-26 18:19:41.824430 questdb-connect-0.0.22/setup.cfg
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.820330 questdb-connect-0.0.22/src/
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.822026 questdb-connect-0.0.22/src/questdb_connect/
+-rw-r--r--   0 marregui   (501) staff       (20)     1402 2023-04-26 17:37:24.000000 questdb-connect-0.0.22/src/questdb_connect/__init__.py
+-rw-r--r--   0 marregui   (501) staff       (20)     9849 2023-04-26 18:19:28.000000 questdb-connect-0.0.22/src/questdb_connect/dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     8316 2023-04-26 17:38:03.000000 questdb-connect-0.0.22/src/questdb_connect/superset_engine.py
+-rw-r--r--   0 marregui   (501) staff       (20)     5786 2023-04-26 17:30:43.000000 questdb-connect-0.0.22/src/questdb_connect/types.py
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.823027 questdb-connect-0.0.22/src/questdb_connect.egg-info/
+-rw-r--r--   0 marregui   (501) staff       (20)     4003 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/PKG-INFO
+-rw-r--r--   0 marregui   (501) staff       (20)      488 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 marregui   (501) staff       (20)        1 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      148 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/entry_points.txt
+-rw-r--r--   0 marregui   (501) staff       (20)      117 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/requires.txt
+-rw-r--r--   0 marregui   (501) staff       (20)       16 2023-04-26 18:19:41.000000 questdb-connect-0.0.22/src/questdb_connect.egg-info/top_level.txt
+drwxr-xr-x   0 marregui   (501) staff       (20)        0 2023-04-26 18:19:41.823818 questdb-connect-0.0.22/tests/
+-rw-r--r--   0 marregui   (501) staff       (20)     9763 2023-04-26 11:45:04.000000 questdb-connect-0.0.22/tests/test_dialect.py
+-rw-r--r--   0 marregui   (501) staff       (20)     2552 2023-04-26 13:30:18.000000 questdb-connect-0.0.22/tests/test_superset.py
+-rw-r--r--   0 marregui   (501) staff       (20)     3245 2023-04-26 12:12:01.000000 questdb-connect-0.0.22/tests/test_types.py
```

### Comparing `questdb-connect-0.0.21/LICENSE` & `questdb-connect-0.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/PKG-INFO` & `questdb-connect-0.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.21
+Version: 0.0.22
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.21/README.md` & `questdb-connect-0.0.22/README.md`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/pyproject.toml` & `questdb-connect-0.0.22/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # https://pip.pypa.io/en/stable/reference/build-system/pyproject-toml/
 [project]
 name = "questdb-connect"
-version = "0.0.21"
+version = "0.0.22"
 authors = [{ name = "questdb.io", email = "miguel@questdb.io" }]
 description = "SqlAlchemy/Superset libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `questdb-connect-0.0.21/src/questdb_connect/__init__.py` & `questdb-connect-0.0.22/src/questdb_connect/__init__.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/src/questdb_connect/dialect.py` & `questdb-connect-0.0.22/src/questdb_connect/dialect.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 from sqlalchemy.orm.exc import NoResultFound
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.compiler import DDLCompiler, GenericTypeCompiler, IdentifierPreparer, SQLCompiler
 from sqlalchemy.sql.visitors import Traversible
 
 from questdb_connect.types import PartitionBy, QDBTypeMixin, quote_identifier, resolve_type_from_name
 
+
 # https://docs.sqlalchemy.org/en/14/ apache-superset requires SQLAlchemy 1.4
 
 # ===== SQLAlchemy Dialect ======
 
 def connection_uri(host: str, port: int, username: str, password: str, database: str = 'main'):
     return f'questdb://{username}:{password}@{host}:{port}/{database}'
 
@@ -84,16 +85,21 @@
 
     def _set_parent(self, parent, **_kwargs):
         parent.engine = self
 
 
 # ===== QUESTDB DIALECT TYPES =====
 
+def _none(_ignore):
+    return None
+
 
 class QDBIdentifierPreparer(IdentifierPreparer, abc.ABC):
+    schema_for_object = staticmethod(_none)
+
     def quote_identifier(self, value):
         return quote_identifier(value)
 
     def _requires_quotes(self, _value):
         return True
 
     def schema_for_object(self, _obj):
```

### Comparing `questdb-connect-0.0.21/src/questdb_connect/superset_engine.py` & `questdb-connect-0.0.22/src/questdb_connect/superset_engine.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/src/questdb_connect/types.py` & `questdb-connect-0.0.22/src/questdb_connect/types.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/src/questdb_connect.egg-info/PKG-INFO` & `questdb-connect-0.0.22/src/questdb_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: questdb-connect
-Version: 0.0.21
+Version: 0.0.22
 Summary: SqlAlchemy/Superset libraries.
 Author-email: "questdb.io" <miguel@questdb.io>
 Project-URL: Homepage, https://github.com/questdb/questdb-connect/
 Project-URL: Bug Tracker, https://github.com/questdb/questdb-connect/issues/
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `questdb-connect-0.0.21/tests/test_dialect.py` & `questdb-connect-0.0.22/tests/test_dialect.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/tests/test_superset.py` & `questdb-connect-0.0.22/tests/test_superset.py`

 * *Files identical despite different names*

### Comparing `questdb-connect-0.0.21/tests/test_types.py` & `questdb-connect-0.0.22/tests/test_types.py`

 * *Files identical despite different names*

