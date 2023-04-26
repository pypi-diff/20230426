# Comparing `tmp/Kvsqlite-0.1.4.tar.gz` & `tmp/Kvsqlite-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kvsqlite-0.1.4.tar", last modified: Wed Feb 22 14:27:12 2023, max compression
+gzip compressed data, was "Kvsqlite-0.2.0.dev0.tar", last modified: Wed Apr 26 10:15:30 2023, max compression
```

## Comparing `Kvsqlite-0.1.4.tar` & `Kvsqlite-0.2.0.dev0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/Kvsqlite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2023-02-22 14:27:12.000000 Kvsqlite-0.1.4/Kvsqlite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      367 2023-02-22 14:27:12.000000 Kvsqlite-0.1.4/Kvsqlite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-02-22 14:27:12.000000 Kvsqlite-0.1.4/Kvsqlite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2023-02-22 14:27:12.000000 Kvsqlite-0.1.4/Kvsqlite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      119 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1416 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/benchmark/
--rw-r--r--   0 runner    (1001) docker     (116)     9783 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/benchmark/benchmark_kvsqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/kvsqlite/
--rw-r--r--   0 runner    (1001) docker     (116)      316 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2608 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     5520 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/client.py
--rw-r--r--   0 runner    (1001) docker     (116)      783 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/encoders.py
--rw-r--r--   0 runner    (1001) docker     (116)     7947 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/kvsqlite/sync/
--rw-r--r--   0 runner    (1001) docker     (116)       49 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4838 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/kvsqlite/sync/client.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1031 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-02-22 14:27:12.804828 Kvsqlite-0.1.4/test/
--rw-r--r--   0 runner    (1001) docker     (116)     4757 2023-02-22 14:27:09.000000 Kvsqlite-0.1.4/test/test_kvsqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.545844 Kvsqlite-0.2.0.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-26 10:15:30.000000 Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/benchmark/benchmark_kvsqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/kvsqlite/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6386 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/kvsqlite/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/kvsqlite/sync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:15:30.545844 Kvsqlite-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:15:30.541844 Kvsqlite-0.2.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-26 10:15:29.000000 Kvsqlite-0.2.0.dev0/test/test_kvsqlite.py
```

### Comparing `Kvsqlite-0.1.4/Kvsqlite.egg-info/PKG-INFO` & `Kvsqlite-0.2.0.dev0/Kvsqlite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kvsqlite
-Version: 0.1.4
+Version: 0.2.0.dev0
 Summary: Easy-to-use synchronous/asynchronous key-value database backed by sqlite3.
 Home-page: https://github.com/AYMENJD/Kvsqlite
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/Kvsqlite
 Project-URL: Tracker, https://github.com/AYMENJD/Kvsqlite/issues
@@ -55,14 +55,17 @@
 
         if await db.exists(key):
             get_key = await db.get(key)
 
             print(get_key) # Hello world. Bye!
 
             await db.delete(key)
+
+            await db.setex(key, "This key has a lifetime of 60 seconds", 60)
+
+            print(await db.get(key))
         else:
             print("Key not found", result)
 
-        await db.close()
 
 asyncio.run(main())
 ```
```

### Comparing `Kvsqlite-0.1.4/LICENSE` & `Kvsqlite-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.1.4/PKG-INFO` & `Kvsqlite-0.2.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kvsqlite
-Version: 0.1.4
+Version: 0.2.0.dev0
 Summary: Easy-to-use synchronous/asynchronous key-value database backed by sqlite3.
 Home-page: https://github.com/AYMENJD/Kvsqlite
 Author: AYMEN Mohammed
 Author-email: let.me.code.safe@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AYMENJD/Kvsqlite
 Project-URL: Tracker, https://github.com/AYMENJD/Kvsqlite/issues
@@ -55,14 +55,17 @@
 
         if await db.exists(key):
             get_key = await db.get(key)
 
             print(get_key) # Hello world. Bye!
 
             await db.delete(key)
+
+            await db.setex(key, "This key has a lifetime of 60 seconds", 60)
+
+            print(await db.get(key))
         else:
             print("Key not found", result)
 
-        await db.close()
 
 asyncio.run(main())
 ```
```

### Comparing `Kvsqlite-0.1.4/README.md` & `Kvsqlite-0.2.0.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,17 @@
 
         if await db.exists(key):
             get_key = await db.get(key)
 
             print(get_key) # Hello world. Bye!
 
             await db.delete(key)
+
+            await db.setex(key, "This key has a lifetime of 60 seconds", 60)
+
+            print(await db.get(key))
         else:
             print("Key not found", result)
 
-        await db.close()
 
 asyncio.run(main())
 ```
```

### Comparing `Kvsqlite-0.1.4/benchmark/benchmark_kvsqlite.py` & `Kvsqlite-0.2.0.dev0/benchmark/benchmark_kvsqlite.py`

 * *Files 20% similar despite different names*

```diff
@@ -76,14 +76,58 @@
         ),
         ENDC,
     )
     print(GREEN, "================Benchmark end================", ENDC)
     print()
 
 
+async def benchmark_setex(db, keys):
+    print(PINK, "================Benchmark setex================", ENDC)
+    timeing = 0
+    start = time.perf_counter()
+    start_memory = psutil.Process(os.getpid()).memory_info().rss
+    print(
+        WARNING,
+        "-> Started with memory usage:",
+        ENDC,
+        start_memory,
+    )
+    for k, v in keys:
+        latncey_start = time.perf_counter()
+        await db.setex(k, v, 60)
+        timeing += time.perf_counter() - latncey_start
+    end_memory = psutil.Process(os.getpid()).memory_info().rss
+    took = time.perf_counter() - start
+    print(
+        WARNING,
+        "-> {} query took:{} {}".format(args.query_count, ENDC, took),
+    )
+    print(
+        WARNING,
+        "-> QRS:",
+        ENDC,
+        int(args.query_count / took),
+    )
+    print(
+        WARNING,
+        "-> Average latancey:",
+        ENDC,
+        timeing / args.query_count,
+    )
+    print(
+        WARNING,
+        "-> Current memory usage:{} {} ({}+{}{})".format(
+            ENDC, end_memory, GREEN, (end_memory - start_memory), ENDC
+        ),
+        ENDC,
+    )
+    print(GREEN, "================Benchmark end================", ENDC)
+    print()
+
+
 async def benchmark_get(db, keys):
     print(PINK, "================Benchmark get================", ENDC)
     timeing = 0
     start = time.perf_counter()
     start_memory = psutil.Process(os.getpid()).memory_info().rss
     print(
         WARNING,
@@ -164,14 +208,102 @@
         ),
         ENDC,
     )
     print(GREEN, "================Benchmark end================", ENDC)
     print()
 
 
+async def benchmark_ttl(db, keys):
+    print(PINK, "================Benchmark ttl=============", ENDC)
+    timeing = 0
+    start = time.perf_counter()
+    start_memory = psutil.Process(os.getpid()).memory_info().rss
+    print(
+        WARNING,
+        "-> Started with memory usage:",
+        ENDC,
+        start_memory,
+    )
+    for k, v in keys:
+        latncey_start = time.perf_counter()
+        await db.ttl(k)
+        timeing += time.perf_counter() - latncey_start
+    end_memory = psutil.Process(os.getpid()).memory_info().rss
+    took = time.perf_counter() - start
+    print(
+        WARNING,
+        "-> {} query took:{} {}".format(args.query_count, ENDC, took),
+    )
+    print(
+        WARNING,
+        "-> QRS:",
+        ENDC,
+        int(args.query_count / took),
+    )
+    print(
+        WARNING,
+        "-> Average latancey:",
+        ENDC,
+        timeing / args.query_count,
+    )
+    print(
+        WARNING,
+        "-> Current memory usage:{} {} ({}+{}{})".format(
+            ENDC, end_memory, GREEN, (end_memory - start_memory), ENDC
+        ),
+        ENDC,
+    )
+    print(GREEN, "================Benchmark end================", ENDC)
+    print()
+
+
+async def benchmark_expire(db, keys):
+    print(PINK, "================Benchmark expire=============", ENDC)
+    timeing = 0
+    start = time.perf_counter()
+    start_memory = psutil.Process(os.getpid()).memory_info().rss
+    print(
+        WARNING,
+        "-> Started with memory usage:",
+        ENDC,
+        start_memory,
+    )
+    for k, v in keys:
+        latncey_start = time.perf_counter()
+        await db.expire(k, 30)
+        timeing += time.perf_counter() - latncey_start
+    end_memory = psutil.Process(os.getpid()).memory_info().rss
+    took = time.perf_counter() - start
+    print(
+        WARNING,
+        "-> {} query took:{} {}".format(args.query_count, ENDC, took),
+    )
+    print(
+        WARNING,
+        "-> QRS:",
+        ENDC,
+        int(args.query_count / took),
+    )
+    print(
+        WARNING,
+        "-> Average latancey:",
+        ENDC,
+        timeing / args.query_count,
+    )
+    print(
+        WARNING,
+        "-> Current memory usage:{} {} ({}+{}{})".format(
+            ENDC, end_memory, GREEN, (end_memory - start_memory), ENDC
+        ),
+        ENDC,
+    )
+    print(GREEN, "================Benchmark end================", ENDC)
+    print()
+
+
 async def benchmark_delete(db, keys):
     print(PINK, "================Benchmark delete=============", ENDC)
     timeing = 0
     start = time.perf_counter()
     start_memory = psutil.Process(os.getpid()).memory_info().rss
     print(
         WARNING,
@@ -345,14 +477,22 @@
         await benchmark_set(db, keys)
         await benchmark_get(db, keys)
         await benchmark_exists(db, keys)
         await benchmark_delete(db, keys)
 
         await db.flush()
 
+    async with kvsqlite.Client(args.db_path) as db:
+        await benchmark_setex(db, keys)
+        await benchmark_get(db, keys)
+        await benchmark_ttl(db, keys)
+        await benchmark_expire(db, keys)
+
+        await db.flush()
+
     async with kvsqlite.Client(args.db_path, autocommit=False) as db:
         await benchmark_no_auto_commit_set(db, keys)
         await db.flush()
 
     async with kvsqlite.Client(args.db_path, workers=5) as db:
         print(
             WARNING,
```

### Comparing `Kvsqlite-0.1.4/kvsqlite/base.py` & `Kvsqlite-0.2.0.dev0/kvsqlite/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,163 @@
+import kvsqlite
+
+
 class BaseClient:
     def get(self, key: str):
         """Get the value of ``key``
 
         Args:
             key (``str``):
-                The key to get.
+                The key to get
         """
         raise NotImplementedError
 
     def set(self, key: str, value):
-        """Get the value of ``key``
+        """Set the value of ``key``
 
         Args:
             key (``str``):
-                The key.
+                The key
 
             value (``Any``):
-                The value to set for ``key``.
+                The value to set for ``key``
 
         Returns:
-            :py:class:`bool`: ``True`` on success.
+            :py:class:`bool`: ``True`` on success
+        """
+        raise NotImplementedError
+
+    def setex(self, key: str, value, ttl: int):
+        """Set the value of ``key`` with a timeout specified by ``ttl``
+
+        Args:
+            key (``str``):
+                The key
+
+            value (``Any``):
+                The value to set for ``key``
+
+            ttl (``int``):
+                The number of seconds for ``key`` timeout (a.k.a ``key`` lifetime)
+
+        .. warning::
+            Timeouted keys aren't deleted by default, you must call :func:`~kvsqlite.BaseClient.cleanex` for time to time
+
+        Returns:
+            :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
     def delete(self, key: str):
         """Delete ``key`` from database
 
         Args:
             key (``str``):
-                The key to delete.
+                The key to delete
         """
         raise NotImplementedError
 
     def commit(self):
         """Commit the current changes
 
         Returns:
-            :py:class:`bool`: ``True`` on success.
+            :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
     def exists(self, key: str):
         """Check if ``key`` already exists in database
 
         Args:
             key (``str``):
-                The key to search for.
+                The key to search for
 
         Returns:
-            :py:class:`bool`: ``True`` if found, otherwise ``False``.
+            :py:class:`bool`: ``True`` if found, otherwise ``False``
+        """
+        raise NotImplementedError
+
+    def ttl(self, key: str):
+        """Returns the remaining time to live of a ``key`` that has a timeout
+
+        Args:
+            key (``str``):
+                The key
+
+        Returns:
+            :py:class:`float`: The remaining time, otherwise ``0``
+        """
+        raise NotImplementedError
+
+    def expire(self, key: str, ttl: int):
+        """Set a timeout on ``key``
+
+        Args:
+            key (``str``):
+                The key
+
+            ttl (``int``):
+                The number of seconds for ``key`` timeout (a.k.a ``key`` lifetime)
+
+        Returns:
+            :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
     def rename(self, key: str, new_key: str):
         """Rename ``key`` with ``new_key``
 
         Args:
             key (``str``):
-                The key to rename.
+                The key to rename
 
             new_key (``str``):
-                The key to rename with.
+                The key to rename with
 
         Returns:
-            :py:class:`bool`: ``True`` if renamed, otherwise ``False``.
+            :py:class:`bool`: ``True`` if renamed, otherwise ``False``
         """
         raise NotImplementedError
 
     def keys(self, like: str = "%"):
         """Return list of keys in database with the given pattern
 
         Args:
             like (``str``, *optional*):
-                SQLite LIKE operator. Defaults to ``%`` (all keys).
+                SQLite LIKE operator. Defaults to ``%`` (all keys)
 
         Returns:
             :py:class:`list`:
-                A list of :py:class:`Tuple` contains keys.
+                A list of :py:class:`Tuple` contains keys
 
             :py:class:`None`:
-                If there is no keys to return.
+                If there is no keys to return
+        """
+        raise NotImplementedError
+
+    def cleanex(self):
+        """Removes all expired keys from database. This reduces disk usage
+
+        Returns:
+            :py:class:`int`: Number of deleted keys
         """
         raise NotImplementedError
 
     def flush(self):
         """Flush and remove everything from the current database
 
         Returns:
-            :py:class:`bool`: ``True`` on success.
+            :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
 
     def close(self, optimize_database: bool = True):
         """Close database connection
 
         Args:
             optimize_database (``bool``, **optional**):
-                Whether optimize database before closing or not. Defaults to ``True``.
+                Whether optimize database before closing or not. Defaults to ``True``
 
         Returns:
-            :py:class:`bool`: ``True`` on success.
+            :py:class:`bool`: ``True`` on success
         """
         raise NotImplementedError
```

### Comparing `Kvsqlite-0.1.4/kvsqlite/client.py` & `Kvsqlite-0.2.0.dev0/kvsqlite/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -105,14 +105,21 @@
 
     async def set(self, key: str, value) -> bool:
         assert isinstance(key, str), "key must be str"
 
         future = self.__invoke(request=REQUEST.SET, key=key, value=value)
         return await future
 
+    async def setex(self, key: str, value, ttl: int) -> bool:
+        assert isinstance(key, str), "key must be str"
+        assert ttl >= 1, "ttl must be greater than 1"
+
+        future = self.__invoke(request=REQUEST.SETEX, key=key, value=[value, ttl])
+        return await future
+
     async def delete(self, key: str) -> bool:
         assert isinstance(key, str), "key must be str"
 
         future = self.__invoke(request=REQUEST.DELETE, key=key)
         return await future
 
     async def commit(self) -> bool:
@@ -121,27 +128,44 @@
 
     async def exists(self, key: str) -> bool:
         assert isinstance(key, str), "key must be str"
 
         future = self.__invoke(request=REQUEST.EXISTS, key=key)
         return await future
 
+    async def ttl(self, key: str) -> float:
+        assert isinstance(key, str), "key must be str"
+
+        future = self.__invoke(request=REQUEST.TTL, key=key)
+        return await future
+
+    async def expire(self, key: str, ttl: int) -> bool:
+        assert isinstance(key, str), "key must be str"
+        assert ttl >= 1, "ttl must be greater than 1"
+
+        future = self.__invoke(request=REQUEST.EXPIRE, key=key, value=ttl)
+        return await future
+
     async def rename(self, key: str, new_key: str) -> bool:
         assert isinstance(key, str), "key must be str"
         assert isinstance(new_key, str), "new_key must be str"
 
         future = self.__invoke(request=REQUEST.RENAME, key=key, value=new_key)
         return await future
 
     async def keys(self, like: str = "%") -> Union[List[Tuple[str]], None]:
         assert isinstance(like, str), "like must be str"
 
         future = self.__invoke(request=REQUEST.KEYS, value=like)
         return await future
 
+    async def cleanex(self) -> int:
+        future = self.__invoke(request=REQUEST.CLEAN_EX)
+        return await future
+
     async def flush(self) -> bool:
         future = self.__invoke(request=REQUEST.FLUSH_DB)
         return await future
 
     async def close(self, optimize_database: bool = True) -> bool:
         assert isinstance(optimize_database, bool), "optimize_database must be bool"
```

### Comparing `Kvsqlite-0.1.4/kvsqlite/encoders.py` & `Kvsqlite-0.2.0.dev0/kvsqlite/encoders.py`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.1.4/kvsqlite/sqlite.py` & `Kvsqlite-0.2.0.dev0/kvsqlite/sqlite.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 import sqlite3
 import logging
 
 from concurrent.futures import ThreadPoolExecutor
 from threading import Lock
 from sys import version_info
+from time import time
 
 logger = logging.getLogger(__name__)
 
 
 class REQUEST:
     GET = "GET"
     SET = "SET"
+    SETEX = "SETEX"
     DELETE = "DELETE"
     COMMIT = "COMMIT"
     EXISTS = "EXISTS"
+    TTL = "TTL"
+    EXPIRE = "EXPIRE"
     RENAME = "RENAME"
     KEYS = "KEYS"
+    CLEAN_EX = "CLEAN_EX"
     FLUSH_DB = "FLUSH_DB"
     CLOSE = "CLOSE"
 
 
-TABLE_STATEMENT = (
-    'CREATE TABLE IF NOT EXISTS "{}" (k VARCHAR(4096) PRIMARY KEY, v BLOB)'
-)
+TABLE_STATEMENT = 'CREATE TABLE IF NOT EXISTS "{}" (k VARCHAR(4096) PRIMARY KEY, v BLOB, expire_time INTEGER DEFAULT NULL)'
 
 
 class Sqlite:
     def __init__(
         self,
         database: str,
         table_name: str,
@@ -63,24 +66,32 @@
 
         logger.debug("Request={}, key={}".format(request, key))
 
         if request == REQUEST.GET:
             return self.__get(key)
         elif request == REQUEST.SET:
             return self.__set(key, value)
+        elif request == REQUEST.SETEX:
+            return self.__setex(key, value)
         elif request == REQUEST.DELETE:
             return self.__delete(key)
         elif request == REQUEST.COMMIT:
             return self.__commit()
         elif request == REQUEST.EXISTS:
             return self.__exists(key)
+        elif request == REQUEST.TTL:
+            return self.__ttl(key)
+        elif request == REQUEST.EXPIRE:
+            return self.__expire(key, value)
         elif request == REQUEST.RENAME:
             return self.__rename(key, value)
         elif request == REQUEST.KEYS:
             return self.__keys(value)
+        elif request == REQUEST.CLEAN_EX:
+            return self.__clean_ex()
         elif request == REQUEST.FLUSH_DB:
             return self.__flush_db()
         elif request == REQUEST.CLOSE:
             return self.__close(value)
         else:
             raise ValueError("Unknown request {}".format(request))
 
@@ -93,116 +104,170 @@
             else:
                 connection = sqlite3.connect(self.database, check_same_thread=False)
 
             # connection.row_factory = sqlite3.Row
             logger.info("Connected to {}".format(self.database))
         except Exception as e:
             logger.exception(
-                "Error while opening sqlite3 self.__connection for database: {}".format(
-                    self.database
-                )
+                "Error while opening sqlite3 for database: {}".format(self.database)
             )
             raise e
 
         try:
             connection.execute("PRAGMA journal_mode = {}".format(self.journal_mode))
             connection.execute("PRAGMA synchronous = {}".format(self.synchronous))
         except Exception as e:
             logger.exception("Error while executing PRAGMA statement")
             raise e
 
         try:
-            connection.execute(TABLE_STATEMENT.format(self.table_name))
+            self.__check_table(connection)
         except Exception as e:
-            logger.exception("Error while executing CREATE TABLE statement")
+            logger.exception("Error while checking table")
             raise e
 
         return connection
 
     def __get(self, key: str):
         try:
             query = self.__connection.execute(
-                'SELECT v FROM "{}" WHERE k = ?'.format(self.table_name),
-                (key,),
+                'SELECT v FROM "{}" WHERE k = ? AND (expire_time IS NULL OR expire_time > ?)'.format(
+                    self.table_name
+                ),
+                (key, time()),
             ).fetchone()
             if query:
                 return self.__encoder.decode(query[0])
             else:
                 return None
         except Exception as e:
-            logger.exception("SELECT statment error")
+            logger.exception("GET command exception")
             raise e
 
     def __set(self, key: str, value):
         with self.__lock:
             try:
                 query = self.__connection.execute(
-                    'REPLACE INTO "{}" (k, v) VALUES(?,?)'.format(self.table_name),
+                    'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,NULL)'.format(
+                        self.table_name
+                    ),
                     (key, self.__encoder.encode(value)),
                 )
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
-                logger.exception("REPLACE INTO statment error")
+                logger.exception("SET command exception")
+                raise e
+
+    def __setex(self, key: str, value):
+        with self.__lock:
+            try:
+                query = self.__connection.execute(
+                    'REPLACE INTO "{}" (k, v, expire_time) VALUES(?,?,?)'.format(
+                        self.table_name
+                    ),
+                    (key, self.__encoder.encode(value[0]), time() + value[1]),
+                )
+                if query.rowcount > 0:
+                    return True
+                else:
+                    return False
+            except Exception as e:
+                logger.exception("SETEX command exception")
                 raise e
 
     def __delete(self, key: str):
         with self.__lock:
             try:
                 query = self.__connection.execute(
                     'DELETE FROM "{}" WHERE k = ?'.format(self.table_name),
                     (key,),
                 )
                 if query.rowcount > 0:
                     return True
                 else:
                     return False
             except Exception as e:
-                logger.exception("DELETE statment error")
+                logger.exception("DELETE command exception")
                 raise e
 
     def __commit(self):
         with self.__lock:
             try:
                 self.__connection.commit()
                 return True
             except Exception as e:
-                logger.exception("COMMIT error")
+                logger.exception("COMMIT command exception")
                 raise e
 
     def __exists(self, key: str):
         try:
             query = self.__connection.execute(
                 'SELECT k FROM "{}" WHERE k = ?'.format(self.table_name),
                 (key,),
             ).fetchone()
 
             if query:
                 return True
             else:
                 return False
         except Exception as e:
-            logger.exception("EXISTS error")
+            logger.exception("EXISTS command exception")
             raise e
 
+    def __ttl(self, key: str):
+        try:
+            query = self.__connection.execute(
+                'SELECT expire_time FROM "{}" WHERE k = ? AND expire_time > ?'.format(
+                    self.table_name
+                ),
+                (key, time()),
+            ).fetchone()
+
+            if query:
+                return query[0] - time()
+            else:
+                return 0
+        except Exception as e:
+            logger.exception("TTL command exception")
+            raise e
+
+    def __expire(self, key: str, ttl: int):
+        with self.__lock:
+            try:
+                query = self.__connection.execute(
+                    'UPDATE "{}" SET expire_time = ? WHERE k = ?'.format(
+                        self.table_name
+                    ),
+                    (time() + ttl, key),
+                )
+
+                if query.rowcount > 0:
+                    return True
+                else:
+                    return False
+            except Exception as e:
+                logger.exception("EXPIRE command exception")
+                raise e
+
     def __rename(self, key: str, new_key: str):
         try:
             query = self.__connection.execute(
                 'UPDATE OR IGNORE "{}" SET k = ? WHERE k = ?'.format(self.table_name),
                 (new_key, key),
             )
 
             if query.rowcount > 0:
                 return True
             else:
                 return False
         except Exception as e:
-            logger.exception("RENAME KEY error")
+            logger.exception("RENAME command exception")
             raise e
 
     def __keys(self, like: str):
         try:
             query = self.__connection.execute(
                 'SELECT k FROM "{}" WHERE k LIKE ? ORDER BY rowid'.format(
                     self.table_name
@@ -210,25 +275,40 @@
                 (like,),
             ).fetchall()
             if query:
                 return query
             else:
                 return None
         except Exception as e:
-            logger.exception("SELECT KEYS statment error")
+            logger.exception("KEYS command exception")
             raise e
 
+    def __clean_ex(self):
+        with self.__lock:
+            try:
+                query = self.__connection.execute(
+                    'DELETE FROM "{}" WHERE expire_time IS NOT NULL AND expire_time <= ?'.format(
+                        self.table_name
+                    ),
+                    (time(),),
+                )
+
+                return query.rowcount
+            except Exception as e:
+                logger.exception("CLEAN_EX command exception")
+                raise e
+
     def __flush_db(self):
         with self.__lock:
             try:
                 self.__connection.execute('DROP TABLE "{}"'.format(self.table_name))
                 self.__connection.execute(TABLE_STATEMENT.format(self.table_name))
                 return True
             except Exception as e:
-                logger.exception("DROP TABLE statment error")
+                logger.exception("FLUSH_DB command exception")
                 raise e
 
     def __close(self, optimize: bool):
         with self.__lock:
             try:
                 if optimize:
                     self.__connection.execute("PRAGMA optimize")
@@ -239,9 +319,37 @@
                     self.__workers.shutdown(False, cancel_futures=True)
                 else:
                     self.__workers.shutdown(False)
 
                 self.is_running = False
                 return True
             except Exception as e:
-                logger.exception("On close error")
+                logger.exception("CLOSE command exception")
                 raise e
+
+    def __check_table(self, connection: sqlite3.Connection):
+        try:
+            table_exists = (
+                connection.execute(
+                    "SELECT name FROM sqlite_master WHERE type = 'table' AND name = ?",
+                    (self.table_name,),
+                ).fetchone()
+                is not None
+            )
+
+            if table_exists:
+                query = connection.execute(
+                    "PRAGMA table_info({})".format((self.table_name))
+                )
+                columns = [row[1] for row in query.fetchall()]
+
+                if "expire_time" not in columns:
+                    connection.execute(
+                        "ALTER TABLE '{}' ADD COLUMN expire_time INTEGER DEFAULT NULL".format(
+                            self.table_name
+                        )
+                    )
+            else:
+
+                connection.execute(TABLE_STATEMENT.format(self.table_name))
+        except Exception:
+            logger.exception("Check table error")
```

### Comparing `Kvsqlite-0.1.4/kvsqlite/sync/client.py` & `Kvsqlite-0.2.0.dev0/kvsqlite/sync/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,38 +94,58 @@
         return self.__invoke(request=REQUEST.GET, key=key)
 
     def set(self, key: str, value) -> bool:
         assert isinstance(key, str), "key must be str"
 
         return self.__invoke(request=REQUEST.SET, key=key, value=value)
 
+    def setex(self, key: str, value, ttl: int) -> bool:
+        assert isinstance(key, str), "key must be str"
+        assert ttl >= 1, "ttl must be greater than 1"
+
+        return self.__invoke(request=REQUEST.SETEX, key=key, value=[value, ttl])
+
     def delete(self, key: str) -> bool:
         assert isinstance(key, str), "key must be str"
 
         return self.__invoke(request=REQUEST.DELETE, key=key)
 
     def commit(self) -> bool:
         return self.__invoke(request=REQUEST.COMMIT)
 
     def exists(self, key: str) -> bool:
         assert isinstance(key, str), "key must be str"
 
         return self.__invoke(request=REQUEST.EXISTS, key=key)
 
+    def ttl(self, key: str) -> float:
+        assert isinstance(key, str), "key must be str"
+
+        return self.__invoke(request=REQUEST.TTL, key=key)
+
+    def expire(self, key: str, ttl: int) -> bool:
+        assert isinstance(key, str), "key must be str"
+        assert ttl >= 1, "ttl must be greater than 1"
+
+        return self.__invoke(request=REQUEST.EXPIRE, key=key, value=ttl)
+
     def rename(self, key: str, new_key: str) -> bool:
         assert isinstance(key, str), "key must be str"
         assert isinstance(new_key, str), "new_key must be str"
 
         return self.__invoke(request=REQUEST.RENAME, key=key, value=new_key)
 
     def keys(self, like: str = "%") -> Union[List[Tuple[str]], None]:
         assert isinstance(like, str), "like must be str"
 
         return self.__invoke(request=REQUEST.KEYS, value=like)
 
+    def cleanex(self) -> int:
+        return self.__invoke(request=REQUEST.CLEAN_EX)
+
     def flush(self) -> bool:
         return self.__invoke(request=REQUEST.FLUSH_DB)
 
     def close(self, optimize_database: bool = True) -> bool:
         assert isinstance(optimize_database, bool), "optimize_database must be bool"
 
         return self.__invoke(request=REQUEST.CLOSE, value=optimize_database)
```

### Comparing `Kvsqlite-0.1.4/setup.py` & `Kvsqlite-0.2.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `Kvsqlite-0.1.4/test/test_kvsqlite.py` & `Kvsqlite-0.2.0.dev0/test/test_kvsqlite.py`

 * *Files identical despite different names*

