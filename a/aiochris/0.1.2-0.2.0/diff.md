# Comparing `tmp/aiochris-0.1.2.tar.gz` & `tmp/aiochris-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiochris-0.1.2.tar", max compression
+gzip compressed data, was "aiochris-0.2.0.tar", max compression
```

## Comparing `aiochris-0.1.2.tar` & `aiochris-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-04-25 22:52:23.461068 aiochris-0.1.2/LICENSE
--rw-r--r--   0        0        0     1735 2023-04-25 22:52:23.461068 aiochris-0.1.2/README.md
--rw-r--r--   0        0        0      550 2023-04-25 22:52:23.461068 aiochris-0.1.2/chris/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 22:52:23.461068 aiochris-0.1.2/chris/client/__init__.py
--rw-r--r--   0        0        0     6191 2023-04-25 22:52:23.461068 aiochris-0.1.2/chris/client/admin.py
--rw-r--r--   0        0        0     1317 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/client/anon.py
--rw-r--r--   0        0        0     9579 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/client/authed.py
--rw-r--r--   0        0        0     3486 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/client/base.py
--rw-r--r--   0        0        0     1692 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/client/normal.py
--rw-r--r--   0        0        0     2229 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/examples.md
--rw-r--r--   0        0        0     4805 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/home.md
--rw-r--r--   0        0        0       97 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/link/__init__.py
--rw-r--r--   0        0        0     1134 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/link/collection_client.py
--rw-r--r--   0        0        0     4957 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/link/http.py
--rw-r--r--   0        0        0     4655 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/link/linked.py
--rw-r--r--   0        0        0     1450 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/link/metaprog.py
--rw-r--r--   0        0        0        0 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/__init__.py
--rw-r--r--   0        0        0     1635 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/collection_links.py
--rw-r--r--   0        0        0     2897 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/data.py
--rw-r--r--   0        0        0      644 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/enums.py
--rw-r--r--   0        0        0     5037 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/logged_in.py
--rw-r--r--   0        0        0      824 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/public.py
--rw-r--r--   0        0        0     3118 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/models/types.py
--rw-r--r--   0        0        0       31 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/util/__init__.py
--rw-r--r--   0        0        0      698 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/util/errors.py
--rw-r--r--   0        0        0     6891 2023-04-25 22:52:23.465068 aiochris-0.1.2/chris/util/search.py
--rw-r--r--   0        0        0      807 2023-04-25 22:52:23.465068 aiochris-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2577 1970-01-01 00:00:00.000000 aiochris-0.1.2/setup.py
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 aiochris-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-25 22:52:21.857534 aiochris-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1738 2023-04-25 22:52:21.857534 aiochris-0.2.0/README.md
+-rw-r--r--   0        0        0      574 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/__init__.py
+-rw-r--r--   0        0        0     6243 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/admin.py
+-rw-r--r--   0        0        0     1335 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/anon.py
+-rw-r--r--   0        0        0     9627 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/authed.py
+-rw-r--r--   0        0        0     3495 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/base.py
+-rw-r--r--   0        0        0     1707 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/client/normal.py
+-rw-r--r--   0        0        0     2284 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/examples.md
+-rw-r--r--   0        0        0     4811 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/home.md
+-rw-r--r--   0        0        0       97 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/__init__.py
+-rw-r--r--   0        0        0     1143 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/collection_client.py
+-rw-r--r--   0        0        0     4969 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/http.py
+-rw-r--r--   0        0        0     4664 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/linked.py
+-rw-r--r--   0        0        0     1450 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/link/metaprog.py
+-rw-r--r--   0        0        0        0 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/collection_links.py
+-rw-r--r--   0        0        0     2912 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/data.py
+-rw-r--r--   0        0        0      644 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/enums.py
+-rw-r--r--   0        0        0     5061 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/logged_in.py
+-rw-r--r--   0        0        0      833 2023-04-25 22:52:21.857534 aiochris-0.2.0/aiochris/models/public.py
+-rw-r--r--   0        0        0     3118 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/models/types.py
+-rw-r--r--   0        0        0       31 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/__init__.py
+-rw-r--r--   0        0        0      698 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/errors.py
+-rw-r--r--   0        0        0     6920 2023-04-25 22:52:21.861534 aiochris-0.2.0/aiochris/util/search.py
+-rw-r--r--   0        0        0      768 2023-04-25 22:52:21.861534 aiochris-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 aiochris-0.2.0/setup.py
+-rw-r--r--   0        0        0     2368 1970-01-01 00:00:00.000000 aiochris-0.2.0/PKG-INFO
```

### Comparing `aiochris-0.1.2/LICENSE` & `aiochris-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiochris-0.1.2/README.md` & `aiochris-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 poetry add aiochris
 ```
 
 ## Quick Example
 
 ```python
 import asyncio
-from chris import ChrisClient
+from aiochris import ChrisClient
 
 
 async def readme_example():
     chris = await ChrisClient.from_login(
         username='chris',
         password='chris1234',
         url='https://cube.chrisproject.org/api/v1/'
```

### Comparing `aiochris-0.1.2/chris/__init__.py` & `aiochris-0.2.0/aiochris/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 .. include:: ./home.md
 
 .. include:: ./examples.md
 """
 
-import chris.client
-import chris.models
-import chris.util
-from chris.util.search import Search, acollect
-from chris.client.normal import ChrisClient
-from chris.client.anon import AnonChrisClient
-from chris.client.admin import ChrisAdminClient
-from chris.models.enums import Status, ParameterTypeName
+import aiochris.client
+import aiochris.models
+import aiochris.util
+from aiochris.util.search import Search, acollect
+from aiochris.client.normal import ChrisClient
+from aiochris.client.anon import AnonChrisClient
+from aiochris.client.admin import ChrisAdminClient
+from aiochris.models.enums import Status, ParameterTypeName
 
 __all__ = [
     "AnonChrisClient",
     "ChrisClient",
     "ChrisAdminClient",
     "Search",
     "acollect",
```

### Comparing `aiochris-0.1.2/chris/client/admin.py` & `aiochris-0.2.0/aiochris/client/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 import json
 from typing import Iterable
 
 import aiohttp
 from async_property import async_cached_property
 from serde import from_dict
 
-from chris.client.authed import AuthenticatedClient
-from chris.link import http
-from chris.link.collection_client import CollectionJsonApiClient
-from chris.link.linked import deserialize_linked
-from chris.models.collection_links import AdminCollectionLinks, AdminApiCollectionLinks
-from chris.models.logged_in import Plugin
-from chris.models.public import ComputeResource
-from chris.models.types import PluginUrl, ComputeResourceName, PfconUrl
-from chris.util.errors import raise_for_status
+from aiochris.client.authed import AuthenticatedClient
+from aiochris.link import http
+from aiochris.link.collection_client import CollectionJsonApiClient
+from aiochris.link.linked import deserialize_linked
+from aiochris.models.collection_links import (
+    AdminCollectionLinks,
+    AdminApiCollectionLinks,
+)
+from aiochris.models.logged_in import Plugin
+from aiochris.models.public import ComputeResource
+from aiochris.models.types import PluginUrl, ComputeResourceName, PfconUrl
+from aiochris.util.errors import raise_for_status
 
 
 class _AdminApiClient(CollectionJsonApiClient[AdminApiCollectionLinks]):
     """
     A client to `/chris-admin/api/v1/`
     """
 
@@ -75,30 +78,30 @@
         ```
 
         The example above is just for show. It's not a good example for several reasons:
 
         - Calls blocking function `subprocess.check_output` in asynchronous context
         - It is preferred to use a versioned string for `dock_image`
         - `host` compute environment is not guaranteed to exist. Instead, you could
-          call `chris.client.authed.AuthenticatedClient.search_compute_resources`
-          or `chris.client.authed.AuthenticatedClient.get_all_compute_resources`:
+          call `aiochris.client.authed.AuthenticatedClient.search_compute_resources`
+          or `aiochris.client.authed.AuthenticatedClient.get_all_compute_resources`:
 
         ```python
         all_computes = await chris_admin.get_all_compute_resources()
         await chris_admin.add_plugin(plugin_description=desc, compute_resources=all_computes)
         ```
 
         Parameters
         ----------
         plugin_description: str | dict
             JSON description of a plugin.
             [spec](https://github.com/FNNDSC/CHRIS_docs/blob/5078aaf934bdbe313e85367f88aff7c14730a1d4/specs/ChRIS_Plugins.adoc#descriptor_file)
         compute_resources
             Compute resources to register the plugin to. Value can be either a comma-separated `str` of names,
-            a `chris.models.public.ComputeResource`, a sequence of `chris.models.public.ComputeResource`,
+            a `aiochris.models.public.ComputeResource`, a sequence of `aiochris.models.public.ComputeResource`,
             or a sequence of compute resource names as `str`.
         fname: str
             File name to send along in the multi-part POST request. Not important.
         """
         compute_names = _serialize_crs(compute_resources)
         if not isinstance(plugin_description, str):
             plugin_description = json.dumps(plugin_description)
```

### Comparing `aiochris-0.1.2/chris/client/anon.py` & `aiochris-0.2.0/aiochris/client/anon.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Optional
 
 import aiohttp
 
-from chris.client.base import BaseChrisClient
-from chris.link import http
-from chris.models.collection_links import AnonymousCollectionLinks
-from chris.models.public import PublicPlugin
-from chris.util.search import Search
+from aiochris.client.base import BaseChrisClient
+from aiochris.link import http
+from aiochris.models.collection_links import AnonymousCollectionLinks
+from aiochris.models.public import PublicPlugin
+from aiochris.util.search import Search
 
 
 class AnonChrisClient(BaseChrisClient[AnonymousCollectionLinks, "AnonChrisClient"]):
     """
     An anonymous ChRIS client. It has access to read-only GET resources,
     such as being able to search for plugins.
     """
@@ -22,15 +22,15 @@
         max_search_requests: int = 100,
         connector: Optional[aiohttp.BaseConnector] = None,
         connector_owner: bool = True,
     ) -> "AnonChrisClient":
         """
         Create an anonymous client.
 
-        See `chris.client.base.BaseChrisClient.new` for parameter documentation.
+        See `aiochris.client.base.BaseChrisClient.new` for parameter documentation.
         """
         return await cls.new(
             url=url,
             max_search_requests=max_search_requests,
             connector=connector,
             connector_owner=connector_owner,
         )
```

### Comparing `aiochris-0.1.2/chris/client/authed.py` & `aiochris-0.2.0/aiochris/client/authed.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import os
 from pathlib import Path
 from typing import Optional, Generic, Callable, Sequence
 
 import aiohttp
 from async_property import async_cached_property
 
-from chris.client.base import BaseChrisClient
-from chris.client.base import L, CSelf
-from chris.link import http
-from chris.link.linked import deserialize_res
-from chris.models.logged_in import Plugin, File, User, PluginInstance, Feed
-from chris.models.public import ComputeResource
-from chris.models.types import ChrisURL, Username, Password
-from chris.util.errors import IncorrectLoginError, raise_for_status
-from chris.util.search import Search, acollect
+from aiochris.client.base import BaseChrisClient
+from aiochris.client.base import L, CSelf
+from aiochris.link import http
+from aiochris.link.linked import deserialize_res
+from aiochris.models.logged_in import Plugin, File, User, PluginInstance, Feed
+from aiochris.models.public import ComputeResource
+from aiochris.models.types import ChrisURL, Username, Password
+from aiochris.util.errors import IncorrectLoginError, raise_for_status
+from aiochris.util.search import Search, acollect
 
 
 class AuthenticatedClient(BaseChrisClient[L, CSelf], Generic[L, CSelf], abc.ABC):
     """
     An authenticated ChRIS client.
     """
 
@@ -31,15 +31,15 @@
         max_search_requests: int = 100,
         connector: Optional[aiohttp.TCPConnector] = None,
         connector_owner: bool = True,
     ) -> CSelf:
         """
         Get authentication token using username and password, then construct the client.
 
-        See `chris.client.base.BaseChrisClient.new` for parameter documentation.
+        See `aiochris.client.base.BaseChrisClient.new` for parameter documentation.
         """
         async with aiohttp.ClientSession(
             connector=connector, connector_owner=False
         ) as session:
             try:
                 c = await cls.__from_login_with(
                     url=url,
@@ -90,15 +90,15 @@
         max_search_requests: int,
         connector: Optional[aiohttp.TCPConnector] = None,
         connector_owner: Optional[bool] = True,
     ) -> CSelf:
         """
         Construct an authenticated client using the given token.
 
-        See `chris.client.base.BaseChrisClient.new` for parameter documentation.
+        See `aiochris.client.base.BaseChrisClient.new` for parameter documentation.
         """
         return await cls.new(
             url=url,
             max_search_requests=max_search_requests,
             connector=connector,
             connector_owner=connector_owner,
             session_modifier=cls.__curry_token(token),
@@ -149,29 +149,29 @@
 
         Examples
         --------
 
         Upload a single file:
 
         ```python
-        chris = await ChrisClient.from_login(
+        aiochris = await ChrisClient.from_login(
             username='chris',
             password='chris1234',
             url='https://cube.chrisproject.org/api/v1/'
         )
-        file = await chris.upload_file("./my_data.dat", 'dir/my_data.dat')
-        assert file.fname == 'chris/uploads/dir/my_data.dat'
+        file = await aiochris.upload_file("./my_data.dat", 'dir/my_data.dat')
+        assert file.fname == 'aiochris/uploads/dir/my_data.dat'
         ```
 
         Upload (in parallel) all `*.txt` files in a directory
-        `'incoming'` to `chris/uploads/big_folder`:
+        `'incoming'` to `aiochris/uploads/big_folder`:
 
         ```python
         upload_jobs = (
-            chris.upload_file(p, f'big_folder/{p}')
+            aiochris.upload_file(p, f'big_folder/{p}')
             for p in Path('incoming')
         )
         await asyncio.gather(upload_jobs)
         ```
 
         Parameters
         ----------
```

### Comparing `aiochris-0.1.2/chris/client/base.py` & `aiochris-0.2.0/aiochris/client/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 from typing import AsyncContextManager, Generic, Optional, Callable, TypeVar
 
 import aiohttp
 from serde import from_dict
 
-from chris.link.collection_client import L, CollectionJsonApiClient
-from chris.util.errors import raise_for_status
+from aiochris.link.collection_client import L, CollectionJsonApiClient
+from aiochris.util.errors import raise_for_status
 
 CSelf = TypeVar(
     "CSelf", bound="BaseChrisClient"
 )  # can't wait for `Self` in Python 3.11!
 
 
 class BaseChrisClient(
@@ -38,15 +38,15 @@
 
         Parameters
         ----------
         url
             ChRIS backend url, e.g. "https://cube.chrisproject.org/api/v1/"
         max_search_requests
             Maximum number of HTTP requests to make while retrieving items from a
-            paginated endpoint before raising `chris.util.search.TooMuchPaginationError`.
+            paginated endpoint before raising `aiochris.util.search.TooMuchPaginationError`.
             Use `max_search_requests=-1` to allow for "infinite" pagination
             (well, you're still limited by Python's stack).
         connector
             [`aiohttp.BaseConnector`](https://docs.aiohttp.org/en/v3.8.3/client_advanced.html#connectors) to use.
             If creating multiple client objects in the same program,
             reusing connectors between them is more efficient.
         connector_owner
```

### Comparing `aiochris-0.1.2/chris/client/normal.py` & `aiochris-0.2.0/aiochris/client/normal.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from contextlib import asynccontextmanager
 from typing import Optional
 
 import aiohttp
 from serde.json import from_json
 
-from chris.client.authed import AuthenticatedClient
-from chris.util.errors import raise_for_status
-from chris.models.collection_links import CollectionLinks
-from chris.models.data import UserData
-from chris.models.types import ChrisURL, Username, Password
+from aiochris.client.authed import AuthenticatedClient
+from aiochris.util.errors import raise_for_status
+from aiochris.models.collection_links import CollectionLinks
+from aiochris.models.data import UserData
+from aiochris.models.types import ChrisURL, Username, Password
 
 
 class ChrisClient(AuthenticatedClient[CollectionLinks, "ChrisClient"]):
     """
     A normal user *ChRIS* client, who may upload files and create plugin instances.
     """
```

### Comparing `aiochris-0.1.2/chris/examples.md` & `aiochris-0.2.0/aiochris/examples.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ## Examples
 
 #### Create a client given username and password
 
 ```python
-from chris import ChrisClient
+from aiochris import ChrisClient
 
 chris = await ChrisClient.from_login(
     url='https://cube.chrisproject.org/api/v1/',
     username='chris',
     password='chris1234'
 )
 ```
@@ -61,16 +61,17 @@
     print(f'"{p.title}" finished on date: {p.end_date}')
 ```
 
 #### Delete all plugin instances with a given title, in parallel
 
 ```python
 import asyncio
-from chris import acollect
+from aiochris import ChrisClient, acollect
 
+chris = ChrisClient.from_login(...)
 search = chris.plugin_instances(title="delete me")
 plugin_instances = await acollect(search)
 await asyncio.gather(*(p.delete() for p in plugin_instances))
 ```
 
 #### Enable Debug Logging
```

### Comparing `aiochris-0.1.2/chris/home.md` & `aiochris-0.2.0/aiochris/home.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # or
 poetry add aiochris
 ```
 
 ## Brief Example
 
 ```python
-from chris import ChrisClient
+from aiochris import ChrisClient
 
 chris = await ChrisClient.from_login(
     username='chris',
     password='chris1234',
     url='https://cube.chrisproject.org/api/v1/'
 )
 dircopy = await chris.search_plugins(name_exact='pl-brainmgz', version='2.0.3').get_only()
@@ -98,15 +98,15 @@
 including all `aiochris` clients and other `aiohttp` clients.
 
 <details>
 <summary>Example: efficiently using multiple aiohttp clients</summary>
 
 ```python
 import aiohttp
-from chris import ChrisClient
+from aiochris import ChrisClient
 
 with aiohttp.TCPConnector() as connector:
     chris_client1 = await ChrisClient.from_login(
         url='https://example.com/cube/api/v1/',
         username='user1',
         password='user1234',
         connector=connector,
```

### Comparing `aiochris-0.1.2/chris/link/collection_client.py` & `aiochris-0.2.0/aiochris/link/collection_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 from typing import TypeVar, Generic, Type
 
 import yarl
 
-from chris.link.linked import Linked
-from chris.link.metaprog import generic_of
-from chris.models.collection_links import AbstractCollectionLinks
+from aiochris.link.linked import Linked
+from aiochris.link.metaprog import generic_of
+from aiochris.models.collection_links import AbstractCollectionLinks
 
 L = TypeVar("L", bound=AbstractCollectionLinks)
 
 
 @dataclasses.dataclass(frozen=True)
 class CollectionJsonApiClient(Generic[L], Linked):
     """
```

### Comparing `aiochris-0.1.2/chris/link/http.py` & `aiochris-0.2.0/aiochris/link/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     AsyncContextManager,
     Coroutine,
 )
 
 import aiohttp
 import yarl
 
-from chris.link.linked import LinkedMeta, Linked, deserialize_res
-from chris.link.metaprog import get_return_hint
-from chris.util.search import Search
+from aiochris.link.linked import LinkedMeta, Linked, deserialize_res
+from aiochris.link.metaprog import get_return_hint
+from aiochris.util.search import Search
 
 logger = logging.getLogger(__name__)
 
 _R = TypeVar("_R")
 
 # Some metaprogramming gotchas:
 # The type annotations of a function given to a decorator might not exist
@@ -95,15 +95,15 @@
 
 def _http_method_decorator(
     link_name: str, method_name: str, request: Request
 ) -> Callable[
     [Callable[..., Coroutine[None, None, _R]]], Callable[..., Coroutine[None, None, _R]]
 ]:
     """
-    Creates a decorator which transforms a method of a subclass of `chris.link.Linked`
+    Creates a decorator which transforms a method of a subclass of `aiochris.link.Linked`
     to one which makes an HTTP request.
     """
 
     def decorator(
         fn: Callable[..., Coroutine[None, None, _R]]
     ) -> Callable[..., Coroutine[None, None, _R]]:
         @functools.wraps(fn)
```

### Comparing `aiochris-0.1.2/chris/link/linked.py` & `aiochris-0.2.0/aiochris/link/linked.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     AsyncContextManager,
 )
 
 import aiohttp
 import serde
 import yarl
 
-from chris.util.errors import raise_for_status, ResponseError
+from aiochris.util.errors import raise_for_status, ResponseError
 
 T = TypeVar("T")
 
 
 class LinkedMeta(abc.ABCMeta):
     """
     A metaclass for HTTP clients which make requests to URIs
@@ -48,15 +48,15 @@
         return issubclass(c, Linked)
 
     @classmethod
     def _validate_collection_names(mcs, cls: Type["Linked"], dct: dict[str, Any]):
         """
         Check that every method marked by `mark_to_check` was given a collection name
         which exists as a field in the class's associated
-        `chris.models.collection_links.AbstractCollectionLinks` type.
+        `aiochris.models.collection_links.AbstractCollectionLinks` type.
         """
         marked_methods = filter(None, map(mcs._get_marked, dct.values()))
         for collection_name, method in marked_methods:
             if not cls._has_link(collection_name):
                 raise TypeError(
                     f'Method {method} needs link "{collection_name}" '
                     f"but {cls} does not have it"
@@ -127,15 +127,15 @@
     def _get_link(self, name: str) -> yarl.URL:
         return yarl.URL(getattr(self, name))
 
 
 def deserialize_linked(client: Linked, t: Type[T], o: dict) -> T:
     """
     Wraps `serde.from_dict`.
-    If `t` is a subclass of `chris.models.connected.Connected`, its session is set.
+    If `t` is a subclass of `aiochris.models.connected.Connected`, its session is set.
 
     Side effect: o is mutated
     """
     if issubclass(t, LinkedModel):
         o["s"] = client.s
         o["max_search_requests"] = client.max_search_requests
     return serde.from_dict(t, o, reuse_instances=True)
```

### Comparing `aiochris-0.1.2/chris/link/metaprog.py` & `aiochris-0.2.0/aiochris/link/metaprog.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.1.2/chris/models/collection_links.py` & `aiochris-0.2.0/aiochris/models/collection_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 import functools
 from dataclasses import dataclass
 from typing import Iterator
 
 from serde import deserialize
 
-from chris.models.types import ApiUrl, UserUrl, AdminUrl
+from aiochris.models.types import ApiUrl, UserUrl, AdminUrl
 
 
 @deserialize
 @dataclass(frozen=True)
 class AbstractCollectionLinks:
     @classmethod
     def has_field(cls, field_name: str) -> bool:
```

### Comparing `aiochris-0.1.2/chris/models/data.py` & `aiochris-0.2.0/aiochris/models/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Dataclasses describing objects returned from CUBE.
 
-These classes are extended in the modules `chris.models.logged_in`
-and `chris.models.public` with methods to get objects from links.
+These classes are extended in the modules `aiochris.models.logged_in`
+and `aiochris.models.public` with methods to get objects from links.
 """
 
 from dataclasses import dataclass
 import datetime
 from typing import Optional
 
 from serde import deserialize
 
-from chris.link.linked import LinkedModel
-from chris.models.enums import PluginType, Status
-from chris.models.types import *
+from aiochris.link.linked import LinkedModel
+from aiochris.models.enums import PluginType, Status
+from aiochris.models.types import *
 
 
 @deserialize
 @dataclass(frozen=True)
 class UserData:
     """A *CUBE* user."""
```

### Comparing `aiochris-0.1.2/chris/models/enums.py` & `aiochris-0.2.0/aiochris/models/enums.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.1.2/chris/models/logged_in.py` & `aiochris-0.2.0/aiochris/models/logged_in.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-Subclasses of classes from `chris.models.data` which are returned
-from an `chris.client.authed.AuthenticatedClient`.
+Subclasses of classes from `aiochris.models.data` which are returned
+from an `aiochris.client.authed.AuthenticatedClient`.
 These classes may have read-write functionality on the *ChRIS* API.
 """
 from dataclasses import dataclass
 from typing import Optional
 
 from serde import deserialize
 
-from chris.link import http
-from chris.link.linked import LinkedModel
-from chris.models.data import PluginInstanceData, FeedData, UserData, FeedNoteData
-from chris.models.enums import PluginType
-from chris.models.public import PublicPlugin
-from chris.models.types import *
+from aiochris.link import http
+from aiochris.link.linked import LinkedModel
+from aiochris.models.data import PluginInstanceData, FeedData, UserData, FeedNoteData
+from aiochris.models.enums import PluginType
+from aiochris.models.public import PublicPlugin
+from aiochris.models.types import *
 
 
 @deserialize
 @dataclass(frozen=True)
 class User(UserData, LinkedModel):
     pass  # TODO change_email, change_password
```

### Comparing `aiochris-0.1.2/chris/models/public.py` & `aiochris-0.2.0/aiochris/models/public.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Read-only models for CUBE resources.
 """
 from dataclasses import dataclass
 
 import serde
 from serde import deserialize
 
-from chris.link.linked import LinkedModel
-from chris.models.enums import PluginType
-from chris.models.types import *
+from aiochris.link.linked import LinkedModel
+from aiochris.models.enums import PluginType
+from aiochris.models.types import *
 
 
 @deserialize
 @dataclass(frozen=True)
 class PublicPlugin(LinkedModel):
     """
     A ChRIS plugin.
```

### Comparing `aiochris-0.1.2/chris/models/types.py` & `aiochris-0.2.0/aiochris/models/types.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.1.2/chris/util/errors.py` & `aiochris-0.2.0/aiochris/util/errors.py`

 * *Files identical despite different names*

### Comparing `aiochris-0.1.2/chris/util/search.py` & `aiochris-0.2.0/aiochris/util/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 )
 
 import aiohttp
 import yarl
 from serde import deserialize
 from serde.json import from_json
 
-from chris.link.linked import deserialize_linked, Linked
-from chris.util.errors import BaseClientError, raise_for_status, NonsenseResponseError
+from aiochris.link.linked import deserialize_linked, Linked
+from aiochris.util.errors import (
+    BaseClientError,
+    raise_for_status,
+    NonsenseResponseError,
+)
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 @deserialize
@@ -95,17 +99,17 @@
         ```
 
         In the example above, a search for plugins given (`name_exact`, `version`)
         is guaranteed to return either 0 or 1 result.
 
         Raises
         ------
-        chris.util.search.NoneSearchError
+        aiochris.util.search.NoneSearchError
             If this search is empty.
-        chris.util.search.ManySearchError
+        aiochris.util.search.ManySearchError
             If this search has more than one item and `allow_multiple` is `False`
 
         See also
         --------
         `first` : does the same thing but without checks.
 
         Parameters
```

### Comparing `aiochris-0.1.2/pyproject.toml` & `aiochris-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 [tool.poetry]
 name = "aiochris"
-version = "0.1.2"
+version = "0.2.0"
 description = "ChRIS client built on aiohttp"
 authors = ["FNNDSC <dev@babyMRI.org>"]
 readme = "README.md"
 license = "MIT"
-packages = [
-    {include = "chris"}
-]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.3"
 
 # https://github.com/yukinarit/pyserde/issues/292
 pyserde = "^0.10.0"
```

### Comparing `aiochris-0.1.2/setup.py` & `aiochris-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['chris', 'chris.client', 'chris.link', 'chris.models', 'chris.util']
+['aiochris',
+ 'aiochris.client',
+ 'aiochris.link',
+ 'aiochris.models',
+ 'aiochris.util']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiofiles>=23.1.0,<24.0.0',
  'aiohttp>=3.8.3,<4.0.0',
  'async-property>=0.2.1,<0.3.0',
  'pyserde>=0.10.0,<0.11.0',
  'yarl>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'aiochris',
-    'version': '0.1.2',
+    'version': '0.2.0',
     'description': 'ChRIS client built on aiohttp',
-    'long_description': '# aiochris\n\n[![Tests](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml/badge.svg)](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/FNNDSC/aiochris/branch/master/graph/badge.svg?token=48EEYZ3PUU)](https://codecov.io/gh/FNNDSC/aiochris)\n[![PyPI](https://img.shields.io/pypi/v/aiochris)](https://pypi.org/project/aiochris/)\n[![License - MIT](https://img.shields.io/pypi/l/aiochris)](https://github.com/FNNDSC/aiochris/blob/master/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n[_ChRIS_](https://chrisproject.org) Python client library built on\n[aiohttp](https://github.com/aio-libs/aiohttp) (async HTTP client) and\n[pyserde](https://github.com/yukinarit/pyserde)\n([dataclasses](https://docs.python.org/3/library/dataclasses.html) deserializer).\n\n## Installation\n\nRequires Python 3.10 or 3.11.\n\n```shell\npip install aiochris\n# or\npoetry add aiochris\n```\n\n## Quick Example\n\n```python\nimport asyncio\nfrom chris import ChrisClient\n\n\nasync def readme_example():\n    chris = await ChrisClient.from_login(\n        username=\'chris\',\n        password=\'chris1234\',\n        url=\'https://cube.chrisproject.org/api/v1/\'\n    )\n    dircopy = await chris.search_plugins(name_exact=\'pl-brainmgz\', version=\'2.0.3\').get_only()\n    plinst = await dircopy.create_instance(compute_resource_name=\'host\')\n    feed = await plinst.get_feed()\n    await feed.set(name="hello, aiochris!")\n    await chris.close()  # do not forget to clean up!\n\n\nasyncio.run(readme_example())\n```\n\n## Documentation Links\n\n- Client documentation: https://fnndsc.github.io/aiochris\n- Developer documentation: https://github.com/FNNDSC/aiochris/wiki\n',
+    'long_description': '# aiochris\n\n[![Tests](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml/badge.svg)](https://github.com/FNNDSC/aiochris/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/FNNDSC/aiochris/branch/master/graph/badge.svg?token=48EEYZ3PUU)](https://codecov.io/gh/FNNDSC/aiochris)\n[![PyPI](https://img.shields.io/pypi/v/aiochris)](https://pypi.org/project/aiochris/)\n[![License - MIT](https://img.shields.io/pypi/l/aiochris)](https://github.com/FNNDSC/aiochris/blob/master/LICENSE)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n[_ChRIS_](https://chrisproject.org) Python client library built on\n[aiohttp](https://github.com/aio-libs/aiohttp) (async HTTP client) and\n[pyserde](https://github.com/yukinarit/pyserde)\n([dataclasses](https://docs.python.org/3/library/dataclasses.html) deserializer).\n\n## Installation\n\nRequires Python 3.10 or 3.11.\n\n```shell\npip install aiochris\n# or\npoetry add aiochris\n```\n\n## Quick Example\n\n```python\nimport asyncio\nfrom aiochris import ChrisClient\n\n\nasync def readme_example():\n    chris = await ChrisClient.from_login(\n        username=\'chris\',\n        password=\'chris1234\',\n        url=\'https://cube.chrisproject.org/api/v1/\'\n    )\n    dircopy = await chris.search_plugins(name_exact=\'pl-brainmgz\', version=\'2.0.3\').get_only()\n    plinst = await dircopy.create_instance(compute_resource_name=\'host\')\n    feed = await plinst.get_feed()\n    await feed.set(name="hello, aiochris!")\n    await chris.close()  # do not forget to clean up!\n\n\nasyncio.run(readme_example())\n```\n\n## Documentation Links\n\n- Client documentation: https://fnndsc.github.io/aiochris\n- Developer documentation: https://github.com/FNNDSC/aiochris/wiki\n',
     'author': 'FNNDSC',
     'author_email': 'dev@babyMRI.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aiochris-0.1.2/PKG-INFO` & `aiochris-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiochris
-Version: 0.1.2
+Version: 0.2.0
 Summary: ChRIS client built on aiohttp
 License: MIT
 Author: FNNDSC
 Author-email: dev@babyMRI.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 poetry add aiochris
 ```
 
 ## Quick Example
 
 ```python
 import asyncio
-from chris import ChrisClient
+from aiochris import ChrisClient
 
 
 async def readme_example():
     chris = await ChrisClient.from_login(
         username='chris',
         password='chris1234',
         url='https://cube.chrisproject.org/api/v1/'
```

