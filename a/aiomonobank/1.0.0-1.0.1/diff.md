# Comparing `tmp/aiomonobank-1.0.0.tar.gz` & `tmp/aiomonobank-1.0.1.tar.gz`

## Comparing `aiomonobank-1.0.0.tar` & `aiomonobank-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/.gitattributes
--rw-r--r--   0        0        0    72366 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/poetry.lock
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/__init__.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/api.py
--rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/base.py
--rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/monobank.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/account.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/client_info.py
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/currency.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/jar.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/statement_item.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/types/webhook_data.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/utils/__init__.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/aiomonobank/utils/exceptions.py
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/examples/webhook.py
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/LICENSE
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/README.md
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4391 2020-02-02 00:00:00.000000 aiomonobank-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/.gitattributes
+-rw-r--r--   0        0        0    72366 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/poetry.lock
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/__init__.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/base.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/monobank.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/account.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/client_info.py
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/currency.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/jar.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/statement_item.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/types/webhook_data.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/utils/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/aiomonobank/utils/exceptions.py
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/examples/webhook.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/README.rst
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 aiomonobank-1.0.1/PKG-INFO
```

### Comparing `aiomonobank-1.0.0/poetry.lock` & `aiomonobank-1.0.1/poetry.lock`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/api.py` & `aiomonobank-1.0.1/aiomonobank/api.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/base.py` & `aiomonobank-1.0.1/aiomonobank/base.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/monobank.py` & `aiomonobank-1.0.1/aiomonobank/monobank.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/account.py` & `aiomonobank-1.0.1/aiomonobank/types/account.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/client_info.py` & `aiomonobank-1.0.1/aiomonobank/types/client_info.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/currency.py` & `aiomonobank-1.0.1/aiomonobank/types/currency.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/jar.py` & `aiomonobank-1.0.1/aiomonobank/types/jar.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/statement_item.py` & `aiomonobank-1.0.1/aiomonobank/types/statement_item.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/utils/exceptions.py` & `aiomonobank-1.0.1/aiomonobank/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/examples/webhook.py` & `aiomonobank-1.0.1/examples/webhook.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/.gitignore` & `aiomonobank-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/LICENSE` & `aiomonobank-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/README.md` & `aiomonobank-1.0.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-# AIOMonobank
-Asynchronous Python library for [monobank](https://api.monobank.ua/docs) API
-
-
-## Setup
-- You get token for your client from [MonobankAPI](https://api.monobank.ua/).
-- Install the **latest version** of the **aiomonobank**: `pip install aiomonobank`
+===========
+AIOMonobank
+===========
 
+Asynchronous Python library for `monobank <https://api.monobank.ua/docs>`_ API
 
 
 .. image:: https://img.shields.io/pypi/l/aiomonobank.svg?style=flat-square
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://img.shields.io/pypi/status/aiomonobank.svg?style=flat-square
@@ -24,97 +21,110 @@
     :target: https://pypi.python.org/pypi/aiomonobank
     :alt: Downloads
 
 .. image:: https://img.shields.io/pypi/pyversions/aiomonobank.svg?style=flat-square
     :target: https://pypi.python.org/pypi/aiomonobank
     :alt: Supported python versions
 
+Setup
+=====
+
+- You get token for your client from `MonobankAPI <https://api.monobank.ua/>`_.
+- Install the **latest version** of the **aiomonobank**: ``pip install aiomonobank``
+
+
+Examples
+========
+
+We currently have 2 different classes for using the Monobank API:
+-----------------------------------------------------------------
+
+- ``MonoPublic`` is simple base class for others, can only get currencies
+- ``MonoPersonal`` - this class for talk to personal Monobank API
+
 
+`get_currency <https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get>`_ request
+-----------------------------------------------------------------------------------------------------
 
-## Examples
+.. code-block:: python
 
-**We currently have 2 different classes for using the Monobank API.:**
-- `MonoPublic` is simple base class for others, can only get currencies
-- `MonoPersonal` - this class for talk to personal Monobank API
+    import json
+    import asyncio
 
+    from aiomonobank import MonoPublic
 
-### [get_currency](https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get) request
 
-```python
-import json
-import asyncio
+    async def main():
+        async with MonoPublic() as mono_client:
+            currency = await mono_client.get_currency()
 
-from aiomonobank import MonoPublic
+        print(json.dumps(currency, ensure_ascii=False, indent=4))
 
 
-async def main():
-    async with MonoPublic() as mono_client:
-        currency = await mono_client.get_currency()
+    if __name__ == '__main__':
+        asyncio.run(main())
 
-    print(json.dumps(currency, ensure_ascii=False, indent=4))
 
+`get_client_info <https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get>`_ request
+----------------------------------------------------------------------------------------------------------------------------
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
+.. code-block:: python
 
+    import json
+    import asyncio
 
-### [get_client_info](https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get) request
+    from aiomonobank import MonoPersonal
 
-```python
-import json
-import asyncio
+    MONOBANK_API_TOKEN = 'your_token'
 
-from aiomonobank import MonoPersonal
 
-MONOBANK_API_TOKEN = 'your_token'
+    async def main():
+        mono_client = MonoPersonal(MONOBANK_API_TOKEN)
+        try:
+            client_info = await mono_client.get_client_info()
 
+            print(json.dumps(client_info, ensure_ascii=False, indent=4))
+        finally:
+            await mono_client.close()
 
-async def main():
-    mono_client = MonoPersonal(MONOBANK_API_TOKEN)
-    try:
-        client_info = await mono_client.get_client_info()
 
-        print(json.dumps(client_info, ensure_ascii=False, indent=4))
-    finally:
-        await mono_client.close()
+    if __name__ == '__main__':
+        asyncio.run(main())
 
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
+`get_statement <https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1statement~1{account}~1{from}~1{to}/get>`_ request
+-------------------------------------------------------------------------------------------------------------------------------------------------
 
+.. code-block:: python
 
-### [get_statement](https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1statement~1{account}~1{from}~1{to}/get) request
+    import json
+    import asyncio
+    from datetime import datetime, timedelta
 
-```python
-import json
-import asyncio
-from datetime import datetime, timedelta
+    from aiomonobank import MonoPersonal
 
-from aiomonobank import MonoPersonal
+    MONOBANK_API_TOKEN = 'your_token'
 
-MONOBANK_API_TOKEN = 'your_token'
 
+    async def main():
+        mono_client = MonoPersonal(MONOBANK_API_TOKEN)
+        try:
+            transactions = await mono_client.get_statement(
+                account_id='0',
+                from_datetime=datetime.utcnow() - timedelta(days=3),
+                to_datetime=datetime.utcnow() - timedelta(days=2)
+            )
 
-async def main():
-    mono_client = MonoPersonal(MONOBANK_API_TOKEN)
-    try:
-        transactions = await mono_client.get_statement(
-            account_id='0', 
-            from_datetime=datetime.utcnow() - timedelta(days=3),
-            to_datetime=datetime.utcnow() - timedelta(days=2)
-        )
+            print(json.dumps(transactions, ensure_ascii=False, indent=4))
+        finally:
+            await mono_client.close()
 
-        print(json.dumps(transactions, ensure_ascii=False, indent=4))
-    finally:
-        await mono_client.close()
 
+    if __name__ == '__main__':
+        asyncio.run(main())
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
 
+Resources:
+==========
 
-## Resources:
-- PyPI: [aiomonobank](https://pypi.org/project/aiomonobank)
-- Documentation: (soon)
+- PyPI: `aiomonobank <https://pypi.org/project/aiomonobank>`_
+- Documentation: (soon)
```

### Comparing `aiomonobank-1.0.0/pyproject.toml` & `aiomonobank-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aiomonobank"
-version = "1.0.0"
 description = "Asynchronous Python library for monobank API"
-readme = "README.md"
+long_description='readme_contents'
+long_description_content_type='text/x-rst'
+readme = "README.rst"
 requires-python = ">=3.10"
 authors = [
     { name = "TT1410", email = "taras@plaksii.cf" }
 ]
 maintainers = [
     { name = "TT1410", email = "taras@plaksii.cf" }
 ]
@@ -40,15 +41,15 @@
     "aiohttp~=3.8.4",
     "pydantic~=1.10.7",
     "certifi>=2022.12.7",
     "pytz>=2023.3",
     "aiocache>=0.12.1",
 
 ]
-#dynamic = ["version"]
+dynamic = ["version"]
 
 [tool.hatch.version]
 path = "aiomonobank/__init__.py"
 
 [project.urls]
 Homepage = "https://github.com/TT1410/aiomonobank"
 Documentation = "https://github.com/TT1410/aiomonobank"
```

### Comparing `aiomonobank-1.0.0/PKG-INFO` & `aiomonobank-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonobank
-Version: 1.0.0
+Version: 1.0.1
 Summary: Asynchronous Python library for monobank API
 Project-URL: Homepage, https://github.com/TT1410/aiomonobank
 Project-URL: Documentation, https://github.com/TT1410/aiomonobank
 Project-URL: Repository, https://github.com/TT1410/aiomonobank
 Author-email: TT1410 <taras@plaksii.cf>
 Maintainer-email: TT1410 <taras@plaksii.cf>
 License-File: LICENSE
@@ -23,24 +23,21 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: aiocache>=0.12.1
 Requires-Dist: aiohttp~=3.8.4
 Requires-Dist: certifi>=2022.12.7
 Requires-Dist: pydantic~=1.10.7
 Requires-Dist: pytz>=2023.3
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-# AIOMonobank
-Asynchronous Python library for [monobank](https://api.monobank.ua/docs) API
-
-
-## Setup
-- You get token for your client from [MonobankAPI](https://api.monobank.ua/).
-- Install the **latest version** of the **aiomonobank**: `pip install aiomonobank`
+===========
+AIOMonobank
+===========
 
+Asynchronous Python library for `monobank <https://api.monobank.ua/docs>`_ API
 
 
 .. image:: https://img.shields.io/pypi/l/aiomonobank.svg?style=flat-square
     :target: https://opensource.org/licenses/MIT
     :alt: MIT License
 
 .. image:: https://img.shields.io/pypi/status/aiomonobank.svg?style=flat-square
@@ -55,97 +52,110 @@
     :target: https://pypi.python.org/pypi/aiomonobank
     :alt: Downloads
 
 .. image:: https://img.shields.io/pypi/pyversions/aiomonobank.svg?style=flat-square
     :target: https://pypi.python.org/pypi/aiomonobank
     :alt: Supported python versions
 
+Setup
+=====
+
+- You get token for your client from `MonobankAPI <https://api.monobank.ua/>`_.
+- Install the **latest version** of the **aiomonobank**: ``pip install aiomonobank``
+
+
+Examples
+========
+
+We currently have 2 different classes for using the Monobank API:
+-----------------------------------------------------------------
+
+- ``MonoPublic`` is simple base class for others, can only get currencies
+- ``MonoPersonal`` - this class for talk to personal Monobank API
+
 
+`get_currency <https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get>`_ request
+-----------------------------------------------------------------------------------------------------
 
-## Examples
+.. code-block:: python
 
-**We currently have 2 different classes for using the Monobank API.:**
-- `MonoPublic` is simple base class for others, can only get currencies
-- `MonoPersonal` - this class for talk to personal Monobank API
+    import json
+    import asyncio
 
+    from aiomonobank import MonoPublic
 
-### [get_currency](https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get) request
 
-```python
-import json
-import asyncio
+    async def main():
+        async with MonoPublic() as mono_client:
+            currency = await mono_client.get_currency()
 
-from aiomonobank import MonoPublic
+        print(json.dumps(currency, ensure_ascii=False, indent=4))
 
 
-async def main():
-    async with MonoPublic() as mono_client:
-        currency = await mono_client.get_currency()
+    if __name__ == '__main__':
+        asyncio.run(main())
 
-    print(json.dumps(currency, ensure_ascii=False, indent=4))
 
+`get_client_info <https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get>`_ request
+----------------------------------------------------------------------------------------------------------------------------
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
+.. code-block:: python
 
+    import json
+    import asyncio
 
-### [get_client_info](https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1client-info/get) request
+    from aiomonobank import MonoPersonal
 
-```python
-import json
-import asyncio
+    MONOBANK_API_TOKEN = 'your_token'
 
-from aiomonobank import MonoPersonal
 
-MONOBANK_API_TOKEN = 'your_token'
+    async def main():
+        mono_client = MonoPersonal(MONOBANK_API_TOKEN)
+        try:
+            client_info = await mono_client.get_client_info()
 
+            print(json.dumps(client_info, ensure_ascii=False, indent=4))
+        finally:
+            await mono_client.close()
 
-async def main():
-    mono_client = MonoPersonal(MONOBANK_API_TOKEN)
-    try:
-        client_info = await mono_client.get_client_info()
 
-        print(json.dumps(client_info, ensure_ascii=False, indent=4))
-    finally:
-        await mono_client.close()
+    if __name__ == '__main__':
+        asyncio.run(main())
 
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
+`get_statement <https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1statement~1{account}~1{from}~1{to}/get>`_ request
+-------------------------------------------------------------------------------------------------------------------------------------------------
 
+.. code-block:: python
 
-### [get_statement](https://api.monobank.ua/docs/#tag/Kliyentski-personalni-dani/paths/~1personal~1statement~1{account}~1{from}~1{to}/get) request
+    import json
+    import asyncio
+    from datetime import datetime, timedelta
 
-```python
-import json
-import asyncio
-from datetime import datetime, timedelta
+    from aiomonobank import MonoPersonal
 
-from aiomonobank import MonoPersonal
+    MONOBANK_API_TOKEN = 'your_token'
 
-MONOBANK_API_TOKEN = 'your_token'
 
+    async def main():
+        mono_client = MonoPersonal(MONOBANK_API_TOKEN)
+        try:
+            transactions = await mono_client.get_statement(
+                account_id='0',
+                from_datetime=datetime.utcnow() - timedelta(days=3),
+                to_datetime=datetime.utcnow() - timedelta(days=2)
+            )
 
-async def main():
-    mono_client = MonoPersonal(MONOBANK_API_TOKEN)
-    try:
-        transactions = await mono_client.get_statement(
-            account_id='0', 
-            from_datetime=datetime.utcnow() - timedelta(days=3),
-            to_datetime=datetime.utcnow() - timedelta(days=2)
-        )
+            print(json.dumps(transactions, ensure_ascii=False, indent=4))
+        finally:
+            await mono_client.close()
 
-        print(json.dumps(transactions, ensure_ascii=False, indent=4))
-    finally:
-        await mono_client.close()
 
+    if __name__ == '__main__':
+        asyncio.run(main())
 
-if __name__ == '__main__':
-    asyncio.run(main())
-```
 
+Resources:
+==========
 
-## Resources:
-- PyPI: [aiomonobank](https://pypi.org/project/aiomonobank)
-- Documentation: (soon)
+- PyPI: `aiomonobank <https://pypi.org/project/aiomonobank>`_
+- Documentation: (soon)
```

