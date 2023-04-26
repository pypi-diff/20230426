# Comparing `tmp/DBPlus-0.3.1.tar.gz` & `tmp/DBPlus-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DBPlus-0.3.1.tar", last modified: Thu Feb 23 10:56:43 2023, max compression
+gzip compressed data, was "DBPlus-0.3.2.tar", last modified: Wed Apr 26 08:04:51 2023, max compression
```

## Comparing `DBPlus-0.3.1.tar` & `DBPlus-0.3.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-23 10:56:43.593669 DBPlus-0.3.1/
-drwxrwxrwx   0        0        0        0 2023-02-23 10:56:43.553658 DBPlus-0.3.1/DBPlus.egg-info/
--rw-rw-rw-   0        0        0     4386 2023-02-23 10:56:43.000000 DBPlus-0.3.1/DBPlus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-02-23 10:56:43.000000 DBPlus-0.3.1/DBPlus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-23 10:56:43.000000 DBPlus-0.3.1/DBPlus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2019-01-24 13:53:59.000000 DBPlus-0.3.1/DBPlus.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-02-23 10:56:43.000000 DBPlus-0.3.1/DBPlus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4386 2023-02-23 10:56:43.592688 DBPlus-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4061 2021-06-08 14:29:09.000000 DBPlus-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-23 10:56:43.571660 DBPlus-0.3.1/dbplus/
--rw-rw-rw-   0        0        0     9935 2023-02-23 10:19:25.000000 DBPlus-0.3.1/dbplus/Database.py
--rw-rw-rw-   0        0        0     2060 2022-07-20 14:54:35.000000 DBPlus-0.3.1/dbplus/Record.py
--rw-rw-rw-   0        0        0     6658 2022-07-19 14:42:00.000000 DBPlus-0.3.1/dbplus/RecordCollection.py
--rw-rw-rw-   0        0        0     2683 2023-02-23 10:09:03.000000 DBPlus-0.3.1/dbplus/Statement.py
--rw-rw-rw-   0        0        0      111 2023-02-23 10:56:16.000000 DBPlus-0.3.1/dbplus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-23 10:56:43.589691 DBPlus-0.3.1/dbplus/drivers/
--rw-rw-rw-   0        0        0     6242 2022-07-20 12:08:06.000000 DBPlus-0.3.1/dbplus/drivers/DB2.py
--rw-rw-rw-   0        0        0     3794 2022-12-02 15:45:48.000000 DBPlus-0.3.1/dbplus/drivers/MySQL.py
--rw-rw-rw-   0        0        0     4141 2021-06-08 14:29:09.000000 DBPlus-0.3.1/dbplus/drivers/Oracle.py
--rw-rw-rw-   0        0        0     4160 2021-06-08 14:29:09.000000 DBPlus-0.3.1/dbplus/drivers/Postgres.py
--rw-rw-rw-   0        0        0     3071 2023-02-23 10:17:33.000000 DBPlus-0.3.1/dbplus/drivers/SQLite.py
--rw-rw-rw-   0        0        0     1247 2023-02-23 10:10:01.000000 DBPlus-0.3.1/dbplus/drivers/__init__.py
--rw-rw-rw-   0        0        0     3520 2022-07-21 12:07:22.000000 DBPlus-0.3.1/dbplus/helpers.py
--rw-rw-rw-   0        0        0      878 2021-06-08 14:29:09.000000 DBPlus-0.3.1/license.txt
--rw-rw-rw-   0        0        0       42 2023-02-23 10:56:43.594662 DBPlus-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      687 2023-02-23 10:55:38.000000 DBPlus-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:04:51.171376 DBPlus-0.3.2/
+drwxrwxrwx   0        0        0        0 2023-04-26 08:04:51.120824 DBPlus-0.3.2/DBPlus.egg-info/
+-rw-rw-rw-   0        0        0     4386 2023-04-26 08:04:50.000000 DBPlus-0.3.2/DBPlus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-04-26 08:04:50.000000 DBPlus-0.3.2/DBPlus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 08:04:50.000000 DBPlus-0.3.2/DBPlus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2019-01-24 13:53:59.000000 DBPlus-0.3.2/DBPlus.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-04-26 08:04:50.000000 DBPlus-0.3.2/DBPlus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4386 2023-04-26 08:04:51.169413 DBPlus-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4061 2021-06-08 14:29:09.000000 DBPlus-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-26 08:04:51.144337 DBPlus-0.3.2/dbplus/
+-rw-rw-rw-   0        0        0    11453 2023-03-01 14:54:25.000000 DBPlus-0.3.2/dbplus/Database.py
+-rw-rw-rw-   0        0        0     4468 2023-02-28 14:44:26.000000 DBPlus-0.3.2/dbplus/QueryStore.py
+-rw-rw-rw-   0        0        0     2369 2023-02-28 14:45:00.000000 DBPlus-0.3.2/dbplus/Record.py
+-rw-rw-rw-   0        0        0     7411 2023-03-16 14:47:17.000000 DBPlus-0.3.2/dbplus/RecordCollection.py
+-rw-rw-rw-   0        0        0     3163 2023-03-01 10:19:39.000000 DBPlus-0.3.2/dbplus/Statement.py
+-rw-rw-rw-   0        0        0      153 2023-02-27 12:37:37.000000 DBPlus-0.3.2/dbplus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-26 08:04:51.166378 DBPlus-0.3.2/dbplus/drivers/
+-rw-rw-rw-   0        0        0     7692 2023-03-16 14:46:34.000000 DBPlus-0.3.2/dbplus/drivers/DB2.py
+-rw-rw-rw-   0        0        0     3865 2023-04-26 07:59:11.000000 DBPlus-0.3.2/dbplus/drivers/MySQL.py
+-rw-rw-rw-   0        0        0     4141 2021-06-08 14:29:09.000000 DBPlus-0.3.2/dbplus/drivers/Oracle.py
+-rw-rw-rw-   0        0        0     4160 2021-06-08 14:29:09.000000 DBPlus-0.3.2/dbplus/drivers/Postgres.py
+-rw-rw-rw-   0        0        0     3071 2023-02-23 10:17:33.000000 DBPlus-0.3.2/dbplus/drivers/SQLite.py
+-rw-rw-rw-   0        0        0     1247 2023-02-23 10:10:01.000000 DBPlus-0.3.2/dbplus/drivers/__init__.py
+-rw-rw-rw-   0        0        0     3520 2023-03-01 09:54:20.000000 DBPlus-0.3.2/dbplus/helpers.py
+-rw-rw-rw-   0        0        0      878 2021-06-08 14:29:09.000000 DBPlus-0.3.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 08:04:51.171376 DBPlus-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      687 2023-04-26 08:04:01.000000 DBPlus-0.3.2/setup.py
```

### Comparing `DBPlus-0.3.1/DBPlus.egg-info/PKG-INFO` & `DBPlus-0.3.2/DBPlus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBPlus
-Version: 0.3.1
+Version: 0.3.2
 Summary: Database-agnostic SQL Interface for Postresql, MySQL, SQLite, DB2 and more
 Home-page: https://github.com/klaasbrant/DBPlus
 Author: Klaas Brant
 Author-email: kbrant@kbce.com
 License: ISC
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `DBPlus-0.3.1/PKG-INFO` & `DBPlus-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DBPlus
-Version: 0.3.1
+Version: 0.3.2
 Summary: Database-agnostic SQL Interface for Postresql, MySQL, SQLite, DB2 and more
 Home-page: https://github.com/klaasbrant/DBPlus
 Author: Klaas Brant
 Author-email: kbrant@kbce.com
 License: ISC
 Description-Content-Type: text/markdown
 License-File: license.txt
```

### Comparing `DBPlus-0.3.1/README.md` & `DBPlus-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/dbplus/Database.py` & `DBPlus-0.3.2/dbplus/Database.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,137 +1,173 @@
 import logging
 import os
 import csv
 from dbplus.Record import Record
 from dbplus.RecordCollection import RecordCollection
 from dbplus.Statement import Statement
-from dbplus.helpers import _parse_database_url, guess_type, fix_sql_type, _reduce_datetimes
+from dbplus.helpers import (
+    _parse_database_url,
+    guess_type,
+    fix_sql_type,
+    _reduce_datetimes,
+)
 from contextlib import contextmanager
 from dbplus.helpers import _debug
 from importlib import import_module
 
+
 class DBError(Exception):
     pass
 
+
 class Database(object):
     """A Database connection."""
-    
+
     def __init__(self, db_url=None, **kwargs):
-        self._logger = logging.getLogger('dbplus')
+        self._logger = logging.getLogger("dbplus")
         self._transaction_active = False
-        
-        # If no db_url was provided, fallback to $DATABASE_URL in environment
-        DATABASE_URL = os.environ.get('DATABASE_URL')
-        self.db_url = db_url or DATABASE_URL
-        dbParameters = None
-        if self.db_url:
-            dbParameters =_parse_database_url(db_url)
+        # If no db_url was provided, we fallback to DATABASE_URL in environment variables
+        self.db_url = db_url or os.environ.get("DATABASE_URL")
+        dbParameters = _parse_database_url(self.db_url)
         if dbParameters == None:  # that means parsing failed!!
-            raise ValueError('Database url missing or invalid')
-        self.db_type= dbParameters.pop('driver').upper()
+            raise ValueError("Database url is missing or has invalid format")
+        self.db_type = dbParameters.pop("driver").upper()
         try:
-            if self.db_type == 'DB2':
+            if self.db_type == "DB2":
                 from dbplus.drivers import DB2
-                self._driver = DB2.DB2Driver(**dbParameters) # and of to the races with DB2!
-            elif self.db_type == 'MYSQL':
+
+                self._driver = DB2.DB2Driver(
+                    **dbParameters
+                )  # and of to the races with DB2!
+            elif self.db_type == "MYSQL":
                 from dbplus.drivers import MySQL
-                self._driver = MySQL.MySQLDriver(**dbParameters) # and of to the races with MySQL!
-            elif self.db_type == 'SQLITE':
-                from dbplus.drivers import SQLite 
-                self._driver = SQLite.SQLiteDriver(**dbParameters) # and of to the races with SQLite!            
-            elif self.db_type == 'ORACLE':
-                from dbplus.drivers import Oracle 
-                self._driver = Oracle.OracleDriver(**dbParameters) # and of to the races with Oracle!   
-            elif self.db_type == 'POSTGRES':
-                from dbplus.drivers import Postgres 
-                self._driver = Postgres.PostgresDriver(**dbParameters) # and of to the races with Oracle!                      
-            else: # add new drivers here
-                raise ValueError('DBPlus has no driver for: {}'.format(self.db_type))
-       
-            self._logger.info("--> Using Database driver: {}".format(self.db_type))
-            if kwargs.pop('open',True):
+
+                self._driver = MySQL.MySQLDriver(
+                    **dbParameters
+                )  # and of to the races with MySQL!
+            elif self.db_type == "SQLITE":
+                from dbplus.drivers import SQLite
+
+                self._driver = SQLite.SQLiteDriver(
+                    **dbParameters
+                )  # and of to the races with SQLite!
+            elif self.db_type == "ORACLE":
+                from dbplus.drivers import Oracle
+
+                self._driver = Oracle.OracleDriver(
+                    **dbParameters
+                )  # and of to the races with Oracle!
+            elif self.db_type == "POSTGRES":
+                from dbplus.drivers import Postgres
+
+                self._driver = Postgres.PostgresDriver(
+                    **dbParameters
+                )  # and of to the races with Oracle!
+            else:  # add new drivers here
+                raise ValueError(f"DBPlus has no driver for: {self.db_type}")
+
+            self._logger.info("--> Using Database driver: {self.db_type}")
+            if kwargs.pop("open", True):
                 self.open()
                 if not self.is_connected():
-                    raise ValueError('DBPlus cannot establish database connection')
-        except:   
-            raise ValueError('DBPlus has trouble initializing the {} driver... mission aborted!'.format(self.db_type.lower())) 
+                    raise ValueError("DBPlus cannot establish database connection")
+        except:
+            raise ValueError(
+                f"DBPlus has trouble initializing the {self.db_type.lower()} driver... mission aborted!"
+            )
 
     def open(self):
         """Opens the connection to the Database."""
         if not self.is_connected():
             self._driver.connect()
 
     def close(self):
         """Closes the connection to the Database."""
         if self.is_connected():
             self._driver.close()
 
     def __del__(self):
         if hasattr(self, "_driver"):
-            #self._driver.close() # Say goodbye and
-            del self._driver     # allow database interface to gracefully exit
+            # self._driver.close() # Say goodbye and
+            del self._driver  # allow database interface to gracefully exit
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc, val, traceback):
         self.close()
 
     def __repr__(self):
-        return '<DBPlus {} database (url: {}), state: connected={}>'.format(self.db_type,self.db_url,self.is_connected())
-    
+        return f"<DBPlus {self.db_type} database url: {self.db_url}), state: connected={self.is_connected()}>"
+
     ################# Experimental feature, driver might offer extra options ############################
     def __getattr__(self, name):
         def method(*args, **kw):
             if hasattr(self._driver, name) and callable(getattr(self._driver, name)):
-                return getattr(self._driver,name)(*args,**kw)
+                return getattr(self._driver, name)(*args, **kw)
+
         return method
 
     def get_driver(self):
         return self._driver
 
     def is_connected(self):
         return self._driver.is_connected()
 
     def ensure_connected(self):
         if not self.is_connected():
             self.open()
 
     #########################################################################################################################
 
-    #def query(self, query, fetchall=False,*args, **kwargs):
+    # def query(self, query, fetchall=False,*args, **kwargs):
     def query(self, query, *args, **kwargs):
         """Executes the given SQL query against the Database. Parameters
         can, optionally, be provided. Returns a RecordCollection, which can be
         iterated over to get result rows as dictionaries.
         """
         self.ensure_connected()
-        cursor=Statement(self)
+        cursor = Statement(self)
         cursor.execute(query, *args, **kwargs)
 
         # Turn the cursor into RecordCollection
         rows = (Record(row) for row in cursor)
-        results = RecordCollection(rows,cursor)
+        results = RecordCollection(rows, cursor)
 
         # Fetch all results if desired otherwise we fetch when needed (open cursor can be locking problem!
-        #if fetchall:
+        # if fetchall:
         #    results.all()
-
+        # do not delete de cursor it is needed in the layer below
         return results
 
+
+    #########################################################################################################################
+
     def execute(self, sql, *args, **kwargs):
-        self._logger.info("--> Execute: {} with arguments [{}]".format(sql,str(args)))
+        self._logger.info(f"--> Execute: {sql} with arguments [{str(args)}]")
         self.ensure_connected()
-        modified = Statement(self).execute(sql, *args, **kwargs)
+        modified = Statement(self).execute(sql, *args, **kwargs) # GC will purge Statement
         return modified
 
+    #########################################################################################################################
+
     def callproc(self, procname, *params):
-        self._logger.info("--> Calling Stored proc: {} with arguments [{}]".format(procname,str(params)))
+        self._logger.info(
+            f"--> Calling Stored proc: {procname} with arguments [{str(params)}]"
+        )
         self.ensure_connected()
-        return self._driver.callproc(procname, *params)
+        result = self._driver.callproc(procname, *params)
+        if result:
+            cursor = Statement(self)
+            cursor._cursor = result[0]
+            rows = (Record(row) for row in cursor)
+            return (RecordCollection(rows, cursor), result[1:]) #  replace stmt by recordcollection
+        return None  # can happen like proc not found or no parameter proc that returns nothing (bad practice)
+
+    #########################################################################################################################
 
     def last_insert_id(self, seq_name=None):
         self.ensure_connected()
         return self._driver.last_insert_id(seq_name)
 
     def error_code(self):
         self.ensure_connected()
@@ -156,85 +192,118 @@
             self._logger.info("--> Transaction rollback because failure in transaction")
             self.rollback()
             raise ex
 
     def begin_transaction(self):
         self.ensure_connected()
         if self._transaction_active == True:
-            raise DBError('Nested transactions is not supported!')
+            raise DBError("Nested transactions is not supported!")
         self._transaction_active = True
         self._driver.begin_transaction()
 
     def commit(self):
         if self._transaction_active == False:
-            raise DBError('Commit on never started transaction?')
+            raise DBError("Commit on never started transaction?")
         self.ensure_connected()
         self._driver.commit()
         self._transaction_active = False
 
     def rollback(self):
         if self._transaction_active == False:
-            raise DBError('Rollback on never started transaction?')
+            raise DBError("Rollback on never started transaction?")
         self.ensure_connected()
         self._transaction_active = False
         self._driver.rollback()
 
     def is_transaction_active(self):
         return self._transaction_active
 
     #########################################################################################################################
 
-
-    def copy_to(self,file,table,sep='\t',null="\\x00",columns=None,header=False,append=False,recsep='\n',**kwargs):
-        col="*" if columns==None else ",".join(columns)
-        sql_query="select {} from {}".format(col,table)
-        cursor=Statement(self)
+    def copy_to(
+        self,
+        file,
+        table,
+        sep="\t",
+        null="\\x00",
+        columns=None,
+        header=False,
+        append=False,
+        recsep="\n",
+        **kwargs,
+    ):
+        col = "*" if columns == None else ",".join(columns)
+        sql_query = "select {} from {}".format(col, table)
+        cursor = Statement(self)
         cursor.execute(sql_query)
         row_count = 0
-        mode = 'a' if append else 'w'
+        mode = "a" if append else "w"
         with open(file, mode) as csvfile:
             for row in cursor:
                 row_count += 1
                 if row_count == 1:
-                    csv_columns=row.keys()
-                    #csv_columns = [each_column_name.upper() for each_column_name in csv_columns]
-                    writer = csv.DictWriter(csvfile,fieldnames=csv_columns,lineterminator=recsep,restval='',delimiter=sep,quoting=csv.QUOTE_MINIMAL,**kwargs)
+                    csv_columns = row.keys()
+                    # csv_columns = [each_column_name.upper() for each_column_name in csv_columns]
+                    writer = csv.DictWriter(
+                        csvfile,
+                        fieldnames=csv_columns,
+                        lineterminator=recsep,
+                        restval="",
+                        delimiter=sep,
+                        quoting=csv.QUOTE_MINIMAL,
+                        **kwargs,
+                    )
                     if header:
                         writer.writeheader()
 
                 for key in row.keys():
-                    if row[key]==None:
-                        row[key]=null
+                    if row[key] == None:
+                        row[key] = null
                 writer.writerow(row)
         return row_count
-                
-    def copy_from(self,file, table, sep='\t',recsep='\n',header=False, null="\\x00", batch=500, columns=None, **kwargs):
-        col="" if columns==None else "({})".format(",".join(columns))
+
+    def copy_from(
+        self,
+        file,
+        table,
+        sep="\t",
+        recsep="\n",
+        header=False,
+        null="\\x00",
+        batch=500,
+        columns=None,
+        **kwargs,
+    ):
+        col = "" if columns == None else "({})".format(",".join(columns))
         row_count = 0
         queue = list()
-        #values = list()
-        with open(file, 'r') as csvfile:
-            reader=csv.reader(csvfile,delimiter=sep,lineterminator=recsep,quoting=csv.QUOTE_MINIMAL,**kwargs)
+        # values = list()
+        with open(file, "r") as csvfile:
+            reader = csv.reader(
+                csvfile,
+                delimiter=sep,
+                lineterminator=recsep,
+                quoting=csv.QUOTE_MINIMAL,
+                **kwargs,
+            )
             if header:
                 xh = next(reader)
-                #print(f'Header: {", ".join(xh)}')
+                # print(f'Header: {", ".join(xh)}')
             for row in reader:
                 row_count += 1
                 values = tuple(None if x == null else x for x in row)
                 queue.append(values)
                 if len(queue) >= batch:
-                    self._insert_values(table,col,queue)
+                    self._insert_values(table, col, queue)
                     queue = list()
             if len(queue) > 0:
-                self._insert_values(table,col,queue)
+                self._insert_values(table, col, queue)
         return row_count
 
-    def _insert_values(self,table,col,queue):
-        values_literal= "({})".format(",".join([self.get_driver().get_placeholder()] * len(queue[0])))
-        sql_query="insert into {} {} values {}".format(table,col,values_literal)
-        self.get_driver().execute_many(self,sql_query,queue)
-
+    def _insert_values(self, table, col, queue):
+        values_literal = "({})".format(
+            ",".join([self.get_driver().get_placeholder()] * len(queue[0]))
+        )
+        sql_query = "insert into {} {} values {}".format(table, col, values_literal)
+        self.get_driver().execute_many(self, sql_query, queue)
 
     #########################################################################################################################
-
-
-
```

### Comparing `DBPlus-0.3.1/dbplus/Record.py` & `DBPlus-0.3.2/dbplus/Record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import json
+import inspect
 from dbplus.helpers import json_handler
 
+
 class Record(object):
     """A row, from a query, from a database."""
-    __slots__ = ('_keys', '_values')
+
+    __slots__ = ("_keys", "_values")
 
     def __init__(self, row):
         self._keys = list(row.keys())
         self._values = list(row.values())
-
         # Ensure that lengths match properly.
         assert len(self._keys) == len(self._values)
 
     def keys(self):
         """Returns the list of column names from the query."""
         return self._keys
 
     def values(self):
         """Returns the list of values from the query."""
         return self._values
 
     def __repr__(self):
-        return f'<Record {format(json.dumps(self.as_dict(),default=json_handler))}>'
+        return f"<Record {format(json.dumps(self.as_dict(),default=json_handler))}>"
 
     def __getitem__(self, key):
         # Support for index-based lookup.
         if isinstance(key, int):
             return self.values()[key]
 
         # Support for string-based lookup.
         if key in self.keys():
             i = self.keys().index(key)
             return self.values()[i]
 
-        raise KeyError("Record contains no '{}' field.".format(key))
+        raise KeyError(f"Record does not contains '{key}' field.")
 
     def __getattr__(self, key):
         try:
             return self[key]
         except KeyError as e:
             raise AttributeError(e)
 
@@ -57,13 +59,21 @@
         """Returns the row as a dictionary, as ordered."""
         items = zip(self.keys(), self.values())
 
         return dict(items)
 
     def as_tuple(self):
         return tuple(self.values())
-    
+
     def as_list(self):
         return list(self.values())
-    
+
     def as_json(self):
-        return json.dumps(self.as_dict(),indent=4, sort_keys=True, default=str)
+        return json.dumps(self.as_dict(), indent=4, sort_keys=True, default=str)
+
+    def as_model(self, model):
+        """return the row as pydantic model"""
+        if inspect.isclass(model):
+            # return model.parse_obj(self.as_dict())
+            return model(**self.as_dict())
+        else:
+            raise ValueError("as_model excepts a class as input")
```

### Comparing `DBPlus-0.3.1/dbplus/RecordCollection.py` & `DBPlus-0.3.2/dbplus/RecordCollection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,46 @@
+from dbplus.Statement import Statement
 from dbplus.helpers import _reduce_datetimes
+import inspect
 from dbplus.Record import Record
+import logging
+from dbplus.helpers import _debug
+
 
 class RecordCollection(object):
     """A set of excellent rows from a query."""
+
     def __init__(self, rows, cursor):
         self._rows = rows
         self._all_rows = []
         self.pending = True
-        self._cursor=cursor
+        self._cursor = cursor
+        self._logger = logging.getLogger("RecordCollection")
 
     def __repr__(self):
-        return '<RecordCollection size={} pending={}>'.format(len(self), self.pending)
+        return "<RecordCollection size={} pending={}>".format(len(self), self.pending)
 
     def __str__(self):
         return self.__unicode__()
 
+    @_debug()
     def __unicode__(self):
-        result=[]
+        result = []
         data = self.all(as_tuple=True)
         if len(self) > 0:
             headers = self[0].as_dict()
             result.append([str(h) for h in headers.keys()])
             result.extend(list(map(str, row)) for row in data)
             lens = [list(map(len, row)) for row in result]
             field_lens = list(map(max, zip(*lens)))
-            result.insert(1, ['-' * length for length in field_lens])
-            format_string = '|'.join('{%s:%s}' % item for item in enumerate(field_lens))
-            return '\n'.join(format_string.format(*row) for row in result)
+            result.insert(1, ["-" * length for length in field_lens])
+            format_string = "|".join("{%s:%s}" % item for item in enumerate(field_lens))
+            return "\n".join(format_string.format(*row) for row in result)
         else:
-            return '\n' #empty set, nothing to report
+            return "\n"  # empty set, nothing to report
 
     def __iter__(self):
         """Iterate over all rows, consuming the underlying generator
         only when necessary."""
         i = 0
         while True:
             # Other code may have iterated between yields,
@@ -49,141 +57,157 @@
             i += 1
 
     def next(self):
         return self.__next__()
 
     def __next__(self):
         try:
-            #print("===== in next ====")
+            #self._logger.debug("===== in next ====")
             nextrow = next(self._rows)
-            #print("======= out next: row ===>",nextrow)
+            #self._logger.debug("======= out next: row ===>",nextrow)
             self._all_rows.append(nextrow)
             return nextrow
         except StopIteration:
             self.pending = False
-            #print("==== EOF ===")
-            raise StopIteration('RecordCollection contains no more rows.')
+            #self._logger.debug("==== EOF ===")
+            raise StopIteration("RecordCollection contains no more rows.")
 
     def __getitem__(self, key):
         """
         Argument: index or slice
         """
         # Verify what we are dealing with
         if isinstance(key, int):
             start = key
-            stop = key+1
+            stop = key + 1
         else:
-            if isinstance( key, slice ):
-                start=key.start
-                if start is None: # used [:x] ?
+            if isinstance(key, slice):
+                start = key.start
+                if start is None:  # used [:x] ?
                     start = 0
-                stop=key.stop
+                stop = key.stop
             else:
                 raise TypeError("Invalid argument type")
 
         # do we need to fetch extra to complete ?
         if self.pending == True:
-            if start < 0 or stop is None: # we must fetch all to evaluate
-                fetcher=-1 # get it all
+            if start < 0 or stop is None:  # we must fetch all to evaluate
+                fetcher = -1  # get it all
             else:
-                fetcher=stop+1 # stop premature (maybe)
-            while fetcher == -1 or fetcher > len(self):  #do it
+                fetcher = stop + 1  # stop premature (maybe)
+            while fetcher == -1 or fetcher > len(self):  # do it
                 try:
                     next(self)
                 except StopIteration:
                     break
 
-        if isinstance( key, slice ) :
-            return RecordCollection(iter(self._all_rows[key]),None)
+        if isinstance(key, slice):
+            return RecordCollection(iter(self._all_rows[key]), None)
         else:
-            if key < 0 : #Handle negative indices
+            if key < 0:  # Handle negative indices
                 key += len(self)
-            if key >= len(self) :
+            if key >= len(self):
                 raise IndexError("Recordcollection index out of range")
-            return self._all_rows[key] 
+            return self._all_rows[key]
 
     def __len__(self):
         return len(self._all_rows)
 
     def __del__(self):
-        self.close()
-    
+        pass
+        #self.close()
+
     def close(self):
-        if self._cursor and self.pending:  #if we have a cursor and cursor is not yet auto closed
+        if (
+            self._cursor and self.pending
+        ):  # if we have a cursor and cursor is not yet auto closed
             self._cursor.close()
 
-    def next_result(self,fetchall=False):
+    def next_result(self, fetchall=False):
+        self._logger.info(f"Resolving next_result {self._cursor}")
         if self._cursor:
-            new_cursor = self._cursor.next_result()  #TODO check if pending if so raise error current cursor is lost...
+            cursor = Statement(self._cursor._connection)
+            next_rs = self._cursor.next_result()  # this the old stmt
+            self._logger.info(f"got new rs from driver {next_rs}")
+            cursor._cursor = next_rs
             # Turn the cursor into RecordCollection
-            rows = (Record(row) for row in new_cursor)
-            results = RecordCollection(rows,new_cursor)
-        
+            rows = (Record(row) for row in cursor)
+            results = RecordCollection(rows, cursor)
             # Fetch all results if desired otherwise we fetch when needed (open cursor can be locking problem!
             if fetchall:
                 results.all()
-
             return results
 
-
     def export(self, format, **kwargs):
         pass
 
     def as_DataFrame(self):
         """A DataFrame representation of the RecordCollection."""
         try:
             from pandas import DataFrame
         except ImportError:
-            raise NotImplementedError("DataFrame needs Pandas... try pip install pandas")
+            raise NotImplementedError(
+                "DataFrame needs Pandas... try pip install pandas"
+            )
         return DataFrame(data=self.all(as_dict=True))
 
     def all(self, as_dict=False, as_tuple=False):
         """Returns a list of all rows for the RecordCollection. If they haven't
         been fetched yet, consume the iterator and cache the results."""
 
         # By calling list it calls the __iter__ method
         rows = list(self)
 
         if as_dict:
             return [r.as_dict() for r in rows]
         elif as_tuple:
-            return [r.as_tuple() for r in rows]    
+            return [r.as_tuple() for r in rows]
 
         return rows  # list of records
 
+    def as_model(self, model):
+        """return an array of pydantic models"""
+        if inspect.isclass(model):
+            rows = list(self)
+            return [r.as_model(model) for r in rows]
+        else:
+            raise ValueError("as_model excepts a class as input")
+
     def as_dict(self):
         return self.all(as_dict=True)
 
     def as_tuple(self):
         return self.all(as_tuple=True)
 
     def one(self, default=None, as_dict=False, as_tuple=False):
         """Returns a single record for the RecordCollection, ensuring that it
-        is the only record, or returns `default`. """
-        
+        is the only record, or returns `default`."""
+
         # Ensure that we don't have more than one row.
         try:
-            test = self[1] # force the cursor to the second rowpass
+            test = self[1]  # force the cursor to the second rowpass
         except:
             pass
-        
+
         if len(self) > 1:
-            raise ValueError('RecordCollection contained more than one row. '
-                             'Expects only one row when using '
-                             'RecordCollection.one')
+            raise ValueError(
+                "RecordCollection contained more than one row. "
+                "Expects only one row when using "
+                "RecordCollection.one"
+            )
 
         # Try to get a record, or return default.
-        if len(self) == 0: # bummer, no rows at all
+        if len(self) == 0:  # bummer, no rows at all
             return default
         record = self[0]
         # Cast and return.
         if as_dict:
             return record.as_dict()
         elif as_tuple:
             return record.as_tuple()
         else:
             return record
 
     def scalar(self, default=None):
         """Returns the first column of the first row, or `default`."""
         row = self.one()
-        return row[0] if row else default
+        return row[0] if row else default
```

### Comparing `DBPlus-0.3.1/dbplus/Statement.py` & `DBPlus-0.3.2/dbplus/Statement.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,91 @@
 import re
 import logging
+from dbplus.QueryStore import Query
 from dbplus.helpers import _debug
 
+
 class Statement:
     _cursor = None
-    
+
     _re_params = re.compile(
-        r"(\?|(?<!:):[a-zA-Z_][a-zA-Z0-9_]*)(?=(?:(?:\\.|[^'\"\\])*['\"](?:\\.|[^'\"\\])*['\"])*(?:\\.|[^'\"\\])*\Z)")
+        r"(\?|(?<!:):[a-zA-Z_][a-zA-Z0-9_]*)(?=(?:(?:\\.|[^'\"\\])*['\"](?:\\.|[^'\"\\])*['\"])*(?:\\.|[^'\"\\])*\Z)"
+    )
 
     def __init__(self, database):
         self._connection = database
-        #self._object_name = database._driver.get_name()+'Row'
-        self._logger = logging.getLogger('dbplus')
+        # self._object_name = database._driver.get_name()+'Row'
+        self._logger = logging.getLogger("Statement")
+        self._cursor = None
+        self._next = None
 
     def __iter__(self):
         return self.iterate()
+    
+    def __repr__(self):
+        return f"<Statement {self._connection=} {self._cursor=} {self._next=} >"
 
     def close(self):
         if self._cursor is not None:
             self._connection.get_driver().clear(self)
 
     def iterate(self):
-        #Driver iterate will return a row as dict
+        # Driver iterate will return a row as dict
         for row in self._connection.get_driver().iterate(self):
             yield row
 
     def execute(self, sql, *args, **kwargs):
-        self._logger.info("--> Execute : {} / {} / {}".format(sql,args,kwargs))
+        if isinstance(sql, Query):
+            sql = sql.sql
+        self._logger.info(f"--> Execute : {sql} :: {args=}, {kwargs=}")
 
         if self._connection.get_driver().get_placeholder() == ":":
             return self._connection.get_driver().execute(self, sql, **kwargs)
 
         for i, arg in enumerate(args):
             if type(arg) is dict:
                 kwargs.update(arg)
             else:
                 kwargs[i] = arg
-        self._logger.info("--> Execute arg : {} ".format(kwargs))    
+        self._logger.info(f"--> Merged args :: {kwargs} ")
         params = []
         sql = Statement._re_params.sub(self._prepare(kwargs, params), sql)
-        self._logger.info("--> Query: {} {}".format(sql,params))
+        self._logger.info(f"--> Formatted Query: {sql} {params}")
         return self._connection.get_driver().execute(self, sql, *params)
 
     def next_result(self):
-        self._connection.get_driver().next_result(self)
+        self._logger.info(f"--> next result {self}")
+        stmt = self._connection.get_driver().next_result(self)
+        self._logger.info(f"--> next result returns {self}")
+        return stmt
 
     def _prepare(self, params, exec_params):
         def replace(match):
             key = match.group()
             if key == "?":
                 key = replace._param_counter
                 replace._param_counter += 1
             else:
                 key = key.lstrip(":")
 
             if key not in params:
                 if isinstance(key, int):
-                    raise LookupError("SQL Positional parameter with index #{} not found in arguments: {}".format(key, params))
+                    raise LookupError(
+                        f"SQL Positional parameter with index #{key} not found in arguments: {params}"
+                    )
                 else:
-                    raise LookupError("SQL Named parameter :{} not found in arguments: {}".format(key, params))
+                    raise LookupError(
+                        f"SQL Named parameter :{key} not found in arguments: {params}"
+                    )
 
             param = params[key]
 
             if isinstance(param, (list, tuple)):
                 exec_params.extend(param)
                 return ", ".join((replace._placeholder,) * len(param))
 
             exec_params.append(param)
             return replace._placeholder
 
         replace._placeholder = self._connection.get_driver().get_placeholder()
         replace._param_counter = 0
-
-        return replace
+        return replace
```

### Comparing `DBPlus-0.3.1/dbplus/drivers/DB2.py` & `DBPlus-0.3.2/dbplus/drivers/DB2.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,130 +3,172 @@
 from dbplus.Statement import Statement
 from dbplus.drivers import BaseDriver
 from dbplus.helpers import _debug
 from dbplus.Record import Record
 from dbplus.Database import DBError
 from dbplus.RecordCollection import RecordCollection
 
+
 class DB2Driver(BaseDriver):
     @_debug()
     def __init__(self, **params):
-    # timeout=5, charset="utf8"
+        # timeout=5, charset="utf8"
         self._driver = "DB2"
-        self._params = params    
-        self._logger = logging.getLogger('dbplus')
+        self._params = params
+        self._logger = logging.getLogger("dbplus")
 
-        self._database = self._params.pop("database",None)
+        self._database = self._params.pop("database", None)
         if self._database is None:
-            raise DBError("Database name missing or incorrect")            
-        
-        self._uid = self._params.pop("uid",None)
-        self._pwd = self._params.pop("pwd",None)
-        
-        self._host = self._params.pop("host",None)
-        if self._host and self._host.upper() == 'LOCALHOST':
+            raise DBError("Database name missing or incorrect")
+
+        self._uid = self._params.pop("uid", None)
+        self._pwd = self._params.pop("pwd", None)
+
+        self._host = self._params.pop("host", None)
+        if self._host and self._host.upper() == "LOCALHOST":
             self._host = None
-        self._port = self._params.pop("port",None)
+        self._port = self._params.pop("port", None)
         if self._port is None:
             self._port = 50000
 
         if self._host and ((self._uid is None) or (self._pwd is None)):
             raise DBError("Userid and/or Password missing")
 
         if self._host:
-            conn_string='DATABASE={};UID={};PWD={};HOSTNAME={};PORT={};PROTOCOL=TCPIP;'.format(self._database,self._uid,self._pwd,self._host,self._port)
+            conn_string = (
+                "DATABASE={};UID={};PWD={};HOSTNAME={};PORT={};PROTOCOL=TCPIP;".format(
+                    self._database, self._uid, self._pwd, self._host, self._port
+                )
+            )
         else:
             if not self._uid:
-                self._uid=''
-                self._pwd=''
-            conn_string='DSN={};UID={};PWD={};'.format(self._database,self._uid,self._pwd)
-        
+                self._uid = ""
+                self._pwd = ""
+            conn_string = "DSN={};UID={};PWD={};".format(
+                self._database, self._uid, self._pwd
+            )
+
         self._conn_string = conn_string
 
     @_debug()
     def connect(self):
-        options = { ibm_db.ATTR_CASE : ibm_db.CASE_LOWER,ibm_db.SQL_ATTR_AUTOCOMMIT : ibm_db.SQL_AUTOCOMMIT_ON}
-        self._logger.info("--> PCONNECT {} - {}".format(self._conn_string,options))
+        options = {
+            ibm_db.ATTR_CASE: ibm_db.CASE_LOWER,
+            ibm_db.SQL_ATTR_AUTOCOMMIT: ibm_db.SQL_AUTOCOMMIT_ON,
+        }
+        self._logger.info("--> PCONNECT {} - {}".format(self._conn_string, options))
         try:
-            self._conn = ibm_db.pconnect(self._conn_string, "", "",options)
+            self._conn = ibm_db.pconnect(self._conn_string, "", "", options)
         except Exception as ex:
             self._error = ibm_db.conn_errormsg()
-            raise DBError('Problem connection to database {} : {}'.format(self._database,ex))
-    
+            raise DBError(
+                "Problem connection to database {} : {}".format(self._database, ex)
+            )
+
     @_debug()
     def close(self):
         if self._conn is not None:
             ibm_db.close(self._conn)
             self._conn = None
-    
+
     @_debug()
     def error_code(self):
         return ibm_db.stmt_error()
 
     @_debug()
     def error_info(self):
         return ibm_db.stmt_errormsg()
 
     @_debug()
     def callproc(self, procname, *params):
         try:
+            result = None
             result = ibm_db.callproc(self._conn, procname, tuple(*params))
-            return list(result[1:])
+            self._logger.debug(f"call proc {procname} returned {result}")
+            # WTF IBM!! a method should not bring back different types!!
+            if type(result) is tuple:
+                return result
+            else:
+                return (result,)  # then make it a tuple!!
         except Exception as ex:
             self._error = ibm_db.stmt_errormsg()
-            raise DBError("Error calling stored proc: {}, with parameters: {} : {}".format(procname, params,ex))
+            raise DBError(
+                "Error calling stored proc: {}, with parameters: {} : {}".format(
+                    procname, params, ex
+                )
+            )
 
     @_debug()
     def execute(self, Statement, sql, *params):
         try:
             stmt = ibm_db.prepare(self._conn, sql)
             ibm_db.execute(stmt, params)
             Statement._cursor = stmt
+            Statement._next = stmt
             return ibm_db.num_rows(stmt)
         except Exception as ex:
             self._error = ibm_db.stmt_errormsg()
-            raise DBError("Error executing SQL: {}, with parameters: {} : {}".format(sql, params,ex))
+            raise DBError(
+                "Error executing SQL: {}, with parameters: {} : {}".format(
+                    sql, params, ex
+                )
+            )
 
     @_debug()
-    def execute_many(self,Statement, sql, params):
+    def execute_many(self, Statement, sql, params):
         try:
             stmt = ibm_db.prepare(self._conn, str(sql))
             ibm_db.execute_many(stmt, tuple(params))
             Statement._cursor = stmt
             return ibm_db.num_rows(stmt)
         except Exception as ex:
             self._error = ibm_db.stmt_errormsg()
-            raise DBError("Error executing SQL: {}, with parameters: {} : {}".format(sql, params,ex))
+            raise DBError(
+                "Error executing SQL: {}, with parameters: {} : {}".format(
+                    sql, params, ex
+                )
+            )
 
     @_debug()
     def iterate(self, Statement):
-        if Statement._cursor is None:
-            raise StopIteration
-        row = ibm_db.fetch_assoc(Statement._cursor)
-        while (row):
-            yield row
+        try:
+            if Statement._cursor is None:
+                raise StopIteration
+            #self._logger.debug(f" >>>>>>>>   About to fetch 1st {Statement}")
             row = ibm_db.fetch_assoc(Statement._cursor)
-        ibm_db.free_result(Statement._cursor)
-        Statement._cursor = None
+            while row:
+                yield row
+                row = ibm_db.fetch_assoc(Statement._cursor)
+            Statement._next = Statement._cursor  # save for possible next
+            #ibm_db.free_result(Statement._cursor)
+            Statement._cursor = None
+        except Exception as ex:
+            self._error = ibm_db.stmt_errormsg()
+            raise DBError(f"Error in iterate cursor statement {Statement} : {ibm_db.stmt_errormsg()} : {ex}")
 
     @_debug()
-    def clear(self,Statement):
-        if Statement._cursor is not None:
-            pass
-            #ibm_db.free_result(Statement._cursor)
-            #Statement._cursor = None
+    def clear(self, Statement):
+        # ibm_db.free_result(Statement._cursor)
+        Statement._cursor = None
 
     @_debug()
-    def next_result(self,cursor):
-        return ibm_db.next_result(cursor)
+    def next_result(self, Statement):
+        try:
+            #self._logger.debug(f"we had a stement {Statement}, with _cursor {Statement._cursor} and _next {Statement._next}")
+            nresult = None
+            nresult = ibm_db.next_result(Statement._next)
+            return nresult
+        except Exception as ex:
+            self._error = ibm_db.stmt_errormsg()
+            raise DBError(f"Error executing next_result: {self._error}")
 
     @_debug()
     def last_insert_id(self, seq_name=None):
         # Code like in ibm_dbi
-        operation = 'values(IDENTITY_VAL_LOCAL()) FROM SYSIBM.SYSDUMMY1'
+        operation = "values(IDENTITY_VAL_LOCAL()) FROM SYSIBM.SYSDUMMY1"
         try:
             stmt_handler = ibm_db.prepare(self._conn, operation)
             ibm_db.execute(stmt_handler)
             row = ibm_db.fetch_tuple(stmt_handler)
             if row[0] is not None:
                 identity_val = int(row[0])
             else:
@@ -156,16 +198,20 @@
     @_debug()
     def get_placeholder(self):
         return "?"
 
     @_debug()
     def get_name(self):
         return self._driver
-    
-    def columns(self,qualifier,schema,table_name,column_name):
-        stmt = Statement(self) # fake a statement in order to supply a generator / cursor
-        stmt._cursor = ibm_db.columns(self._conn,qualifier,schema,table_name,column_name) 
-        rows = (Record(row) for row in stmt) # create the generator
-        return RecordCollection(rows,stmt) # make a record collection
-    
+
+    def columns(self, qualifier, schema, table_name, column_name):
+        stmt = Statement(
+            self
+        )  # fake a statement in order to supply a generator / cursor
+        stmt._cursor = ibm_db.columns(
+            self._conn, qualifier, schema, table_name, column_name
+        )
+        rows = (Record(row) for row in stmt)  # create the generator
+        return RecordCollection(rows, stmt)  # make a record collection
+
     def get_driver(self):  # needed for the extra methods in order to close the cursor
         return self
```

### Comparing `DBPlus-0.3.1/dbplus/drivers/MySQL.py` & `DBPlus-0.3.2/dbplus/drivers/MySQL.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     def __init__(self, timeout=0, charset="utf8", timezone="SYSTEM", port=3306, **params):
         #self._params = dict(charset=charset, time_zone = timezone, connect_timeout=timeout, autocommit=True)
         #print('>>>',params)
         self._params = dict()
         self._params["user"] = params.pop('uid')
         self._params["password"] = params.pop('pwd')
         self._params["database"] = params.pop('database')
-        self._params["host"] = params.pop('host')
-        self._params["port"] = int(params.pop('port'))
+        self._params["host"] = params.pop('host','localhost')
+        self._port = self._params.pop("port",None)
+        if self._port is None:
+            self._port = 3306
 
     def _get_server_version_info(self):
         return getattr(self._conn, "_server_version", None)
 
     def get_database(self):
         if "database" in self._params:
             return self._params["db"]
```

### Comparing `DBPlus-0.3.1/dbplus/drivers/Oracle.py` & `DBPlus-0.3.2/dbplus/drivers/Oracle.py`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/dbplus/drivers/Postgres.py` & `DBPlus-0.3.2/dbplus/drivers/Postgres.py`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/dbplus/drivers/SQLite.py` & `DBPlus-0.3.2/dbplus/drivers/SQLite.py`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/dbplus/drivers/__init__.py` & `DBPlus-0.3.2/dbplus/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/dbplus/helpers.py` & `DBPlus-0.3.2/dbplus/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,119 +1,138 @@
 from inspect import isclass
 import decimal
 import sys
 import logging
 import time
 import datetime
-import ast 
+import ast
+
 
 def isexception(obj):
     """Given an object, return a boolean indicating whether it is an instance
     or subclass of :py:class:`Exception`.
     """
     if isinstance(obj, Exception):
         return True
     if isclass(obj) and issubclass(obj, Exception):
         return True
     return False
 
+
 def guess_type(x):
     # This function guesses the input and returns that type
-    attempt_fns = [ ast.literal_eval,
-                    lambda x: datetime.datetime.strptime(x,"%Y-%m-%d"),
-                    lambda x: datetime.datetime.strptime(x,"%Y-%m-%d %H:%M:%S"),
-                   int, 
-                   float
-                   ]
+    attempt_fns = [
+        ast.literal_eval,
+        lambda x: datetime.datetime.strptime(x, "%Y-%m-%d"),
+        lambda x: datetime.datetime.strptime(x, "%Y-%m-%d %H:%M:%S"),
+        int,
+        float,
+    ]
     for fn in attempt_fns:
         try:
             return fn(x)
         except (ValueError, SyntaxError):
             pass
-    return x # not a string, number or date? Just return input
+    return x  # not a string, number or date? Just return input
 
-def fix_sql_type(x,null):
-    x=null if x == null else x
+
+def fix_sql_type(x, null):
+    x = null if x == null else x
     return x
 
+
 def is_number(s):
     try:
         float(s)
         return True
     except ValueError:
         return False
 
+
 def _reduce_datetimes(row):
     """Receives a row, converts datetimes to strings."""
 
     row = list(row)
 
     for i in range(len(row)):
-        if hasattr(row[i], 'isoformat'):
+        if hasattr(row[i], "isoformat"):
             row[i] = row[i].isoformat()
     return tuple(row)
 
+
 def json_handler(obj):
     if isinstance(obj, decimal.Decimal):
         return str(obj)
-    elif hasattr(obj, 'isoformat'):
+    elif hasattr(obj, "isoformat"):
         return obj.isoformat()
     else:
         return obj
     # return obj.isoformat() if hasattr(obj, 'isoformat') else obj
 
+
 # Parsing code is simplified version from SQLAlchemy
 
+
 def _parse_database_url(name):
     import re
-    pattern = re.compile(r'''
+
+    pattern = re.compile(
+        r"""
             (?P<driver>[\w\+]+)://
             (?:
                 (?P<uid>[^:/]*)
                 (?::(?P<pwd>.*))?
             @)?
             (?:
                 (?:
                     \[(?P<ipv6host>[^/]+)\] |
                     (?P<ipv4host>[^/:]+)
                 )?
                 (?::(?P<port>[^/]*))?
             )?
             (?:/(?P<database>.*))?
-            ''', re.X)
+            """,
+        re.X,
+    )
 
     m = pattern.match(name)
     if m is not None:
         components = m.groupdict()
-        if components['database'] is not None:
-            tokens = components['database'].split('?', 2)
-            components['database'] = tokens[0]
-            #todo parse parameters from ?x=;y=
-        ipv4host = components.pop('ipv4host')
-        ipv6host = components.pop('ipv6host')
-        components['host'] = ipv4host or ipv6host
+        if components["database"] is not None:
+            tokens = components["database"].split("?", 2)
+            components["database"] = tokens[0]
+            # todo parse parameters from ?x=;y=
+        ipv4host = components.pop("ipv4host")
+        ipv6host = components.pop("ipv6host")
+        components["host"] = ipv4host or ipv6host
         return components
     else:
         return None
 
+
 # @debug only works in python3 using __qualname__
 def debug(loggername):
     logger = logging.getLogger(loggername)
+
     def log_():
         def wrapper(f):
             def wrapped(*args, **kargs):
-                if (sys.version_info > (3, 0)):
-                    func=f.__qualname__
-                else:
-                    func=""
-                logger.debug('>>> enter {0} args: {1} - kwargs: {2}'.format(func,str(args[1:]),str(kargs))) #omit self in the args...
+                func = f.__qualname__
+                logger.debug(
+                    ">>> enter {0} args: {1} - kwargs: {2}".format(
+                        func, str(args[1:]), str(kargs)
+                    )
+                )  # omit self in the args...
                 tic = time.perf_counter()
                 r = f(*args, **kargs)
                 toc = time.perf_counter()
-                logger.debug('<<< leave {} - time: {:0.4f} sec'.format(func,toc-tic))
+                logger.debug("<<< leave {} - time: {:0.4f} sec".format(func, toc - tic))
                 return r
+
             return wrapped
+
         return wrapper
+
     return log_
 
-_debug = debug('dbplus')
 
+_debug = debug("dbplus")
```

### Comparing `DBPlus-0.3.1/license.txt` & `DBPlus-0.3.2/license.txt`

 * *Files identical despite different names*

### Comparing `DBPlus-0.3.1/setup.py` & `DBPlus-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='DBPlus',
-      version='0.3.1',
+      version='0.3.2',
       description='Database-agnostic SQL Interface for Postresql, MySQL, SQLite, DB2 and more',
       url='https://github.com/klaasbrant/DBPlus',
       author='Klaas Brant',
       author_email='kbrant@kbce.com',
       license='ISC',
       packages=['dbplus','dbplus.drivers'],
       install_requires=[],
```

