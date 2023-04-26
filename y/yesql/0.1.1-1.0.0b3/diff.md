# Comparing `tmp/yesql-0.1.1.tar.gz` & `tmp/yesql-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yesql-0.1.1.tar", max compression
+gzip compressed data, was "yesql-1.0.0b3.tar", max compression
```

## Comparing `yesql-0.1.1.tar` & `yesql-1.0.0b3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0       46 2022-01-04 02:46:42.434046 yesql-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2029 2022-09-14 14:14:39.829671 yesql-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       19 2021-11-10 12:39:13.487021 yesql-0.1.1/yesql/__init__.py
--rw-r--r--   0        0        0     5172 2022-09-13 01:54:54.697210 yesql-0.1.1/yesql/api.py
--rw-r--r--   0        0        0        0 2021-06-29 13:20:14.841205 yesql-0.1.1/yesql/bin/__init__.py
--rw-r--r--   0        0        0        0 2021-09-30 00:51:46.778888 yesql-0.1.1/yesql/core/__init__.py
--rw-r--r--   0        0        0     1824 2022-04-21 13:01:11.930982 yesql-0.1.1/yesql/core/drivers/__init__.py
--rw-r--r--   0        0        0     4856 2022-09-14 13:49:35.121831 yesql-0.1.1/yesql/core/drivers/base.py
--rw-r--r--   0        0        0     1993 2022-04-20 13:56:38.559380 yesql-0.1.1/yesql/core/drivers/postgresql/__init__.py
--rw-r--r--   0        0        0    12566 2022-04-25 16:22:07.210291 yesql-0.1.1/yesql/core/drivers/postgresql/_asyncpg.py
--rw-r--r--   0        0        0    20809 2022-04-25 16:34:05.052924 yesql-0.1.1/yesql/core/drivers/postgresql/_psycopg.py
--rw-r--r--   0        0        0     2355 2022-05-11 13:03:58.382522 yesql-0.1.1/yesql/core/middleware.py
--rw-r--r--   0        0        0    10185 2022-09-14 14:14:57.381900 yesql-0.1.1/yesql/core/parse.py
--rw-r--r--   0        0        0     6726 2022-04-20 00:15:17.090009 yesql-0.1.1/yesql/core/support.py
--rw-r--r--   0        0        0     2599 2022-09-14 14:15:38.070821 yesql-0.1.1/yesql/core/types.py
--rw-r--r--   0        0        0    11291 2022-05-10 00:28:40.729092 yesql-0.1.1/yesql/dynamic.py
--rw-r--r--   0        0        0    12833 2022-09-13 22:51:43.300358 yesql-0.1.1/yesql/repository.py
--rw-r--r--   0        0        0    15469 2022-09-13 13:25:18.788501 yesql-0.1.1/yesql/statement.py
--rw-r--r--   0        0        0     1565 2022-09-14 14:15:59.886281 yesql-0.1.1/setup.py
--rw-r--r--   0        0        0     1706 2022-09-14 14:15:59.886746 yesql-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-04-26 21:26:33.956511 yesql-1.0.0b3/LICENSE.md
+-rw-r--r--   0        0        0     2624 2023-04-26 21:26:33.956511 yesql-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/__init__.py
+-rw-r--r--   0        0        0     5117 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/api.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/bin/__init__.py
+-rw-r--r--   0        0        0      847 2023-04-26 21:26:33.956511 yesql-1.0.0b3/yesql/bin/main.py
+-rw-r--r--   0        0        0     5133 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/bin/stubgen.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/__init__.py
+-rw-r--r--   0        0        0     1878 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/__init__.py
+-rw-r--r--   0        0        0     4945 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/base.py
+-rw-r--r--   0        0        0     2056 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/__init__.py
+-rw-r--r--   0        0        0    13088 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/_asyncpg.py
+-rw-r--r--   0        0        0    21761 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/drivers/postgresql/_psycopg.py
+-rw-r--r--   0        0        0     2432 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/middleware.py
+-rw-r--r--   0        0        0    11217 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/parse.py
+-rw-r--r--   0        0        0     6988 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/support.py
+-rw-r--r--   0        0        0     2857 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/core/types.py
+-rw-r--r--   0        0        0    11577 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/dynamic.py
+-rw-r--r--   0        0        0        0 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/py.typed
+-rw-r--r--   0        0        0    13182 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/repository.py
+-rw-r--r--   0        0        0    16048 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/statement.py
+-rw-r--r--   0        0        0     7049 2023-04-26 21:26:33.972135 yesql-1.0.0b3/yesql/stubgen.py
+-rw-r--r--   0        0        0     1614 1970-01-01 00:00:00.000000 yesql-1.0.0b3/PKG-INFO
```

### Comparing `yesql-0.1.1/yesql/api.py` & `yesql-1.0.0b3/yesql/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,157 +1,153 @@
-from __future__ import annotations
-
-import functools
-import pathlib
-from typing import Any, Tuple, Type
-
-import inflection
-import typic
-
-from .core import drivers, parse, support, types
-from .core.middleware import *
-from .repository import *
-from .statement import *
-
-__all__ = (
-    "Affected",
-    "AsyncQueryRepository",
-    "BaseQueryRepository",
-    "drivers",
-    "ExplainFormatT",
-    "Many",
-    "ManyCursor",
-    "middleware",
-    "Multi",
-    "MultiCursor",
-    "parse",
-    "QueryMetadata",
-    "Raw",
-    "RawCursor",
-    "service",
-    "servicemaker",
-    "Scalar",
-    "Statement",
-    "statements",
-    "SyncQueryRepository",
-    "support",
-    "types",
-)
-
-
-def service(
-    model: types.ModelT,
-    querylib: pathlib.Path,
-    *,
-    tablename: str = None,
-    dialect: drivers.SupportedDialectsT = "postgresql",
-    isaio: bool = True,
-    exclude_fields: frozenset[str] = frozenset(),
-    scalar_queries: frozenset[str] = frozenset(),
-    executor: drivers.BaseQueryExecutor = None,
-    base_service: Type[BaseQueryRepository[types.ModelT]] = None,
-    **connect_kwargs,
-) -> AsyncQueryRepository[types.ModelT] | SyncQueryRepository[types.ModelT]:
-    """Create and instantiate a Query Service object.
-
-    Args:
-        model:
-            The data model to bind this service to.
-        querylib:
-            The directory path pointing to your queries.
-        tablename: optional
-            The name of the table for this query service.
-        dialect: defaults "postgresql"
-            The SQL Dialect of your database.
-        isaio: defaults True
-            Whether to use asyncio-based execution or syncio-based.
-        exclude_fields: optional
-            Any fields which should be automatically excluded when dumping your model.
-        scalar_queries: optional
-            Any queries in your library that do not resolve to your model.
-        base_service: optional
-            Optionally provide your own base class for your query service.
-        executor: optional
-            An externally-managed query executor to attach to the service.
-        **connect_kwargs:
-            Any connection parameters to pass to the downstream connector.
-
-    Returns:
-        An instance of a new Query Service.
-    """
-    Repository = servicemaker(
-        model=model,
-        querylib=querylib,
-        tablename=tablename,
-        dialect=dialect,
-        isaio=isaio,
-        exclude_fields=exclude_fields,
-        scalar_queries=scalar_queries,
-        base_service=base_service,  # type: ignore
-    )
-    return Repository(executor=executor, **connect_kwargs)  # type: ignore
-
-
-@functools.lru_cache(maxsize=None)
-def servicemaker(
-    model: types.ModelT,
-    querylib: pathlib.Path,
-    *,
-    tablename: str = None,
-    dialect: drivers.SupportedDialectsT = "postgresql",
-    isaio: bool = True,
-    exclude_fields: frozenset[str] = frozenset(),
-    scalar_queries: frozenset[str] = frozenset(),
-    base_repository: Type[BaseQueryRepository] = None,
-    custom_queries: Tuple[types.QueryExecutorMethodT, ...] = (),
-) -> Type[AsyncQueryRepository[types.ModelT]] | Type[SyncQueryRepository[types.ModelT]]:
-    """A factory for producing a Query Service class which can be instantiated later.
-
-    Notes:
-        This factory caches results based upon the call signature. Multiple calls with
-        the same parameters will produce the same class.
-
-    Args:
-        model:
-            The data model to bind this service to.
-        querylib:
-            The directory path pointing to your queries.
-        tablename: optional
-            The name of the table for this query service.
-        dialect: defaults "postgresql"
-            The SQL dialect for connecting to your database.
-        isaio: defaults True
-            Whether to use asyncio-based execution or sync-io-based.
-        exclude_fields: optional
-            Any fields which should be automatically excluded when dumping your model.
-        scalar_queries: optional
-            Any queries in your library that do not resolve to your model.
-        base_repository: optional
-            Optionally provide your own base class for your query service.
-        custom_queries: optional
-            Optionally provide custom implementations of query methods.
-
-    Returns:
-        A new query service class.
-    """
-    BaseRepository = base_repository or (
-        AsyncQueryRepository if isaio else SyncQueryRepository
-    )
-    tablename = tablename or typic.get_name(model).lower()  # type: ignore
-    Metadata = type(
-        f"{tablename.title()}Metadata",
-        (BaseRepository.metadata,),
-        {
-            "__querylib__": querylib,
-            "__tablename__": tablename,
-            "__dialect__": dialect,
-            "__exclude_fields__": exclude_fields,
-            "__scalar_queries__": scalar_queries,
-        },
-    )
-    namespace: dict[str, Any] = {f.__name__: f for f in custom_queries}
-    namespace.update(metadata=Metadata, model=model)
-    repo_name = inflection.camelize(
-        inflection.pluralize(tablename), uppercase_first_letter=True
-    ).title()
-    Repository = type(repo_name, (BaseRepository,), namespace)
-    return Repository
+from __future__ import annotations
+
+import functools
+import pathlib
+from typing import Any, Tuple, Type
+
+import inflection
+import typic
+
+from .core import drivers, parse, support, types
+from .core.middleware import *
+from .repository import *
+from .statement import *
+
+__all__ = (
+    "Affected",
+    "AsyncQueryRepository",
+    "BaseQueryRepository",
+    "drivers",
+    "ExplainFormatT",
+    "Many",
+    "ManyCursor",
+    "middleware",
+    "Multi",
+    "MultiCursor",
+    "parse",
+    "QueryMetadata",
+    "Raw",
+    "RawCursor",
+    "service",
+    "servicemaker",
+    "Scalar",
+    "Statement",
+    "statements",
+    "SyncQueryRepository",
+    "support",
+    "types",
+)
+
+
+def service(
+    model: types.ModelT,
+    querylib: pathlib.Path,
+    *,
+    tablename: str = None,
+    dialect: drivers.SupportedDialectsT = "postgresql",
+    isaio: bool = True,
+    exclude_fields: frozenset[str] = frozenset(),
+    scalar_queries: frozenset[str] = frozenset(),
+    executor: drivers.BaseQueryExecutor = None,
+    base_service: Type[BaseQueryRepository[types.ModelT]] = None,
+    **connect_kwargs,
+) -> AsyncQueryRepository[types.ModelT] | SyncQueryRepository[types.ModelT]:
+    """Create and instantiate a Query Service object.
+
+    Args:
+        model:
+            The data model to bind this service to.
+        querylib:
+            The directory path pointing to your queries.
+        tablename: optional
+            The name of the table for this query service.
+        dialect: defaults "postgresql"
+            The SQL Dialect of your database.
+        isaio: defaults True
+            Whether to use asyncio-based execution or syncio-based.
+        exclude_fields: optional
+            Any fields which should be automatically excluded when dumping your model.
+        scalar_queries: optional
+            Any queries in your library that do not resolve to your model.
+        base_service: optional
+            Optionally provide your own base class for your query service.
+        executor: optional
+            An externally-managed query executor to attach to the service.
+        **connect_kwargs:
+            Any connection parameters to pass to the downstream connector.
+
+    Returns:
+        An instance of a new Query Service.
+    """
+    Repository = servicemaker(
+        model=model,
+        querylib=querylib,
+        tablename=tablename,
+        dialect=dialect,
+        isaio=isaio,
+        exclude_fields=exclude_fields,
+        scalar_queries=scalar_queries,
+        base_service=base_service,  # type: ignore
+    )
+    return Repository(executor=executor, **connect_kwargs)  # type: ignore
+
+
+@functools.lru_cache(maxsize=None)
+def servicemaker(
+    model: types.ModelT,
+    querylib: pathlib.Path,
+    *,
+    tablename: str = None,
+    dialect: drivers.SupportedDialectsT = "postgresql",
+    isaio: bool = True,
+    exclude_fields: frozenset[str] = frozenset(),
+    base_repository: Type[BaseQueryRepository] = None,
+    custom_queries: Tuple[types.QueryExecutorMethodT, ...] = (),
+) -> Type[AsyncQueryRepository[types.ModelT]] | Type[SyncQueryRepository[types.ModelT]]:
+    """A factory for producing a Query Service class which can be instantiated later.
+
+    Notes:
+        This factory caches results based upon the call signature. Multiple calls with
+        the same parameters will produce the same class.
+
+    Args:
+        model:
+            The data model to bind this service to.
+        querylib:
+            The directory path pointing to your queries.
+        tablename: optional
+            The name of the table for this query service.
+        dialect: defaults "postgresql"
+            The SQL dialect for connecting to your database.
+        isaio: defaults True
+            Whether to use asyncio-based execution or sync-io-based.
+        exclude_fields: optional
+            Any fields which should be automatically excluded when dumping your model.
+        base_repository: optional
+            Optionally provide your own base class for your query service.
+        custom_queries: optional
+            Optionally provide custom implementations of query methods.
+
+    Returns:
+        A new query service class.
+    """
+    BaseRepository = base_repository or (
+        AsyncQueryRepository if isaio else SyncQueryRepository
+    )
+    tablename = tablename or typic.get_name(model).lower()  # type: ignore
+    Metadata = type(
+        f"{tablename.title()}Metadata",
+        (BaseRepository.metadata,),
+        {
+            "__querylib__": querylib,
+            "__tablename__": tablename,
+            "__dialect__": dialect,
+            "__exclude_fields__": exclude_fields,
+        },
+    )
+    namespace: dict[str, Any] = {f.__name__: f for f in custom_queries}
+    namespace.update(metadata=Metadata, model=model)
+    repo_name = inflection.camelize(
+        inflection.pluralize(tablename), uppercase_first_letter=True
+    ).title()
+    Repository = type(repo_name, (BaseRepository,), namespace)
+    return Repository
```

### Comparing `yesql-0.1.1/yesql/core/drivers/__init__.py` & `yesql-1.0.0b3/yesql/core/drivers/__init__.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from __future__ import annotations
-
-from typing import Literal, NamedTuple
-
-from yesql.core.drivers import postgresql
-from yesql.core.drivers.base import BaseQueryExecutor
-
-
-def get_driver(
-    *, dialect: SupportedDialectsT = "postgresql", aio: bool = True
-) -> Driver:
-    """Get the driver configuration for the given dialect and IO protocol.
-
-    Args:
-        dialect: The SQL dialect for the driver.
-        aio: Whether to use the asyncio-based query executor.
-
-    Raises:
-        RuntimeError: If the required SDK is not installed.
-    """
-    if dialect not in _SUPPORTED_DIALECTS:
-        raise RuntimeError(
-            f"{dialect!r} is not supported. "
-            f"Supported dialects are: {(*_SUPPORTED_DIALECTS,)}."
-        )
-    if (dialect, aio) not in _DIALECT_AIO_TO_EXECUTOR:
-        raise RuntimeError(f"{dialect!r} is not implemented for {aio=}.")
-    executor = _DIALECT_AIO_TO_EXECUTOR[(dialect, aio)]
-    if executor is NotImplemented:
-        drivers = _DIALECT_AIO_TO_DRIVERS[(dialect, aio)]
-        raise RuntimeError(f"Required driver(s) {' or '.join(drivers)} not installed.")
-    return Driver(executor=executor)
-
-
-class Driver(NamedTuple):
-    executor: type[BaseQueryExecutor]
-
-
-SupportedDialectsT = Literal["postgresql"]
-SupportedDriversT = Literal["asyncpg", "psycopg"]
-
-_SUPPORTED_DIALECTS: set[SupportedDialectsT] = {"postgresql"}
-_DIALECT_AIO_TO_EXECUTOR: dict[tuple[SupportedDialectsT, bool], type[BaseQueryExecutor]]
-_DIALECT_AIO_TO_EXECUTOR = {
-    ("postgresql", True): postgresql.AsyncQueryExecutor,
-    ("postgresql", False): postgresql.SyncQueryExecutor,
-}
-_DIALECT_AIO_TO_DRIVERS: dict[
-    tuple[SupportedDialectsT, bool], tuple[SupportedDriversT, ...]
-]
-_DIALECT_AIO_TO_DRIVERS = {
-    ("postgresql", True): ("psycopg", "asyncpg"),
-    ("postgresql", False): ("psycopg",),
-}
+from __future__ import annotations
+
+from typing import Literal, NamedTuple
+
+from yesql.core.drivers import postgresql
+from yesql.core.drivers.base import BaseQueryExecutor
+
+
+def get_driver(
+    *, dialect: SupportedDialectsT = "postgresql", aio: bool = True
+) -> Driver:
+    """Get the driver configuration for the given dialect and IO protocol.
+
+    Args:
+        dialect: The SQL dialect for the driver.
+        aio: Whether to use the asyncio-based query executor.
+
+    Raises:
+        RuntimeError: If the required SDK is not installed.
+    """
+    if dialect not in _SUPPORTED_DIALECTS:
+        raise RuntimeError(
+            f"{dialect!r} is not supported. "
+            f"Supported dialects are: {(*_SUPPORTED_DIALECTS,)}."
+        )
+    if (dialect, aio) not in _DIALECT_AIO_TO_EXECUTOR:
+        raise RuntimeError(f"{dialect!r} is not implemented for {aio=}.")
+    executor = _DIALECT_AIO_TO_EXECUTOR[(dialect, aio)]
+    if executor is NotImplemented:
+        drivers = _DIALECT_AIO_TO_DRIVERS[(dialect, aio)]
+        raise RuntimeError(f"Required driver(s) {' or '.join(drivers)} not installed.")
+    return Driver(executor=executor)
+
+
+class Driver(NamedTuple):
+    executor: type[BaseQueryExecutor]
+
+
+SupportedDialectsT = Literal["postgresql"]
+SupportedDriversT = Literal["asyncpg", "psycopg"]
+
+_SUPPORTED_DIALECTS: set[SupportedDialectsT] = {"postgresql"}
+_DIALECT_AIO_TO_EXECUTOR: dict[tuple[SupportedDialectsT, bool], type[BaseQueryExecutor]]
+_DIALECT_AIO_TO_EXECUTOR = {
+    ("postgresql", True): postgresql.AsyncQueryExecutor,
+    ("postgresql", False): postgresql.SyncQueryExecutor,
+}
+_DIALECT_AIO_TO_DRIVERS: dict[
+    tuple[SupportedDialectsT, bool], tuple[SupportedDriversT, ...]
+]
+_DIALECT_AIO_TO_DRIVERS = {
+    ("postgresql", True): ("psycopg", "asyncpg"),
+    ("postgresql", False): ("psycopg",),
+}
```

### Comparing `yesql-0.1.1/yesql/core/drivers/base.py` & `yesql-1.0.0b3/yesql/core/drivers/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,220 +1,206 @@
-from __future__ import annotations
-
-import abc
-from typing import (
-    Any,
-    Callable,
-    Collection,
-    Generic,
-    Iterable,
-    Mapping,
-    Sequence,
-    TypeVar,
-    Union,
-)
-
-from yesql.core import parse
-
-_T = TypeVar("_T")
-_CT = TypeVar("_CT")
-
-__all__ = ("BaseQueryExecutor",)
-
-
-class BaseQueryExecutor(abc.ABC, Generic[_CT]):
-    __driver__: str
-    __slots__ = ("pool", "managed", "pool_kwargs", "_lock")
-
-    def __init__(
-        self,
-        *,
-        pool=None,
-        **pool_kwargs,
-    ):
-        self.pool = pool
-        self.managed = pool is None
-        self.pool_kwargs = pool_kwargs
-
-    def __repr__(self) -> str:
-        return (
-            "<"
-            f"{self.__class__.__name__} "
-            f"managed={self.managed}, "
-            f"initialized={self.pool is not None}"
-            ">"
-        )
-
-    @abc.abstractmethod
-    def connection(self, *, timeout: float = 10, connection: _CT | None = None):
-        ...
-
-    @abc.abstractmethod
-    def transaction(
-        self,
-        *,
-        timeout: float = 10,
-        connection: _CT | None = None,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def initialize(self):
-        ...
-
-    @abc.abstractmethod
-    def teardown(self, *, timeout: int = 10):
-        ...
-
-    @abc.abstractmethod
-    def many(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        deserializer: DeserializerT[_T] | None = None,
-        **kwargs,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def many_cursor(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        ...
-
-    def raw(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        return self.many(
-            query,
-            *args,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **kwargs,
-        )
-
-    def raw_cursor(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        return self.many_cursor(
-            query,
-            *args,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **kwargs,
-        )
-
-    @abc.abstractmethod
-    def one(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        deserializer: DeserializerT[_T] | None = None,
-        **kwargs,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def scalar(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def multi(
-        self,
-        query: parse.QueryDatum,
-        *,
-        params: Iterable[Union[Sequence, Mapping[str, Any]]],
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        returns: bool = True,
-        deserializer: DeserializerT[_T] | None,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def multi_cursor(
-        self,
-        query: parse.QueryDatum,
-        *,
-        params: Iterable[Union[Sequence, Mapping[str, Any]]],
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-    ):
-        ...
-
-    @abc.abstractmethod
-    def affected(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: _CT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        ...
-
-    @classmethod
-    def get_explain_command(cls, analyze: bool = False, format: str = None) -> str:
-        options = (
-            f"{'ANALYZE, ' if analyze else ''}"
-            f"{'FORMAT ' if format else ''}"
-            f"{format or ''}"
-        )
-        if options:
-            return f"{cls.EXPLAIN_PREFIX} ({options})"
-        return cls.EXPLAIN_PREFIX
-
-    EXPLAIN_PREFIX = "EXPLAIN"
-
-
-DeserializerT = Callable[[Any], _T]
-SerializerT = Callable[[_T], Collection]
+from __future__ import annotations
+
+import abc
+from typing import Any, Generic, Iterable, Mapping, Sequence, TypeVar, Union
+
+from yesql.core import parse, types
+
+_T = TypeVar("_T")
+_CT = TypeVar("_CT")
+
+__all__ = ("BaseQueryExecutor",)
+
+
+class BaseQueryExecutor(abc.ABC, Generic[_CT]):
+    __driver__: str
+    __slots__ = ("pool", "managed", "pool_kwargs", "_lock")
+
+    def __init__(
+        self,
+        *,
+        pool=None,
+        **pool_kwargs,
+    ):
+        self.pool = pool
+        self.managed = pool is None
+        self.pool_kwargs = pool_kwargs
+
+    def __repr__(self) -> str:
+        return (
+            "<"
+            f"{self.__class__.__name__} "
+            f"managed={self.managed}, "
+            f"initialized={self.pool is not None}"
+            ">"
+        )
+
+    @abc.abstractmethod
+    def connection(self, *, timeout: float = 10, connection: _CT | None = None):
+        ...
+
+    @abc.abstractmethod
+    def transaction(
+        self,
+        *,
+        timeout: float = 10,
+        connection: _CT | None = None,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def initialize(self):
+        ...
+
+    @abc.abstractmethod
+    def teardown(self, *, timeout: int = 10):
+        ...
+
+    @abc.abstractmethod
+    def many(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        deserializer: types.DeserializerT[_T] | None = None,
+        **kwargs,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def many_cursor(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        ...
+
+    def raw(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        return self.many(
+            query,
+            *args,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **kwargs,
+        )
+
+    def raw_cursor(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        return self.many_cursor(
+            query,
+            *args,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **kwargs,
+        )
+
+    @abc.abstractmethod
+    def one(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        deserializer: types.DeserializerT[_T] | None = None,
+        **kwargs,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def scalar(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def multi(
+        self,
+        query: parse.QueryDatum,
+        *,
+        params: Iterable[Union[Sequence, Mapping[str, Any]]],
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        returns: bool = True,
+        deserializer: types.DeserializerT[_T] | None,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def multi_cursor(
+        self,
+        query: parse.QueryDatum,
+        *,
+        params: Iterable[Union[Sequence, Mapping[str, Any]]],
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+    ):
+        ...
+
+    @abc.abstractmethod
+    def affected(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: _CT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        ...
+
+    @classmethod
+    def get_explain_command(cls, analyze: bool = False, format: str = None) -> str:
+        options = (
+            f"{'ANALYZE, ' if analyze else ''}"
+            f"{'FORMAT ' if format else ''}"
+            f"{format or ''}"
+        )
+        if options:
+            return f"{cls.EXPLAIN_PREFIX} ({options})"
+        return cls.EXPLAIN_PREFIX
+
+    EXPLAIN_PREFIX = "EXPLAIN"
```

### Comparing `yesql-0.1.1/yesql/core/drivers/postgresql/__init__.py` & `yesql-1.0.0b3/yesql/core/drivers/postgresql/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-from __future__ import annotations
-
-from typing import TYPE_CHECKING, Callable
-
-if TYPE_CHECKING:
-
-    from ._asyncpg import (
-        AsyncPGConnectionSettings,
-        AsyncPGPoolSettings,
-        AsyncPGQueryExecutor,
-    )
-    from ._psycopg import (
-        AsyncPsycoPGQueryExecutor,
-        PsycoPGConnectionSettings,
-        PsycoPGPoolSettings,
-        PsycoPGQueryExecutor,
-        create_sync_pool,
-    )
-
-    AsyncQueryExecutor: type[AsyncPGQueryExecutor] | type[AsyncPsycoPGQueryExecutor]
-    SyncQueryExecutor: type[PsycoPGQueryExecutor]
-    create_async_pool: (
-        Callable[..., AsyncPGQueryExecutor] | Callable[..., AsyncPsycoPGQueryExecutor]
-    )
-
-else:
-    AsyncPGConnectionSettings = NotImplemented
-    AsyncPGPoolSettings = NotImplemented
-    AsyncQueryExecutor = NotImplemented
-    create_async_pool = NotImplemented
-    PsycoPGConnectionSettings = NotImplemented
-    PsycoPGPoolSettings = NotImplemented
-    SyncQueryExecutor = NotImplemented
-    create_sync_pool = NotImplemented
-
-    try:
-        from ._asyncpg import AsyncPGConnectionSettings, AsyncPGPoolSettings
-        from ._asyncpg import AsyncPGQueryExecutor as AsyncQueryExecutor
-        from ._asyncpg import create_pool as create_async_pool
-    except (ImportError, ModuleNotFoundError):
-        pass
-
-    try:
-        if AsyncQueryExecutor is NotImplemented:
-            from ._psycopg import (
-                AsyncPsycoPGQueryExecutor as AsyncQueryExecutor,
-                create_async_pool,
-            )
-        from ._psycopg import PsycoPGConnectionSettings, PsycoPGPoolSettings
-        from ._psycopg import PsycoPGQueryExecutor as SyncQueryExecutor
-        from ._psycopg import create_sync_pool
-    except (ImportError, ModuleNotFoundError):
-        pass
-
-
-__all__ = (
-    "AsyncPGConnectionSettings",
-    "AsyncPGPoolSettings",
-    "AsyncQueryExecutor",
-    "create_async_pool",
-    "create_sync_pool",
-    "PsycoPGConnectionSettings",
-    "PsycoPGPoolSettings",
-    "SyncQueryExecutor",
-)
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, Callable
+
+if TYPE_CHECKING:
+    from ._asyncpg import (
+        AsyncPGConnectionSettings,
+        AsyncPGPoolSettings,
+        AsyncPGQueryExecutor,
+    )
+    from ._psycopg import (
+        AsyncPsycoPGQueryExecutor,
+        PsycoPGConnectionSettings,
+        PsycoPGPoolSettings,
+        PsycoPGQueryExecutor,
+        create_sync_pool,
+    )
+
+    AsyncQueryExecutor: type[AsyncPGQueryExecutor] | type[AsyncPsycoPGQueryExecutor]
+    SyncQueryExecutor: type[PsycoPGQueryExecutor]
+    create_async_pool: (
+        Callable[..., AsyncPGQueryExecutor] | Callable[..., AsyncPsycoPGQueryExecutor]
+    )
+
+else:
+    AsyncPGConnectionSettings = NotImplemented
+    AsyncPGPoolSettings = NotImplemented
+    AsyncQueryExecutor = NotImplemented
+    create_async_pool = NotImplemented
+    PsycoPGConnectionSettings = NotImplemented
+    PsycoPGPoolSettings = NotImplemented
+    SyncQueryExecutor = NotImplemented
+    create_sync_pool = NotImplemented
+
+    try:
+        from ._asyncpg import AsyncPGConnectionSettings, AsyncPGPoolSettings
+        from ._asyncpg import AsyncPGQueryExecutor as AsyncQueryExecutor
+        from ._asyncpg import create_pool as create_async_pool
+    except (ImportError, ModuleNotFoundError):
+        pass
+
+    try:
+        if AsyncQueryExecutor is NotImplemented:
+            from ._psycopg import (
+                AsyncPsycoPGQueryExecutor as AsyncQueryExecutor,
+                create_async_pool,
+            )
+        from ._psycopg import PsycoPGConnectionSettings, PsycoPGPoolSettings
+        from ._psycopg import PsycoPGQueryExecutor as SyncQueryExecutor
+        from ._psycopg import create_sync_pool
+    except (ImportError, ModuleNotFoundError):
+        pass
+
+
+__all__ = (
+    "AsyncPGConnectionSettings",
+    "AsyncPGPoolSettings",
+    "AsyncQueryExecutor",
+    "create_async_pool",
+    "create_sync_pool",
+    "PsycoPGConnectionSettings",
+    "PsycoPGPoolSettings",
+    "SyncQueryExecutor",
+)
```

### Comparing `yesql-0.1.1/yesql/core/drivers/postgresql/_asyncpg.py` & `yesql-1.0.0b3/yesql/core/drivers/postgresql/_asyncpg.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,411 +1,411 @@
-from __future__ import annotations
-
-import asyncio
-import contextlib
-from typing import (
-    Any,
-    AsyncIterator,
-    Iterable,
-    Mapping,
-    Optional,
-    Sequence,
-    TypeVar,
-    Union,
-)
-
-import asyncpg
-import typic
-
-from yesql.core import parse, support
-from yesql.core.drivers import base
-
-__all__ = (
-    "AsyncPGQueryExecutor",
-    "AsyncPGPoolSettings",
-    "AsyncPGConnectionSettings",
-    "create_pool",
-)
-
-
-_T = TypeVar("_T")
-
-
-class AsyncPGQueryExecutor(base.BaseQueryExecutor):
-    __driver__: str = "asyncpg"
-    pool: asyncpg.Pool | None
-
-    TRANSIENT = (
-        asyncpg.DeadlockDetectedError,
-        asyncpg.TooManyConnectionsError,
-        asyncpg.PostgresConnectionError,
-    )
-
-    def __init__(
-        self,
-        *,
-        pool: asyncpg.Pool = None,
-        **pool_kwargs,
-    ):
-        super().__init__(pool=pool, **pool_kwargs)
-        self._lock = asyncio.Lock()
-
-    def __await__(self):
-        return self.initialize().__await__()
-
-    async def __aenter__(self):
-        await self.initialize()
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.teardown()
-
-    async def initialize(self):
-        if self.pool:
-            return
-        async with self._lock:
-            if self.pool:
-                return
-            self.pool = await create_pool(**self.pool_kwargs)
-
-    async def teardown(self, *, timeout: int = 10):
-        if not self.pool or not self.managed:
-            return
-        async with self._lock:
-            if not self.pool or not self.managed:
-                return
-            try:
-                await asyncio.wait_for(self.pool.close(), timeout=timeout)
-            except asyncio.TimeoutError:
-                self.pool.terminate()
-            finally:
-                self.pool = None
-
-    @contextlib.asynccontextmanager
-    async def connection(
-        self, *, timeout: float = 10, connection: asyncpg.Connection = None
-    ) -> AsyncIterator[asyncpg.Connection]:
-        await self.initialize()
-        if connection:
-            yield connection
-        else:
-            async with self.pool.acquire(timeout=timeout) as conn:
-                yield conn
-
-    @contextlib.asynccontextmanager
-    async def transaction(
-        self,
-        *,
-        timeout: float = 10,
-        connection: asyncpg.Connection = None,
-        rollback: bool = False,
-        isolation: Optional[str] = None,
-        readonly: bool = False,
-        deferrable: bool = False,
-    ) -> AsyncIterator[asyncpg.Connection]:
-        conn: asyncpg.Connection
-        async with self.connection(timeout=timeout, connection=connection) as conn:
-            tctx = (
-                RollbackTransaction(conn, isolation, readonly, deferrable)
-                if rollback
-                else conn.transaction(
-                    isolation=isolation, readonly=readonly, deferrable=deferrable
-                )
-            )
-            async with tctx:
-                yield conn
-
-    @support.retry
-    async def many(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        deserializer: base.DeserializerT[_T] | None = None,
-        **kwargs,
-    ):
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        c: asyncpg.Connection
-        async with ctx as c:
-            results = await c.fetch(
-                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
-            )
-            if results and deserializer:
-                return deserializer(results)
-            return results
-
-    @support.retry_cursor
-    @contextlib.asynccontextmanager
-    async def many_cursor(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ) -> asyncpg.connection.cursor.Cursor:
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        async with ctx as connection:
-            yield await connection.cursor(
-                query=query.sql, *self._remap_kwargs(query, args, kwargs)
-            )
-
-    @support.retry
-    async def one(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        deserializer: Optional[base.DeserializerT[_T]] = None,
-        **kwargs,
-    ):
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        c: asyncpg.Connection
-        async with ctx as c:
-            result = await c.fetchrow(
-                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
-            )
-            if result and deserializer:
-                return deserializer(result)
-            return result
-
-    @support.retry
-    async def scalar(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        c: asyncpg.Connection
-        async with ctx as c:
-            return await c.fetchval(
-                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
-            )
-
-    @support.retry
-    async def multi(
-        self,
-        query: parse.QueryDatum,
-        *,
-        params: Iterable[Union[Sequence, Mapping[str, Any]]],
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        returns: bool = False,
-        deserializer: Optional[base.DeserializerT[_T]] = None,
-    ):
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        c: asyncpg.Connection
-        async with ctx as c:
-            params = [*self._remap_multi_params(query, params)]
-            return await c.executemany(query.sql, params, timeout=timeout)
-
-    async def multi_cursor(
-        self,
-        query: parse.QueryDatum,
-        *,
-        params: Iterable[Sequence | Mapping[str, Any]],
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-    ):
-        raise TypeError("asyncpg doesn't support multi-exec cursors.")
-
-    @support.retry
-    async def affected(
-        self,
-        query: parse.QueryDatum,
-        *args,
-        connection: asyncpg.Connection = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        **kwargs,
-    ):
-        await self.initialize()
-        if transaction:
-            ctx = self.transaction(
-                timeout=timeout, connection=connection, rollback=rollback
-            )
-        else:
-            ctx = self.connection(timeout=timeout, connection=connection)
-        c: asyncpg.Connection
-        async with ctx as c:
-            response = await c.execute(
-                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
-            )
-            return self._get_affected(response)
-
-    def _remap_multi_params(
-        self, query: parse.QueryDatum, params: Iterable[Sequence | Mapping[str, Any]]
-    ):
-        return (
-            (*self._remap_kwargs(query, (), p),) if isinstance(p, Mapping) else p
-            for p in params
-        )
-
-    @staticmethod
-    def _remap_kwargs(
-        query: parse.QueryDatum, args: Sequence, kwargs: Mapping[str, Any]
-    ) -> Iterable:
-        remapped = dict(enumerate(args, start=1))
-        if kwargs:
-            if not query.remapping:
-                raise TypeError(
-                    f"{query.name!r} cannot take keyword arguments: "
-                    f"({', '.join(f'{k}={v!r}' for k, v in kwargs.items())})"
-                ) from None
-            remapped.update(
-                (query.remapping[k], kwargs[k])
-                for k in query.remapping.keys() & kwargs.keys()
-            )
-        yield from (v for i, v in sorted(remapped.items(), key=lambda o: o[0]))
-
-    @staticmethod
-    def _get_affected(response: str) -> int | None:
-        if not response:
-            return None
-        affected = response.rsplit(" ", maxsplit=1)[-1]
-        if affected.isdigit():
-            return int(affected)
-        return 0
-
-
-class RollbackTransaction:
-    """A transaction proxy which rolls back the owned transaction on exit."""
-
-    __slots__ = ("transaction",)
-
-    def __init__(
-        self,
-        connection: asyncpg.Connection,
-        isolation: Optional[str] = None,
-        readonly: bool = False,
-        deferrable: bool = False,
-    ):
-        self.transaction = connection.transaction(
-            isolation=isolation,
-            readonly=readonly,
-            deferrable=deferrable,
-        )
-
-    def __aenter__(self):
-        return self.transaction.__aenter__()
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        if exc_type is None:
-            exc_type = _Rollback
-            exc_val = _Rollback("Client-requested rollback.")
-            try:
-                return await self.transaction.__aexit__(exc_type, exc_val, exc_tb)
-            except asyncpg.InterfaceError:
-                # The transaction is either closed or errored already. Move on.
-                pass
-
-
-class _Rollback(Exception):
-    """A fake exception to pass on to the asyncpg to trigger a rollback on context exit."""
-
-    ...
-
-
-def create_pool(**overrides) -> asyncpg.Pool:
-    pool_settings = AsyncPGPoolSettings()
-    connect_settings = AsyncPGConnectionSettings()
-    kwargs = {k: v for k, v in connect_settings if v is not None}
-    kwargs.update((k, v) for k, v in pool_settings if v is not None)
-    kwargs.update(overrides)
-    kwargs.setdefault("init", _init_connection)
-    return asyncpg.create_pool(**kwargs)
-
-
-async def _init_connection(connection: asyncpg.Connection):
-    await connection.set_type_codec(
-        "jsonb",
-        encoder=support.dumpsb,
-        decoder=support.loads,
-        schema="pg_catalog",
-        format="binary",
-    )
-    await connection.set_type_codec(
-        "json",
-        encoder=support.dumps,
-        decoder=support.loads,
-        schema="pg_catalog",
-    )
-
-
-@typic.settings(prefix="POSTGRES_POOL_", aliases={"database_url": "postgres_pool_dsn"})
-class AsyncPGPoolSettings:
-    """Settings to pass into the asyncpg pool constructor."""
-
-    dsn: Optional[typic.DSN] = None
-    min_size: Optional[int] = None
-    max_size: Optional[int] = None
-    max_queries: Optional[int] = None
-    max_inactive_connection_lifetime: Optional[float] = None
-
-
-@typic.settings(
-    prefix="POSTGRES_CONNECTION_", aliases={"database_url": "postgres_connection_dsn"}
-)
-class AsyncPGConnectionSettings:
-    """Settings to pass into the asyncpg connection constructor."""
-
-    dsn: Optional[typic.DSN] = None
-    host: Optional[str] = None
-    port: Optional[str] = None
-    user: Optional[str] = None
-    password: Optional[typic.SecretStr] = None
-    passfile: Optional[typic.SecretStr] = None
-    database: Optional[str] = None
-    timeout: Optional[float] = None
-    statement_cache_size: Optional[int] = None
-    max_cached_statement_lifetime: Optional[int] = None
-    max_cacheable_statement_size: Optional[int] = None
-    command_timeout: Optional[float] = None
-    ssl: Optional[str] = None
+from __future__ import annotations
+
+import asyncio
+import contextlib
+from typing import (
+    Any,
+    AsyncIterator,
+    Iterable,
+    Mapping,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+)
+
+import asyncpg
+import typic
+
+from yesql.core import parse, support, types
+from yesql.core.drivers import base
+
+__all__ = (
+    "AsyncPGQueryExecutor",
+    "AsyncPGPoolSettings",
+    "AsyncPGConnectionSettings",
+    "create_pool",
+)
+
+
+_T = TypeVar("_T")
+
+
+class AsyncPGQueryExecutor(base.BaseQueryExecutor):
+    __driver__: str = "asyncpg"
+    pool: asyncpg.Pool | None
+
+    TRANSIENT = (
+        asyncpg.DeadlockDetectedError,
+        asyncpg.TooManyConnectionsError,
+        asyncpg.PostgresConnectionError,
+    )
+
+    def __init__(
+        self,
+        *,
+        pool: asyncpg.Pool = None,
+        **pool_kwargs,
+    ):
+        super().__init__(pool=pool, **pool_kwargs)
+        self._lock = asyncio.Lock()
+
+    def __await__(self):
+        return self.initialize().__await__()
+
+    async def __aenter__(self):
+        await self.initialize()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.teardown()
+
+    async def initialize(self):
+        if self.pool:
+            return
+        async with self._lock:
+            if self.pool:
+                return
+            self.pool = await create_pool(**self.pool_kwargs)
+
+    async def teardown(self, *, timeout: int = 10):
+        if not self.pool or not self.managed:
+            return
+        async with self._lock:
+            if not self.pool or not self.managed:
+                return
+            try:
+                await asyncio.wait_for(self.pool.close(), timeout=timeout)
+            except asyncio.TimeoutError:
+                self.pool.terminate()
+            finally:
+                self.pool = None
+
+    @contextlib.asynccontextmanager
+    async def connection(
+        self, *, timeout: float = 10, connection: asyncpg.Connection = None
+    ) -> AsyncIterator[asyncpg.Connection]:
+        await self.initialize()
+        if connection:
+            yield connection
+        else:
+            async with self.pool.acquire(timeout=timeout) as conn:
+                yield conn
+
+    @contextlib.asynccontextmanager
+    async def transaction(  # type: ignore[override]
+        self,
+        *,
+        timeout: float = 10,
+        connection: asyncpg.Connection = None,
+        rollback: bool = False,
+        isolation: Optional[str] = None,
+        readonly: bool = False,
+        deferrable: bool = False,
+    ) -> AsyncIterator[asyncpg.Connection]:
+        conn: asyncpg.Connection
+        async with self.connection(timeout=timeout, connection=connection) as conn:
+            tctx = (
+                RollbackTransaction(conn, isolation, readonly, deferrable)
+                if rollback
+                else conn.transaction(
+                    isolation=isolation, readonly=readonly, deferrable=deferrable
+                )
+            )
+            async with tctx:
+                yield conn
+
+    @support.retry
+    async def many(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        deserializer: types.DeserializerT[_T] | None = None,
+        **kwargs,
+    ):
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        c: asyncpg.Connection
+        async with ctx as c:
+            results = await c.fetch(
+                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
+            )
+            if results and deserializer:
+                return deserializer(results)
+            return results
+
+    @support.retry_cursor
+    @contextlib.asynccontextmanager
+    async def many_cursor(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ) -> AsyncIterator[asyncpg.connection.cursor.Cursor]:
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        async with ctx as connection:
+            yield await connection.cursor(
+                query=query.sql, *self._remap_kwargs(query, args, kwargs)
+            )
+
+    @support.retry
+    async def one(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        deserializer: Optional[types.DeserializerT[_T]] = None,
+        **kwargs,
+    ):
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        c: asyncpg.Connection
+        async with ctx as c:
+            result = await c.fetchrow(
+                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
+            )
+            if result and deserializer:
+                return deserializer(result)
+            return result
+
+    @support.retry
+    async def scalar(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        c: asyncpg.Connection
+        async with ctx as c:
+            return await c.fetchval(
+                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
+            )
+
+    @support.retry
+    async def multi(
+        self,
+        query: parse.QueryDatum,
+        *,
+        params: Iterable[Union[Sequence, Mapping[str, Any]]],
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        returns: bool = False,
+        deserializer: Optional[types.DeserializerT[_T]] = None,
+    ):
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        c: asyncpg.Connection
+        async with ctx as c:
+            params = [*self._remap_multi_params(query, params)]
+            return await c.executemany(query.sql, params, timeout=timeout)
+
+    async def multi_cursor(
+        self,
+        query: parse.QueryDatum,
+        *,
+        params: Iterable[Sequence | Mapping[str, Any]],
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+    ):
+        raise TypeError("asyncpg doesn't support multi-exec cursors.")
+
+    @support.retry
+    async def affected(
+        self,
+        query: parse.QueryDatum,
+        *args,
+        connection: asyncpg.Connection = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        **kwargs,
+    ):
+        await self.initialize()
+        if transaction:
+            ctx = self.transaction(
+                timeout=timeout, connection=connection, rollback=rollback
+            )
+        else:
+            ctx = self.connection(timeout=timeout, connection=connection)
+        c: asyncpg.Connection
+        async with ctx as c:
+            response = await c.execute(
+                query.sql, *self._remap_kwargs(query, args, kwargs), timeout=timeout
+            )
+            return self._get_affected(response)
+
+    def _remap_multi_params(
+        self, query: parse.QueryDatum, params: Iterable[Sequence | Mapping[str, Any]]
+    ):
+        return (
+            (*self._remap_kwargs(query, (), p),) if isinstance(p, Mapping) else p
+            for p in params
+        )
+
+    @staticmethod
+    def _remap_kwargs(
+        query: parse.QueryDatum, args: Sequence, kwargs: Mapping[str, Any]
+    ) -> Iterable:
+        remapped = dict(enumerate(args, start=1))
+        if kwargs:
+            if not query.remapping:
+                raise TypeError(
+                    f"{query.name!r} cannot take keyword arguments: "
+                    f"({', '.join(f'{k}={v!r}' for k, v in kwargs.items())})"
+                ) from None
+            remapped.update(
+                (query.remapping[k], kwargs[k])
+                for k in query.remapping.keys() & kwargs.keys()
+            )
+        yield from (v for i, v in sorted(remapped.items(), key=lambda o: o[0]))
+
+    @staticmethod
+    def _get_affected(response: str) -> int | None:
+        if not response:
+            return None
+        affected = response.rsplit(" ", maxsplit=1)[-1]
+        if affected.isdigit():
+            return int(affected)
+        return 0
+
+
+class RollbackTransaction:
+    """A transaction proxy which rolls back the owned transaction on exit."""
+
+    __slots__ = ("transaction",)
+
+    def __init__(
+        self,
+        connection: asyncpg.Connection,
+        isolation: Optional[str] = None,
+        readonly: bool = False,
+        deferrable: bool = False,
+    ):
+        self.transaction = connection.transaction(
+            isolation=isolation,
+            readonly=readonly,
+            deferrable=deferrable,
+        )
+
+    def __aenter__(self):
+        return self.transaction.__aenter__()
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is None:
+            exc_type = _Rollback
+            exc_val = _Rollback("Client-requested rollback.")
+            try:
+                return await self.transaction.__aexit__(exc_type, exc_val, exc_tb)
+            except asyncpg.InterfaceError:
+                # The transaction is either closed or errored already. Move on.
+                pass
+
+
+class _Rollback(Exception):
+    """A fake exception to pass on to the asyncpg to trigger a rollback on context exit."""
+
+    ...
+
+
+def create_pool(**overrides) -> asyncpg.Pool:
+    pool_settings = AsyncPGPoolSettings()
+    connect_settings = AsyncPGConnectionSettings()
+    kwargs = {k: v for k, v in connect_settings if v is not None}  # type: ignore[attr-defined]
+    kwargs.update((k, v) for k, v in pool_settings if v is not None)  # type: ignore[attr-defined]
+    kwargs.update(overrides)
+    kwargs.setdefault("init", _init_connection)
+    return asyncpg.create_pool(**kwargs)
+
+
+async def _init_connection(connection: asyncpg.Connection):
+    await connection.set_type_codec(
+        "jsonb",
+        encoder=support.dumpsb,
+        decoder=support.loads,
+        schema="pg_catalog",
+        format="binary",
+    )
+    await connection.set_type_codec(
+        "json",
+        encoder=support.dumps,
+        decoder=support.loads,
+        schema="pg_catalog",
+    )
+
+
+@typic.settings(prefix="POSTGRES_POOL_", aliases={"database_url": "postgres_pool_dsn"})
+class AsyncPGPoolSettings:
+    """Settings to pass into the asyncpg pool constructor."""
+
+    dsn: Optional[typic.DSN] = None
+    min_size: Optional[int] = None
+    max_size: Optional[int] = None
+    max_queries: Optional[int] = None
+    max_inactive_connection_lifetime: Optional[float] = None
+
+
+@typic.settings(
+    prefix="POSTGRES_CONNECTION_", aliases={"database_url": "postgres_connection_dsn"}
+)
+class AsyncPGConnectionSettings:
+    """Settings to pass into the asyncpg connection constructor."""
+
+    dsn: Optional[typic.DSN] = None
+    host: Optional[str] = None
+    port: Optional[str] = None
+    user: Optional[str] = None
+    password: Optional[typic.SecretStr] = None
+    passfile: Optional[typic.SecretStr] = None
+    database: Optional[str] = None
+    timeout: Optional[float] = None
+    statement_cache_size: Optional[int] = None
+    max_cached_statement_lifetime: Optional[int] = None
+    max_cacheable_statement_size: Optional[int] = None
+    command_timeout: Optional[float] = None
+    ssl: Optional[str] = None
```

### Comparing `yesql-0.1.1/yesql/core/middleware.py` & `yesql-1.0.0b3/yesql/core/middleware.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,77 @@
-try:
-    from typing import TypeGuard  # type: ignore[attr-defined]
-except (ImportError, ModuleNotFoundError):
-    from typing_extensions import TypeGuard
-
-from . import types
-
-__all__ = ("middleware",)
-
-
-def middleware(*names: str):
-    """Flag to the service that this method is a 'middleware' for the target query.
-
-    A 'middleware' method allows for pre- and post-processing of for the assigned query
-    methods. Doing so matkes the flagged callable behave more like a staticmethod than
-    a bound method.
-
-    Notes:
-        Middlewares should always be a coroutine function.
-
-    Args:
-        *names: str
-            The queries for which this middelwares should be run.
-
-    Examples:
-
-        >>> from __future__ import annotations
-        >>>
-        >>> import dataclasses
-        >>> import pathlib
-        >>> import yesql
-        >>> from tests.unit.queries import QUERIES
-        >>>
-        >>>
-        >>> @dataclasses.dataclass
-        ... class Foo:
-        ...     bar: str
-        ...
-        >>>
-        >>> class FooService(yesql.AsyncQueryRepository[Foo]):
-        ...
-        ...     class metadata(yesql.QueryMetadata):
-        ...         __querylib__ = QUERIES
-        ...
-        ...     @yesql.middleware("get", "get_cursor")
-        ...     async def intercept_gets(
-        ...         statement: yesql.Statement,
-        ...         *args,
-        ...         connection: "types.ConnectionT | None" = None,
-        ...         timeout: float = 10,
-        ...         transaction: bool = True,
-        ...         rollback: bool = False,
-        ...         **kwargs
-        ...    ) -> Foo:
-        ...         print(f"Executing {statement.query!r}.")
-        ...         ...  # do stuff to foo
-        ...         return await statement.execute(
-        ...             *args,
-        ...             connection=connection,
-        ...             timeout=timeout,
-        ...             transaction=transaction,
-        ...             rollback=rollback,
-        ...             **kwargs,
-        ...         )
-        ...
-
-    """
-
-    def _middleware_wrapper(func: types.MiddlewareMethodProtocolT):
-        func.__intercepts__ = names
-        return func
-
-    return _middleware_wrapper
-
-
-def ismiddleware(o) -> TypeGuard[types.MiddlewareMethodProtocolT]:
-    return callable(o) and hasattr(o, "__intercepts__")
+try:
+    from typing import TypeGuard  # type: ignore[attr-defined]
+except (ImportError, ModuleNotFoundError):
+    from typing_extensions import TypeGuard
+
+from . import types
+
+__all__ = ("middleware",)
+
+
+def middleware(*names: str):
+    """Flag to the service that this method is a 'middleware' for the target query.
+
+    A 'middleware' method allows for pre- and post-processing of for the assigned query
+    methods. Doing so matkes the flagged callable behave more like a staticmethod than
+    a bound method.
+
+    Notes:
+        Middlewares should always be a coroutine function.
+
+    Args:
+        *names: str
+            The queries for which this middelwares should be run.
+
+    Examples:
+
+        >>> from __future__ import annotations
+        >>>
+        >>> import dataclasses
+        >>> import pathlib
+        >>> import yesql
+        >>> from tests.unit.queries import QUERIES
+        >>>
+        >>>
+        >>> @dataclasses.dataclass
+        ... class Foo:
+        ...     bar: str
+        ...
+        >>>
+        >>> class FooService(yesql.AsyncQueryRepository[Foo]):
+        ...
+        ...     class metadata(yesql.QueryMetadata):
+        ...         __querylib__ = QUERIES
+        ...
+        ...     @yesql.middleware("get", "get_cursor")
+        ...     async def intercept_gets(
+        ...         statement: yesql.Statement,
+        ...         *args,
+        ...         connection: "types.ConnectionT | None" = None,
+        ...         timeout: float = 10,
+        ...         transaction: bool = True,
+        ...         rollback: bool = False,
+        ...         **kwargs
+        ...    ) -> Foo:
+        ...         print(f"Executing {statement.query!r}.")
+        ...         ...  # do stuff to foo
+        ...         return await statement.execute(
+        ...             *args,
+        ...             connection=connection,
+        ...             timeout=timeout,
+        ...             transaction=transaction,
+        ...             rollback=rollback,
+        ...             **kwargs,
+        ...         )
+        ...
+
+    """
+
+    def _middleware_wrapper(func: types.MiddlewareMethodProtocolT):
+        func.__intercepts__ = names
+        return func
+
+    return _middleware_wrapper
+
+
+def ismiddleware(o) -> TypeGuard[types.MiddlewareMethodProtocolT]:
+    return callable(o) and hasattr(o, "__intercepts__")
```

### Comparing `yesql-0.1.1/yesql/core/parse.py` & `yesql-1.0.0b3/yesql/core/parse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,339 +1,354 @@
-from __future__ import annotations
-
-import collections
-import dataclasses
-import functools
-import inspect
-import pathlib
-import re
-import sys
-import warnings
-from typing import TYPE_CHECKING, Deque, Final, Literal, Optional, Tuple, cast
-
-import sqlparse
-import typic
-
-if TYPE_CHECKING:
-    from yesql.core.drivers import SupportedDriversT
-
-
-__all__ = (
-    "parse",
-    "AFFECTED",
-    "MANY",
-    "MULTI",
-    "ONE",
-    "SCALAR",
-    "RAW",
-    "ModifierT",
-    "QueryPackage",
-    "QueryDatum",
-    "QueryModule",
-)
-
-
-@functools.lru_cache(maxsize=None)
-def parse(
-    queries: str | pathlib.Path,
-    *,
-    driver: SupportedDriversT,
-    modname: str | None = None,
-) -> QueryPackage:
-    """Parse a string or path, returning a QueryPackage, for building a query library."""
-
-    # If we have a raw string or a single module, create a package from that.
-    if isinstance(queries, str) or queries.is_file():
-        if isinstance(queries, pathlib.Path):
-            path = queries.parent
-            modname = modname or queries.stem
-        else:
-            path = pathlib.Path.cwd()
-            modname = modname or "<locals>"
-        module = parse_module(queries=queries, modname=modname, driver=driver)
-        return QueryPackage(name=modname, path=path, modules={module.name: module})
-    # Otherwise, traverse the package with BFS, building the query tree.
-    # Create the root package.
-    package = QueryPackage(name=modname or queries.stem, modules={}, path=queries)
-    stack: Deque[QueryPackage] = collections.deque([package])
-    while stack:
-        pkg = stack.popleft()
-        # Traverse the directory, looking for modules to parse into QueryDatum
-        for child in pkg.path.iterdir():
-            # If we found a directory, add it to the stack and attach it to the parent.
-            if child.is_dir():
-                cpkg = QueryPackage(name=child.stem, modules={}, path=child)
-                stack.append(cpkg)
-                pkg.packages[cpkg.name] = cpkg
-                continue
-            # Otherwise, parse the module and attach it to the package.
-            module = parse_module(queries=child, modname=child.stem, driver=driver)
-            pkg.modules[module.name] = module
-
-    return package
-
-
-def parse_module(
-    *, queries: str | pathlib.Path, modname: str, driver: SupportedDriversT
-) -> QueryModule:
-    if isinstance(queries, str):
-        data = {
-            datum.name: datum
-            for statement in sqlparse.parse(queries)
-            if (datum := get_query_datum(statement, driver=driver))
-        }
-        return QueryModule(modname, queries=data, path=pathlib.Path.cwd())
-    with queries.open() as file:
-        data = {
-            d.name: d
-            for statement in sqlparse.parsestream(file)
-            if (d := get_query_datum(statement, driver=driver))
-        }
-        return QueryModule(modname, queries=data, path=queries)
-
-
-def get_query_datum(
-    statement: sqlparse.sql.Statement, driver: SupportedDriversT
-) -> QueryDatum | None:
-    lead, doc, start = get_preamble(statement)
-    if not lead:
-        return None
-
-    name, modifier = get_funcop(lead)
-    if not name:
-        return None
-
-    processed: _ProcessedT = process_sql(statement, start, driver)
-    if processed is None:
-        return None
-
-    sql, sig, remapping = processed
-    return QueryDatum(
-        name=name,
-        doc=doc,
-        sql=sql,
-        signature=sig,
-        modifier=modifier,
-        remapping=remapping,
-    )
-
-
-def get_preamble(statement: sqlparse.sql.Statement) -> tuple[str, str, int]:
-    docs: list[str]
-    lead, docs, i = "", [], 0
-    gen = _iter_comments(statement)
-    i, lead = next(gen, (0, ""))
-    if not lead:
-        return "", "", 0
-    docs.extend(c for (i, c) in gen)
-    return lead, "\n".join(docs), i
-
-
-def _iter_comments(statement: sqlparse.sql.Statement):
-    for ix, token in enumerate(statement.tokens):
-        if token.is_keyword:
-            break
-        # Skip any newline or whitespace.
-        if not isinstance(token, sqlparse.sql.Comment):
-            continue
-        # Test whether we have a multiline comment.
-        token, ismultiline = next(
-            (
-                (i, multi)
-                for i in token
-                if (multi := i.ttype == sqlparse.tokens.Comment.Multiline)
-            ),
-            (token, False),
-        )
-        # If we do, extract it and yield from that.
-        if ismultiline:
-            yield from (
-                (ix, cs) for c in _split_comments(token.value) if (cs := c.strip())
-            )
-        # Otherwise, yield from the token group of single-line comments.
-        else:
-            yield from ((ix, c) for t in token.tokens if (c := _clean_comment(t.value)))
-
-
-def get_funcop(lead: str) -> tuple[str | None, ModifierT]:
-    """Extract the name of the function and the fetch-modifier."""
-
-    match = FUNC_PATTERN.match(lead)
-    if not match:
-        return None, MANY
-    name = match.group("name")
-    modifier = match.group("modifier")
-    if not modifier:
-        warnings.warn(
-            f"Unrecognized query modifier: {modifier!r}. "
-            f"Recognized modifiers are: {(*MODIFIERS,)}. "
-            f"Defaulting to {MANY!r}.",
-            stacklevel=10,
-        )
-        modifier = MANY
-    elif modifier in _SHORT_TO_LONG:
-        modifier = _SHORT_TO_LONG[modifier]
-    return name, cast(ModifierT, modifier)
-
-
-def process_sql(
-    statement: sqlparse.sql.Statement,
-    start: int,
-    driver: SupportedDriversT,
-) -> _ProcessedT:
-    op = statement.get_type()
-    if op is None:
-        return None
-    posargs, kwdargs = {}, {}
-    for token in statement.tokens[start:]:
-        pos, kwd = _gather_parameters(token)
-        posargs.update(pos)
-        kwdargs.update(kwd)
-
-    sig = inspect.Signature([*posargs.values(), *kwdargs.values()])
-    sql, remapping = _normalize_parameters(str(statement), driver, posargs, kwdargs)
-    return sql, sig, remapping
-
-
-def _gather_parameters(
-    token: sqlparse.tokens.Token,
-) -> tuple[dict[str, inspect.Parameter], dict[str, inspect.Parameter]]:
-    kwdargs = {}
-    posargs = {}
-    argnum = 0
-    for token in token.flatten():
-        if not token.ttype == sqlparse.tokens.Name.Placeholder:
-            continue
-        name = token.value[2:-2] if token.value.startswith("%(") else token.value[1:]
-        if not name:
-            argnum += 1
-            name = str(argnum)
-        if name.isdigit():
-            name = f"arg{name}"
-            kind = inspect.Parameter.POSITIONAL_ONLY
-            posargs[token.value] = inspect.Parameter(name, kind)
-            continue
-        kwdargs[token.value] = inspect.Parameter(name, inspect.Parameter.KEYWORD_ONLY)
-    return posargs, kwdargs
-
-
-def _normalize_parameters(
-    statement: str,
-    driver: SupportedDriversT,
-    posargs: dict[str, inspect.Parameter],
-    kwdargs: dict[str, inspect.Parameter],
-) -> tuple[str, dict[str, int] | None]:
-    sql, remapping = statement, None
-    if not kwdargs:
-        return sql, remapping
-
-    if driver == "asyncpg":
-        remapping = {}
-        start = 1
-        if posargs:
-            start = [int(a.name.replace("arg", "")) for a in posargs.values()][-1] + 1
-        for i, (name, param) in enumerate(kwdargs.items(), start=start):
-            sql = _replace(name=name, replacement=f"${i}", sql=sql)
-            remapping[param.name] = i
-    elif driver == "psycopg":
-        for name, param in kwdargs.items():
-            sql = _replace(name=name, replacement=f"%({param.name})s", sql=sql)
-    return sql, remapping
-
-
-def _replace(*, name: str, replacement: str, sql: str) -> str:
-    return re.sub(r"(?<!:)" + name, replacement, sql)
-
-
-if sys.version_info >= (3, 9):
-
-    def _clean_comment(comment: str) -> str:
-        return comment.strip().removeprefix(_PRE).strip()
-
-    def _split_comments(comment: str) -> list[str]:
-        return [
-            c.strip()
-            for c in comment.strip()
-            .removeprefix("/**")
-            .removesuffix("**/")
-            .strip()
-            .splitlines()
-        ]
-
-else:
-
-    def _clean_comment(comment: str) -> str:
-        return comment.strip().strip(_PRE).strip()
-
-    def _split_comments(comment: str) -> list[str]:
-        return [
-            c.strip()
-            for c in comment.strip().strip("/**").rstrip("**/").strip().splitlines()
-        ]
-
-
-_PRE = "--"
-
-FUNC_PATTERN = re.compile(
-    # The name of the query
-    r":name\s+(?P<name>(\w+([-_])?\w+)+)"
-    # The operation modifier
-    r"(\s+:(?P<modifier>[*^$!#~]|many|one|scalar|multi|affected|raw))?"
-)
-
-MANY: Final = "many"
-ONE: Final = "one"
-SCALAR: Final = "scalar"
-MULTI: Final = "multi"
-AFFECTED: Final = "affected"
-RAW: Final = "raw"
-MODIFIERS = frozenset((MANY, ONE, SCALAR, MULTI, AFFECTED, RAW))
-ModifierT = Literal["many", "one", "scalar", "multi", "affected", "raw"]
-_SHORT_TO_LONG: dict[str, ModifierT] = {
-    "*": MANY,
-    "^": ONE,
-    "$": SCALAR,
-    "!": MULTI,
-    "#": AFFECTED,
-    "~": RAW,
-}
-_ProcessedT = Optional[Tuple[str, inspect.Signature, Optional[dict]]]
-
-
-@typic.slotted(dict=False, weakref=True)
-@dataclasses.dataclass(frozen=True)
-class QueryDatum:
-    name: str
-    doc: str
-    sql: str
-    signature: inspect.Signature
-    modifier: ModifierT
-    remapping: dict | None = dataclasses.field(default=None, hash=False)
-
-
-@typic.slotted(dict=False, weakref=True)
-@dataclasses.dataclass
-class QueryModule:
-    name: str
-    path: pathlib.Path
-    queries: dict[str, QueryDatum]
-
-    def __getattr__(self, item: str) -> QueryDatum:
-        if item not in self.queries:
-            raise AttributeError(f"{item!r}")
-        return self.queries[item]
-
-
-@typic.slotted(dict=False, weakref=True)
-@dataclasses.dataclass
-class QueryPackage:
-    name: str
-    path: pathlib.Path
-    modules: dict[str, QueryModule] = dataclasses.field(default_factory=dict)
-    packages: dict[str, QueryPackage] = dataclasses.field(default_factory=dict)
-
-    def __getattr__(self, item: str) -> QueryModule | QueryPackage:
-        if item in self.packages:
-            return self.packages[item]
-        if item in self.modules:
-            return self.modules[item]
-        raise AttributeError(f"{item!r}")
+from __future__ import annotations
+
+import collections
+import dataclasses
+import functools
+import inspect
+import pathlib
+import re
+import sys
+import warnings
+from typing import TYPE_CHECKING, Deque, Final, Literal, Optional, Tuple, cast
+
+import sqlparse
+import typic
+
+if TYPE_CHECKING:
+    from yesql.core.drivers import SupportedDriversT
+
+
+__all__ = (
+    "parse",
+    "AFFECTED",
+    "MANY",
+    "MULTI",
+    "ONE",
+    "SCALAR",
+    "RAW",
+    "ModifierT",
+    "QueryPackage",
+    "QueryDatum",
+    "QueryModule",
+)
+
+
+@functools.lru_cache(maxsize=None)
+def parse(
+    queries: str | pathlib.Path,
+    *,
+    driver: SupportedDriversT,
+    modname: str | None = None,
+) -> QueryPackage:
+    """Parse a string or path, returning a QueryPackage, for building a query library.
+
+    Args:
+        queries:
+            Either the query/queries as string, or a pathlib.Path object pointing
+            to a query library.
+    Keyword Args:
+        driver:
+            The SDK which is in use for this query library. The driver name affects how
+            parameters are normalized in your query library to comply with the format
+            style of the SDK.
+        modname: optional
+            The name root name of the "module" for this library. Defaults to the name
+            of the root directory or file of the query library.
+    """
+
+    # If we have a raw string or a single module, create a package from that.
+    if isinstance(queries, str) or queries.is_file():
+        if isinstance(queries, pathlib.Path):
+            path = queries.parent
+            modname = modname or queries.stem
+        else:
+            path = pathlib.Path.cwd()
+            modname = modname or "<locals>"
+        module = parse_module(queries=queries, modname=modname, driver=driver)
+        return QueryPackage(name=modname, path=path, modules={module.name: module})
+    # Otherwise, traverse the package with BFS, building the query tree.
+    # Create the root package.
+    package = QueryPackage(name=modname or queries.stem, modules={}, path=queries)
+    stack: Deque[QueryPackage] = collections.deque([package])
+    while stack:
+        pkg = stack.popleft()
+        # Traverse the directory, looking for modules to parse into QueryDatum
+        for child in pkg.path.iterdir():
+            # If we found a directory, add it to the stack and attach it to the parent.
+            if child.is_dir() and child.name != "__pycache__":
+                cpkg = QueryPackage(name=child.stem, modules={}, path=child)
+                stack.append(cpkg)
+                pkg.packages[cpkg.name] = cpkg
+                continue
+            if child.suffix != ".sql":
+                continue
+            # Otherwise, parse the module and attach it to the package.
+            module = parse_module(queries=child, modname=child.stem, driver=driver)
+            pkg.modules[module.name] = module
+
+    return package
+
+
+def parse_module(
+    *, queries: str | pathlib.Path, modname: str, driver: SupportedDriversT
+) -> QueryModule:
+    if isinstance(queries, str):
+        data = {
+            datum.name: datum
+            for statement in sqlparse.parse(queries)
+            if (datum := get_query_datum(statement, driver=driver))
+        }
+        return QueryModule(modname, queries=data, path=pathlib.Path.cwd())
+    with queries.open() as file:
+        data = {
+            d.name: d
+            for statement in sqlparse.parsestream(file)
+            if (d := get_query_datum(statement, driver=driver))
+        }
+        return QueryModule(modname, queries=data, path=queries)
+
+
+def get_query_datum(
+    statement: sqlparse.sql.Statement, driver: SupportedDriversT
+) -> QueryDatum | None:
+    lead, doc, start = get_preamble(statement)
+    if not lead:
+        return None
+
+    name, modifier = get_funcop(lead)
+    if not name:
+        return None
+
+    processed: _ProcessedT = process_sql(statement, start, driver)
+    if processed is None:
+        return None
+
+    sql, sig, remapping = processed
+    return QueryDatum(
+        name=name,
+        doc=doc,
+        sql=sql,
+        signature=sig,
+        modifier=modifier,
+        remapping=remapping,
+    )
+
+
+def get_preamble(statement: sqlparse.sql.Statement) -> tuple[str, str, int]:
+    docs: list[str]
+    lead, docs, i = "", [], 0
+    gen = _iter_comments(statement)
+    i, lead = next(gen, (0, ""))
+    if not lead:
+        return "", "", 0
+    docs.extend(c for (i, c) in gen)
+    return lead, "\n".join(docs), i
+
+
+def _iter_comments(statement: sqlparse.sql.Statement):
+    for ix, token in enumerate(statement.tokens):
+        # We've encountered a sql statement, halt processing.
+        if token.is_keyword:
+            break
+        # Skip any newline or whitespace.
+        if not isinstance(token, sqlparse.sql.Comment):
+            continue
+        # Test whether we have a multiline comment.
+        token, ismultiline = next(
+            (
+                (i, multi)
+                for i in token
+                if (multi := i.ttype == sqlparse.tokens.Comment.Multiline)
+            ),
+            (token, False),
+        )
+        # If we do, extract it and yield from that.
+        if ismultiline:
+            yield from (
+                (ix, cs) for c in _split_comments(token.value) if (cs := c.strip())
+            )
+        # Otherwise, yield from the token group of single-line comments.
+        else:
+            yield from ((ix, c) for t in token.tokens if (c := _clean_comment(t.value)))
+
+
+def get_funcop(lead: str) -> tuple[str | None, ModifierT]:
+    """Extract the name of the function and the fetch-modifier."""
+
+    match = FUNC_PATTERN.match(lead)
+    if not match:
+        return None, MANY
+    name = match.group("name")
+    modifier = match.group("modifier")
+    if not modifier:
+        warnings.warn(
+            f"Unrecognized query modifier: {modifier!r}. "
+            f"Recognized modifiers are: {(*MODIFIERS,)}. "
+            f"Defaulting to {MANY!r}.",
+            stacklevel=10,
+        )
+        modifier = MANY
+    elif modifier in _SHORT_TO_LONG:
+        modifier = _SHORT_TO_LONG[modifier]
+    return name, cast(ModifierT, modifier)
+
+
+def process_sql(
+    statement: sqlparse.sql.Statement,
+    start: int,
+    driver: SupportedDriversT,
+) -> _ProcessedT:
+    op = statement.get_type()
+    if op is None:
+        return None
+    posargs, kwdargs = {}, {}
+    for token in statement.tokens[start:]:
+        pos, kwd = _gather_parameters(token)
+        posargs.update(pos)
+        kwdargs.update(kwd)
+
+    sig = inspect.Signature([*posargs.values(), *kwdargs.values()])
+    sql, remapping = _normalize_parameters(str(statement), driver, posargs, kwdargs)
+    return sql, sig, remapping
+
+
+def _gather_parameters(
+    token: sqlparse.tokens.Token,
+) -> tuple[dict[str, inspect.Parameter], dict[str, inspect.Parameter]]:
+    kwdargs = {}
+    posargs = {}
+    argnum = 0
+    for token in token.flatten():
+        if not token.ttype == sqlparse.tokens.Name.Placeholder:
+            continue
+        name = token.value[2:-2] if token.value.startswith("%(") else token.value[1:]
+        if not name:
+            argnum += 1
+            name = str(argnum)
+        if name.isdigit():
+            name = f"arg{name}"
+            kind = inspect.Parameter.POSITIONAL_ONLY
+            posargs[token.value] = inspect.Parameter(name, kind)
+            continue
+        kwdargs[token.value] = inspect.Parameter(name, inspect.Parameter.KEYWORD_ONLY)
+    return posargs, kwdargs
+
+
+def _normalize_parameters(
+    statement: str,
+    driver: SupportedDriversT,
+    posargs: dict[str, inspect.Parameter],
+    kwdargs: dict[str, inspect.Parameter],
+) -> tuple[str, dict[str, int] | None]:
+    sql, remapping = statement, None
+    if not kwdargs:
+        return sql, remapping
+
+    if driver == "asyncpg":
+        remapping = {}
+        start = 1
+        if posargs:
+            start = [int(a.name.replace("arg", "")) for a in posargs.values()][-1] + 1
+        for i, (name, param) in enumerate(kwdargs.items(), start=start):
+            sql = _replace(name=name, replacement=f"${i}", sql=sql)
+            remapping[param.name] = i
+    elif driver == "psycopg":
+        for name, param in kwdargs.items():
+            sql = _replace(name=name, replacement=f"%({param.name})s", sql=sql)
+    return sql, remapping
+
+
+def _replace(*, name: str, replacement: str, sql: str) -> str:
+    return re.sub(r"(?<!:)" + name, replacement, sql)
+
+
+if sys.version_info >= (3, 9):
+
+    def _clean_comment(comment: str) -> str:
+        return comment.strip().removeprefix(_PRE).strip()
+
+    def _split_comments(comment: str) -> list[str]:
+        return [
+            c.strip()
+            for c in comment.strip()
+            .removeprefix("/**")
+            .removesuffix("**/")
+            .splitlines()
+        ]
+
+else:
+
+    def _clean_comment(comment: str) -> str:
+        return comment.strip().strip(_PRE).strip()
+
+    def _split_comments(comment: str) -> list[str]:
+        return [
+            c.strip() for c in comment.strip().strip("/**").rstrip("**/").splitlines()
+        ]
+
+
+_PRE = "--"
+
+FUNC_PATTERN = re.compile(
+    # The name of the query
+    r":name\s+(?P<name>(\w+([-_])?\w+)+)"
+    # The operation modifier
+    r"(\s+:(?P<modifier>[*^$!#~]|many|one|scalar|multi|affected|raw))?"
+)
+
+MANY: Final = "many"
+ONE: Final = "one"
+SCALAR: Final = "scalar"
+MULTI: Final = "multi"
+AFFECTED: Final = "affected"
+RAW: Final = "raw"
+MODIFIERS = frozenset((MANY, ONE, SCALAR, MULTI, AFFECTED, RAW))
+ModifierT = Literal["many", "one", "scalar", "multi", "affected", "raw"]
+_SHORT_TO_LONG: dict[str, ModifierT] = {
+    "*": MANY,
+    "^": ONE,
+    "$": SCALAR,
+    "!": MULTI,
+    "#": AFFECTED,
+    "~": RAW,
+}
+_ProcessedT = Optional[Tuple[str, inspect.Signature, Optional[dict]]]
+
+
+@typic.slotted(dict=False, weakref=True)
+@dataclasses.dataclass(frozen=True)
+class QueryDatum:
+    name: str
+    doc: str
+    sql: str
+    signature: inspect.Signature
+    modifier: ModifierT
+    remapping: dict | None = dataclasses.field(default=None, hash=False)
+
+
+@typic.slotted(dict=False, weakref=True)
+@dataclasses.dataclass
+class QueryModule:
+    name: str
+    path: pathlib.Path
+    queries: dict[str, QueryDatum]
+
+    def __getattr__(self, item: str) -> QueryDatum:
+        if item not in self.queries:
+            raise AttributeError(f"{item!r}")
+        return self.queries[item]
+
+
+@typic.slotted(dict=False, weakref=True)
+@dataclasses.dataclass
+class QueryPackage:
+    name: str
+    path: pathlib.Path
+    modules: dict[str, QueryModule] = dataclasses.field(default_factory=dict)
+    packages: dict[str, QueryPackage] = dataclasses.field(default_factory=dict)
+
+    def __getattr__(self, item: str) -> QueryModule | QueryPackage:
+        if item in self.packages:
+            return self.packages[item]
+        if item in self.modules:
+            return self.modules[item]
+        raise AttributeError(f"{item!r}")
```

### Comparing `yesql-0.1.1/yesql/core/support.py` & `yesql-1.0.0b3/yesql/core/support.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,262 +1,262 @@
-from __future__ import annotations
-
-import asyncio
-import dataclasses
-import functools
-import inspect
-import time
-import typing
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    AsyncContextManager,
-    Awaitable,
-    Callable,
-    ContextManager,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-)
-
-import orjson
-import typic
-
-if TYPE_CHECKING:
-    from yesql.core import types
-
-
-__all__ = (
-    "retry",
-    "retry_cursor",
-    "dumps",
-    "dumpsb",
-    "loads",
-)
-
-_T = TypeVar("_T")
-
-
-def retry(
-    func: Callable[..., Awaitable[_T]] | Callable[..., _T] = None,
-    /,
-    *errors: type[BaseException],
-    retries: int = 10,
-    delay: float = 0.1,
-    isaio: bool = False,
-):
-    """Automatically retry a database operation on a transient error.
-
-    "Transient" errors are configured by the query executor.
-    """
-
-    def _retry_impl(
-        func_: Callable[..., Awaitable[_T]] | Callable[..., _T],
-        *,
-        _retries: int = retries,
-        _errors: tuple[type[BaseException], ...] = errors,
-    ):
-        _isaio = isaio or _isasync(func_)
-        if _isaio:
-            afunc = cast(Callable[..., Awaitable[_T]], func_)
-
-            @functools.wraps(afunc)
-            async def _retry(self: types.RepositoryProtocolT, *args, **kwargs):
-                errs = (*_errors, *self.TRANSIENT)
-                async with _AsyncRetryContext(
-                    svc=self,
-                    func=afunc,
-                    args=args,
-                    kwargs=kwargs,
-                    errors=errs,
-                    retries=_retries,
-                    delay=delay,
-                ) as result:
-                    return result
-
-        else:
-
-            @functools.wraps(func_)
-            def _retry(self: types.RepositoryProtocolT, *args, **kwargs):
-                errs = (*_errors, *self.TRANSIENT)
-                with _SyncRetryContext(
-                    svc=self,
-                    func=func_,
-                    args=args,
-                    kwargs=kwargs,
-                    errors=errs,
-                    retries=_retries,
-                    delay=delay,
-                ) as result:
-                    return result
-
-        return _retry
-
-    return _retry_impl(func) if func else _retry_impl
-
-
-def retry_cursor(
-    func: Callable[..., AsyncContextManager] | Callable[..., ContextManager] = None,
-    /,
-    *errors: Type[BaseException],
-    retries: int = 10,
-    delay: float = 0.1,
-    isaio: bool = False,
-):
-    """Automatically retry a database operation on a transient error.
-
-    "Transient" errors are configured by the connector protocol.
-    """
-
-    def _retry_impl(
-        func_: Callable[..., Union[AsyncContextManager, ContextManager]],
-        *,
-        _retries: int = retries,
-        _errors: tuple[type[BaseException], ...] = errors,
-    ):
-        _isaio = isaio or _isasync(func_)
-        context_cls = _AsyncRetryCursorContext if _isaio else _SyncRetryCursorContext
-
-        @functools.wraps(func_)
-        def _retry_cursor(self: types.RepositoryProtocolT, *args, **kwargs):
-            errs = (*_errors, *self.TRANSIENT)
-            return context_cls(
-                svc=self,
-                func=func_,
-                args=args,
-                kwargs=kwargs,
-                errors=errs,
-                retries=retries,
-                delay=delay,
-            )
-
-        return _retry_cursor
-
-    return _retry_impl(func) if func else _retry_impl
-
-
-@typic.slotted(dict=False, weakref=True)
-@dataclasses.dataclass
-class _RetryContext:
-    svc: types.RepositoryProtocolT
-    func: Callable
-    args: tuple
-    kwargs: dict
-    errors: tuple[Type[BaseException], ...]
-    retries: int
-    delay: float
-
-    def _do_exec(self):
-        return self.func(self.svc, *self.args, **self.kwargs)
-
-
-class _SyncRetryContext(_RetryContext):
-    def __enter__(self):
-        do, tries, retries, errors, delay = (
-            self._do_exec,
-            0,
-            self.retries,
-            self.errors,
-            self.delay,
-        )
-        try:
-            return do()
-        except errors as e:
-            time.sleep(delay)
-            while tries < retries:
-                tries += 1
-                try:
-                    return do()
-                except errors:
-                    time.sleep(delay)
-            raise e
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        pass
-
-
-class _SyncRetryCursorContext(_SyncRetryContext):
-    __slots__ = ("ctx",)
-
-    func: Callable[..., ContextManager]
-
-    def _do_exec(self):
-        self.ctx = self.func(self.svc, *self.args, **self.kwargs)
-        return self.ctx.__enter__()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        return self.ctx.__exit__(exc_type, exc_val, exc_tb)
-
-
-class _AsyncRetryContext(_RetryContext):
-    async def __aenter__(self):
-        do, tries, retries, errors, delay = (
-            self._do_exec,
-            0,
-            self.retries,
-            self.errors,
-            self.delay,
-        )
-        try:
-            return await do()
-        except errors as e:
-            await asyncio.sleep(delay)
-            while tries < retries:
-                tries += 1
-                try:
-                    return await do()
-                except errors:
-                    await asyncio.sleep(delay)
-            raise e
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        pass
-
-
-class _AsyncRetryCursorContext(_AsyncRetryContext):
-    __slots__ = ("ctx",)
-
-    def _do_exec(self):
-        self.ctx = self.func(self.svc, *self.args, **self.kwargs)
-        return self.ctx.__aenter__()
-
-    def __aexit__(self, exc_type, exc_val, exc_tb):
-        return self.ctx.__aexit__(exc_type, exc_val, exc_tb)
-
-
-def _isasync(f):
-    unwrapped = inspect.unwrap(f)
-    hints = typic.get_type_hints(unwrapped)
-    returns = oreturns = hints.get("returns")
-    if returns:
-        oreturns = typing.get_origin(returns)
-    return (
-        inspect.iscoroutinefunction(unwrapped)
-        or inspect.isasyncgenfunction(unwrapped)
-        or typic.get_name(oreturns)
-        in {
-            "Awaitable",
-            "AsyncIterable",
-            "AsyncIterator",
-            "AsyncGenerator",
-            "Coroutine",
-        }
-    )
-
-
-def dumpsb(o: Any) -> bytes:
-    """Encode any object to a JSON byte-string."""
-    return orjson.dumps(typic.primitive(o))
-
-
-def dumps(o: Any) -> str:
-    """Encode any object to a JSON string."""
-
-    # orjson encodes to binary, but libpq (the c bindings for postgres)
-    # can't write binary data to JSONB columns.
-    # https://github.com/lib/pq/issues/528
-    # This is still orders of magnitude faster than any other lib.
-    return orjson.dumps(typic.primitive(o)).decode()
-
-
-loads = orjson.loads
+from __future__ import annotations
+
+import asyncio
+import dataclasses
+import functools
+import inspect
+import time
+import typing
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    AsyncContextManager,
+    Awaitable,
+    Callable,
+    ContextManager,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import orjson
+import typic
+
+if TYPE_CHECKING:
+    from yesql.core import types
+
+
+__all__ = (
+    "retry",
+    "retry_cursor",
+    "dumps",
+    "dumpsb",
+    "loads",
+)
+
+_T = TypeVar("_T")
+
+
+def retry(
+    func: Callable[..., Awaitable[_T]] | Callable[..., _T] = None,
+    /,
+    *errors: type[BaseException],
+    retries: int = 10,
+    delay: float = 0.1,
+    isaio: bool = False,
+):
+    """Automatically retry a database operation on a transient error.
+
+    "Transient" errors are configured by the query executor.
+    """
+
+    def _retry_impl(
+        func_: Callable[..., Awaitable[_T]] | Callable[..., _T],
+        *,
+        _retries: int = retries,
+        _errors: tuple[type[BaseException], ...] = errors,
+    ):
+        _isaio = isaio or _isasync(func_)
+        if _isaio:
+            afunc = cast(Callable[..., Awaitable[_T]], func_)
+
+            @functools.wraps(afunc)
+            async def _retry(self: types.RepositoryProtocolT, *args, **kwargs):
+                errs = (*_errors, *self.TRANSIENT)
+                async with _AsyncRetryContext(
+                    svc=self,
+                    func=afunc,
+                    args=args,
+                    kwargs=kwargs,
+                    errors=errs,
+                    retries=_retries,
+                    delay=delay,
+                ) as result:
+                    return result
+
+        else:
+
+            @functools.wraps(func_)
+            def _retry(self: types.RepositoryProtocolT, *args, **kwargs):
+                errs = (*_errors, *self.TRANSIENT)
+                with _SyncRetryContext(
+                    svc=self,
+                    func=func_,
+                    args=args,
+                    kwargs=kwargs,
+                    errors=errs,
+                    retries=_retries,
+                    delay=delay,
+                ) as result:
+                    return result
+
+        return _retry
+
+    return _retry_impl(func) if func else _retry_impl
+
+
+def retry_cursor(
+    func: Callable[..., AsyncContextManager] | Callable[..., ContextManager] = None,
+    /,
+    *errors: Type[BaseException],
+    retries: int = 10,
+    delay: float = 0.1,
+    isaio: bool = False,
+):
+    """Automatically retry a database operation on a transient error.
+
+    "Transient" errors are configured by the connector protocol.
+    """
+
+    def _retry_impl(
+        func_: Callable[..., Union[AsyncContextManager, ContextManager]],
+        *,
+        _retries: int = retries,
+        _errors: tuple[type[BaseException], ...] = errors,
+    ):
+        _isaio = isaio or _isasync(func_)
+        context_cls = _AsyncRetryCursorContext if _isaio else _SyncRetryCursorContext
+
+        @functools.wraps(func_)
+        def _retry_cursor(self: types.RepositoryProtocolT, *args, **kwargs):
+            errs = (*_errors, *self.TRANSIENT)
+            return context_cls(
+                svc=self,
+                func=func_,
+                args=args,
+                kwargs=kwargs,
+                errors=errs,
+                retries=retries,
+                delay=delay,
+            )
+
+        return _retry_cursor
+
+    return _retry_impl(func) if func else _retry_impl
+
+
+@typic.slotted(dict=False, weakref=True)
+@dataclasses.dataclass
+class _RetryContext:
+    svc: types.RepositoryProtocolT
+    func: Callable
+    args: tuple
+    kwargs: dict
+    errors: tuple[Type[BaseException], ...]
+    retries: int
+    delay: float
+
+    def _do_exec(self):
+        return self.func(self.svc, *self.args, **self.kwargs)
+
+
+class _SyncRetryContext(_RetryContext):
+    def __enter__(self):
+        do, tries, retries, errors, delay = (
+            self._do_exec,
+            0,
+            self.retries,
+            self.errors,
+            self.delay,
+        )
+        try:
+            return do()
+        except errors as e:
+            time.sleep(delay)
+            while tries < retries:
+                tries += 1
+                try:
+                    return do()
+                except errors:
+                    time.sleep(delay)
+            raise e
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+
+class _SyncRetryCursorContext(_SyncRetryContext):
+    __slots__ = ("ctx",)
+
+    func: Callable[..., ContextManager]
+
+    def _do_exec(self):
+        self.ctx = self.func(self.svc, *self.args, **self.kwargs)
+        return self.ctx.__enter__()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        return self.ctx.__exit__(exc_type, exc_val, exc_tb)
+
+
+class _AsyncRetryContext(_RetryContext):
+    async def __aenter__(self):
+        do, tries, retries, errors, delay = (
+            self._do_exec,
+            0,
+            self.retries,
+            self.errors,
+            self.delay,
+        )
+        try:
+            return await do()
+        except errors as e:
+            await asyncio.sleep(delay)
+            while tries < retries:
+                tries += 1
+                try:
+                    return await do()
+                except errors:
+                    await asyncio.sleep(delay)
+            raise e
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        pass
+
+
+class _AsyncRetryCursorContext(_AsyncRetryContext):
+    __slots__ = ("ctx",)
+
+    def _do_exec(self):
+        self.ctx = self.func(self.svc, *self.args, **self.kwargs)
+        return self.ctx.__aenter__()
+
+    def __aexit__(self, exc_type, exc_val, exc_tb):
+        return self.ctx.__aexit__(exc_type, exc_val, exc_tb)
+
+
+def _isasync(f):
+    unwrapped = inspect.unwrap(f)
+    hints = typic.get_type_hints(unwrapped)
+    returns = oreturns = hints.get("returns")
+    if returns:
+        oreturns = typing.get_origin(returns)
+    return (
+        inspect.iscoroutinefunction(unwrapped)
+        or inspect.isasyncgenfunction(unwrapped)
+        or typic.get_name(oreturns)
+        in {
+            "Awaitable",
+            "AsyncIterable",
+            "AsyncIterator",
+            "AsyncGenerator",
+            "Coroutine",
+        }
+    )
+
+
+def dumpsb(o: Any) -> bytes:
+    """Encode any object to a JSON byte-string."""
+    return orjson.dumps(typic.primitive(o))
+
+
+def dumps(o: Any) -> str:
+    """Encode any object to a JSON string."""
+
+    # orjson encodes to binary, but libpq (the c bindings for postgres)
+    # can't write binary data to JSONB columns.
+    # https://github.com/lib/pq/issues/528
+    # This is still orders of magnitude faster than any other lib.
+    return orjson.dumps(typic.primitive(o)).decode()
+
+
+loads = orjson.loads
```

### Comparing `yesql-0.1.1/yesql/dynamic.py` & `yesql-1.0.0b3/yesql/dynamic.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,300 +1,300 @@
-from __future__ import annotations
-
-import inspect
-from typing import TYPE_CHECKING, Any, Awaitable, Generic, Iterable, TypeVar, Union
-
-import pypika
-
-from yesql.core import parse, types
-
-if TYPE_CHECKING:
-    from yesql import drivers
-
-__all__ = ("DynamicQueryService",)
-
-_MT = TypeVar("_MT")
-_RT = TypeVar("_RT")
-_ConnT = TypeVar("_ConnT")
-_CtxT = TypeVar("_CtxT")
-_ReturnT = Union[Iterable[_MT], Iterable[types.ScalarT]]
-
-
-class DynamicQueryService(Generic[_MT]):
-    """Query Library for building ad-hoc queries in-memory.
-
-    This service acts as glue between the `pypika` query-builder library and Norma's
-    `QueryRepository`.
-
-    It is intended as an escape-hatch for the small subset of situations where
-    dynamically-built queries are actually needed (think an admin tool, like
-    Flask-Admin, for instance).
-    """
-
-    __slots__ = (
-        "service",
-        "table",
-        "builder",
-        "cursor_proxy",
-    )
-
-    def __init__(
-        self,
-        service: types.RepositoryProtocolT[_MT],  # noqa: F811
-        *,
-        schema: str = None,
-    ):
-        self.service = service
-        self.table = self._get_table(service.metadata.__tablename__, schema=schema)
-        self.builder = self._get_query_builder(
-            self.table, dialect=service.metadata.__dialect__
-        )
-
-    def execute(
-        self,
-        query: Union[str, pypika.queries.QueryBuilder],
-        *args,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        coerce: bool = True,
-        deserializer: drivers.base.DeserializerT | None = None,
-        modifier: parse.ModifierT = parse.MANY,
-        **kwargs,
-    ) -> Union[_ReturnT, Awaitable[_ReturnT]]:
-        """Execute any arbitrary query and return the result.
-
-        Args:
-            query:
-               Either a SQL string or a pypika Query.
-            *args:
-               Any args which should be passed on to the query.
-            connection: optional
-               A DBAPI connectable to use during executions.
-               Whether to coerce the query result into the model bound to the service.
-            timeout: defaults 10
-                The number of seconds to wait for the query to complete.
-            transaction: defaults True
-                Whether to execute this query within a transaction block.
-            rollback: defaults False
-                Whether to rollback the transaction scope of this query execution.
-            coerce: defaults True
-                Whether to coerce the query result into the model bound to the service.
-                Will only be applied if the execution modifier returns a full row object.
-            deserializer: optional
-                A custom deserializer for the query result. If none provided, this method
-                will make use of the default deserializer on the associated repository.
-            modifier: The execution modifier for this query.
-                Fetch all rows, one row, the first value in the first row,
-                or just the affected rows.
-            **kwargs:
-               Any keyword args to pass on to the query.
-        Returns:
-            The query result.
-        """
-        query = self._resolve_query(sql=query, modifier=modifier)
-        executor = getattr(self.service.executor, modifier)
-        if modifier in {parse.MANY, parse.ONE, parse.MULTI} and coerce:
-            deserializer = deserializer or (
-                self.service.serdes.deserializer
-                if modifier == parse.ONE
-                else self.service.serdes.bulk_deserializer
-            )
-            kwargs.update(deserializer=deserializer)
-        return executor(
-            query,
-            *args,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **kwargs,
-        )
-
-    def execute_cursor(
-        self,
-        query: Union[str, pypika.queries.QueryBuilder],
-        *args,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        modifier: parse.ModifierT = parse.MANY,
-        **kwargs,
-    ):
-        """Execute any arbitrary query and enter a cursor context.
-
-        Args:
-            query:
-               Either a SQL string or a pypika Query.
-            *args:
-               Any args which should be passed on to the query.
-            connection: optional
-               A DBAPI connectable to use during executions.
-               Whether to coerce the query result into the model bound to the service.
-            timeout: defaults 10
-                The number of seconds to wait for the query to complete.
-            transaction: defaults True
-                Whether to execute this query within a transaction block.
-            rollback: defaults False
-                Whether to rollback the transaction scope of this query execution.
-            modifier: The execution modifier for this query.
-                Fetch all rows, one row, the first value in the first row,
-                or just the affected rows.
-            **kwargs:
-               Any keyword args to pass on to the query.
-        """
-        query = self._resolve_query(sql=query, modifier=modifier)
-        executor = getattr(self.service.executor, modifier + "_cursor")
-        return executor(
-            query,
-            *args,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **kwargs,
-        )
-
-    def select(
-        self,
-        *fields,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        coerce: bool = True,
-        deserializer: drivers.base.DeserializerT | None = None,
-        modifier: parse.ModifierT = parse.MANY,
-        **where: Any,
-    ) -> Union[_ReturnT, Awaitable[_ReturnT]]:
-        """A convenience method for executing an arbitrary SELECT query.
-
-        Notes:
-            This method assumes that the result is coerceable into the model bound to
-            the QueryService. If that is not the case, then make sure to pass in
-            `coerce=False` to the call.
-
-        Args:
-            *fields:
-                Optionally specify specific fields to return.
-            connection: optional
-               A DBAPI connectable to use during executions.
-               Whether to coerce the query result into the model bound to the service.
-            timeout: defaults 10
-                The number of seconds to wait for the query to complete.
-            transaction: defaults True
-                Whether to execute this query within a transaction block.
-            rollback: defaults False
-                Whether to rollback the transaction scope of this query execution.
-            coerce: defaults True
-                Whether to coerce the query result into the model bound to the service.
-                Will only be applied if the execution modifier returns a full row object.
-            deserializer: optional
-                A custom deserializer for the query result. If none provided, this method
-                will make use of the default deserializer on the associated repository.
-            modifier: The execution modifier for this query.
-                Fetch all rows, one row, the first value in the first row,
-                or just the affected rows.
-            **where:
-                Optionally specify direct equality comparisons for the WHERE clause.
-        """
-        query = self.build_select(*fields, **where)
-        return self.execute(
-            query,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            coerce=coerce,
-            deserializer=deserializer,
-            modifier=modifier,
-        )
-
-    def select_cursor(
-        self,
-        *fields,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        modifier: parse.ModifierT = parse.MANY,
-        **where: Any,
-    ):
-        """A convenience method for executing an arbitrary SELECT query and entering a cursor context.
-
-        Notes:
-            This method assumes that the result is coerceable into the model bound to
-            the QueryService. If that is not the case, then make sure to pass in
-            `coerce=False` to the call.
-
-        Args:
-            *fields:
-                Optionally specify specific fields to return.
-            connection: optional
-               A DBAPI connectable to use during executions.
-               Whether to coerce the query result into the model bound to the service.
-            timeout: defaults 10
-                The number of seconds to wait for the query to complete.
-            transaction: defaults True
-                Whether to execute this query within a transaction block.
-            rollback: defaults False
-                Whether to rollback the transaction scope of this query execution.
-            modifier: The execution modifier for this query.
-                Fetch all rows, one row, the first value in the first row,
-                or just the affected rows.
-            **where:
-                Optionally specify direct equality comparisons for the WHERE clause.
-        """
-        query = self.build_select(*fields, **where)
-        return self.execute_cursor(
-            query,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            modifier=modifier,
-        )
-
-    def build_select(self, *fields: str, **where: Any) -> pypika.queries.QueryBuilder:
-        """A convenience method for building a simple SELECT statement.
-
-        Args:
-            *fields:
-                Optionally specify specific fields to return.
-            **where:
-                Optionally specify direct equality comparisons for the WHERE clause.
-        """
-        fs: Iterable[str] = fields or [self.builder.star]
-        criterion: pypika.Criterion = pypika.Criterion.all(
-            [getattr(self.table, c) == v for c, v in where.items()]
-        )
-        return self.builder.select(*fs).where(criterion)
-
-    @staticmethod
-    def _get_table(name: str, *, schema: str = None) -> pypika.Table:
-        return pypika.Table(name, schema=schema)
-
-    @classmethod
-    def _get_query_builder(
-        cls,
-        table: pypika.Table,
-        *,
-        dialect: drivers.SupportedDialectsT = pypika.Dialects.POSTGRESQL,
-    ) -> pypika.queries.QueryBuilder:
-        return pypika.Query.from_(table, dialect=dialect)
-
-    @staticmethod
-    def _resolve_query(
-        sql: Union[str, pypika.queries.QueryBuilder], modifier: parse.ModifierT
-    ) -> parse.QueryDatum:
-        if isinstance(sql, pypika.queries.QueryBuilder):
-            sql = sql.get_sql()
-
-        return parse.QueryDatum(
-            name="execute",
-            doc="",
-            sql=sql,
-            signature=inspect.Signature(),
-            modifier=modifier,
-        )
+from __future__ import annotations
+
+import inspect
+from typing import TYPE_CHECKING, Any, Awaitable, Generic, Iterable, TypeVar, Union
+
+import pypika
+
+from yesql.core import parse, types
+
+if TYPE_CHECKING:
+    from yesql import drivers
+
+__all__ = ("DynamicQueryService",)
+
+_MT = TypeVar("_MT")
+_RT = TypeVar("_RT")
+_ConnT = TypeVar("_ConnT")
+_CtxT = TypeVar("_CtxT")
+_ReturnT = Union[Iterable[_MT], Iterable[types.ScalarT]]
+
+
+class DynamicQueryService(Generic[_MT]):
+    """Query Library for building ad-hoc queries in-memory.
+
+    This service acts as glue between the `pypika` query-builder library and Norma's
+    `QueryRepository`.
+
+    It is intended as an escape-hatch for the small subset of situations where
+    dynamically-built queries are actually needed (think an admin tool, like
+    Flask-Admin, for instance).
+    """
+
+    __slots__ = (
+        "service",
+        "table",
+        "builder",
+        "cursor_proxy",
+    )
+
+    def __init__(
+        self,
+        service: types.RepositoryProtocolT[_MT],  # noqa: F811
+        *,
+        schema: str = None,
+    ):
+        self.service = service
+        self.table = self._get_table(service.metadata.__tablename__, schema=schema)
+        self.builder = self._get_query_builder(
+            self.table, dialect=service.metadata.__dialect__
+        )
+
+    def execute(
+        self,
+        query: Union[str, pypika.queries.QueryBuilder],
+        *args,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        coerce: bool = True,
+        deserializer: types.DeserializerT | None = None,
+        modifier: parse.ModifierT = parse.MANY,
+        **kwargs,
+    ) -> Union[_ReturnT, Awaitable[_ReturnT]]:
+        """Execute any arbitrary query and return the result.
+
+        Args:
+            query:
+               Either a SQL string or a pypika Query.
+            *args:
+               Any args which should be passed on to the query.
+            connection: optional
+               A DBAPI connectable to use during executions.
+               Whether to coerce the query result into the model bound to the service.
+            timeout: defaults 10
+                The number of seconds to wait for the query to complete.
+            transaction: defaults True
+                Whether to execute this query within a transaction block.
+            rollback: defaults False
+                Whether to rollback the transaction scope of this query execution.
+            coerce: defaults True
+                Whether to coerce the query result into the model bound to the service.
+                Will only be applied if the execution modifier returns a full row object.
+            deserializer: optional
+                A custom deserializer for the query result. If none provided, this method
+                will make use of the default deserializer on the associated repository.
+            modifier: The execution modifier for this query.
+                Fetch all rows, one row, the first value in the first row,
+                or just the affected rows.
+            **kwargs:
+               Any keyword args to pass on to the query.
+        Returns:
+            The query result.
+        """
+        query = self._resolve_query(sql=query, modifier=modifier)
+        executor = getattr(self.service.executor, modifier)
+        if modifier in {parse.MANY, parse.ONE, parse.MULTI} and coerce:
+            deserializer = deserializer or (
+                self.service.serdes.deserializer
+                if modifier == parse.ONE
+                else self.service.serdes.bulk_deserializer
+            )
+            kwargs.update(deserializer=deserializer)
+        return executor(
+            query,
+            *args,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **kwargs,
+        )
+
+    def execute_cursor(
+        self,
+        query: Union[str, pypika.queries.QueryBuilder],
+        *args,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        modifier: parse.ModifierT = parse.MANY,
+        **kwargs,
+    ):
+        """Execute any arbitrary query and enter a cursor context.
+
+        Args:
+            query:
+               Either a SQL string or a pypika Query.
+            *args:
+               Any args which should be passed on to the query.
+            connection: optional
+               A DBAPI connectable to use during executions.
+               Whether to coerce the query result into the model bound to the service.
+            timeout: defaults 10
+                The number of seconds to wait for the query to complete.
+            transaction: defaults True
+                Whether to execute this query within a transaction block.
+            rollback: defaults False
+                Whether to rollback the transaction scope of this query execution.
+            modifier: The execution modifier for this query.
+                Fetch all rows, one row, the first value in the first row,
+                or just the affected rows.
+            **kwargs:
+               Any keyword args to pass on to the query.
+        """
+        query = self._resolve_query(sql=query, modifier=modifier)
+        executor = getattr(self.service.executor, modifier + "_cursor")
+        return executor(
+            query,
+            *args,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **kwargs,
+        )
+
+    def select(
+        self,
+        *fields,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        coerce: bool = True,
+        deserializer: types.DeserializerT | None = None,
+        modifier: parse.ModifierT = parse.MANY,
+        **where: Any,
+    ) -> Union[_ReturnT, Awaitable[_ReturnT]]:
+        """A convenience method for executing an arbitrary SELECT query.
+
+        Notes:
+            This method assumes that the result is coerceable into the model bound to
+            the QueryService. If that is not the case, then make sure to pass in
+            `coerce=False` to the call.
+
+        Args:
+            *fields:
+                Optionally specify specific fields to return.
+            connection: optional
+               A DBAPI connectable to use during executions.
+               Whether to coerce the query result into the model bound to the service.
+            timeout: defaults 10
+                The number of seconds to wait for the query to complete.
+            transaction: defaults True
+                Whether to execute this query within a transaction block.
+            rollback: defaults False
+                Whether to rollback the transaction scope of this query execution.
+            coerce: defaults True
+                Whether to coerce the query result into the model bound to the service.
+                Will only be applied if the execution modifier returns a full row object.
+            deserializer: optional
+                A custom deserializer for the query result. If none provided, this method
+                will make use of the default deserializer on the associated repository.
+            modifier: The execution modifier for this query.
+                Fetch all rows, one row, the first value in the first row,
+                or just the affected rows.
+            **where:
+                Optionally specify direct equality comparisons for the WHERE clause.
+        """
+        query = self.build_select(*fields, **where)
+        return self.execute(
+            query,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            coerce=coerce,
+            deserializer=deserializer,
+            modifier=modifier,
+        )
+
+    def select_cursor(
+        self,
+        *fields,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        modifier: parse.ModifierT = parse.MANY,
+        **where: Any,
+    ):
+        """A convenience method for executing an arbitrary SELECT query and entering a cursor context.
+
+        Notes:
+            This method assumes that the result is coerceable into the model bound to
+            the QueryService. If that is not the case, then make sure to pass in
+            `coerce=False` to the call.
+
+        Args:
+            *fields:
+                Optionally specify specific fields to return.
+            connection: optional
+               A DBAPI connectable to use during executions.
+               Whether to coerce the query result into the model bound to the service.
+            timeout: defaults 10
+                The number of seconds to wait for the query to complete.
+            transaction: defaults True
+                Whether to execute this query within a transaction block.
+            rollback: defaults False
+                Whether to rollback the transaction scope of this query execution.
+            modifier: The execution modifier for this query.
+                Fetch all rows, one row, the first value in the first row,
+                or just the affected rows.
+            **where:
+                Optionally specify direct equality comparisons for the WHERE clause.
+        """
+        query = self.build_select(*fields, **where)
+        return self.execute_cursor(
+            query,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            modifier=modifier,
+        )
+
+    def build_select(self, *fields: str, **where: Any) -> pypika.queries.QueryBuilder:
+        """A convenience method for building a simple SELECT statement.
+
+        Args:
+            *fields:
+                Optionally specify specific fields to return.
+            **where:
+                Optionally specify direct equality comparisons for the WHERE clause.
+        """
+        fs: Iterable[str] = fields or [self.builder.star]
+        criterion: pypika.Criterion = pypika.Criterion.all(
+            [getattr(self.table, c) == v for c, v in where.items()]
+        )
+        return self.builder.select(*fs).where(criterion)
+
+    @staticmethod
+    def _get_table(name: str, *, schema: str = None) -> pypika.Table:
+        return pypika.Table(name, schema=schema)
+
+    @classmethod
+    def _get_query_builder(
+        cls,
+        table: pypika.Table,
+        *,
+        dialect: drivers.SupportedDialectsT = pypika.Dialects.POSTGRESQL,
+    ) -> pypika.queries.QueryBuilder:
+        return pypika.Query.from_(table, dialect=dialect)
+
+    @staticmethod
+    def _resolve_query(
+        sql: Union[str, pypika.queries.QueryBuilder], modifier: parse.ModifierT
+    ) -> parse.QueryDatum:
+        if isinstance(sql, pypika.queries.QueryBuilder):
+            sql = sql.get_sql()
+
+        return parse.QueryDatum(
+            name="execute",
+            doc="",
+            sql=sql,
+            signature=inspect.Signature(),
+            modifier=modifier,
+        )
```

### Comparing `yesql-0.1.1/yesql/repository.py` & `yesql-1.0.0b3/yesql/repository.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,369 +1,369 @@
-from __future__ import annotations
-
-import collections
-import dataclasses
-import inspect
-import logging
-import pathlib
-from types import SimpleNamespace
-from typing import (
-    Any,
-    ClassVar,
-    Deque,
-    Dict,
-    FrozenSet,
-    Iterable,
-    Literal,
-    Optional,
-    Tuple,
-    Type,
-    TypeVar,
-    Union,
-    cast,
-)
-
-import inflection
-import typic
-
-from yesql import statement
-from yesql.core import drivers, middleware, parse, types
-
-__all__ = (
-    "AsyncQueryRepository",
-    "BaseQueryRepository",
-    "ExplainFormatT",
-    "QueryMetadata",
-    "SyncQueryRepository",
-)
-
-logger = logging.getLogger(__name__)
-
-
-ExplainFormatT = Literal["json", "yaml", "xml"]
-
-_MT = TypeVar("_MT")
-_ConnT = TypeVar("_ConnT")
-_RT = TypeVar("_RT")
-
-
-class QueryMetadata(types.MetadataT):
-    """Default metadata for the query repository.
-
-    Query Metadata provides simple configuration for binding an execution Statement,
-    a parsed QueryDatum, and a repository's data model.
-    """
-
-    __slots__ = ()
-    __dialect__: ClassVar[drivers.SupportedDialectsT] = "postgresql"
-    __exclude_fields__: ClassVar[FrozenSet[str]] = frozenset(
-        ("id", "created_at", "updated_at")
-    )
-    __querylib__: ClassVar[Union[str, pathlib.Path]]
-
-
-class BaseQueryRepository(types.RepositoryProtocolT[_MT]):
-    """The base class for a 'repository'.
-
-    A 'repository' is responsible for querying a specific table.
-    It also is semi-aware of in-memory dataclass representing the table data.
-
-    By default, a repository will coerce the query result to the bound model.
-    """
-
-    # User-defined class attributes
-    model: ClassVar[Type[_MT]] = Any  # type: ignore
-    metadata: ClassVar[Type[types.MetadataT]] = QueryMetadata
-    # Generated attributes
-    queries: ClassVar[parse.QueryPackage]
-    driver: ClassVar[drivers.Driver]
-    # Generated or Initialized Attributes
-    executor: drivers.BaseQueryExecutor
-    serdes: statement.SerDes[_MT]
-    # Private attributes.
-    _protocol: ClassVar[typic.SerdeProtocol[_MT | None]]
-    _bulk_protocol: ClassVar[typic.SerdeProtocol[Iterable[_MT]]]
-
-    __slots__ = ()
-
-    __statements__: dict[str, statement.Statement[_MT]]
-
-    def __init__(
-        self,
-        *,
-        executor: drivers.BaseQueryExecutor = None,
-        serdes: statement.SerDes[_MT] = None,
-        **connect_kwargs,
-    ):
-        # If we're overriding the default connector, then propagate it.
-        if executor:
-            self.executor = executor
-            for stat in self.__statements__.values():
-                stat.executor = self.executor
-        # If we're overriding the default serdes, then propagate it.
-        if serdes:
-            self.serdes = serdes
-            for stat in self.__statements__.values():
-                stat.serdes = self.serdes
-        # Ingest custom connection args.
-        # This will only matter if we haven't already connected to the database.
-        self.executor.pool_kwargs.update(connect_kwargs)
-
-    def initialize(self):
-        """Initialize the query executor's connection to the underlying database."""
-        return self.executor.initialize()
-
-    def teardown(self, *, timeout: int = 10):
-        """Tear down the query executor's connection to the underlying database."""
-        return self.executor.teardown(timeout=timeout)
-
-    def __init_subclass__(cls, **kwargs):
-        if cls.__name__ in {"AsyncQueryRepository", "SyncQueryRepository"}:
-            return super().__init_subclass__(**kwargs)
-
-        for pcls in inspect.getmro(cls)[1:]:  # the first entry is always `cls`
-            if not issubclass(pcls, BaseQueryRepository):
-                continue
-            cls.metadata.__exclude_fields__ |= pcls.metadata.__exclude_fields__
-
-        if not hasattr(cls.metadata, "__tablename__"):
-            cls.metadata.__tablename__ = cls._get_table_name()
-
-        cls._protocol = typic.protocol(cls.model, is_optional=True)
-        cls._bulk_protocol = typic.protocol(Iterable[cls.model])
-        cls.serdes = statement.SerDes(
-            serializer=cls.get_kvs,
-            deserializer=cls._protocol.transmute,
-            bulk_deserializer=cls._bulk_protocol.transmute,
-        )
-        cls.driver = drivers.get_driver(dialect=cls.metadata.__dialect__, aio=cls.isaio)
-        cls.executor = cls.driver.executor()
-        cls.queries = cls._get_query_library()
-        cls.__statements__ = cls._resolve_statements()
-        return super().__init_subclass__(**kwargs)
-
-    @classmethod
-    def get_kvs(cls, model: types.ModelT) -> Dict[str, Any]:
-        """Get a mapping of key-value pairs for your model without excluded fields."""
-        return {
-            field: value
-            for field, value in cls._protocol.iterate(model)
-            if field not in cls.metadata.__exclude_fields__
-        }
-
-    @classmethod
-    def _get_table_name(cls) -> str:
-        """Get the name of the table for this query lib
-
-        Overload this method to customize how your determine the table name of your
-        Query library.
-
-        Notes:
-            This is run if Metadata.__tablename__ is not set by the user.
-        """
-        return inflection.underscore(typic.get_name(cls.model))
-
-    @classmethod
-    def _get_query_library(cls) -> parse.QueryPackage:
-        """Load the query library from disk into memory.
-
-        Overload this method to customize how your query library is loaded.
-
-        Notes:
-            By default, this will join `Metadata.__querylib__` &
-            `Metadata.__tablename__` as a path and attempt to load all sql files found.
-        """
-        if not hasattr(cls.metadata, "__querylib__"):
-            cls.metadata.__querylib__ = pathlib.Path.cwd().resolve()
-        if isinstance(cls.metadata.__querylib__, str):
-            cls.metadata.__querylib__ = pathlib.Path(
-                cls.metadata.__querylib__
-            ).resolve()
-        path = cls.metadata.__querylib__ / cls.metadata.__tablename__
-        lib = parse.parse(path, driver=cls.driver.executor.__driver__)
-        return lib
-
-    @classmethod
-    def _resolve_statements(cls) -> dict[str, statement.Statement]:
-        """Bootstrap all raw Query functions and attach them to this service.
-
-        Overload this method to customize how your queries are bootstrapped.
-        """
-        mwares = {
-            qname: mware
-            for _, mware in cls._iter_middlewares()
-            for qname in mware.__intercepts__
-        }
-        available = cls._bootstrap_package(cls.queries, mwares)
-        for name, stmt in available.items():
-            # Don't override a custom impl, but let them use it if they want.
-            if hasattr(cls, name):
-                name = name + "_default"
-            setattr(cls, name, stmt)
-        stack: _QueryPackageStack = collections.deque(
-            (cls, pkg) for pkg in cls.queries.packages.values()
-        )
-        # Build the tree of queries associated to this repository.
-        while stack:
-            parent, package = stack.popleft()
-            queries = cls._bootstrap_package(package, mwares)
-            ns = SimpleNamespace(**queries)
-            setattr(parent, package.name, ns)
-            stack.extend((ns, pkg) for pkg in package.packages.values())
-            available.update(queries)
-
-        return available
-
-    @classmethod
-    def _bootstrap_package(
-        cls,
-        package: parse.QueryPackage,
-        middlewares: dict[str, types.MiddlewareMethodProtocolT],
-    ) -> dict[str, statement.Statement]:
-        available = {}
-        # For every module in the package...
-        for mname, module in package.modules.items():
-            # For every query in the module...
-            for name, datum in module.queries.items():
-                # Get the unit-of-work statements for this query
-                statements = statement.statements(
-                    datum,
-                    executor=cls.executor,
-                    serdes=cls.serdes,
-                )
-                # For every statement...
-                for stat in statements:
-                    # Check if there is an associated middleware
-                    mware = middlewares.get(stat.query.name)
-                    if mware:
-                        stat.middleware = mware
-                    # Add the statement to the mapping of available units of work
-                    #   for this package.
-                    available[stat.query.name] = stat
-        return available
-
-    @classmethod
-    def _iter_middlewares(cls) -> Iterable[tuple[str, types.MiddlewareMethodProtocolT]]:
-        for name, call in inspect.getmembers(cls, middleware.ismiddleware):
-            yield name, call
-
-    def count(
-        self,
-        query: Union[str, statement.Statement],
-        *args,
-        estimate_ok: bool = True,
-        **kwargs,
-    ):
-        """Get the number of rows returned by this query.
-
-        Args:
-            query:
-                Either the query function, or the name of the query in your library
-                which you wish to get a count from.
-            *args:
-                Any positional arguments which the query requires.
-            **kwargs:
-                Any keyword-arguments you'll pass on to the query.
-
-        Returns:
-            The number of rows.
-        """
-        if isinstance(query, str):
-            query = cast(statement.Statement, getattr(self, query))
-        datum = query.query
-        sql = f"SELECT count(*) FROM ({query.query.sql.rstrip(';')}) AS q;"
-        stat = dataclasses.replace(datum, sql=sql)
-        return self.executor.scalar(stat, *args, **kwargs)
-
-    def explain(
-        self,
-        query: Union[str, statement.Statement],
-        *args,
-        analyze: bool = True,
-        format: Optional[ExplainFormatT] = "json",
-        **kwargs,
-    ):
-        """Get profiling information from the database about your query.
-
-        EXPLAIN is a useful tool to debug how the RDBMS's query optimizer will execute
-        your query in the database so that you can tune either it or the schema for
-        your use-case.
-
-        Notes:
-            We run our EXPLAIN under a transaction which is automatically rolled back,
-            so this operation is considered "safe" to use with queries which would
-            result in mutation.
-
-            The exact command run is determined by the Executor's
-            `get_explain_command`, which will return a compliant command for the
-            selected dialect. Consult your dialect's documentation for more information.
-
-        Args:
-            query:
-                Either the query function, or the name of the query in your library
-                which you wish to analyze.
-            *args:
-                Any positional arguments which the query requires.
-            analyze: defaults True
-                If true and supported by your dialect, run `EXPLAIN ANALYZE`,
-                else run `EXPLAIN`. Consult the documentation for your dialect for an
-                in-depth explanation of the two options.
-            format: defaults "json"
-                If supported, the output format for the EXPLAIN result.
-                Consult the documentation for your dialect to get a full list of options.
-            **kwargs:
-                Any keyword-arguments you'll pass on to the query.
-        Returns:
-            The raw results of the EXPLAIN query.
-        """
-        if isinstance(query, str):
-            query = cast(statement.Statement, getattr(self, query))
-        datum = query.query
-        op = self.executor.get_explain_command(analyze, format)
-        sql = f"{op}{datum.sql}"
-        stat = dataclasses.replace(datum, sql=sql)
-        kwargs.update(transaction=True, rollback=True)
-        if op == self.executor.EXPLAIN_PREFIX:
-            kwargs["coerce"] = False
-            return self.executor.one(
-                stat,
-                *args,
-                **kwargs,
-            )
-
-        return self.executor.scalar(
-            stat,
-            *args,
-            **kwargs,
-        )
-
-
-class AsyncQueryRepository(BaseQueryRepository[_MT]):
-    """An event-loop compatible query repository (async/await)."""
-
-    isaio = True
-
-    async def __aenter__(self):
-        await self.executor.initialize()
-        return self
-
-    async def __aexit__(self, exc_type, exc_val, exc_tb):
-        await self.executor.teardown()
-        return
-
-
-class SyncQueryRepository(BaseQueryRepository[_MT]):
-    """A blocking-IO query repository."""
-
-    isaio = False
-
-    def __enter__(self):
-        self.executor.initialize()
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.executor.teardown()
-        return
-
-
-_QueryNamespaceT = Union[Type[types.RepositoryProtocolT], SimpleNamespace]
-_QueryPackageStack = Deque[Tuple[_QueryNamespaceT, parse.QueryPackage]]
+from __future__ import annotations
+
+import collections
+import dataclasses
+import inspect
+import logging
+import pathlib
+from types import SimpleNamespace
+from typing import (
+    Any,
+    ClassVar,
+    Deque,
+    Dict,
+    FrozenSet,
+    Iterable,
+    Literal,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import inflection
+import typic
+
+from yesql import statement
+from yesql.core import drivers, middleware, parse, types
+
+__all__ = (
+    "AsyncQueryRepository",
+    "BaseQueryRepository",
+    "ExplainFormatT",
+    "QueryMetadata",
+    "SyncQueryRepository",
+)
+
+logger = logging.getLogger(__name__)
+
+
+ExplainFormatT = Literal["json", "yaml", "xml"]
+
+_MT = TypeVar("_MT")
+_ConnT = TypeVar("_ConnT")
+_RT = TypeVar("_RT")
+
+
+class QueryMetadata(types.MetadataT):
+    """Default metadata for the query repository.
+
+    Query Metadata provides simple configuration for binding an execution Statement,
+    a parsed QueryDatum, and a repository's data model.
+    """
+
+    __slots__ = ()
+    __dialect__: ClassVar[drivers.SupportedDialectsT] = "postgresql"
+    __exclude_fields__: ClassVar[FrozenSet[str]] = frozenset(
+        ("id", "created_at", "updated_at")
+    )
+    __querylib__: ClassVar[Union[str, pathlib.Path]]
+
+
+class BaseQueryRepository(types.RepositoryProtocolT[_MT]):
+    """The base class for a 'repository'.
+
+    A 'repository' is responsible for querying a specific table.
+    It also is semi-aware of in-memory dataclass representing the table data.
+
+    By default, a repository will coerce the query result to the bound model.
+    """
+
+    # User-defined class attributes
+    model: ClassVar[Type[_MT]] = Any  # type: ignore
+    metadata: ClassVar[Type[types.MetadataT]] = QueryMetadata
+    # Generated attributes
+    queries: ClassVar[parse.QueryPackage]
+    driver: ClassVar[drivers.Driver]
+    # Generated or Initialized Attributes
+    executor: drivers.BaseQueryExecutor
+    serdes: statement.SerDes[_MT]
+    # Private attributes.
+    _protocol: typic.SerdeProtocol[_MT | None]
+    _bulk_protocol: typic.SerdeProtocol[Iterable[_MT]]
+
+    __slots__ = ()
+
+    __statements__: dict[str, statement.Statement[_MT]]
+
+    def __init__(
+        self,
+        *,
+        executor: drivers.BaseQueryExecutor = None,
+        serdes: statement.SerDes[_MT] = None,
+        **connect_kwargs,
+    ):
+        # If we're overriding the default connector, then propagate it.
+        if executor:
+            self.executor = executor
+            for stat in self.__statements__.values():
+                stat.executor = self.executor
+        # If we're overriding the default serdes, then propagate it.
+        if serdes:
+            self.serdes = serdes
+            for stat in self.__statements__.values():
+                stat.serdes = self.serdes
+        # Ingest custom connection args.
+        # This will only matter if we haven't already connected to the database.
+        self.executor.pool_kwargs.update(connect_kwargs)
+
+    def initialize(self):
+        """Initialize the query executor's connection to the underlying database."""
+        return self.executor.initialize()
+
+    def teardown(self, *, timeout: int = 10):
+        """Tear down the query executor's connection to the underlying database."""
+        return self.executor.teardown(timeout=timeout)
+
+    def __init_subclass__(cls, **kwargs):
+        if cls.__name__ in {"AsyncQueryRepository", "SyncQueryRepository"}:
+            return super().__init_subclass__(**kwargs)
+
+        for pcls in inspect.getmro(cls)[1:]:  # the first entry is always `cls`
+            if not issubclass(pcls, BaseQueryRepository):
+                continue
+            cls.metadata.__exclude_fields__ |= pcls.metadata.__exclude_fields__
+
+        if not hasattr(cls.metadata, "__tablename__"):
+            cls.metadata.__tablename__ = cls._get_table_name()
+
+        cls._protocol = typic.protocol(cls.model, is_optional=True)
+        cls._bulk_protocol = typic.protocol(Iterable[cls.model])
+        cls.serdes = statement.SerDes(
+            serializer=cls.get_kvs,
+            deserializer=cls._protocol.transmute,
+            bulk_deserializer=cls._bulk_protocol.transmute,
+        )
+        cls.driver = drivers.get_driver(dialect=cls.metadata.__dialect__, aio=cls.isaio)
+        cls.executor = cls.driver.executor()
+        cls.queries = cls._get_query_library()
+        cls.__statements__ = cls._resolve_statements()
+        return super().__init_subclass__(**kwargs)
+
+    @classmethod
+    def get_kvs(cls, model: types.ModelT) -> Dict[str, Any]:
+        """Get a mapping of key-value pairs for your model without excluded fields."""
+        return {
+            field: value
+            for field, value in cls._protocol.iterate(model)
+            if field not in cls.metadata.__exclude_fields__
+        }
+
+    @classmethod
+    def _get_table_name(cls) -> str:
+        """Get the name of the table for this query lib
+
+        Overload this method to customize how your determine the table name of your
+        Query library.
+
+        Notes:
+            This is run if Metadata.__tablename__ is not set by the user.
+        """
+        return inflection.underscore(typic.get_name(cls.model))
+
+    @classmethod
+    def _get_query_library(cls) -> parse.QueryPackage:
+        """Load the query library from disk into memory.
+
+        Overload this method to customize how your query library is loaded.
+
+        Notes:
+            By default, this will join `Metadata.__querylib__` &
+            `Metadata.__tablename__` as a path and attempt to load all sql files found.
+        """
+        if not hasattr(cls.metadata, "__querylib__"):
+            cls.metadata.__querylib__ = pathlib.Path.cwd().resolve()
+        if isinstance(cls.metadata.__querylib__, str):
+            cls.metadata.__querylib__ = pathlib.Path(
+                cls.metadata.__querylib__
+            ).resolve()
+        path = cls.metadata.__querylib__ / cls.metadata.__tablename__
+        lib = parse.parse(path, driver=cls.driver.executor.__driver__)
+        return lib
+
+    @classmethod
+    def _resolve_statements(cls) -> dict[str, statement.Statement]:
+        """Bootstrap all raw Query functions and attach them to this service.
+
+        Overload this method to customize how your queries are bootstrapped.
+        """
+        mwares = {
+            qname: mware
+            for _, mware in cls._iter_middlewares()
+            for qname in mware.__intercepts__
+        }
+        available = cls._bootstrap_package(cls.queries, mwares)
+        for name, stmt in available.items():
+            # Don't override a custom impl, but let them use it if they want.
+            if hasattr(cls, name):
+                name = name + "_default"
+            setattr(cls, name, stmt)
+        stack: _QueryPackageStack = collections.deque(
+            (cls, pkg) for pkg in cls.queries.packages.values()
+        )
+        # Build the tree of queries associated to this repository.
+        while stack:
+            parent, package = stack.popleft()
+            queries = cls._bootstrap_package(package, mwares)
+            ns = SimpleNamespace(**queries)
+            setattr(parent, package.name, ns)
+            stack.extend((ns, pkg) for pkg in package.packages.values())
+            available.update(queries)
+
+        return available
+
+    @classmethod
+    def _bootstrap_package(
+        cls,
+        package: parse.QueryPackage,
+        middlewares: dict[str, types.MiddlewareMethodProtocolT],
+    ) -> dict[str, statement.Statement]:
+        available = {}
+        # For every module in the package...
+        for mname, module in package.modules.items():
+            # For every query in the module...
+            for name, datum in module.queries.items():
+                # Get the unit-of-work statements for this query
+                statements = statement.statements(
+                    datum,
+                    executor=cls.executor,
+                    serdes=cls.serdes,
+                )
+                # For every statement...
+                for stat in statements:
+                    # Check if there is an associated middleware
+                    mware = middlewares.get(stat.query.name)
+                    if mware:
+                        stat.middleware = mware
+                    # Add the statement to the mapping of available units of work
+                    #   for this package.
+                    available[stat.query.name] = stat
+        return available
+
+    @classmethod
+    def _iter_middlewares(cls) -> Iterable[tuple[str, types.MiddlewareMethodProtocolT]]:
+        for name, call in inspect.getmembers(cls, middleware.ismiddleware):
+            yield name, call
+
+    def count(
+        self,
+        query: Union[str, statement.Statement],
+        *args,
+        estimate_ok: bool = True,
+        **kwargs,
+    ):
+        """Get the number of rows returned by this query.
+
+        Args:
+            query:
+                Either the query function, or the name of the query in your library
+                which you wish to get a count from.
+            *args:
+                Any positional arguments which the query requires.
+            **kwargs:
+                Any keyword-arguments you'll pass on to the query.
+
+        Returns:
+            The number of rows.
+        """
+        if isinstance(query, str):
+            query = cast(statement.Statement, getattr(self, query))
+        datum = query.query
+        sql = f"SELECT count(*) FROM ({query.query.sql.rstrip(';')}) AS q;"
+        stat = dataclasses.replace(datum, sql=sql)
+        return self.executor.scalar(stat, *args, **kwargs)
+
+    def explain(
+        self,
+        query: Union[str, statement.Statement],
+        *args,
+        analyze: bool = True,
+        format: Optional[ExplainFormatT] = "json",
+        **kwargs,
+    ):
+        """Get profiling information from the database about your query.
+
+        EXPLAIN is a useful tool to debug how the RDBMS's query optimizer will execute
+        your query in the database so that you can tune either it or the schema for
+        your use-case.
+
+        Notes:
+            We run our EXPLAIN under a transaction which is automatically rolled back,
+            so this operation is considered "safe" to use with queries which would
+            result in mutation.
+
+            The exact command run is determined by the Executor's
+            `get_explain_command`, which will return a compliant command for the
+            selected dialect. Consult your dialect's documentation for more information.
+
+        Args:
+            query:
+                Either the query function, or the name of the query in your library
+                which you wish to analyze.
+            *args:
+                Any positional arguments which the query requires.
+            analyze: defaults True
+                If true and supported by your dialect, run `EXPLAIN ANALYZE`,
+                else run `EXPLAIN`. Consult the documentation for your dialect for an
+                in-depth explanation of the two options.
+            format: defaults "json"
+                If supported, the output format for the EXPLAIN result.
+                Consult the documentation for your dialect to get a full list of options.
+            **kwargs:
+                Any keyword-arguments you'll pass on to the query.
+        Returns:
+            The raw results of the EXPLAIN query.
+        """
+        if isinstance(query, str):
+            query = cast(statement.Statement, getattr(self, query))
+        datum = query.query
+        op = self.executor.get_explain_command(analyze, format)
+        sql = f"{op}{datum.sql}"
+        stat = dataclasses.replace(datum, sql=sql)
+        kwargs.update(transaction=True, rollback=True)
+        if op == self.executor.EXPLAIN_PREFIX:
+            kwargs["coerce"] = False
+            return self.executor.one(
+                stat,
+                *args,
+                **kwargs,
+            )
+
+        return self.executor.scalar(
+            stat,
+            *args,
+            **kwargs,
+        )
+
+
+class AsyncQueryRepository(BaseQueryRepository[_MT]):
+    """An event-loop compatible query repository (async/await)."""
+
+    isaio = True
+
+    async def __aenter__(self):
+        await self.executor.initialize()
+        return self
+
+    async def __aexit__(self, exc_type, exc_val, exc_tb):
+        await self.executor.teardown()
+        return
+
+
+class SyncQueryRepository(BaseQueryRepository[_MT]):
+    """A blocking-IO query repository."""
+
+    isaio = False
+
+    def __enter__(self):
+        self.executor.initialize()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.executor.teardown()
+        return
+
+
+_QueryNamespaceT = Union[Type[types.RepositoryProtocolT], SimpleNamespace]
+_QueryPackageStack = Deque[Tuple[_QueryNamespaceT, parse.QueryPackage]]
```

### Comparing `yesql-0.1.1/yesql/statement.py` & `yesql-1.0.0b3/yesql/statement.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,548 +1,548 @@
-from __future__ import annotations
-
-import dataclasses
-import functools
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Generic,
-    Iterable,
-    Mapping,
-    Sequence,
-    TypeVar,
-    Union,
-    cast,
-)
-
-import typic
-
-from yesql.core import parse
-
-if TYPE_CHECKING:
-    from yesql.core import types
-    from yesql.core.drivers import base
-
-
-__all__ = (
-    "statements",
-    "Statement",
-    "Affected",
-    "Many",
-    "ManyCursor",
-    "Multi",
-    "MultiCursor",
-    "One",
-    "Raw",
-    "RawCursor",
-    "Scalar",
-)
-
-
-def statements(
-    query: parse.QueryDatum,
-    *,
-    executor: base.BaseQueryExecutor = None,
-    middleware: types.MiddlewareMethodProtocolT = None,
-    serdes: SerDes[_T] = None,
-) -> Iterable[Statement[_T]]:
-    """Get the statements for a given QueryDatum.
-
-    Queries which may return multiple results or perform multiple executions will have a
-    standard statement and a cursor statement.
-    """
-    return [
-        cls(query=query, executor=executor, middleware=middleware, serdes=serdes)
-        for cls in _MODIFIER_TO_STATEMENTS[query.modifier]
-    ]
-
-
-_T = TypeVar("_T")
-
-
-SentinelType = type("NoneType")
-Sentinel = SentinelType()
-
-
-class Statement(Generic[_T]):
-    """A callable representing a single execution context for the associated query.
-
-    A Statement represents a parsed SQL query, the execution of that query, and the
-    methodology for serializing parameters and deserializing a response.
-
-    Statement instances are directly callable. The callable signature is determined
-    by the :py::meth:`~yesql.uow.Statement.execute` method for each subclass.
-
-    Attributes:
-        query: :py::class:`~yesql.core.parse.QueryDatum`
-        name: The modifier name for this unit of work.
-        executor: :py::class:`~yesql.core.drivers.base.BaseQueryExecutor`.
-        serdes: :py::class:`~yesql.uow.SerDes`.
-        middleware: A callable which will be passed the executable, query, and parameters
-    """
-
-    __slots__ = (
-        "query",
-        "name",
-        "executor",
-        "serdes",
-        "_middleware",
-        "__call__",
-    )
-    query: parse.QueryDatum
-    executor: base.BaseQueryExecutor
-    serdes: SerDes[_T]
-
-    def __init__(
-        self,
-        *,
-        query: parse.QueryDatum,
-        executor: base.BaseQueryExecutor = None,
-        middleware: types.MiddlewareMethodProtocolT = None,
-        serdes: SerDes[_T] = None,
-    ):
-        self.query = query
-        self.name = query.modifier
-        self.executor = executor
-        self.serdes = serdes or cast("SerDes[_T]", generic_serdes())
-        self._middleware = middleware
-        self.__call__ = self.execute_middleware if middleware else self.execute
-
-    def __repr__(self):
-        return (
-            f"<{self.__class__.__name__} "
-            f"query={self.query.name!r}, "
-            f"modifier={self.name!r}, "
-            f"middleware={self._middleware and self._middleware.__name__!r}"
-            f">"
-        )
-
-    @property
-    def middleware(self) -> types.MiddlewareMethodProtocolT:
-        return self._middleware
-
-    @middleware.setter
-    def middleware(self, m: types.MiddlewareMethodProtocolT | None):
-        self._middleware = m
-        self.__call__ = self.execute_middleware if m else self.execute
-
-    @middleware.deleter
-    def middleware(self):
-        self._middleware = None
-        self.__call__ = self.execute
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        """Execute the associated :py::class:`~yesql.core.parse.QueryDatum`."""
-        raise NotImplementedError()
-
-    def execute_middleware(
-        self,
-        *args,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        deserializer: base.DeserializerT | None = None,
-        **kwargs,
-    ):
-        """Execute the associated middleware.
-
-        This will pass the :py::class:`~yesql.uow.Statement` instance to the middleware
-        alongside the parameters provided at call-time.
-        """
-        deserializer = deserializer or self.serdes.bulk_deserializer
-        if deserializer:
-            kwargs["deserializer"] = deserializer
-
-        return self._middleware(
-            self,
-            *args,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **kwargs,
-        )
-
-    def _serialize_instance(
-        self,
-        *,
-        instance: _T,
-        serializer: base.SerializerT | None,
-        args: Sequence,
-        kwargs: dict,
-    ) -> tuple[Sequence, dict]:
-        if instance is None:
-            return args, kwargs
-
-        serializer = serializer or self.serdes.serializer
-        serialized = serializer(instance)
-        if isinstance(serialized, Mapping):
-            kwargs.update(serialized)
-        else:
-            args = (
-                *args,
-                *serialized,
-            )
-
-        return args, kwargs
-
-    def _serialize_instances(
-        self,
-        *,
-        instances: Iterable[_T] = (),
-        params: Iterable,
-        serializer: base.SerializerT | None,
-    ):
-        if not instances:
-            return params
-        serializer = serializer or self.serdes.serializer
-        serialized = [*params, *(serializer(i) for i in instances)]
-        return serialized
-
-
-class StatementCursor(Statement[_T]):
-    """The StatementCursor provides direct access to a query result cursor."""
-
-    def __init__(
-        self,
-        *,
-        query: parse.QueryDatum,
-        executor: base.BaseQueryExecutor = None,
-        middleware: types.MiddlewareMethodProtocolT = None,
-        serdes: SerDes[_T] = None,
-    ):
-        query = self._cursor_datum(query)
-        super().__init__(
-            query=query, executor=executor, middleware=middleware, serdes=serdes
-        )
-
-    @typic.fastcachedmethod
-    def _cursor_datum(self, query: parse.QueryDatum) -> parse.QueryDatum:
-        if query.name.endswith("_cursor"):
-            return query
-        return dataclasses.replace(query, name=query.name + "_cursor")
-
-
-class Many(Statement[_T]):
-    """Execute a query, returning all results as a list."""
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        coerce: bool = True,
-        deserializer: base.DeserializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        deserializer = deserializer or self.serdes.bulk_deserializer
-        return self.executor.many(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            deserializer=deserializer if coerce else None,
-            **skwargs,
-        )
-
-
-class ManyCursor(StatementCursor):
-    """Execute a query, returning all results as a cursor."""
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        return self.executor.many_cursor(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **skwargs,
-        )
-
-
-class Raw(Statement):
-    """Execute a query, returning all results as a list, without deserialization."""
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        return self.executor.raw(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **skwargs,
-        )
-
-
-class RawCursor(StatementCursor):
-    """Execute a query, returning all results as a cursor."""
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        return self.executor.raw_cursor(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **skwargs,
-        )
-
-
-class One(Statement):
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT = None,
-        coerce: bool = True,
-        deserializer: base.DeserializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        deserializer = deserializer or self.serdes.deserializer
-        return self.executor.one(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            deserializer=deserializer if coerce else None,
-            **skwargs,
-        )
-
-
-class Scalar(Statement):
-    """Execute a query, returning a single value from the first result."""
-
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance, serializer=serializer, args=args, kwargs=kwargs
-        )
-        return self.executor.scalar(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **skwargs,
-        )
-
-
-class Multi(Statement):
-    """Execute a query with multiple sets of parameters, returning all results."""
-
-    def execute(  # type: ignore[override]
-        self,
-        *,
-        instances: Iterable[_T] = (),
-        params: Iterable[Sequence | Mapping[str, Any]] = (),
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        coerce: bool = True,
-        returns: bool = False,
-        deserializer: base.DeserializerT | None = None,
-        serializer: base.SerializerT | None = None,
-    ):
-        params = self._serialize_instances(
-            instances=instances, params=params, serializer=serializer
-        )
-        deserializer = deserializer or self.serdes.bulk_deserializer
-        return self.executor.multi(
-            self.query,
-            params=params,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            returns=returns,
-            deserializer=deserializer if coerce else None,
-        )
-
-
-class MultiCursor(StatementCursor):
-    """Execute a query with multiple sets of parameters, returning a cursor."""
-
-    def execute(  # type: ignore[override]
-        self,
-        *,
-        instances: Iterable[_T] = (),
-        params: Iterable[Sequence | Mapping[str, Any]] = (),
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **_,
-    ):
-        params = self._serialize_instances(
-            instances=instances, params=params, serializer=serializer
-        )
-        return self.executor.multi_cursor(
-            self.query,
-            params=params,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-        )
-
-
-class Affected(Statement):
-    def execute(
-        self,
-        *args,
-        instance: _T = None,
-        connection: types.ConnectionT = None,
-        timeout: float = 10,
-        transaction: bool = True,
-        rollback: bool = False,
-        serializer: base.SerializerT | None = None,
-        **kwargs,
-    ):
-        sargs, skwargs = self._serialize_instance(
-            instance=instance,
-            serializer=serializer,
-            args=args,
-            kwargs=kwargs,
-        )
-        return self.executor.affected(
-            self.query,
-            *sargs,
-            connection=connection,
-            timeout=timeout,
-            transaction=transaction,
-            rollback=rollback,
-            **skwargs,
-        )
-
-
-@typic.slotted(dict=False, weakref=True)
-@dataclasses.dataclass
-class SerDes(Generic[_T]):
-    """A container for Serializer and Deserializers bound to a specifc type.
-
-    This is used by the :py::class:`~yesql.uow.Statement` to serialize model instances
-    for query execution and also deserialize query responses.
-    """
-
-    serializer: base.SerializerT[_T]
-    deserializer: base.DeserializerT[_T | None]
-    bulk_deserializer: base.DeserializerT[Iterable[_T]]
-
-
-@functools.lru_cache(maxsize=1)
-def generic_serdes() -> SerDes[dict]:
-    serdes = SerDes(
-        serializer=cast("base.SerializerT[dict]", typic.primitive),
-        deserializer=cast(
-            "base.DeserializerT[dict | None]",
-            typic.protocol(dict, is_optional=True).transmute,
-        ),
-        bulk_deserializer=cast(
-            "base.DeserializerT[Iterable[dict]]",
-            typic.protocol(Iterable[dict]).transmute,  # type: ignore[misc]
-        ),
-    )
-    return serdes
-
-
-StatementsT = Union[
-    Affected,
-    Many,
-    ManyCursor,
-    Multi,
-    MultiCursor,
-    One,
-    Raw,
-    RawCursor,
-    Scalar,
-]
-_MODIFIER_TO_STATEMENTS: dict[parse.ModifierT, list[type[StatementsT]]] = {
-    parse.AFFECTED: [Affected],
-    parse.MANY: [Many, ManyCursor],
-    parse.MULTI: [Multi, MultiCursor],
-    parse.ONE: [One],
-    parse.RAW: [Raw, RawCursor],
-    parse.SCALAR: [Scalar],
-}
+from __future__ import annotations
+
+import dataclasses
+import functools
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Generic,
+    Iterable,
+    Mapping,
+    Sequence,
+    TypeVar,
+    Union,
+    cast,
+)
+
+import typic
+
+from yesql.core import parse
+
+if TYPE_CHECKING:
+    from yesql.core import types
+    from yesql.core.drivers import base
+
+
+__all__ = (
+    "statements",
+    "Statement",
+    "Affected",
+    "Many",
+    "ManyCursor",
+    "Multi",
+    "MultiCursor",
+    "One",
+    "Raw",
+    "RawCursor",
+    "Scalar",
+)
+
+
+def statements(
+    query: parse.QueryDatum,
+    *,
+    executor: base.BaseQueryExecutor = None,
+    middleware: types.MiddlewareMethodProtocolT = None,
+    serdes: SerDes[_T] = None,
+) -> Iterable[Statement[_T]]:
+    """Get the statements for a given QueryDatum.
+
+    Queries which may return multiple results or perform multiple executions will have a
+    standard statement and a cursor statement.
+    """
+    return [
+        cls(query=query, executor=executor, middleware=middleware, serdes=serdes)
+        for cls in _MODIFIER_TO_STATEMENTS[query.modifier]
+    ]
+
+
+_T = TypeVar("_T")
+
+
+SentinelType = type("NoneType")
+Sentinel = SentinelType()
+
+
+class Statement(Generic[_T]):
+    """A callable representing a single execution context for the associated query.
+
+    A Statement represents a parsed SQL query, the execution of that query, and the
+    methodology for serializing parameters and deserializing a response.
+
+    Statement instances are directly callable. The callable signature is determined
+    by the :py::meth:`~yesql.uow.Statement.execute` method for each subclass.
+
+    Attributes:
+        query: :py::class:`~yesql.core.parse.QueryDatum`
+        name: The modifier name for this unit of work.
+        executor: :py::class:`~yesql.core.drivers.base.BaseQueryExecutor`.
+        serdes: :py::class:`~yesql.uow.SerDes`.
+        middleware: A callable which will be passed the executable, query, and parameters
+    """
+
+    __slots__ = (
+        "query",
+        "name",
+        "executor",
+        "serdes",
+        "_middleware",
+        "__call__",
+    )
+    query: parse.QueryDatum
+    executor: base.BaseQueryExecutor
+    serdes: SerDes[_T]
+
+    def __init__(
+        self,
+        *,
+        query: parse.QueryDatum,
+        executor: base.BaseQueryExecutor = None,
+        middleware: types.MiddlewareMethodProtocolT = None,
+        serdes: SerDes[_T] = None,
+    ):
+        self.query = query
+        self.name = query.modifier
+        self.executor = executor
+        self.serdes = serdes or cast("SerDes[_T]", generic_serdes())
+        self._middleware = middleware
+        self.__call__ = self.execute_middleware if middleware else self.execute
+
+    def __repr__(self):
+        return (
+            f"<{self.__class__.__name__} "
+            f"query={self.query.name!r}, "
+            f"modifier={self.name!r}, "
+            f"middleware={self._middleware and self._middleware.__name__!r}"
+            f">"
+        )
+
+    @property
+    def middleware(self) -> types.MiddlewareMethodProtocolT:
+        return self._middleware
+
+    @middleware.setter
+    def middleware(self, m: types.MiddlewareMethodProtocolT | None):
+        self._middleware = m
+        self.__call__ = self.execute_middleware if m else self.execute
+
+    @middleware.deleter
+    def middleware(self):
+        self._middleware = None
+        self.__call__ = self.execute
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        """Execute the associated :py::class:`~yesql.core.parse.QueryDatum`."""
+        raise NotImplementedError()
+
+    def execute_middleware(
+        self,
+        *args,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        deserializer: types.DeserializerT | None = None,
+        **kwargs,
+    ):
+        """Execute the associated middleware.
+
+        This will pass the :py::class:`~yesql.uow.Statement` instance to the middleware
+        alongside the parameters provided at call-time.
+        """
+        deserializer = deserializer or self.serdes.bulk_deserializer
+        if deserializer:
+            kwargs["deserializer"] = deserializer
+
+        return self._middleware(
+            self,
+            *args,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **kwargs,
+        )
+
+    def _serialize_instance(
+        self,
+        *,
+        instance: _T,
+        serializer: types.SerializerT | None,
+        args: Sequence,
+        kwargs: dict,
+    ) -> tuple[Sequence, dict]:
+        if instance is None:
+            return args, kwargs
+
+        serializer = serializer or self.serdes.serializer
+        serialized = serializer(instance)
+        if isinstance(serialized, Mapping):
+            kwargs.update(serialized)
+        else:
+            args = (
+                *args,
+                *serialized,
+            )
+
+        return args, kwargs
+
+    def _serialize_instances(
+        self,
+        *,
+        instances: Iterable[_T] = (),
+        params: Iterable,
+        serializer: types.SerializerT | None,
+    ):
+        if not instances:
+            return params
+        serializer = serializer or self.serdes.serializer
+        serialized = [*params, *(serializer(i) for i in instances)]
+        return serialized
+
+
+class StatementCursor(Statement[_T]):
+    """The StatementCursor provides direct access to a query result cursor."""
+
+    def __init__(
+        self,
+        *,
+        query: parse.QueryDatum,
+        executor: base.BaseQueryExecutor = None,
+        middleware: types.MiddlewareMethodProtocolT = None,
+        serdes: SerDes[_T] = None,
+    ):
+        query = self._cursor_datum(query)
+        super().__init__(
+            query=query, executor=executor, middleware=middleware, serdes=serdes
+        )
+
+    @typic.fastcachedmethod
+    def _cursor_datum(self, query: parse.QueryDatum) -> parse.QueryDatum:
+        if query.name.endswith("_cursor"):
+            return query
+        return dataclasses.replace(query, name=query.name + "_cursor")
+
+
+class Many(Statement[_T]):
+    """Execute a query, returning all results as a list."""
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        coerce: bool = True,
+        deserializer: types.DeserializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        deserializer = deserializer or self.serdes.bulk_deserializer
+        return self.executor.many(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            deserializer=deserializer if coerce else None,
+            **skwargs,
+        )
+
+
+class ManyCursor(StatementCursor):
+    """Execute a query, returning all results as a cursor."""
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        return self.executor.many_cursor(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **skwargs,
+        )
+
+
+class Raw(Statement):
+    """Execute a query, returning all results as a list, without deserialization."""
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        return self.executor.raw(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **skwargs,
+        )
+
+
+class RawCursor(StatementCursor):
+    """Execute a query, returning all results as a cursor."""
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        return self.executor.raw_cursor(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **skwargs,
+        )
+
+
+class One(Statement):
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT = None,
+        coerce: bool = True,
+        deserializer: types.DeserializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        deserializer = deserializer or self.serdes.deserializer
+        return self.executor.one(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            deserializer=deserializer if coerce else None,
+            **skwargs,
+        )
+
+
+class Scalar(Statement):
+    """Execute a query, returning a single value from the first result."""
+
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance, serializer=serializer, args=args, kwargs=kwargs
+        )
+        return self.executor.scalar(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **skwargs,
+        )
+
+
+class Multi(Statement):
+    """Execute a query with multiple sets of parameters, returning all results."""
+
+    def execute(  # type: ignore[override]
+        self,
+        *,
+        instances: Iterable[_T] = (),
+        params: Iterable[Sequence | Mapping[str, Any]] = (),
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        coerce: bool = True,
+        returns: bool = False,
+        deserializer: types.DeserializerT | None = None,
+        serializer: types.SerializerT | None = None,
+    ):
+        params = self._serialize_instances(
+            instances=instances, params=params, serializer=serializer
+        )
+        deserializer = deserializer or self.serdes.bulk_deserializer
+        return self.executor.multi(
+            self.query,
+            params=params,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            returns=returns,
+            deserializer=deserializer if coerce else None,
+        )
+
+
+class MultiCursor(StatementCursor):
+    """Execute a query with multiple sets of parameters, returning a cursor."""
+
+    def execute(  # type: ignore[override]
+        self,
+        *,
+        instances: Iterable[_T] = (),
+        params: Iterable[Sequence | Mapping[str, Any]] = (),
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **_,
+    ):
+        params = self._serialize_instances(
+            instances=instances, params=params, serializer=serializer
+        )
+        return self.executor.multi_cursor(
+            self.query,
+            params=params,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+        )
+
+
+class Affected(Statement):
+    def execute(
+        self,
+        *args,
+        instance: _T = None,
+        connection: types.ConnectionT = None,
+        timeout: float = 10,
+        transaction: bool = True,
+        rollback: bool = False,
+        serializer: types.SerializerT | None = None,
+        **kwargs,
+    ):
+        sargs, skwargs = self._serialize_instance(
+            instance=instance,
+            serializer=serializer,
+            args=args,
+            kwargs=kwargs,
+        )
+        return self.executor.affected(
+            self.query,
+            *sargs,
+            connection=connection,
+            timeout=timeout,
+            transaction=transaction,
+            rollback=rollback,
+            **skwargs,
+        )
+
+
+@typic.slotted(dict=False, weakref=True)
+@dataclasses.dataclass
+class SerDes(Generic[_T]):
+    """A container for Serializer and Deserializers bound to a specifc type.
+
+    This is used by the :py::class:`~yesql.uow.Statement` to serialize model instances
+    for query execution and also deserialize query responses.
+    """
+
+    serializer: types.SerializerT[_T]
+    deserializer: types.DeserializerT[_T | None]
+    bulk_deserializer: types.DeserializerT[Iterable[_T]]
+
+
+@functools.lru_cache(maxsize=1)
+def generic_serdes() -> SerDes[dict]:
+    serdes = SerDes(
+        serializer=cast("types.SerializerT[dict]", typic.primitive),
+        deserializer=cast(
+            "types.DeserializerT[dict | None]",
+            typic.protocol(dict, is_optional=True).transmute,
+        ),
+        bulk_deserializer=cast(
+            "types.DeserializerT[Iterable[dict]]",
+            typic.protocol(Iterable[dict]).transmute,  # type: ignore[type-abstract]
+        ),
+    )
+    return serdes
+
+
+StatementsT = Union[
+    Affected,
+    Many,
+    ManyCursor,
+    Multi,
+    MultiCursor,
+    One,
+    Raw,
+    RawCursor,
+    Scalar,
+]
+_MODIFIER_TO_STATEMENTS: dict[parse.ModifierT, list[type[StatementsT]]] = {
+    parse.AFFECTED: [Affected],
+    parse.MANY: [Many, ManyCursor],
+    parse.MULTI: [Multi, MultiCursor],
+    parse.ONE: [One],
+    parse.RAW: [Raw, RawCursor],
+    parse.SCALAR: [Scalar],
+}
```

