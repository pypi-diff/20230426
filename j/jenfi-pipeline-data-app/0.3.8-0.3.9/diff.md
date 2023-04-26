# Comparing `tmp/jenfi-pipeline-data-app-0.3.8.tar.gz` & `tmp/jenfi_pipeline_data_app-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenfi-pipeline-data-app-0.3.8.tar", max compression
+gzip compressed data, was "jenfi_pipeline_data_app-0.3.9.tar", max compression
```

## Comparing `jenfi-pipeline-data-app-0.3.8.tar` & `jenfi_pipeline_data_app-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      506 2022-09-28 01:48:11.362394 jenfi-pipeline-data-app-0.3.8/README.md
--rw-r--r--   0        0        0     1313 2022-09-28 02:32:06.697627 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/API.md
--rw-r--r--   0        0        0      699 2022-09-28 07:28:44.984055 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/__init__.py
--rw-r--r--   0        0        0      352 2022-09-27 12:01:11.538904 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/_pdoc.py
--rw-r--r--   0        0        0     2159 2022-09-28 05:35:29.110840 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app.py
--rw-r--r--   0        0        0      290 2022-09-28 02:41:44.164337 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_constants.py
--rw-r--r--   0        0        0      986 2022-09-23 02:13:28.813212 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_db_handler.py
--rw-r--r--   0        0        0      644 2022-09-28 03:11:48.896815 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_exit_program.py
--rw-r--r--   0        0        0     1071 2022-09-26 02:09:40.339139 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_models_s3.py
--rw-r--r--   0        0        0     1229 2022-09-26 02:09:40.339356 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_parameters.py
--rw-r--r--   0        0        0     1152 2022-09-28 01:29:43.344757 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_query.py
--rw-r--r--   0        0        0     2937 2022-09-28 07:27:48.368864 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_result.py
--rw-r--r--   0        0        0      543 2022-09-23 02:13:28.814271 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
--rw-r--r--   0        0        0     1105 2022-09-23 02:13:28.816141 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/config/db.py
--rw-r--r--   0        0        0      403 2022-09-26 02:09:40.340068 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/config/s3.py
--rw-r--r--   0        0        0       30 2022-09-26 02:09:40.340419 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_cache/__init__.py
--rw-r--r--   0        0        0     3846 2022-09-26 02:09:40.340623 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_cache/cacher.py
--rw-r--r--   0        0        0     1610 2022-09-26 04:22:14.607584 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_cache/db_cache.py
--rw-r--r--   0        0        0     1268 2022-09-28 07:27:40.985696 jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_models.py
--rw-r--r--   0        0        0      692 2022-09-28 07:28:44.705904 jenfi-pipeline-data-app-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1615 2022-09-28 07:28:50.433550 jenfi-pipeline-data-app-0.3.8/setup.py
--rw-r--r--   0        0        0     1203 2022-09-28 07:28:50.433709 jenfi-pipeline-data-app-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      506 2022-09-28 01:48:11.362394 jenfi_pipeline_data_app-0.3.9/README.md
+-rw-r--r--   0        0        0     1313 2022-09-28 02:32:06.697627 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/API.md
+-rw-r--r--   0        0        0      699 2022-11-01 07:55:16.205711 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/__init__.py
+-rw-r--r--   0        0        0      352 2022-09-27 12:01:11.538904 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/_pdoc.py
+-rw-r--r--   0        0        0     2159 2022-09-28 05:35:29.110840 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app.py
+-rw-r--r--   0        0        0      290 2022-11-01 06:52:43.710759 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_constants.py
+-rw-r--r--   0        0        0     1171 2022-11-01 04:25:15.307222 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_db_handler.py
+-rw-r--r--   0        0        0      644 2022-09-28 03:11:48.896815 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_exit_program.py
+-rw-r--r--   0        0        0     1071 2022-09-26 02:09:40.339139 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_models_s3.py
+-rw-r--r--   0        0        0     1229 2022-09-26 02:09:40.339356 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_parameters.py
+-rw-r--r--   0        0        0     1152 2022-09-28 01:29:43.344757 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_query.py
+-rw-r--r--   0        0        0     2937 2022-09-28 07:27:48.368864 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_result.py
+-rw-r--r--   0        0        0      543 2022-09-23 02:13:28.814271 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_test_funcs.py
+-rw-r--r--   0        0        0     1414 2022-11-01 04:23:14.674255 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/db.py
+-rw-r--r--   0        0        0      403 2022-09-26 02:09:40.340068 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/s3.py
+-rw-r--r--   0        0        0       30 2022-09-26 02:09:40.340419 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/__init__.py
+-rw-r--r--   0        0        0     3846 2022-09-26 02:09:40.340623 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/cacher.py
+-rw-r--r--   0        0        0     1610 2022-09-26 04:22:14.607584 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/db_cache.py
+-rw-r--r--   0        0        0     2199 2022-11-01 07:44:20.436236 jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_models.py
+-rw-r--r--   0        0        0      862 2022-11-01 07:55:16.050538 jenfi_pipeline_data_app-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.3.9/setup.py
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 jenfi_pipeline_data_app-0.3.9/PKG-INFO
```

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/API.md` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/API.md`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/__init__.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.8"
+__version__ = "0.3.9"
 
 from ._pdoc import __pdoc__
 
 from .app import Application
 
 PipelineDataApp = Application()
```

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_db_handler.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_db_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,16 +25,23 @@
         from ..config.db import ProductionConfig
 
         db_config = ProductionConfig()
     elif self.PYTHON_ENV == "staging":
         from ..config.db import StagingConfig
 
         db_config = StagingConfig()
+    elif self.PYTHON_ENV == "test":
+        # TEST - take environment variables from .env
+        load_dotenv()
+
+        from ..config.db import TestConfig
+
+        db_config = TestConfig()
     else:
-        # ONLY DEV - take environment variables from .env
+        # DEV - take environment variables from .env
         load_dotenv()
 
         from ..config.db import DevelopmentConfig
 
         db_config = DevelopmentConfig()
 
     return db_config
```

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_exit_program.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_exit_program.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_models_s3.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_models_s3.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_parameters.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_parameters.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_query.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_query.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_result.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_result.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/app_funcs/_test_funcs.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/app_funcs/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/config/db.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/config/db.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,14 +24,23 @@
     PG_USERNAME = os.getenv("PG_USERNAME")
     PG_PASSWORD = os.getenv("PG_PASSWORD")
     PG_HOST = os.getenv("PG_HOST")
     DB_PORT = os.getenv("PG_PORT", 5432)
     DB_NAME = os.getenv("DB_NAME", "jenfi_com_staging")
 
 
+class TestConfig(Config):
+    DEBUG = os.getenv("DEBUG", True)
+    PG_USERNAME = os.getenv("PG_USERNAME", "postgres")
+    PG_PASSWORD = os.getenv("PG_PASSWORD", "")
+    PG_HOST = os.getenv("PG_HOST", "localhost")
+    DB_PORT = os.getenv("PG_PORT", 5432)
+    DB_NAME = os.getenv("DB_NAME", "jenfi_com_test")
+
+
 class DevelopmentConfig(Config):
     DEBUG = os.getenv("DEBUG", True)
     PG_USERNAME = os.getenv("PG_USERNAME", "postgres")
     PG_PASSWORD = os.getenv("PG_PASSWORD", "")
     PG_HOST = os.getenv("PG_HOST", "localhost")
     DB_PORT = os.getenv("PG_PORT", 5432)
     DB_NAME = os.getenv("DB_NAME", "jenfi_com_development")
```

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_cache/cacher.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/cacher.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_cache/db_cache.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_cache/db_cache.py`

 * *Files identical despite different names*

### Comparing `jenfi-pipeline-data-app-0.3.8/jenfi_pipeline_data_app/db_models.py` & `jenfi_pipeline_data_app-0.3.9/jenfi_pipeline_data_app/db_models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,59 @@
-from sqlalchemy import Table, MetaData, Column, JSON
+from sqlalchemy import ForeignKey, Table, MetaData, Column, JSON
 from sqlalchemy.ext.mutable import MutableDict
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy.ext.declarative import declarative_base
 
 from sqlalchemy.orm.attributes import flag_modified
 
+import datetime
+
+from sqlalchemy import Table, Column, Integer, DateTime
+
 # This shouldn't be a function, but I can't figure out how to pass a db_engine before the class creation on import.
 # ATM, all classes will have to be loaded via function =\
-# 
+#
 # https://stackoverflow.com/questions/4215920/how-to-bind-engine-when-i-want-when-using-declarative-base-in-sqlalchemy
 # The above is the same problem. It recommends using a DeferredRefelection, but that didn't work for me.
 def state_machine_run_model(app):
     Base = declarative_base()
     metadata = MetaData(bind=app.db_engine)
 
     class StateMachineRun(Base):
         __table__ = Table(
             "pipeline_state_machine_runs",
             metadata,
+            Column("id", Integer, primary_key=True),
             Column("result", MutableDict.as_mutable(JSON)),
+            Column('created_at', DateTime, default=datetime.datetime.now),
+            Column('updated_at', DateTime, default=datetime.datetime.now),
             autoload=True,
         )
 
         def result_to_db(self, logical_step_name, state_machine_run_id, results):
-            sm_run = app.db.query(StateMachineRun).get(state_machine_run_id)
+            sm_run = (
+                app.db.query(StateMachineRun)
+                .populate_existing()
+                .with_for_update(of=StateMachineRun, nowait=False)
+                .get(state_machine_run_id)
+            )
             sm_run.result[logical_step_name] = results
 
             return app.db.commit()
 
-    return StateMachineRun
+    return StateMachineRun
+
+def state_machine_model(app):
+    Base = declarative_base()
+    metadata = MetaData(bind=app.db_engine)
+
+    class StateMachine(Base):
+        __table__ = Table(
+            "pipeline_state_machines",
+            metadata,
+            Column("id", Integer, primary_key=True),
+            Column('created_at', DateTime, default=datetime.datetime.now),
+            Column('updated_at', DateTime, default=datetime.datetime.now),
+            autoload=True,
+        )
+
+    return StateMachine
```

### Comparing `jenfi-pipeline-data-app-0.3.8/setup.py` & `jenfi_pipeline_data_app-0.3.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,22 +22,22 @@
  'sqlparse>=0.4.2,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['pipeline-data-app = pipeline_data_app:main']}
 
 setup_kwargs = {
     'name': 'jenfi-pipeline-data-app',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': '',
     'long_description': "# Jenfi Pipeline Data App\n\nDesigned to allow teams to access Jenfi's data sources in a Jupyter Notebook.\n\n## Docs\n\n[View public API doc](https://jenfi-eng.github.io/pipeline-data) for using in Jupyter notebook.\n\n## Basic Usage\n\n```python\nfrom jenfi_pipeline_data_app import PipelineDataApp as Jenfi\n\nJenfi.ROOT_DIR # => /Your/app/root/dir\n```\n\nSetup a `.env` file in the folder of `Jenfi.ROOT_DIR`\n\n## Maintaining this repo\n\n- Build pdoc - `pdoc --html --force --output-dir ./docs jenfi_pipeline_data_app`\n",
     'author': 'Justin Louie',
     'author_email': '224840+nitsujri@users.noreply.github.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<3.11',
 }
```

### Comparing `jenfi-pipeline-data-app-0.3.8/PKG-INFO` & `jenfi_pipeline_data_app-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jenfi-pipeline-data-app
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Author: Justin Louie
 Author-email: 224840+nitsujri@users.noreply.github.com
 Requires-Python: >=3.10,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0)
```

