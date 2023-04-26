# Comparing `tmp/aiomonobank-1.0.0.tar.gz` & `tmp/aiomonobank-1.0.2.tar.gz`

## Comparing `aiomonobank-1.0.0.tar` & `aiomonobank-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
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
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/.gitattributes
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/__init__.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/api.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/base.py
+-rw-r--r--   0        0        0     7761 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/monobank.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/__init__.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/account.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/client_info.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/currency.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/jar.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/statement_item.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/types/webhook_data.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/utils/__init__.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/aiomonobank/utils/exceptions.py
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/examples/webhook.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/LICENSE
+-rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/README.rst
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 aiomonobank-1.0.2/PKG-INFO
```

### Comparing `aiomonobank-1.0.0/aiomonobank/api.py` & `aiomonobank-1.0.2/aiomonobank/api.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/base.py` & `aiomonobank-1.0.2/aiomonobank/base.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/monobank.py` & `aiomonobank-1.0.2/aiomonobank/monobank.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/aiomonobank/types/account.py` & `aiomonobank-1.0.2/aiomonobank/types/account.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from enum import StrEnum
 from typing import Optional
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, validator
 
 
 class AccountTypeEnum(StrEnum):
     BLACK = "black"
     WHITE = "white"
     PLATINUM = "platinum"
     IRON = "iron"
@@ -20,27 +20,36 @@
     MILES = "Miles"
 
 
 class Account(BaseModel):
     """Рахунок клієнта"""
     id: str
     """Ідентифікатор рахунку"""
-    send_id: str = Field(..., alias='sendId')
+    send_id: str
     """Ідентифікатор для сервісу https://send.monobank.ua/{sendId}"""
     balance: float
     """Баланс рахунку в мінімальних одиницях валюти (копійках, центах)"""
-    credit_limit: float = Field(..., alias='creditLimit')
+    credit_limit: float
     """Кредитний ліміт"""
     type: AccountTypeEnum
     """Тип рахунку"""
-    currency_code: int = Field(..., alias='currencyCode')
+    currency_code: int
     """Код валюти рахунку відповідно ISO 4217"""
-    cashback_type: Optional[CashbackType] = Field(None, alias='cashbackType')
+    cashback_type: Optional[CashbackType]
     """Тип кешбеку який нараховується на рахунок"""
-    masked_pan: list[str] = Field(..., alias='maskedPan')
+    masked_pan: list[str]
     """Перелік замаскованих номерів карт (більше одного може бути у преміальних карт)"""
     iban: str
     """IBAN рахунку"""
 
     @validator('balance', 'credit_limit', pre=True, allow_reuse=True)
     def _convert_from_integer_to_currency_sum(cls, value: int):
         return value / 100
+
+    class Config:
+        fields = {
+            'send_id': 'sendId',
+            'credit_limit': 'creditLimit',
+            'currency_code': 'currencyCode',
+            'cashback_type': 'cashbackType',
+            'masked_pan': 'maskedPan',
+        }
```

### Comparing `aiomonobank-1.0.0/aiomonobank/types/client_info.py` & `aiomonobank-1.0.2/aiomonobank/types/client_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-from pydantic import BaseModel, Field, constr
+from pydantic import BaseModel
 
 from .account import Account
 from .jar import Jar
 
 
 class Client(BaseModel):
     """Інформація про клієнта"""
-    id: str = Field(..., alias='clientId')
+    id: str
     """Ідентифікатор клієнта (збігається з id для send.monobank.ua)"""
     name: str
     """Ім'я клієнта"""
-    webhook_url: str = Field(..., alias='webHookUrl')
+    webhook_url: str
     """URL для надсилання подій по зміні балансу рахунку"""
     permissions: str
     """Перелік прав, які надає сервіс (1 літера на 1 permission)."""
     accounts: list[Account]
     """Перелік доступних рахунків"""
     jars: list[Jar] = []
     """Перелік банок"""
+
+    class Config:
+        fields = {
+            'client_id': 'clientId',
+            'web_hook_url': 'webHookUrl',
+        }
```

### Comparing `aiomonobank-1.0.0/aiomonobank/types/jar.py` & `aiomonobank-1.0.2/aiomonobank/types/jar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 from typing import Optional
 
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, validator
 
 
 class Jar(BaseModel):
     """Банка клієнта"""
     id: str
     """Ідентифікатор банки"""
-    send_id: str = Field(..., alias='sendId')
+    send_id: str
     """Ідентифікатор для сервісу https://send.monobank.ua/{sendId}"""
     title: str
     """Назва банки"""
     description: str
     """Опис банки"""
-    currency_code: int = Field(..., alias='currencyCode')
+    currency_code: int
     """Код валюти банки відповідно ISO 4217"""
     balance: float
     """Баланс банки"""
     goal: Optional[float]
     """Цільова сума для накопичення в банці"""
 
     @validator('balance', 'goal', pre=True, allow_reuse=True)
     def _convert_from_integer_to_currency_sum(cls, value: int) -> Optional[float]:
         if value is None:
             return value
 
         return value / 100
+
+    class Config:
+        fields = {
+            'send_id': 'sendId',
+            'currency_code': 'currencyCode',
+        }
```

### Comparing `aiomonobank-1.0.0/aiomonobank/utils/exceptions.py` & `aiomonobank-1.0.2/aiomonobank/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/examples/webhook.py` & `aiomonobank-1.0.2/examples/webhook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import json
 import logging
 from http import HTTPStatus
 
 from aiohttp import web
 from aiomonobank import MonoPersonal, types
 
 WEBHOOK_HOST = "https://example.com"
 WEBAPP_HOST = "localhost"
 WEBAPP_PORT = 8822
-MONOBANK_API_TOKEN = 'your_token'
+MONOBANK_API_TOKEN = 'your_token'  # TODO don't forget to replace with your real token
 
 logger = logging.getLogger(__name__)
 
 mono_client = MonoPersonal(MONOBANK_API_TOKEN)
 
 router = web.RouteTableDef()
 
@@ -49,15 +48,15 @@
         **await request.json()
     )
 
     if webhook_data.type == "StatementItem":
         logger.debug(f"The account ID of the new transaction: {webhook_data.data.account_id}. "
                      f"Sum: {webhook_data.data.statement.amount} UAH")
 
-        print(json.dumps(webhook_data, ensure_ascii=False, indent=4))
+        print(webhook_data)
 
     return web.json_response(status=HTTPStatus.OK)
 
 
 async def on_startup(app: web.Application):
     result = await mono_client.set_webhook(f"{WEBHOOK_HOST}/{MONOBANK_API_TOKEN}")
     logger.debug(f'Wet webhook result: {result}')
```

### Comparing `aiomonobank-1.0.0/.gitignore` & `aiomonobank-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/LICENSE` & `aiomonobank-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomonobank-1.0.0/README.md` & `aiomonobank-1.0.2/README.rst`

 * *Files 27% similar despite different names*

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
 
 
-## Examples
+`get_currency <https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get>`_ request
+-----------------------------------------------------------------------------------------------------
 
-**We currently have 2 different classes for using the Monobank API.:**
-- `MonoPublic` is simple base class for others, can only get currencies
-- `MonoPersonal` - this class for talk to personal Monobank API
+.. code-block:: python
 
+    import json
+    import asyncio
 
-### [get_currency](https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get) request
+    from aiomonobank import MonoPublic, types
 
-```python
-import json
-import asyncio
 
-from aiomonobank import MonoPublic
+    async def main():
+        async with MonoPublic() as mono_client:
+            currencies: list[types.Currency] = await mono_client.get_currency()
 
+        for currency in currencies:
+            print(currency)
 
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
 
+            print(f"Client name: {client_info.name}")
+            print(client_info)
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
+            for transaction in transactions:
+                print(transaction)
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

### Comparing `aiomonobank-1.0.0/pyproject.toml` & `aiomonobank-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

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
@@ -40,24 +41,16 @@
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
 Repository = "https://github.com/TT1410/aiomonobank"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-aiohttp = "^3.8.4"
-pydantic = "^1.10.7"
-certifi = "^2022.12.7"
-pytz = "^2023.3"
-aiocache = "^0.12.1"
```

### Comparing `aiomonobank-1.0.0/PKG-INFO` & `aiomonobank-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomonobank
-Version: 1.0.0
+Version: 1.0.2
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
 
 
-## Examples
+`get_currency <https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get>`_ request
+-----------------------------------------------------------------------------------------------------
 
-**We currently have 2 different classes for using the Monobank API.:**
-- `MonoPublic` is simple base class for others, can only get currencies
-- `MonoPersonal` - this class for talk to personal Monobank API
+.. code-block:: python
 
+    import json
+    import asyncio
 
-### [get_currency](https://api.monobank.ua/docs/#tag/Publichni-dani/paths/~1bank~1currency/get) request
+    from aiomonobank import MonoPublic, types
 
-```python
-import json
-import asyncio
 
-from aiomonobank import MonoPublic
+    async def main():
+        async with MonoPublic() as mono_client:
+            currencies: list[types.Currency] = await mono_client.get_currency()
 
+        for currency in currencies:
+            print(currency)
 
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
 
+            print(f"Client name: {client_info.name}")
+            print(client_info)
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
+            for transaction in transactions:
+                print(transaction)
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

