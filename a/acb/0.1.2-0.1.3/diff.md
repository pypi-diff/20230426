# Comparing `tmp/acb-0.1.2.tar.gz` & `tmp/acb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.1.2.tar", last modified: Wed Apr 26 08:05:40 2023, max compression
+gzip compressed data, was "acb-0.1.3.tar", last modified: Wed Apr 26 13:19:22 2023, max compression
```

## Comparing `acb-0.1.2.tar` & `acb-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      695 2023-04-22 16:43:07.483057 acb-0.1.2/README.md
--rw-r--r--   0        0        0      126 2023-04-26 02:25:22.898091 acb-0.1.2/acb/__init__.py
--rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.2/acb/actions/__init__.py
--rw-r--r--   0        0        0    12770 2023-04-22 16:43:13.206258 acb-0.1.2/acb/actions/backup.py
--rw-r--r--   0        0        0        0 2023-04-20 13:41:24.197946 acb-0.1.2/acb/actions/debug.py
--rw-r--r--   0        0        0     2972 2023-04-26 08:04:43.989897 acb-0.1.2/acb/actions/encode.py
--rw-r--r--   0        0        0     1268 2023-04-16 01:26:47.450605 acb-0.1.2/acb/actions/hash.py
--rw-r--r--   0        0        0        0 2023-04-20 14:27:02.585564 acb-0.1.2/acb/actions/log.py
--rw-r--r--   0        0        0     5589 2023-04-22 16:43:13.213127 acb-0.1.2/acb/actions/mail.py
--rw-r--r--   0        0        0       85 2023-04-22 16:43:07.423269 acb-0.1.2/acb/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 01:47:22.926037 acb-0.1.2/acb/adapters/analytic/__init__.py
--rw-r--r--   0        0        0      841 2023-04-22 16:43:13.241412 acb-0.1.2/acb/adapters/analytic/google.py
--rw-r--r--   0        0        0        1 2023-04-26 01:26:41.151825 acb-0.1.2/acb/adapters/auth/__init__.py
--rw-r--r--   0        0        0     6731 2023-04-22 16:43:13.191539 acb-0.1.2/acb/adapters/auth/firebase.py
--rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.2/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0    11585 2023-04-22 16:43:13.136632 acb-0.1.2/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.2/acb/adapters/database/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 01:48:03.525185 acb-0.1.2/acb/adapters/database/redis.py
--rw-r--r--   0        0        0     3697 2023-04-26 02:25:26.619067 acb-0.1.2/acb/adapters/database/sqlalchemy.py
--rw-r--r--   0        0        0     4250 2023-04-22 16:43:13.165155 acb-0.1.2/acb/adapters/dns/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.2/acb/adapters/mail/__init__.py
--rw-r--r--   0        0        0     8442 2023-04-22 16:43:13.151029 acb-0.1.2/acb/adapters/mail/mailgun.py
--rw-r--r--   0        0        0     2429 2023-04-22 16:43:13.219816 acb-0.1.2/acb/adapters/recaptcha/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.2/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0     7126 2023-04-22 16:43:13.120483 acb-0.1.2/acb/adapters/secret/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.2/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     4701 2023-04-26 02:25:26.614937 acb-0.1.2/acb/adapters/storage/google.py
--rw-r--r--   0        0        0        0 2023-04-26 01:34:56.225464 acb-0.1.2/acb/adapters/storage/universal.py
--rw-r--r--   0        0        0      407 2023-04-26 02:25:26.622784 acb-0.1.2/acb/adapters/template/jinja/__init__.py
--rw-r--r--   0        0        0     1298 2023-04-22 16:43:13.227506 acb-0.1.2/acb/adapters/template/jinja/bccache.py
--rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 acb-0.1.2/acb/adapters/template/jinja/compiler.py
--rw-r--r--   0        0        0     1778 2023-04-22 16:43:13.142919 acb-0.1.2/acb/adapters/template/jinja/environment.py
--rw-r--r--   0        0        0    17755 2023-04-22 16:43:13.179588 acb-0.1.2/acb/adapters/template/jinja/loaders.py
--rw-r--r--   0        0        0     3624 2023-04-22 16:43:13.172026 acb-0.1.2/acb/config.py
--rw-r--r--   0        0        0     1553 2023-04-26 08:05:40.818291 acb-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 acb-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      694 2023-04-26 10:42:56.638728 acb-0.1.3/README.md
+-rw-r--r--   0        0        0      126 2023-04-26 02:25:22.898091 acb-0.1.3/acb/__init__.py
+-rw-r--r--   0        0        0      124 2023-04-22 16:43:07.429717 acb-0.1.3/acb/actions/__init__.py
+-rw-r--r--   0        0        0    12869 2023-04-26 10:43:29.503944 acb-0.1.3/acb/actions/backup.py
+-rw-r--r--   0        0        0        0 2023-04-20 13:41:24.197946 acb-0.1.3/acb/actions/debug.py
+-rw-r--r--   0        0        0     2944 2023-04-26 10:43:25.703934 acb-0.1.3/acb/actions/encode.py
+-rw-r--r--   0        0        0     1268 2023-04-16 01:26:47.450605 acb-0.1.3/acb/actions/hash.py
+-rw-r--r--   0        0        0        0 2023-04-20 14:27:02.585564 acb-0.1.3/acb/actions/log.py
+-rw-r--r--   0        0        0     5597 2023-04-26 10:43:30.248567 acb-0.1.3/acb/actions/mail.py
+-rw-r--r--   0        0        0       85 2023-04-22 16:43:07.423269 acb-0.1.3/acb/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:47:22.926037 acb-0.1.3/acb/adapters/analytic/__init__.py
+-rw-r--r--   0        0        0      841 2023-04-22 16:43:13.241412 acb-0.1.3/acb/adapters/analytic/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 10:42:56.660227 acb-0.1.3/acb/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     6739 2023-04-26 10:43:27.144404 acb-0.1.3/acb/adapters/auth/firebase.py
+-rw-r--r--   0        0        0        0 2023-04-20 12:04:32.606819 acb-0.1.3/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0    11625 2023-04-26 10:43:33.424885 acb-0.1.3/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:28:40.559756 acb-0.1.3/acb/adapters/database/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:48:03.525185 acb-0.1.3/acb/adapters/database/redis.py
+-rw-r--r--   0        0        0     3737 2023-04-26 10:43:27.141502 acb-0.1.3/acb/adapters/database/sqlalchemy.py
+-rw-r--r--   0        0        0     4258 2023-04-26 10:43:30.602745 acb-0.1.3/acb/adapters/dns/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:36:40.098734 acb-0.1.3/acb/adapters/mail/__init__.py
+-rw-r--r--   0        0        0     8506 2023-04-26 10:43:30.062321 acb-0.1.3/acb/adapters/mail/mailgun.py
+-rw-r--r--   0        0        0     2437 2023-04-26 10:43:31.462644 acb-0.1.3/acb/adapters/recaptcha/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:43:28.269577 acb-0.1.3/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0     7171 2023-04-26 10:43:33.604151 acb-0.1.3/acb/adapters/secret/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:31:02.544210 acb-0.1.3/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     4725 2023-04-26 10:43:26.946619 acb-0.1.3/acb/adapters/storage/google.py
+-rw-r--r--   0        0        0        0 2023-04-26 01:34:56.225464 acb-0.1.3/acb/adapters/storage/universal.py
+-rw-r--r--   0        0        0      407 2023-04-26 02:25:26.622784 acb-0.1.3/acb/adapters/template/jinja/__init__.py
+-rw-r--r--   0        0        0     1314 2023-04-26 10:43:25.386904 acb-0.1.3/acb/adapters/template/jinja/bccache.py
+-rw-r--r--   0        0        0     5079 2023-04-16 01:42:22.123633 acb-0.1.3/acb/adapters/template/jinja/compiler.py
+-rw-r--r--   0        0        0     1786 2023-04-26 10:43:29.925170 acb-0.1.3/acb/adapters/template/jinja/environment.py
+-rw-r--r--   0        0        0    17777 2023-04-26 10:43:34.008658 acb-0.1.3/acb/adapters/template/jinja/loaders.py
+-rw-r--r--   0        0        0     3640 2023-04-26 10:43:25.943243 acb-0.1.3/acb/config.py
+-rw-r--r--   0        0        0     1514 2023-04-26 13:19:22.387954 acb-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 acb-0.1.3/PKG-INFO
```

### Comparing `acb-0.1.2/README.md` & `acb-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
 from acb.configure import (
     AppConfig,
     AppSettings,
 )
 ```
 
 ## Adapters
-
```

### Comparing `acb-0.1.2/acb/actions/backup.py` & `acb-0.1.3/acb/actions/backup.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,42 +10,46 @@
 from itertools import chain
 from pathlib import Path
 from re import search
 from typing import Any
 
 # from actions.load import load
 from adapters.database import async_session
+
 # from re import sub
 # from adapters.database_ import async_session
 from adapters.database import db_engine
 from config import ac
 from config import debug
 from models import AppModelBase
 from resize import clear_resized_images
+
 # from sqlalchemy.exc import IntegrityError
 # from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.ext.serializer import dumps as sdumps
 from sqlalchemy.ext.serializer import loads as sloads
 from sqlmodel import select
 from sqlmodel import SQLModel
+
 # from sqlalchemy.orm.exc import UnmappedInstanceError
 from storage import stor
 
 import arrow
+
 # from plugins import plugin_source
 from pydantic import BaseModel
 
 logger = asyncio.run(get_app_logger(__file__))(debug)
 
 sure_delete = False
 
 
 class BackupDbUtils(BaseModel):
     @staticmethod
-    def get_timestamp(name):
+    def get_timestamp(name: str):
         pattern = r"(.*)(-)(?P<timestamp>[\d]{10})(-)(.*)"
         match = search(pattern, name)
         return match.group("timestamp") if match else False
 
     def get_files(self):
         blobs = stor.db.list()
         for blob in blobs:
@@ -67,33 +71,33 @@
         if not self.files:
             self.files = tuple(self.get_files())
 
         for name in self.files:
             if timestamp == self.get_timestamp(name):
                 yield name
 
-    def valid(self, timestamp):
+    def valid(self, timestamp) -> bool:
         if timestamp and timestamp in self.get_timestamps():
             return True
         # print('==> Invalid id. Use "history" to list existing downloads')
         return False
 
-    def get_path(self, class_name, timestamp=None):
+    def get_path(self, class_name: str, timestamp=None):
         timestamp = timestamp or arrow.utcnow().int_timestamp
         self.backup_path = Path(f"{ac.app.name}-{timestamp}-{class_name}.sqla")
         return self.backup_path
 
 
 class BackupDbDates(BaseModel):
     today = arrow.utcnow()
     white_list = []
     black_list = []
     dates = list()
 
-    def __init__(self, dates=None, **data: Any):
+    def __init__(self, dates=None, **data: Any) -> None:
         super().__init__(**data)
         self.dates = sorted(dates, reverse=True) if dates else []
         self.run()  # feed self.white_list & self.black_list
 
     def get_last_month_length(self):
         return monthrange(self.today.year, self.today.shift(months=-1).month)[1]
 
@@ -113,15 +117,15 @@
             comp_date = datetime.fromtimestamp(int(date))
             comparison = method_mapping.get(period)(comp_date)
             ref_date = datetime.fromtimestamp(int(reference))
             if comparison != method_mapping.get(period)(ref_date):
                 reference = date
                 yield date
 
-    def run(self):
+    def run(self) -> None:
         last_w = self.today.shift(days=-7).int_timestamp
         last_m = self.today.shift(days=-(self.get_last_month_length())).int_timestamp
         last_y = self.today.shift(days=-(self.get_last_year_length())).int_timestamp
         backups_week = []
         backups_month = []
         backups_year = []
         backups_older = []
@@ -157,15 +161,15 @@
             if isinstance(m, type) and issubclass(m, AppModelBase)
         ]
 
     def get_mapped_classes(self):
         self.add_subclasses(AppModelBase)
         return self.models
 
-    def add_subclasses(self, model):
+    def add_subclasses(self, model) -> None:
         if model.__subclasses__():
             for submodel in model.__subclasses__():
                 self.add_subclasses(submodel)
         else:
             self.models.append(model)
 
     def get_data(self):
@@ -183,19 +187,19 @@
                 contents,
                 metadata=SQLModel.metadata,
                 engine=db_engine,
                 scoped_session=async_session(),
             )
         return contents
 
-    async def backup(self, class_name, data, now):
+    async def backup(self, class_name: str, data, now) -> None:
         path = self.get_path(class_name, now)
         await stor.db.save(data, path)
 
-    async def save(self):
+    async def save(self) -> None:
         data = self.get_data()
         now = arrow.utcnow().int_timestamp
 
         for class_name in data.keys():
             path = self.get_path(class_name, now)
             logger.debug(f"Backing up - {path.name}")
             await self.backup(class_name, data[class_name], now)
@@ -220,15 +224,15 @@
         if not len(timestamps):
             return False
         timestamp = sorted(timestamps, reverse=True)[0]
         adate = arrow.Arrow.fromtimestamp(timestamp)
         logger.info(f"Last backup: {adate.format('MM-DD-YYYY HH:mm:ss ZZ')}")
         return timestamp
 
-    def restore_rows(self, path: Path):
+    def restore_rows(self, path: Path) -> None:
         stor.db.get(path)
         # try:
         #     model = search("-(\D+).sqla", path.name).group(1)
         #     if contents:
         #         contents = sub(
         #             b"_sp.{31,32}\.",
         #             bytes(f"{plugin_source.spaceid}.", encoding="utf8"),
@@ -260,30 +264,30 @@
         #             status = f"\t!=> No or bad data for {model}."
         #     else:
         #         status = f"\t!=> File {path.name} does not exist."
         # except Exception as err:
         #     status = err
         # return status, fails
 
-    def restore_backup(self, timestamp):
+    def restore_backup(self, timestamp) -> None:
         paths = [Path(b.name) for b in stor.db.list() if timestamp in b.name]
         when = arrow.Arrow.fromtimestamp(timestamp).humanize()
         logger.info(f"Restoring backup from {when}.....")
         with ThreadPoolExecutor(max_workers=5) as executor:
             all_tasks = []
             for path in paths:
                 logger.debug(f"\tRestoring:  {path.name}")
                 all_tasks.append(executor.submit(self.restore_rows, path))
 
             for future in as_completed(all_tasks):
                 status, fails = future.result()
                 for f in fails:
                     logger.error(f"\t\tRestore of {f} failed!")
 
-    def delete_backups(self, delete_list):
+    def delete_backups(self, delete_list) -> None:
         delete_me = stor.db.delete(delete_list)
         if delete_me:
             for name in delete_list:
                 logger.debug(f"Deleted {name}")
 
     def clean(self):
         """
@@ -319,15 +323,15 @@
                 if debug.database:
                     logger.debug(f)
                 delete_list.append(f)
 
         self.delete_backups(delete_list)
         return "cleandb"
 
-    def run(self):
+    def run(self) -> None:
         if not ac.app.is_deployed:
             last_backup = self.get_last_backup()
             if debug.database and sure_delete:
                 blobs = [b.name for b in stor.db.list()]
                 for b in blobs:
                     stor.db.delete(b)
                 clear_resized_images()
```

### Comparing `acb-0.1.2/acb/actions/encode.py` & `acb-0.1.3/acb/actions/encode.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from addict import Dict as adict
 from aiopath import AsyncPath
 from itsdangerous import Serializer as SecureSerializer
 from pathy import Path as PathyPath
 
 
 class AcbEncoder:
-    def __init__(self):
+    def __init__(self) -> None:
         self.serializers = adict(
             json=msgspec.json,
             yaml=msgspec.yaml,
             msgpack=msgspec.msgpack,
             pickle=pickle,
             toml=tomllib,
         )
@@ -27,15 +27,15 @@
         tomllib.encode = tomlkit.dumps
         tomllib.dumps = tomlkit.dumps
         tomllib.decode = tomllib.loads
         for s in self.serializers.keys():
             setattr(self, s, self.__call__)
 
     async def process(
-            self, obj, path, action, serializer, sort_keys, use_list, **kwargs
+        self, obj, path, action, serializer, sort_keys, use_list, **kwargs
     ) -> adict | bytes:
         if action in ("load", "decode"):
             if serializer is msgspec.msgpack:
                 kwargs.use_list = use_list
             if isinstance(obj, AsyncPath):
                 obj = await obj.read_text()
             return adict(serializer.decode(obj, **kwargs))
@@ -59,22 +59,22 @@
         return (
             SecureSerializer(secret_key, secure_salt, serializer=serializer)
             if secure
             else serializer
         )
 
     async def __call__(
-            self,
-            obj: str | Path | AsyncPath | Path | bytes | dict | adict = None,
-            path: AsyncPath | Path | PathyPath | str | None = None,
-            sort_keys: bool = True,
-            use_list: bool = False,
-            secret_key: str = None,
-            secure_salt: str = None,
-            **kwargs,
+        self,
+        obj: str | Path | AsyncPath | Path | bytes | dict | adict = None,
+        path: AsyncPath | Path | PathyPath | str | None = None,
+        sort_keys: bool = True,
+        use_list: bool = False,
+        secret_key: str = None,
+        secure_salt: str = None,
+        **kwargs,
     ) -> adict | bytes:
         obj = obj if not isinstance(obj, Path | AsyncPath) else AsyncPath(obj)
         path = AsyncPath(path) if isinstance(path, Path | str) else path
         action, serializer = self.get_vars(sys._getframe(1))
         serializer = self.get_serializer(serializer, secret_key, secure_salt)
         return await self.process(
             obj, path, action, serializer, sort_keys, use_list, **kwargs
```

### Comparing `acb-0.1.2/acb/actions/hash.py` & `acb-0.1.3/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.2/acb/actions/mail.py` & `acb-0.1.3/acb/actions/mail.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,12 +168,12 @@
 
     @staticmethod
     async def default_checker():
         checker = DefaultChecker(db_provider="redis")
         await checker.init_redis()
         return checker
 
-    async def init(self):
+    async def init(self) -> None:
         self.set_logger()
 
 
 mail = Mail()
```

### Comparing `acb-0.1.2/acb/adapters/analytic/google.py` & `acb-0.1.3/acb/adapters/analytic/google.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.2/acb/adapters/auth/firebase.py` & `acb-0.1.3/acb/adapters/auth/firebase.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         return self.user_data.get("owner")
 
     @property
     def is_contributor(self):
         return self.user_data.get("contributor")
 
     @property
-    def is_superuser(self):
+    def is_superuser(self) -> bool:
         return not self.user_data.get("user")
 
     @property
     def uid(self):
         return self.user_data.get("uid")
 
     @property
```

### Comparing `acb-0.1.2/acb/adapters/cache/redis.py` & `acb-0.1.3/acb/adapters/cache/redis.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import anyio
 from acb import AppSettings
 from aiopath import AsyncPath
 from httpx import Request
 from httpx import Response
 from pydantic import BaseSettings
+
 # from httpx_cache.serializer.base import BaseSerializer
 # from httpx_cache.serializer.common import MsgPackSerializer
 # from httpx_cache.utils import get_cache_key
 from redis.asyncio import Redis as AsyncRedis
 
 
 class CacheSettings(AppSettings):
@@ -31,15 +32,15 @@
         # password=ac.secrets.redis_password if deployed else None,
         port=6379,
         db=0,
         health_check_interval=15,
         # expire_after=cache.default_timeout,
     )
 
-    def __init__(self, **data: t.Any):
+    def __init__(self, **data: t.Any) -> None:
         super().__init__(**data)
 
         class CacheConfig(BaseSettings):
             session = {**self.kwargs}
             starlette = {**self.kwargs, **dict(db=1)}
             theme = {**self.kwargs, **dict(db=2)}
             jinja = {**self.kwargs, **dict(db=3)}
@@ -47,20 +48,20 @@
             httpx = {**self.kwargs, **dict(db=5)}
             settings = {**self.kwargs, **dict(db=6)}
 
         self.configs = CacheConfig()
 
 
 class SetKeyAioRedis(AsyncRedis):
-    def __init__(self, prefix: t.Optional[str] = None, **configs):
+    def __init__(self, prefix: t.Optional[str] = None, **configs) -> None:
         super().__init__(**configs)
         self.prefix = prefix or ac.app.name
 
     @contextmanager
-    async def transaction(self, unique_key: str, ttl=600) -> t.AsyncGenerator:
+    async def transaction(self, unique_key: str, ttl: int = 600) -> t.AsyncGenerator:
         tkey = "_transaction_".join([self.prefix, unique_key])
 
         if self.set(tkey, str(getpid()), nx=True):
             await self.expire(tkey, ttl)
         else:
             yield False
         try:
@@ -112,20 +113,20 @@
             await self.set(key, to_cache)
 
     async def adelete(self, request: Request) -> None:
         key = get_cache_key(request)
         async with self.async_lock:
             await self.delete(key)
 
-    async def aclose(self):
+    async def aclose(self) -> None:
         await self.close()
 
 
 class AppAioRedis(AioRedis):
-    def __init__(self, namespace: t.Optional[str] = None, **configs):
+    def __init__(self, namespace: t.Optional[str] = None, **configs) -> None:
         super().__init__(**configs)
         self.prefix = prefix or ac.app.name
 
     async def clear(self, namespace: str = None, key: str = None):
         namespace = namespace or self.prefix
         if namespace:
             async for k in self.scan_iter(f"{namespace}:*"):
```

### Comparing `acb-0.1.2/acb/adapters/database/sqlalchemy.py` & `acb-0.1.3/acb/adapters/database/sqlalchemy.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     host: str = ac.secrets.database_host if deployed else "127.0.0.1"
     user: str = ac.secrets.database_user
     port = 3306
     async_url: t.Optional[URL]
     url: t.Optional[URL]
     engine_kwargs = dict(poolclass=NullPool, pool_pre_ping=True)
 
-    def __init__(self, **data: t.Any):
+    def __init__(self, **data: t.Any) -> None:
         super().__init__(**data)
         self.async_url_kwargs = adict(
             drivername="mysql+asyncmy",
             username=ac.secrets.database_user,
             password=ac.secrets.database_password,
             port=self.port,
             host=self.host,
@@ -41,15 +41,15 @@
         self.url = URL.create(**{**self.async_url_kwargs, **self.url_kwargs})
 
 
 class Database:
     engine: t.Any = None
     async_session: t.Any = None
 
-    async def create(self, demo=False):
+    async def create(self, demo: bool = False) -> None:
         exists = database_exists(ac.db.url)
         if exists:
             logger.debug("Database exists.")
 
         if (
             (debug.database or debug.models)
             and not (ac.app.is_deployed or debug.production)
@@ -81,15 +81,15 @@
             yield session
 
     @staticmethod
     def get_table_names(conn):
         inspector = inspect(conn)
         return inspector.get_table_names()
 
-    async def init(self, demo=False):
+    async def init(self, demo: bool = False) -> None:
         self.engine = create_async_engine(ac.db.async_url, **ac.db.engine_kwargs)
         self.async_session = asynccontextmanager(self.get_async_session)
         # print(debug.database)
         # print(type(debug.database))
         await self.create(demo)
         async with self.engine.connect() as conn:
             if debug.database:
```

### Comparing `acb-0.1.2/acb/adapters/dns/google.py` & `acb-0.1.3/acb/adapters/dns/google.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 class DnsRecord:
     name: str = ac.mail_domain
     type: str = "TXT"
     ttl: int = 300
     rrdata: str = ""
 
 
-def create_dns_zone():
+def create_dns_zone() -> None:
     if not dns_zone.exists():
         print(f"Creating gdns zone '{ac.app_name}...")
         dns_zone.create()
         print(f"Zone '{dns_zone.name}' successfully created.")
     else:
         print(f"Zone for '{dns_zone.name}' exists.")
```

### Comparing `acb-0.1.2/acb/adapters/mail/mailgun.py` & `acb-0.1.3/acb/adapters/mail/mailgun.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 from config import debug
 
 from httpx import AsyncClient
 from pydantic import BaseModel
 
 
 class Mailgun(BaseModel):
-    def __init__(self, **data: Any):
+    def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     # conf = ConnectionConfig(
     #     MAIL_SERVER="smtp.ac.mail.mailgun.org",
     #     MAIL_PORT=587,
     #     MAIL_USERNAME=f"postmaster@{app.domain}",
     #     MAIL_PASSWORD=secrets.app_mail_password,
     #     MAIL_FROM="info@{app.domain}",
     #     MAIL_TLS=True,
     #     MAIL_SSL=False,
     #     TEMPLATE_FOLDER=theme.path / "utility" / "mail",
     # )
 
-    def get_response(self, req_type: str, domain=None, data=None, params=None):
+    def get_response(self, req_type: str, domain=None, data=None, params=None) -> None:
         pass
 
     #     caller = inspect_.calling_function()
     #     match caller:
     #         case search(caller, "domain"):
     #             caller = "domain"
     #         case search(caller, "route"):
@@ -110,15 +110,15 @@
         record = DnsRecord(name=domain, type="MX", rrdata=rrdata)
         records.append(record)
         for r in sending_records:
             record = DnsRecord(name=r["name"], type=r["record_type"], rrdata=r["value"])
             records.append(record)
         return records
 
-    async def create_dns_records(self):
+    async def create_dns_records(self) -> None:
         # if not ac.mail.mailgun.domain in list_domains(self):
         await self.create_domain(ac.mail.mailgun.domain)
         await self.create_domain_credentials(ac.mail.mailgun.domain)
         records = await self.get_dns_records(ac.mail.mailgun.domain)
         if ac.mail.mailgun.gmail.enabled:
             await self.delete_domain(ac.mail.mailgun.domain)
             rrdata = ac.mail.gmail.mx_servers
@@ -150,15 +150,15 @@
         return resp
 
     @staticmethod
     def get_name(address: str):
         name = search("'(.+)@.+", address)
         return name.group(1) if name else ""
 
-    async def delete_routes(self, delete_all=False):
+    async def delete_routes(self, delete_all: bool = False) -> None:
         forwards = await load.yaml(Path("mail.yml")).keys()
         routes = await self.list_routes()
         deletes = []
         deletes.extend(
             [r for r in routes if self.get_name(r["expression"]) not in forwards]
         )
         if debug.mail:
@@ -209,24 +209,24 @@
         resp = await self.get_response("post", data=route)
         logger.info(
             f"Created route for {domain_address}  ==> "
             f" {', '.join(forwarding_addresses)}"
         )
         return resp
 
-    async def create_routes(self, ordered=True):
+    async def create_routes(self, ordered: bool = True) -> None:
         if ac.mail.mailgun.gmail.enabled:
             logger.info("Using gmail mx servers. No routes created.")
             return
         else:
             forwards = await load.yaml(Path("mail.yml"), ordered=ordered)
             async for k, v in forwards.items():
                 await self.create_route(k, v)
 
-    def setup_mail(self):
+    def setup_mail(self) -> bool:
         self.create_dns_records()
         if not (Path("mail.yml").exists()):
             logger.info("No mail routes to configre - mail.yml not found.")
             return False
         self.delete_routes(delete_all=False)
         self.create_routes()
```

### Comparing `acb-0.1.2/acb/adapters/recaptcha/google.py` & `acb-0.1.3/acb/adapters/recaptcha/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class Recaptcha(BaseModel):
     headers = {
         "Content-type": "application/x-www-form-urlencoded",
         "Accept": "text/plain",
     }
 
-    async def init(self):
+    async def init(self) -> None:
         logger.info("Recaptcha initialized.")
 
     # def request(payload):
     #     params = urllib.parse.urlencode(payload)
     #     conn = http.client.HTTPSConnection("www.google.com")
     #     conn.request("POST", "/recaptcha/api/siteverify", params, headers)
     #     return json.loads(conn.getresponse().read())
```

### Comparing `acb-0.1.2/acb/adapters/secret/google.py` & `acb-0.1.3/acb/adapters/secret/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     google_upload_json: Optional[str]
     recaptcha_dev_key: Optional[str]
     recaptcha_production_key: Optional[str]
     app_secret_key = token_urlsafe(32)
     app_secure_salt: Optional[str] = str(token_bytes(32))
     app_mail_password: Optional[str] = gen_password(10)
 
-    def __init__(self, **data: Any):
+    def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     class Config:
         extra = "forbid"
 
 
 class SecretManager:
@@ -122,15 +122,15 @@
         path = f"projects/{self.project}/secrets/{name}/versions/latest"
         version = self.client.access_secret_version(request={"name": path})
         payload = str(version.payload.data.decode())
         if not deployed:
             logger.info(f"Fetched secret - {name.removeprefix('000_')}")
         return payload
 
-    async def create(self, name: str, value: str):
+    async def create(self, name: str, value: str) -> None:
         name = self.get_name(name)
         parent = f"projects/{self.project}"
         with suppress(AlreadyExists):
             version = self.client.create_secret(
                 request={
                     "parent": parent,
                     "secret_id": name,
@@ -142,34 +142,34 @@
                     "parent": version.name,
                     "payload": {"data": bytes(str.encode(f"{value}"))},
                 }
             )
             if not deployed:
                 logger.debug(f"Created secret - {name}")
 
-    async def update(self, name: str, value: str):
+    async def update(self, name: str, value: str) -> None:
         name = self.get_name(name)
         secret = self.client.secret_path(self.project, name)
         self.client.add_secret_version(
             request={
                 "parent": secret,
                 "payload": {"data": bytes(str.encode(f"{value}"))},
             }
         )
         if not deployed:
             logger.debug(f"Updated secret - {name}")
 
-    async def delete(self, name: str):
+    async def delete(self, name: str) -> None:
         name = self.get_name(name)
         secret = self.client.secret_path(self.project, name)
         self.client.delete_secret(request={"name": secret})
         if not deployed:
             logger.debug(f"Deleted secret - {secret}")
 
-    async def load(self, name, secrets, cls_dict):
+    async def load(self, name: str, secrets, cls_dict):
         if name not in secrets:
             await self.create(name, cls_dict[name])
         secret = await self.get(name)
         return secret
 
     async def load_all(self, cls_dict):
         secrets = await self.list()
@@ -185,15 +185,15 @@
 
     async def init(self):
         if not await AsyncPath(secret_manager.secret_dir).exists():
             return await secret_manager.load_all(AppSecrets().dict())
         else:
             return AppSecrets(_secrets_dir=secret_manager.secret_dir)
 
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.debug = None
         self.target_audience = f"https://{self.domain}"
         with catch_warnings():
             filterwarnings("ignore", category=Warning)
             creds, projects = default()
         self.creds = creds
```

### Comparing `acb-0.1.2/acb/adapters/storage/google.py` & `acb-0.1.3/acb/adapters/storage/google.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,25 +67,25 @@
     logger: Logger = None
     ic: t.Any = None
     pf: t.Any = None
 
     class Config:
         arbitrary_types_allowed = True
 
-    def __init__(self, bucket: str, prefix: str = None, **data: t.Any):
+    def __init__(self, bucket: str, prefix: str = None, **data: t.Any) -> None:
         super().__init__(**data)
         self.prefix = prefix if prefix else self.prefix
         self.bucket = (
             f"splashstand-{bucket}"
             if bucket not in [ac.storage.bucket.media, ac.storage.bucket.upload]
             else bucket
         )
         self.path = Pathy(f"gs://{self.bucket}/{self.prefix}/")
 
-    def save(self, obj_path: AsyncPath, data: t.Any):
+    def save(self, obj_path: AsyncPath, data: t.Any) -> None:
         stor_path = self.get_path(obj_path)
         logger.debug(f"Saving {stor_path}...")
         if isinstance(data, bytes):
             stor_path.write_bytes(data)
         else:
             stor_path.write_text(data)
         logger.debug(f"Saved - {stor_path}")
@@ -126,15 +126,15 @@
     upload = CloudStorageBucket(ac.storage.bucket.upload)
     database = CloudStorageBucket("database")
     settings = CloudStorageBucket("settings")
     plugins = CloudStorageBucket("plugins")
     migrations = CloudStorageBucket("migrations")
     theme = CloudStorageBucket("theme")
 
-    async def init(self):
+    async def init(self) -> None:
         set_client_params("gs", project=ac.app.project)
         use_fs_cache(root=tmp / "storage")
 
         for bucket in [
             b for b in self.__dict__.values() if isinstance(b, CloudStorageBucket)
         ]:
             ic(type(bucket))
```

### Comparing `acb-0.1.2/acb/adapters/template/jinja/bccache.py` & `acb-0.1.3/acb/adapters/template/jinja/bccache.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 from jinja2.bccache import Bucket
 
 from environment import AsyncEnvironment
 from redis.asyncio import Redis as AioRedis
 
 
 class AsyncRedisBytecodeCache(AioRedis, BytecodeCache):
-    def __init__(self, prefix: t.Optional[str] = None, **configs):
+    def __init__(self, prefix: t.Optional[str] = None, **configs) -> None:
         super().__init__(**configs)
         self.prefix = prefix
 
     def get_bucket_name(self, key):
         return ":".join([self.prefix, key])
 
     async def load_bytecode(self, key_bucket):
         code = await self.get(self.get_bucket_name(key_bucket.key))
         if code is not None:
             return key_bucket.bytecode_from_string(code)
 
-    async def dump_bytecode(self, key_bucket):
+    async def dump_bytecode(self, key_bucket) -> None:
         await self.set(
             self.get_bucket_name(key_bucket.key), key_bucket.bytecode_to_string()
         )
 
     async def get_bucket(
         self,
         environment: "AsyncEnvironment",
```

### Comparing `acb-0.1.2/acb/adapters/template/jinja/compiler.py` & `acb-0.1.3/acb/adapters/template/jinja/compiler.py`

 * *Files identical despite different names*

### Comparing `acb-0.1.2/acb/adapters/template/jinja/environment.py` & `acb-0.1.3/acb/adapters/template/jinja/environment.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 class AsyncEnvironment(Environment):
     code_generator_class = AsyncCodeGenerator
     loader: AsyncBaseLoader = None
     bytecode_cache: AsyncRedisBytecodeCache = None
 
-    def __init__(self, **env_options):
+    def __init__(self, **env_options) -> None:
         super().__init__(**env_options)
 
     @internalcode
     async def get_template(
         self,
         name: t.Union[str, "Template"],
         parent: t.Optional[str] = None,
```

### Comparing `acb-0.1.2/acb/adapters/template/jinja/loaders.py` & `acb-0.1.3/acb/adapters/template/jinja/loaders.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     """Raised if a loader is not found."""
 
 
 class AsyncBaseLoader:
     has_source_access = True
     loaders: list = None
 
-    def __init__(self, searchpath: str | AsyncPath | t.Sequence[str | AsyncPath]):
+    def __init__(
+        self, searchpath: str | AsyncPath | t.Sequence[str | AsyncPath]
+    ) -> None:
         self.searchpath = searchpath
         if not isinstance(searchpath, abc.Iterable) or isinstance(searchpath, str):
             self.searchpath = [searchpath]
         self.searchpath = [AsyncPath(p) for p in searchpath]
 
     async def get_source(
         self, environment: "AsyncEnvironment", template: str | AsyncPath
```

### Comparing `acb-0.1.2/acb/config.py` & `acb-0.1.3/acb/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     class Config:
         extra = "allow"
         arbitrary_types_allowed = True
         json_loads = load.json
         json_dumps = dump.json
 
-    def __init__(self, **values: t.Any):
+    def __init__(self, **values: t.Any) -> None:
         super().__init__(**values)
         # name = self.__class__.__name__.replace("Settings", "").lower()
         # settings = ac.basedir / "settings"
         # for path in [
         #     p for p in settings.iterdir() if p.suffix == ".yml" and p.stem == name
         # ]:
         #     self.yml_settings = path.read_text()
@@ -73,15 +73,15 @@
         #         self.formatted = True
         #     super().__init__(**values)
 
     # @classmethod
     # async def add_settings(self):
     #     setattr(ac, self.cls_name, self)
 
-    async def __call__(self, ac):
+    async def __call__(self, ac) -> None:
         print("call")
         self.cls_name = self.__class__.__name__.replace("Settings", "").lower()
         settings = ac.basedir / "settings"
         for path in [
             AsyncPath(p)
             for p in settings.iterdir()
             if p.suffix == ".yml" and p.stem == self.cls_name
```

### Comparing `acb-0.1.2/pyproject.toml` & `acb-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 [tool.pdm.dev-dependencies]
 dev = [
-    "Crackerjack @ file:///${PROJECT_ROOT}/../crackerjack",
+    "pytest>=7.3.0",
+    "icecream>=2.1.3",
+    "pre-commit>=3.2.2",
+    "crackerjack>=0.1.6",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
+fix = true
+show-fixes = true
+show-source = true
 
 [tool.ruff.isort]
-split-on-trailing-comma = true
-force-wrap-aliases = true
-force-sort-within-sections = true
 force-single-line = true
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
-[tool.isort]
-profile = "black"
-py-version = 311
-multiple-lines-output = 3
-
 [tool.black]
 target-version = [
     "py311",
 ]
 
 [tool.mypy]
 strict = true
-
-[tool.deptry]
+pretty = true
 
 [tool.refurb]
+enable_all = true
+
+[tool.pytype]
+inputs = [
+    "package_name",
+]
 
 [project]
 name = "acb"
-version = "0.1.2"
+version = "0.1.3"
 description = "Asynchronus Code Base"
-authors = [
-    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
-]
 dependencies = [
     "pydantic>=1.10.7",
     "itsdangerous>=2.1.2",
     "msgspec>=0.14.1",
     "addict>=2.4.0",
     "aiopath>=0.6.11",
     "arrow>=1.2.3",
     "google-crc32c>=1.5.0",
     "icecream>=2.1.3",
-    "httpx>=0.24.0",
     "pathy>=0.10.1",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
+authors = [
+    { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
+]
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
 Homepage = "https://github.com/lesleslie/acb"
 Documentation = "https://github.com/lesleslie/acb"
```

### Comparing `acb-0.1.2/PKG-INFO` & `acb-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.1.2
+Version: 0.1.3
 Summary: Asynchronus Code Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/lesleslie/acb
 Project-URL: Documentation, https://github.com/lesleslie/acb
 Project-URL: Repository, https://github.com/lesleslie/acb
 Requires-Python: >=3.11
@@ -12,15 +12,14 @@
 Requires-Dist: itsdangerous>=2.1.2
 Requires-Dist: msgspec>=0.14.1
 Requires-Dist: addict>=2.4.0
 Requires-Dist: aiopath>=0.6.11
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: google-crc32c>=1.5.0
 Requires-Dist: icecream>=2.1.3
-Requires-Dist: httpx>=0.24.0
 Requires-Dist: pathy>=0.10.1
 Requires-Dist: cashews[redis]>=6.0.2; extra == "cache"
 Requires-Dist: firebase-admin>=6.1.0; extra == "auth"
 Requires-Dist: google-cloud-storage>=2.8.0; extra == "storage"
 Requires-Dist: google-cloud-secret-manager>=2.16.1; extra == "secret"
 Requires-Dist: google-cloud-dns>=0.34.1; extra == "dns"
 Provides-Extra: cache
@@ -71,8 +70,7 @@
 from acb.configure import (
     AppConfig,
     AppSettings,
 )
 ```
 
 ## Adapters
-
```

