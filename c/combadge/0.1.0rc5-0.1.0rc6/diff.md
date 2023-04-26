# Comparing `tmp/combadge-0.1.0rc5.tar.gz` & `tmp/combadge-0.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "combadge-0.1.0rc5.tar", max compression
+gzip compressed data, was "combadge-0.1.0rc6.tar", max compression
```

## Comparing `combadge-0.1.0rc5.tar` & `combadge-0.1.0rc6.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    11350 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/LICENSE
--rw-r--r--   0        0        0     2682 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/README.md
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/__init__.py
--rw-r--r--   0        0        0     1259 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/backend.py
--rw-r--r--   0        0        0     3377 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/binder.py
--rw-r--r--   0        0        0     3016 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/markers/__init__.py
--rw-r--r--   0        0        0     2568 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/markers/method.py
--rw-r--r--   0        0        0      902 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/markers/parameter.py
--rw-r--r--   0        0        0     2026 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/request.py
--rw-r--r--   0        0        0     6814 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/response.py
--rw-r--r--   0        0        0     1830 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/service.py
--rw-r--r--   0        0        0     2372 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/signature.py
--rw-r--r--   0        0        0      343 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/typevars.py
--rw-r--r--   0        0        0      203 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/core/warnings.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/py.typed
--rw-r--r--   0        0        0       50 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/__init__.py
--rw-r--r--   0        0        0       40 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/__init__.py
--rw-r--r--   0        0        0     1470 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/abc.py
--rw-r--r--   0        0        0      807 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/aliases.py
--rw-r--r--   0        0        0      264 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/headers.py
--rw-r--r--   0        0        0     7338 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/markers.py
--rw-r--r--   0        0        0      398 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/http/request.py
--rw-r--r--   0        0        0      124 2023-04-17 12:10:49.210241 combadge-0.1.0rc5/combadge/support/httpx/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/httpx/backends/__init__.py
--rw-r--r--   0        0        0     3374 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/httpx/backends/async_.py
--rw-r--r--   0        0        0     1542 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/httpx/backends/base.py
--rw-r--r--   0        0        0     3232 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/httpx/backends/sync.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/shared/__init__.py
--rw-r--r--   0        0        0      348 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/shared/async_.py
--rw-r--r--   0        0        0      308 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/shared/contextlib.py
--rw-r--r--   0        0        0      338 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/shared/sync.py
--rw-r--r--   0        0        0       39 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/soap/__init__.py
--rw-r--r--   0        0        0      256 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/soap/abc.py
--rw-r--r--   0        0        0     2198 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/soap/markers.py
--rw-r--r--   0        0        0      212 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/soap/request.py
--rw-r--r--   0        0        0      741 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/soap/response.py
--rw-r--r--   0        0        0      131 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/zeep/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/zeep/backends/__init__.py
--rw-r--r--   0        0        0     3475 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/zeep/backends/async_.py
--rw-r--r--   0        0        0     3059 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/zeep/backends/base.py
--rw-r--r--   0        0        0     3334 2023-04-17 12:10:49.214241 combadge-0.1.0rc5/combadge/support/zeep/backends/sync.py
--rw-r--r--   0        0        0     3397 2023-04-17 12:11:03.471392 combadge-0.1.0rc5/pyproject.toml
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 combadge-0.1.0rc5/PKG-INFO
+-rw-r--r--   0        0        0    11350 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/LICENSE
+-rw-r--r--   0        0        0     2682 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/__init__.py
+-rw-r--r--   0        0        0     1259 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/backend.py
+-rw-r--r--   0        0        0     3377 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/binder.py
+-rw-r--r--   0        0        0     3016 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/__init__.py
+-rw-r--r--   0        0        0     2568 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/method.py
+-rw-r--r--   0        0        0      902 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/markers/parameter.py
+-rw-r--r--   0        0        0     1997 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/request.py
+-rw-r--r--   0        0        0     6303 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/response.py
+-rw-r--r--   0        0        0     1830 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/service.py
+-rw-r--r--   0        0        0     2372 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/signature.py
+-rw-r--r--   0        0        0      343 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/typevars.py
+-rw-r--r--   0        0        0      203 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/core/warnings.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/py.typed
+-rw-r--r--   0        0        0       50 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/__init__.py
+-rw-r--r--   0        0        0     1470 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/abc.py
+-rw-r--r--   0        0        0      807 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/aliases.py
+-rw-r--r--   0        0        0      264 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/headers.py
+-rw-r--r--   0        0        0     7338 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/markers.py
+-rw-r--r--   0        0        0      398 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/http/request.py
+-rw-r--r--   0        0        0      124 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/__init__.py
+-rw-r--r--   0        0        0     3374 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/async_.py
+-rw-r--r--   0        0        0     1542 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/base.py
+-rw-r--r--   0        0        0     3232 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/httpx/backends/sync.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/__init__.py
+-rw-r--r--   0        0        0      348 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/async_.py
+-rw-r--r--   0        0        0      308 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/contextlib.py
+-rw-r--r--   0        0        0      338 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/shared/sync.py
+-rw-r--r--   0        0        0       39 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/__init__.py
+-rw-r--r--   0        0        0      256 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/abc.py
+-rw-r--r--   0        0        0     2198 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/markers.py
+-rw-r--r--   0        0        0      212 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/request.py
+-rw-r--r--   0        0        0      870 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/soap/response.py
+-rw-r--r--   0        0        0      131 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/__init__.py
+-rw-r--r--   0        0        0     3475 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/async_.py
+-rw-r--r--   0        0        0     3059 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/base.py
+-rw-r--r--   0        0        0     3334 2023-04-26 16:23:38.362406 combadge-0.1.0rc6/combadge/support/zeep/backends/sync.py
+-rw-r--r--   0        0        0     3397 2023-04-26 16:23:59.259021 combadge-0.1.0rc6/pyproject.toml
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 combadge-0.1.0rc6/PKG-INFO
```

### Comparing `combadge-0.1.0rc5/LICENSE` & `combadge-0.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/README.md` & `combadge-0.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/backend.py` & `combadge-0.1.0rc6/combadge/core/backend.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/binder.py` & `combadge-0.1.0rc6/combadge/core/binder.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/interfaces.py` & `combadge-0.1.0rc6/combadge/core/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from types import TracebackType
-from typing import Any, Optional, Type
+from typing import Any, Optional, Protocol, Type
 
 from pydantic import BaseModel
-from typing_extensions import Protocol, Self
+from typing_extensions import Self
 
 from combadge.core.binder import BaseBoundService, bind
 from combadge.core.signature import Signature
 from combadge.core.typevars import BackendT
 
 
 class SupportsService(Protocol):
```

### Comparing `combadge-0.1.0rc5/combadge/core/markers/method.py` & `combadge-0.1.0rc6/combadge/core/markers/method.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/markers/parameter.py` & `combadge-0.1.0rc6/combadge/core/markers/parameter.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/request.py` & `combadge-0.1.0rc6/combadge/core/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from typing import Any, Iterable, Mapping, Type, Union
+from typing import Any, Iterable, Mapping, NoReturn, Type, Union
 
 from pydantic import validate_model
-from typing_extensions import NoReturn
 
 from combadge.core.binder import BaseBoundService
 from combadge.core.signature import Signature
 from combadge.core.typevars import RequestT
 
 
 def build_request(
```

### Comparing `combadge-0.1.0rc5/combadge/core/response.py` & `combadge-0.1.0rc6/combadge/core/response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Generic response models."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Any, Generic, Iterable, Type, Union
+from typing import Any, Generic, Iterable, NoReturn, Optional, Type, Union
 
 from pydantic import BaseModel
-from typing_extensions import NoReturn, Self, TypeAlias
+from typing_extensions import Self, TypeAlias
 
 from combadge.core.typevars import ResponseT
 
 
 class BaseResponse(ABC, BaseModel):
     """
     Base model representing any possible service response.
@@ -19,15 +19,15 @@
 
     Notes:
         - `#!python BaseResponse` is the lower-level API,
           users should consider inheriting from `#!python SuccessfulResponse` and `#!python ErrorResponse`.
     """
 
     @abstractmethod
-    def raise_for_result(self) -> Union[None, NoReturn]:
+    def raise_for_result(self, exception: Optional[BaseException] = None) -> Union[None, NoReturn]:
         """
         Raise an exception if the service call has failed.
 
         Raises:
             ErrorResponse.Error: an error derived from `ErrorResponse`
 
         Returns:
@@ -41,28 +41,14 @@
 
             The advice is to use [`unwrap()`][combadge.core.response.BaseResponse.unwrap]
             for the time being.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def expect(self, exception_type: Type[BaseException], *args: Any) -> Union[None, NoReturn]:
-        """
-        Raise the specified exception if the service call has failed.
-
-        This method is similar to the [`unwrap()`][combadge.core.response.BaseResponse.unwrap],
-        but allows raising a custom exception instead.
-
-        Args:
-            exception_type: exception class to be raised
-            args: exception positional arguments
-        """
-        raise NotImplementedError
-
-    @abstractmethod
     def unwrap(self) -> Union[Self, NoReturn]:
         """
         Return itself if the call was successful, raises an exception otherwise.
 
         This method allows «unpacking» a response with proper type hinting.
         The trick here is that all error responses' `unwrap()` are annotated with `NoReturn`,
         which suggests a type linter, that `unwrap()` may never return an error.
@@ -92,24 +78,21 @@
 class SuccessfulResponse(BaseResponse):
     """
     Parent model for successful responses.
 
     Users should not use it directly, but inherit their response models from it.
     """
 
-    def raise_for_result(self) -> None:
+    def raise_for_result(self, exception: Optional[BaseException] = None) -> None:
         """
         Do nothing.
 
         This call is a no-op since the response is successful.
         """
 
-    def expect(self, _exception_type: Type[BaseException], *_args: Any) -> None:
-        """Do nothing."""
-
     def unwrap(self) -> Self:
         """Return itself since there's no error."""
         return self
 
 
 class ErrorResponse(BaseResponse, ABC):
     """
@@ -181,21 +164,24 @@
             """
 
         DerivedException.__name__ = f"{cls.__name__}.Error"
         DerivedException.__qualname__ = f"{cls.__qualname__}.Error"
         DerivedException.__doc__ = cls.__doc__ or DerivedException.__doc__
         cls.Error = DerivedException  # type: ignore
 
-    def raise_for_result(self) -> NoReturn:
-        """Raise the derived exception."""
-        raise self.Error(self)
+    def raise_for_result(self, exception: Optional[BaseException] = None) -> NoReturn:
+        """
+        Raise the derived exception.
 
-    def expect(self, exception_type: Type[BaseException], *args: Any) -> NoReturn:
-        """Raise the specified exception with the derived exception context."""
-        raise exception_type(*args) from self.Error(self)
+        Args:
+            exception: if set, raise the specified exception instead of the derived one.
+        """
+        if not exception:
+            raise self.Error(self)
+        raise exception from self.Error(self)
 
     def unwrap(self) -> NoReturn:
         """Raise the derived exception."""
         raise self.Error(self)
 
 
 BaseError: TypeAlias = ErrorResponse.Error
```

### Comparing `combadge-0.1.0rc5/combadge/core/service.py` & `combadge-0.1.0rc6/combadge/core/service.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/core/signature.py` & `combadge-0.1.0rc6/combadge/core/signature.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/http/abc.py` & `combadge-0.1.0rc6/combadge/support/http/abc.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/http/aliases.py` & `combadge-0.1.0rc6/combadge/support/http/aliases.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/http/markers.py` & `combadge-0.1.0rc6/combadge/support/http/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/httpx/backends/async_.py` & `combadge-0.1.0rc6/combadge/support/httpx/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/httpx/backends/base.py` & `combadge-0.1.0rc6/combadge/support/httpx/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/httpx/backends/sync.py` & `combadge-0.1.0rc6/combadge/support/httpx/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/soap/markers.py` & `combadge-0.1.0rc6/combadge/support/soap/markers.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/soap/response.py` & `combadge-0.1.0rc6/combadge/support/soap/response.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Response extensions for SOAP."""
 
-from typing import NoReturn, TypeVar
+from typing import NoReturn, Optional, TypeVar
 
 from combadge.core.response import ErrorResponse
 
 
 class BaseSoapFault(ErrorResponse):
     """
     SOAP Fault model.
@@ -17,14 +17,16 @@
     See Also:
         - https://www.w3.org/TR/2000/NOTE-SOAP-20000508/#_Toc478383507
     """
 
     code: str
     message: str
 
-    def raise_for_result(self) -> NoReturn:
+    def raise_for_result(self, exception: Optional[BaseException] = None) -> NoReturn:
         """Raise the derived error for this fault."""
-        raise self.Error(self)
+        if not exception:
+            raise self.Error(self)
+        raise exception from self.Error(self)
 
 
 SoapFaultT = TypeVar("SoapFaultT", bound=BaseSoapFault)
 """Specific SOAP Fault model type."""
```

### Comparing `combadge-0.1.0rc5/combadge/support/zeep/backends/async_.py` & `combadge-0.1.0rc6/combadge/support/zeep/backends/async_.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/zeep/backends/base.py` & `combadge-0.1.0rc6/combadge/support/zeep/backends/base.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/combadge/support/zeep/backends/sync.py` & `combadge-0.1.0rc6/combadge/support/zeep/backends/sync.py`

 * *Files identical despite different names*

### Comparing `combadge-0.1.0rc5/pyproject.toml` & `combadge-0.1.0rc6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ]
 description = "Generic API client based on Pydantic"
 keywords = ["api", "api-client", "pydantic"]
 license = "Apache-2.0"
 name = "combadge"
 readme = "README.md"
 repository = "https://github.com/kpn/combadge"
-version = "0.1.0rc5"
+version = "0.1.0rc6"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -132,15 +132,15 @@
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 mypy = "^1.0.0"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 types-requests = "^2.28.11.8"
-ruff = "^0.0.236"
+ruff = "^0.0.263"
 pytest-recording = "^0.12.1"
 pytest-asyncio = "^0.20.3"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `combadge-0.1.0rc5/PKG-INFO` & `combadge-0.1.0rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: combadge
-Version: 0.1.0rc5
+Version: 0.1.0rc6
 Summary: Generic API client based on Pydantic
 Home-page: https://github.com/kpn/combadge
 License: Apache-2.0
 Keywords: api,api-client,pydantic
 Author: Pavel Perestoronin
 Author-email: pavel.perestoronin@kpn.com
 Requires-Python: >=3.8.1,<4.0.0
```

