# Comparing `tmp/potyk-lib-0.6.0.tar.gz` & `tmp/potyk-lib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potyk-lib-0.6.0.tar", last modified: Tue Jan 31 14:23:43 2023, max compression
+gzip compressed data, was "potyk-lib-0.6.1.tar", last modified: Wed Apr 26 13:34:36 2023, max compression
```

## Comparing `potyk-lib-0.6.0.tar` & `potyk-lib-0.6.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0        0 2022-11-23 18:07:54.505011 potyk-lib-0.6.0/potyk_lib/__init__.py
--rw-r--r--   0        0        0       42 2022-11-24 07:16:19.162279 potyk-lib-0.6.0/potyk_lib/dt/__init__.py
--rw-r--r--   0        0        0      193 2022-11-24 07:18:37.710325 potyk-lib-0.6.0/potyk_lib/dt/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1542 2023-01-09 12:36:59.035444 potyk-lib-0.6.0/potyk_lib/dt/__pycache__/end.cpython-39.pyc
--rw-r--r--   0        0        0     1295 2022-11-24 06:50:27.008881 potyk-lib-0.6.0/potyk_lib/dt/__pycache__/parse.cpython-39.pyc
--rw-r--r--   0        0        0     1347 2022-11-24 07:27:13.663482 potyk-lib-0.6.0/potyk_lib/dt/end.py
--rw-r--r--   0        0        0     1066 2022-11-24 06:50:26.842481 potyk-lib-0.6.0/potyk_lib/dt/parse.py
--rw-r--r--   0        0        0      150 2022-11-24 07:16:19.180279 potyk-lib-0.6.0/potyk_lib/fp/__init__.py
--rw-r--r--   0        0        0      278 2022-11-24 07:18:37.732354 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1286 2022-11-24 06:58:08.871052 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/either.cpython-39.pyc
--rw-r--r--   0        0        0     5098 2022-11-24 06:58:08.876052 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/http.cpython-39.pyc
--rw-r--r--   0        0        0     2400 2023-01-31 14:10:55.543878 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/if_.cpython-39.pyc
--rw-r--r--   0        0        0      925 2022-11-24 07:18:37.743334 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/match.cpython-39.pyc
--rw-r--r--   0        0        0     4325 2023-01-31 14:23:21.738373 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/maybe.cpython-39.pyc
--rw-r--r--   0        0        0      528 2023-01-09 12:36:59.055446 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/pipe.cpython-39.pyc
--rw-r--r--   0        0        0     3232 2022-11-24 06:58:08.885066 potyk-lib-0.6.0/potyk_lib/fp/__pycache__/result.cpython-39.pyc
--rw-r--r--   0        0        0      859 2022-11-23 18:10:24.753050 potyk-lib-0.6.0/potyk_lib/fp/either.py
--rw-r--r--   0        0        0     3573 2022-11-05 09:32:50.225000 potyk-lib-0.6.0/potyk_lib/fp/http.py
--rw-r--r--   0        0        0     1251 2023-01-31 14:00:31.083097 potyk-lib-0.6.0/potyk_lib/fp/if_.py
--rw-r--r--   0        0        0      857 2022-11-24 07:16:19.065760 potyk-lib-0.6.0/potyk_lib/fp/match.py
--rw-r--r--   0        0        0     3828 2023-01-31 14:23:21.158543 potyk-lib-0.6.0/potyk_lib/fp/maybe.py
--rw-r--r--   0        0        0      321 2022-11-24 08:13:52.264039 potyk-lib-0.6.0/potyk_lib/fp/pipe.py
--rw-r--r--   0        0        0     2940 2022-11-04 15:08:51.344000 potyk-lib-0.6.0/potyk_lib/fp/result.py
--rw-r--r--   0        0        0       64 2022-11-24 07:16:19.039759 potyk-lib-0.6.0/potyk_lib/iter_/__init__.py
--rw-r--r--   0        0        0      215 2022-11-24 07:18:37.762326 potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      523 2023-01-09 12:36:16.655591 potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/dict_.cpython-39.pyc
--rw-r--r--   0        0        0     2506 2023-01-09 12:40:23.784916 potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/iter_.cpython-39.pyc
--rw-r--r--   0        0        0     1685 2023-01-10 11:10:06.972564 potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/list_.cpython-39.pyc
--rw-r--r--   0        0        0      189 2022-11-24 07:27:13.627480 potyk-lib-0.6.0/potyk_lib/iter_/dict_.py
--rw-r--r--   0        0        0     2285 2023-01-09 12:40:20.993874 potyk-lib-0.6.0/potyk_lib/iter_/iter_.py
--rw-r--r--   0        0        0     1292 2023-01-09 12:40:51.822119 potyk-lib-0.6.0/potyk_lib/iter_/list_.py
--rw-r--r--   0        0        0       43 2022-11-24 07:27:13.646687 potyk-lib-0.6.0/potyk_lib/num/__init__.py
--rw-r--r--   0        0        0      197 2023-01-09 12:36:59.096446 potyk-lib-0.6.0/potyk_lib/num/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      663 2022-11-24 07:25:41.667198 potyk-lib-0.6.0/potyk_lib/num/__pycache__/decimal.cpython-39.pyc
--rw-r--r--   0        0        0     1052 2023-01-09 12:36:59.099482 potyk-lib-0.6.0/potyk_lib/num/__pycache__/try_.cpython-39.pyc
--rw-r--r--   0        0        0      472 2022-11-24 07:23:03.133785 potyk-lib-0.6.0/potyk_lib/num/decimal.py
--rw-r--r--   0        0        0      789 2022-11-24 07:27:13.593478 potyk-lib-0.6.0/potyk_lib/num/try_.py
--rw-r--r--   0        0        0       48 2022-11-24 07:27:13.720871 potyk-lib-0.6.0/potyk_lib/phone/__init__.py
--rw-r--r--   0        0        0      202 2023-01-09 12:36:59.109449 potyk-lib-0.6.0/potyk_lib/phone/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      520 2023-01-09 12:36:59.112464 potyk-lib-0.6.0/potyk_lib/phone/__pycache__/mobile.cpython-39.pyc
--rw-r--r--   0        0        0      670 2022-11-24 07:18:37.785326 potyk-lib-0.6.0/potyk_lib/phone/__pycache__/sanitize.cpython-39.pyc
--rw-r--r--   0        0        0      325 2022-11-24 07:27:13.700596 potyk-lib-0.6.0/potyk_lib/phone/mobile.py
--rw-r--r--   0        0        0      511 2022-11-24 07:18:36.390512 potyk-lib-0.6.0/potyk_lib/phone/sanitize.py
--rw-r--r--   0        0        0      367 2023-01-31 14:23:37.645561 potyk-lib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-01-31 14:23:43.877513 potyk-lib-0.6.0/setup.py
--rw-r--r--   0        0        0      333 2023-01-31 14:23:43.877513 potyk-lib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-23 18:07:54.505011 potyk-lib-0.6.1/potyk_lib/__init__.py
+-rw-r--r--   0        0        0       42 2022-11-24 07:16:19.162279 potyk-lib-0.6.1/potyk_lib/dt/__init__.py
+-rw-r--r--   0        0        0      193 2022-11-24 07:18:37.710325 potyk-lib-0.6.1/potyk_lib/dt/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1542 2023-01-09 12:36:59.035444 potyk-lib-0.6.1/potyk_lib/dt/__pycache__/end.cpython-39.pyc
+-rw-r--r--   0        0        0     1295 2022-11-24 06:50:27.008881 potyk-lib-0.6.1/potyk_lib/dt/__pycache__/parse.cpython-39.pyc
+-rw-r--r--   0        0        0     1347 2022-11-24 07:27:13.663482 potyk-lib-0.6.1/potyk_lib/dt/end.py
+-rw-r--r--   0        0        0     1066 2022-11-24 06:50:26.842481 potyk-lib-0.6.1/potyk_lib/dt/parse.py
+-rw-r--r--   0        0        0      150 2022-11-24 07:16:19.180279 potyk-lib-0.6.1/potyk_lib/fp/__init__.py
+-rw-r--r--   0        0        0      278 2022-11-24 07:18:37.732354 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1286 2022-11-24 06:58:08.871052 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/either.cpython-39.pyc
+-rw-r--r--   0        0        0     5098 2022-11-24 06:58:08.876052 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/http.cpython-39.pyc
+-rw-r--r--   0        0        0     2400 2023-01-31 14:10:55.543878 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/if_.cpython-39.pyc
+-rw-r--r--   0        0        0      925 2022-11-24 07:18:37.743334 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/match.cpython-39.pyc
+-rw-r--r--   0        0        0     4325 2023-01-31 14:23:21.738373 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/maybe.cpython-39.pyc
+-rw-r--r--   0        0        0      528 2023-01-09 12:36:59.055446 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/pipe.cpython-39.pyc
+-rw-r--r--   0        0        0     3232 2022-11-24 06:58:08.885066 potyk-lib-0.6.1/potyk_lib/fp/__pycache__/result.cpython-39.pyc
+-rw-r--r--   0        0        0      859 2022-11-23 18:10:24.753050 potyk-lib-0.6.1/potyk_lib/fp/either.py
+-rw-r--r--   0        0        0     3573 2022-11-05 09:32:50.225000 potyk-lib-0.6.1/potyk_lib/fp/http.py
+-rw-r--r--   0        0        0     1251 2023-01-31 14:00:31.083097 potyk-lib-0.6.1/potyk_lib/fp/if_.py
+-rw-r--r--   0        0        0      857 2022-11-24 07:16:19.065760 potyk-lib-0.6.1/potyk_lib/fp/match.py
+-rw-r--r--   0        0        0     3828 2023-01-31 14:23:21.158543 potyk-lib-0.6.1/potyk_lib/fp/maybe.py
+-rw-r--r--   0        0        0      321 2022-11-24 08:13:52.264039 potyk-lib-0.6.1/potyk_lib/fp/pipe.py
+-rw-r--r--   0        0        0     3043 2023-04-26 13:33:16.283253 potyk-lib-0.6.1/potyk_lib/fp/result.py
+-rw-r--r--   0        0        0       64 2022-11-24 07:16:19.039759 potyk-lib-0.6.1/potyk_lib/iter_/__init__.py
+-rw-r--r--   0        0        0      215 2022-11-24 07:18:37.762326 potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      523 2023-01-09 12:36:16.655591 potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/dict_.cpython-39.pyc
+-rw-r--r--   0        0        0     2506 2023-01-09 12:40:23.784916 potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/iter_.cpython-39.pyc
+-rw-r--r--   0        0        0     1685 2023-01-10 11:10:06.972564 potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/list_.cpython-39.pyc
+-rw-r--r--   0        0        0      189 2022-11-24 07:27:13.627480 potyk-lib-0.6.1/potyk_lib/iter_/dict_.py
+-rw-r--r--   0        0        0     2285 2023-01-09 12:40:20.993874 potyk-lib-0.6.1/potyk_lib/iter_/iter_.py
+-rw-r--r--   0        0        0     1292 2023-01-09 12:40:51.822119 potyk-lib-0.6.1/potyk_lib/iter_/list_.py
+-rw-r--r--   0        0        0       43 2022-11-24 07:27:13.646687 potyk-lib-0.6.1/potyk_lib/num/__init__.py
+-rw-r--r--   0        0        0      197 2023-01-09 12:36:59.096446 potyk-lib-0.6.1/potyk_lib/num/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      663 2022-11-24 07:25:41.667198 potyk-lib-0.6.1/potyk_lib/num/__pycache__/decimal.cpython-39.pyc
+-rw-r--r--   0        0        0     1052 2023-01-09 12:36:59.099482 potyk-lib-0.6.1/potyk_lib/num/__pycache__/try_.cpython-39.pyc
+-rw-r--r--   0        0        0      472 2022-11-24 07:23:03.133785 potyk-lib-0.6.1/potyk_lib/num/decimal.py
+-rw-r--r--   0        0        0      789 2022-11-24 07:27:13.593478 potyk-lib-0.6.1/potyk_lib/num/try_.py
+-rw-r--r--   0        0        0       48 2022-11-24 07:27:13.720871 potyk-lib-0.6.1/potyk_lib/phone/__init__.py
+-rw-r--r--   0        0        0      202 2023-01-09 12:36:59.109449 potyk-lib-0.6.1/potyk_lib/phone/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      520 2023-01-09 12:36:59.112464 potyk-lib-0.6.1/potyk_lib/phone/__pycache__/mobile.cpython-39.pyc
+-rw-r--r--   0        0        0      670 2022-11-24 07:18:37.785326 potyk-lib-0.6.1/potyk_lib/phone/__pycache__/sanitize.cpython-39.pyc
+-rw-r--r--   0        0        0      325 2022-11-24 07:27:13.700596 potyk-lib-0.6.1/potyk_lib/phone/mobile.py
+-rw-r--r--   0        0        0      511 2022-11-24 07:18:36.390512 potyk-lib-0.6.1/potyk_lib/phone/sanitize.py
+-rw-r--r--   0        0        0      367 2023-04-26 13:34:17.299391 potyk-lib-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-04-26 13:34:36.727631 potyk-lib-0.6.1/setup.py
+-rw-r--r--   0        0        0      333 2023-04-26 13:34:36.727631 potyk-lib-0.6.1/PKG-INFO
```

### Comparing `potyk-lib-0.6.0/potyk_lib/dt/__pycache__/end.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/dt/__pycache__/end.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/dt/__pycache__/parse.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/dt/__pycache__/parse.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/dt/end.py` & `potyk-lib-0.6.1/potyk_lib/dt/end.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/dt/parse.py` & `potyk-lib-0.6.1/potyk_lib/dt/parse.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/either.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/either.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/http.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/http.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/if_.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/if_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/match.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/match.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/maybe.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/maybe.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/pipe.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/pipe.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/__pycache__/result.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/fp/__pycache__/result.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/either.py` & `potyk-lib-0.6.1/potyk_lib/fp/either.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/http.py` & `potyk-lib-0.6.1/potyk_lib/fp/http.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/if_.py` & `potyk-lib-0.6.1/potyk_lib/fp/if_.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/match.py` & `potyk-lib-0.6.1/potyk_lib/fp/match.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/maybe.py` & `potyk-lib-0.6.1/potyk_lib/fp/maybe.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/fp/result.py` & `potyk-lib-0.6.1/potyk_lib/fp/result.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,80 +4,76 @@
 
 __all__ = ['Result', 'Ok', 'Err']
 
 T = TypeVar('T')
 
 OkT = TypeVar('OkT')
 ErrT = TypeVar('ErrT')
+NewT = TypeVar('NewT')
 
 
 class Result(Generic[OkT, ErrT]):
-    def __iter__(self):
-        # type: () -> Iterator[Tuple[Optional[OkT], Optional[ErrT]]]
+    def __iter__(self) -> Iterator[Tuple[Optional[OkT], Optional[ErrT]]]:
         if isinstance(self, Ok):
             return iter(cast(Iterable[Tuple[Optional[OkT], Optional[ErrT]]], (self.value, None)))
         elif isinstance(self, Err):
             return iter(cast(Iterable[Tuple[Optional[OkT], Optional[ErrT]]], (None, self.value)))
         else:
             raise RuntimeError('Наследовать Result могут только Ok и Err')
 
-    def map(self, any_):
-        # type: (Callable[..., object]) -> Result
+    def map(self, any_: Callable[[OkT], NewT]) -> 'Result[NewT, ErrT]':
         """
         >>> Ok(2).map(lambda v: v + 2)
         Ok(value=4)
         >>> Err(2).map(lambda v: v + 2)
         Err(value=2)
         """
         if isinstance(self, Err):
             return self
         else:
             return Result.safe(partial(any_, cast(Ok, self).value))
 
-    def map_err(self, any_):
-        # type: (Callable[..., object]) -> Result
+    def map_err(self, any_: Callable[[ErrT], NewT]) -> 'Result[OkT, NewT]':
         """
         >>> Ok(2).map_err(lambda v: v + 2)
         Ok(value=2)
         >>> Err(2).map_err(lambda v: v + 2)
         Err(value=4)
         """
         if isinstance(self, Ok):
             return self
         else:
             return Err(any_(cast(Err, self).value))
 
-    def or_else(self, any_):
-        # type: (Callable[..., Result]) -> Result
+    def or_else(self, any_: Callable[[ErrT], 'Result[NewT, NewT]']) -> 'Result[OkT, NewT]':
         """
         >>> Ok(2).or_else(lambda v: Ok(v + 2))
         Ok(value=2)
         >>> Err(2).or_else(lambda v: Ok(v + 2))
         Ok(value=4)
         """
         if isinstance(self, Ok):
             return self
         else:
             return any_(cast(Err, self).value)
 
-    def and_then(self, any_):
-        # type: (Callable[..., Result]) -> Result
+    def and_then(self, any_: Callable[[OkT], 'Result[NewT, NewT]']) -> 'Result[NewT, ErrT]':
         """
         >>> Ok(2).and_then(lambda v: Ok(v + 2))
         Ok(value=4)
         >>> Err(2).and_then(lambda v: Ok(v + 2))
         Err(value=2)
         """
         if isinstance(self, Ok):
             return any_(cast(Ok, self).value)
         else:
             return self
 
     @classmethod
-    def safe(cls, callable_):
+    def safe(cls, callable_: Callable[[], OkT]) -> 'Result[OkT, Exception]':
         """
         >>> Result.safe(lambda: 2)
         Ok(value=2)
         >>> def raise_e():
         ...   raise Exception('err')
         >>> Result.safe(raise_e)
         Err(value=Exception('err'))
@@ -91,14 +87,14 @@
         if isinstance(self.value, Result):
             return self.value
         else:
             return self
 
 
 @dataclasses.dataclass(frozen=True)
-class Ok(Result):
-    value: Any = None
+class Ok(Generic[T], Result[T, Any]):
+    value: T = None
 
 
 @dataclasses.dataclass(frozen=True)
-class Err(Result):
-    value: Any = None
+class Err(Generic[T], Result[Any, T]):
+    value: T = None
```

### Comparing `potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/dict_.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/dict_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/iter_.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/iter_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/iter_/__pycache__/list_.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/iter_/__pycache__/list_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/iter_/iter_.py` & `potyk-lib-0.6.1/potyk_lib/iter_/iter_.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/iter_/list_.py` & `potyk-lib-0.6.1/potyk_lib/iter_/list_.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/num/__pycache__/decimal.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/num/__pycache__/decimal.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/num/__pycache__/try_.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/num/__pycache__/try_.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/num/try_.py` & `potyk-lib-0.6.1/potyk_lib/num/try_.py`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/phone/__pycache__/mobile.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/phone/__pycache__/mobile.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/potyk_lib/phone/__pycache__/sanitize.cpython-39.pyc` & `potyk-lib-0.6.1/potyk_lib/phone/__pycache__/sanitize.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `potyk-lib-0.6.0/setup.py` & `potyk-lib-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['phonenumbers>=8.13.0,<9.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'potyk-lib',
-    'version': '0.6.0',
+    'version': '0.6.1',
     'description': '',
     'long_description': None,
     'author': 'potykion',
     'author_email': 'potykion@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

