# Comparing `tmp/starlette-securecookies-1.0.2.tar.gz` & `tmp/starlette_securecookies-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette-securecookies-1.0.2.tar", max compression
+gzip compressed data, was "starlette_securecookies-1.1.0.tar", last modified: Tue Apr 25 21:24:36 2023, max compression
```

## Comparing `starlette-securecookies-1.0.2.tar` & `starlette_securecookies-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,14 @@
--rw-r--r--   0        0        0      673 2022-05-19 02:58:14.878342 starlette-securecookies-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0     1521 2022-05-19 02:25:27.525844 starlette-securecookies-1.0.2/LICENSE
--rw-r--r--   0        0        0      844 2022-05-19 02:58:12.244534 starlette-securecookies-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     3258 2022-05-19 02:54:13.457504 starlette-securecookies-1.0.2/README.md
--rw-r--r--   0        0        0      159 2022-05-19 02:25:27.533836 starlette-securecookies-1.0.2/securecookies/__init__.py
--rw-r--r--   0        0        0     6414 2022-05-19 02:35:18.142240 starlette-securecookies-1.0.2/securecookies/middleware.py
--rw-r--r--   0        0        0        0 2022-05-19 02:25:27.533836 starlette-securecookies-1.0.2/securecookies/py.typed
--rw-r--r--   0        0        0     4069 2022-05-19 03:03:26.650427 starlette-securecookies-1.0.2/setup.py
--rw-r--r--   0        0        0     4194 2022-05-19 03:03:26.650427 starlette-securecookies-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      673 2022-05-19 02:58:14.878342 starlette_securecookies-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1521 2022-05-19 02:25:27.525844 starlette_securecookies-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4494 2023-04-25 21:21:43.979609 starlette_securecookies-1.1.0/README.md
+-rw-r--r--   0        0        0     1360 2023-04-25 21:24:36.033554 starlette_securecookies-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-25 21:21:43.984607 starlette_securecookies-1.1.0/securecookies/__init__.py
+-rw-r--r--   0        0        0      551 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.0/securecookies/extras/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-25 21:21:43.985607 starlette_securecookies-1.1.0/securecookies/extras/csrf.py
+-rw-r--r--   0        0        0     6991 2023-04-25 21:21:43.986607 starlette_securecookies-1.1.0/securecookies/middleware.py
+-rw-r--r--   0        0        0        0 2022-05-19 02:25:27.533836 starlette_securecookies-1.1.0/securecookies/py.typed
+-rw-r--r--   0        0        0     3146 2023-04-25 21:21:43.987607 starlette_securecookies-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1078 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.0/tests/extras/test_csrf.py
+-rw-r--r--   0        0        0      943 2023-04-25 21:21:43.988607 starlette_securecookies-1.1.0/tests/test_other-party.py
+-rw-r--r--   0        0        0     3900 2023-04-24 01:08:05.010116 starlette_securecookies-1.1.0/tests/test_securecookies.py
+-rw-r--r--   0        0        0     7120 1970-01-01 00:00:00.000000 starlette_securecookies-1.1.0/PKG-INFO
```

### Comparing `starlette-securecookies-1.0.2/CHANGELOG.md` & `starlette_securecookies-1.1.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `starlette-securecookies-1.0.2/LICENSE` & `starlette_securecookies-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette-securecookies-1.0.2/README.md` & `starlette_securecookies-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,81 @@
 # starlette-securecookies
 
-![GitHub Workflow Status](https://img.shields.io/github/workflow/status/thearchitector/starlette-securecookies/CI?label=tests&style=flat-square)
+![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/thearchitector/starlette-securecookies/CI.yaml?label=tests&style=flat-square)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/starlette-securecookies?style=flat-square)
 ![GitHub](https://img.shields.io/github/license/thearchitector/starlette-securecookies?style=flat-square)
 [![Buy a tree](https://img.shields.io/badge/Treeware-%F0%9F%8C%B3-lightgreen?style=flat-square)](https://ecologi.com/eliasgabriel?r=6128126916bfab8bd051026c)
 
 Customizable middleware for adding automatic cookie encryption and decryption to Starlette applications.
 
-Tested support on Python 3.7, 3.8, 3.9, and 3.10 on macOS, Windows, and Linux.
+Tested support on Python 3.7, 3.8, 3.9, and 3.10, 3.11 on macOS, Windows, and Linux.
 
 ## How it works?
 
 ```mermaid
 sequenceDiagram
-    Browser->>+Middleware: Encrypted cookies
-    Middleware->>+Application: Filtered / Decrypted cookies
+    Browser->>+Middleware: Encrypted 'Cookie' header
+    Middleware->>+Application: Decrypted cookies
     Application->>-Middleware: Plaintext cookies
-    Middleware->>-Browser: Encrypted 'Set-Cookie' headers
+    Middleware->>-Browser: Encrypted 'Set-Cookie' header
+    Note over Application: *The Application may be your service<br />or any additional middleware.
 ```
 
 For any incoming cookies:
 
 1. Requests sent from the client's browser to your application are intercepted by `SecureCookiesMiddleware`.
 2. All `Cookie` headers are parsed and filter. Only cookies in the `included_cookies` and `excluded_cookies` parameters are parsed. All cookies are included by default.
 3. The cookies are decrypted. If cookie cannot be decrypted, or is otherwise invalid, it is discarded by default (`discard_invalid=True`).
 4. Any included and valid encrypted cookies in the ASGI request scope are replaced by the decrypted ones.
 5. The request scope is passed to any future middleware, and eventually your application. Cookies can be read normally anywhere downstream.
 
 For any outgoing cookies:
 
 7. Your application sets cookies with `response.set_cookie` as usual.
-8. All responses returned by your application are intercepted by `SecureCookiesMiddleware`.
-9. Cookies in the `included_cookies` and `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by the parameters set in `SecureCookiesMiddleware`.
-10. The cookies in the response are replaced by the re-encrypted cookies, and the response is propagated to Starlette to return to the client's browser.
+8. Other middleware run and add additional cookies, like [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware).
+9. All responses returned by your application are intercepted by `SecureCookiesMiddleware`.
+10. Cookies in the `included_cookies` and `excluded_cookies` parameters are re-encrypted, and their attributes (like `"SameSite"` and `"HttpOnly"`) are overridden by the parameters set in `SecureCookiesMiddleware` if set.
+11. The cookies in the response are replaced by the re-encrypted cookies, and the response is eventually propagated to the client's browser.
 
 ## Installation
 
 ```sh
-$ poetry add starlette-securecookies
+$ pdm add starlette-securecookies
 # or
 $ python -m pip install --user starlette-securecookies
 ```
 
 ## Usage
 
-This is a Starlette-based middleware, so it can be used in any Starlette application or Starlette-based application (like [FastAPI](https://fastapi.tiangolo.com/advanced/middleware/) or [Starlite](https://starlite-api.github.io/starlite/usage/7-middleware/)).
+This is a Starlette-based middleware, so it can be used in any Starlette application or Starlette-based framework (like [FastAPI](https://fastapi.tiangolo.com/advanced/middleware/)).
 
 For example,
 
 ```python
 from starlette.applications import Starlette
 from starlette.middleware import Middleware
 
 from securecookies import SecureCookiesMiddleware
 
 middleware = [
     Middleware(
-        SecureCookiesMiddleware, secrets=["SUPER SECRET SECRET"]
+        SecureCookiesMiddleware, secrets=["SUPER SECRET SECRET"],
+        # your other middleware
     )
 ]
 
 app = Starlette(routes=..., middleware=middleware)
 ```
 
+Note that if you're using another middleware that injects cookies into the response (such as [SessionMiddleware](https://www.starlette.io/middleware/#sessionmiddleware)), you have to make sure `SecureCookiesMiddleware` executes _after_ it so the cookie is present at encryption-time. Counter intuitively, in practice this means ensuring `SecureCookiesMiddleware` is _first_ in the list of middleware.
+
+### Extras
+
+`starlette-securecookies` provides some extras that introduce or patch secure cookie functionality into existing tools. They all reside in the `securecookies.extras` module. Currently there is only one, but more are welcome by recommendation or Pull Request!
+
+- **`csrf.SecureCSRFMiddleware`**: Adds compatibility to the CSRF middleware provided by [starlette_csrf](https://github.com/frankie567/starlette-csrf). To use it, simply add it to your list of middleware (keep in mind the ordering). If you don't want to specify `starlette_csrf` as a direct dependency, you can also install it through the `[csrf]` package extra.
+
 ## License
 
 This software is licensed under the [BSD 3-Clause License](LICENSE).
 
 This package is Treeware. If you use it in production, consider buying the world a tree to thank me for my work. By contributing to my forest, you’ll be creating employment for local families and restoring wildlife habitats.
```

### Comparing `starlette-securecookies-1.0.2/securecookies/middleware.py` & `starlette_securecookies-1.1.0/securecookies/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+import sys
 from http.cookies import SimpleCookie
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from cryptography.fernet import Fernet, InvalidToken, MultiFernet
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.responses import Response
 from starlette.types import ASGIApp
 
+if sys.version_info >= (3, 8):  # pragma: no cover
+    from typing import Literal
+else:  # pragma: no cover
+    from typing_extensions import Literal
+
 
 class BadArgumentError(Exception):
     """
     Generic error arguments with invalid values, or combinations of conflicting
     arguments.
     """
 
 
 class SecureCookiesMiddleware(BaseHTTPMiddleware):
     """
     Provides automatic secure cookie support through symmetric Fernet encryption. As per
     the `cryptography` docs, security is achieved through:
 
-    - 128-bit key AES in CBC mode using PKCS7 padding for encryption
+    - 128-bit key AES in CBC mode using PKCS7 padding for encryption.
     - HMAC using SHA256 for authentication.
     """
 
     secrets: List[str]
     """
     A list of secrets to use when encrypting and decrypting secure cookies. Supplying
     multiple secrets enables the use of key rotation, whereby the first key is used for
@@ -37,15 +43,15 @@
         app: ASGIApp,
         secrets: List[str],
         discard_invalid: bool = True,
         cookie_path: Optional[str] = None,
         cookie_domain: Optional[str] = None,
         cookie_secure: Optional[bool] = None,
         cookie_httponly: Optional[bool] = None,
-        cookie_samesite: Optional[str] = None,
+        cookie_samesite: Optional[Literal["strict", "lax", "none"]] = None,
         excluded_cookies: Optional[List[str]] = None,
         included_cookies: Optional[List[str]] = None,
     ) -> None:
         super().__init__(app)
         self.mfernet = MultiFernet(Fernet(s) for s in secrets)
         self.discard_invalid = discard_invalid
         """ Discard any invalid / unencrypted cookies present in the request."""
@@ -70,78 +76,88 @@
         The list of cookies to decrypt and encrypt in the request --> response cycle.
         This option is mutually exclusive with `excluded_cookies`.
         """
 
         if excluded_cookies and included_cookies:
             raise BadArgumentError(
                 "It doesn't make sense to specify both excluded and included cookies."
-                " Supply with `excluded_cookies` or `included_cookies` to restrict"
+                " Supply either `excluded_cookies` or `included_cookies` to restrict"
                 " which cookies should be secure."
             )
 
         if cookie_samesite and cookie_samesite.lower() not in ["strict", "lax", "none"]:
             raise BadArgumentError(
                 "SameSite attribute must be either 'strict', 'lax' or 'none'"
             )
 
+    def set_header(self, request: Request, header: str, value: str) -> None:
+        """
+        Adds the given Header to the available Request headers. If the Header already
+        exists, its value is overwritten.
+        """
+        hkey = header.encode("latin-1")
+        request.scope["headers"] = [
+            *(h for h in request.scope["headers"] if h[0] != hkey),
+            (hkey, value.encode("latin-1")),
+        ]
+
+    def decrypt(self, value: str) -> str:
+        """Decrypt the given value using any of the configured secrets."""
+        return self.mfernet.decrypt(value.encode()).decode()
+
+    def encrypt(self, value: str) -> str:
+        """Encrypt the given value using the first configured secret."""
+        return self.mfernet.encrypt(value.encode()).decode()
+
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> Response:
-        # request cookies are only passed along and mutable within the asgi scope
-        headers = request.scope["headers"]
-        raw_cookies = [h for h in headers if h[0] == b"cookie"]
-        if len(raw_cookies):
-            # if encrypted cookies are present, remove and parse them
-            headers.remove(raw_cookies[0])
-            cookies: SimpleCookie = SimpleCookie(raw_cookies[0][1].decode())
-
-            for cookie, morsel in list(cookies.items()):
+        if len(request.cookies):
+            cookies: SimpleCookie[Any] = SimpleCookie()
+            for cookie, value in request.cookies.items():
                 # if the cookie is included or not excluded
                 if (
                     (not self.included_cookies and not self.excluded_cookies)
                     or (self.included_cookies and cookie in self.included_cookies)
                     or (self.excluded_cookies and cookie not in self.excluded_cookies)
                 ):
                     try:
-                        # try to decrypt the token. if you can, then it's already
-                        # encrypted and can be passed along
-                        cookies[cookie] = self.mfernet.decrypt(
-                            morsel.value.encode()
-                        ).decode()
+                        # try to decrypt the cookie and pass it along
+                        cookies[cookie] = self.decrypt(value)
                     except InvalidToken:
-                        # delete invalid or unencrypted cookies if enabled
-                        if self.discard_invalid:
-                            del cookies[cookie]
-
-            # serialize and append the decrypted cookies to the asgi scope headers
-            new_cookie = (
-                b"cookie",
-                cookies.output(header="", sep=";").strip().encode(),
+                        # delete invalid or unencrypted cookies unless disabled
+                        if not self.discard_invalid:
+                            cookies[cookie] = value
+
+            # serialize and set the decrypted cookies to the asgi scope headers
+            # we have to modify the scope directly because request objects are not
+            # passed between ASGI applications / middleware.
+            self.set_header(
+                request, "cookie", cookies.output(header="", sep=";").strip()
             )
-            headers.append(new_cookie)
 
         # propagate the modified request
         response: Response = await call_next(request)
 
         # for every cookie in the response
-        for raw_cookie in response.headers.getlist("set-cookie"):
+        for cookie in response.headers.getlist("set-cookie"):
             # decode it
-            ncookie: SimpleCookie = SimpleCookie(raw_cookie)
+            ncookie: SimpleCookie[Any] = SimpleCookie(cookie)
             key = [*ncookie.keys()][0]
 
             # if the cookie is included or not excluded
             if (
                 (not self.included_cookies and not self.excluded_cookies)
                 or (self.included_cookies and key in self.included_cookies)
                 or (self.excluded_cookies and key not in self.excluded_cookies)
             ):
                 # create a new encrypted cookie with the desired attributes
                 response.set_cookie(
                     key,
-                    value=self.mfernet.encrypt(ncookie[key].value.encode()).decode(),
+                    value=self.encrypt(ncookie[key].value),
                     path=self.cookie_path or ncookie[key]["path"],
                     domain=self.cookie_domain or ncookie[key]["domain"],
                     secure=self.cookie_secure or ncookie[key]["secure"],
                     httponly=self.cookie_httponly or ncookie[key]["httponly"],
                     samesite=self.cookie_samesite or ncookie[key]["samesite"],
                 )
```

