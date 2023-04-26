# Comparing `tmp/ichi_auth-1.0.post1-py3-none-any.whl.zip` & `tmp/ichi_auth-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12249 bytes, number of entries: 9
--rw-r--r--  2.0 unx      147 b- defN 22-Nov-27 16:09 ichi_auth/__init__.py
--rw-r--r--  2.0 unx     4939 b- defN 22-Nov-17 15:34 ichi_auth/auth_config.py
--rw-r--r--  2.0 unx    35218 b- defN 22-Nov-17 15:34 ichi_auth/auth_jwt.py
--rw-r--r--  2.0 unx     4080 b- defN 22-Nov-17 15:34 ichi_auth/config.py
--rw-r--r--  2.0 unx     2218 b- defN 22-Nov-17 15:34 ichi_auth/exceptions.py
--rw-r--r--  2.0 unx     1115 b- defN 22-Nov-17 15:34 ichi_auth-1.0.post1.dist-info/LICENSE
-?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 ichi_auth-1.0.post1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2885 b- defN 16-Jan-01 00:00 ichi_auth-1.0.post1.dist-info/METADATA
-?rw-r--r--  2.0 unx      711 b- defN 16-Jan-01 00:00 ichi_auth-1.0.post1.dist-info/RECORD
-9 files, 51394 bytes uncompressed, 11035 bytes compressed:  78.5%
+Zip file size: 12546 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      145 b- defN 23-Apr-26 00:14 ichi_auth/__init__.py
+-rw-r--r--  2.0 unx     4948 b- defN 23-Apr-26 00:11 ichi_auth/auth_config.py
+-rw-r--r--  2.0 unx    36977 b- defN 23-Apr-26 00:11 ichi_auth/auth_jwt.py
+-rw-r--r--  2.0 unx     4318 b- defN 23-Apr-26 00:11 ichi_auth/config.py
+-rw-r--r--  2.0 unx     1733 b- defN 23-Apr-26 00:14 ichi_auth/exceptions.py
+-rw-r--r--  2.0 unx     1117 b- defN 23-Apr-26 00:02 ichi_auth-1.1.dist-info/LICENSE
+?rw-r--r--  2.0 unx       81 b- defN 16-Jan-01 00:00 ichi_auth-1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2871 b- defN 16-Jan-01 00:00 ichi_auth-1.1.dist-info/METADATA
+?rw-r--r--  2.0 unx      687 b- defN 16-Jan-01 00:00 ichi_auth-1.1.dist-info/RECORD
+9 files, 52877 bytes uncompressed, 11380 bytes compressed:  78.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: ichi_auth/config.py
 Comment: 
 
 Filename: ichi_auth/exceptions.py
 Comment: 
 
-Filename: ichi_auth-1.0.post1.dist-info/LICENSE
+Filename: ichi_auth-1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ichi_auth-1.0.post1.dist-info/WHEEL
+Filename: ichi_auth-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ichi_auth-1.0.post1.dist-info/METADATA
+Filename: ichi_auth-1.1.dist-info/METADATA
 Comment: 
 
-Filename: ichi_auth-1.0.post1.dist-info/RECORD
+Filename: ichi_auth-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ichi_auth/__init__.py

```diff
@@ -1,5 +1,5 @@
 """FastAPI extension that provides JWT Auth support (secure, easy to use and lightweight)"""
 
-__version__ = "1.0-1"
+__version__ = "1.1"
 
 from .auth_jwt import AuthJWT
```

## ichi_auth/auth_config.py

```diff
@@ -1,27 +1,28 @@
 from ichi_auth.config import LoadConfig
 from pydantic import ValidationError
 from typing import Callable, List
 from datetime import timedelta
 
+
 class AuthConfig:
     _token = None
-    _token_location = {'headers'}
+    _token_location = {"headers"}
 
     _secret_key = None
     _public_key = None
     _private_key = None
     _algorithm = "HS256"
     _decode_algorithms = None
     _decode_leeway = 0
     _encode_issuer = None
     _decode_issuer = None
     _decode_audience = None
     _denylist_enabled = False
-    _denylist_token_checks = {'access','refresh'}
+    _denylist_token_checks = {"access", "refresh"}
     _header_name = "Authorization"
     _header_type = "Bearer"
     _token_in_denylist_callback = None
     _access_token_expires = timedelta(minutes=15)
     _refresh_token_expires = timedelta(days=30)
 
     # option for create cookies
@@ -38,28 +39,28 @@
     _cookie_csrf_protect = True
     _access_csrf_cookie_key = "csrf_access_token"
     _refresh_csrf_cookie_key = "csrf_refresh_token"
     _access_csrf_cookie_path = "/"
     _refresh_csrf_cookie_path = "/"
     _access_csrf_header_name = "X-CSRF-Token"
     _refresh_csrf_header_name = "X-CSRF-Token"
-    _csrf_methods = {'POST','PUT','PATCH','DELETE'}
+    _csrf_methods = {"POST", "PUT", "PATCH", "DELETE"}
 
     @property
     def jwt_in_cookies(self) -> bool:
-        return 'cookies' in self._token_location
+        return "cookies" in self._token_location
 
     @property
     def jwt_in_headers(self) -> bool:
-        return 'headers' in self._token_location
+        return "headers" in self._token_location
 
     @classmethod
-    def load_config(cls, settings: Callable[...,List[tuple]]) -> "AuthConfig":
+    def load_config(cls, settings: Callable[..., List[tuple]]) -> "AuthConfig":
         try:
-            config = LoadConfig(**{key.lower():value for key,value in settings()})
+            config = LoadConfig(**{key.lower(): value for key, value in settings()})
 
             cls._token_location = config.authjwt_token_location
             cls._secret_key = config.authjwt_secret_key
             cls._public_key = config.authjwt_public_key
             cls._private_key = config.authjwt_private_key
             cls._algorithm = config.authjwt_algorithm
             cls._decode_algorithms = config.authjwt_decode_algorithms
@@ -93,15 +94,15 @@
             cls._csrf_methods = config.authjwt_csrf_methods
         except ValidationError:
             raise
         except Exception:
             raise TypeError("Config must be pydantic 'BaseSettings' or list of tuple")
 
     @classmethod
-    def token_in_denylist_loader(cls, callback: Callable[...,bool]) -> "AuthConfig":
+    def token_in_denylist_loader(cls, callback: Callable[..., bool]) -> "AuthConfig":
         """
         This decorator sets the callback function that will be called when
         a protected endpoint is accessed and will check if the JWT has been
         been revoked. By default, this callback is not used.
 
         *HINT*: The callback must be a function that takes decrypted_token argument,
         args for object AuthJWT and this is not used, decrypted_token is decode
```

## ichi_auth/auth_jwt.py

```diff
@@ -8,19 +8,20 @@
     InvalidHeaderError,
     CSRFError,
     JWTDecodeError,
     RevokedTokenError,
     MissingTokenError,
     AccessTokenRequired,
     RefreshTokenRequired,
-    FreshTokenRequired
+    FreshTokenRequired,
 )
 
+
 class AuthJWT(AuthConfig):
-    def __init__(self,req: Request = None, res: Response = None):
+    def __init__(self, req: Request = None, res: Response = None):
         """
         Get jwt header from incoming request or get
         request and response object if jwt in the cookie
 
         :param req: all incoming request
         :param res: response from endpoint
         """
@@ -30,107 +31,123 @@
         if req:
             # get request object when cookies in token location
             if self.jwt_in_cookies:
                 self._request = req
             # get jwt in headers when headers in token location
             if self.jwt_in_headers:
                 auth = req.headers.get(self._header_name.lower())
-                if auth: self._get_jwt_from_headers(auth)
+                if auth:
+                    self._get_jwt_from_headers(auth)
 
-    def _get_jwt_from_headers(self,auth: str) -> "AuthJWT":
+    def _get_jwt_from_headers(self, auth: str) -> "AuthJWT":
         """
         Get token from the headers
 
         :param auth: value from HeaderName
         """
         header_name, header_type = self._header_name, self._header_type
 
         parts = auth.split()
 
         # Make sure the header is in a valid format that we are expecting, ie
         if not header_type:
             # <HeaderName>: <JWT>
             if len(parts) != 1:
                 msg = "Bad {} header. Expected value '<JWT>'".format(header_name)
-                raise InvalidHeaderError(status_code=422,message=msg)
+                raise InvalidHeaderError(status_code=422, message=msg)
             self._token = parts[0]
         else:
             # <HeaderName>: <HeaderType> <JWT>
-            if not re.match(r"{}\s".format(header_type),auth) or len(parts) != 2:
-                msg = "Bad {} header. Expected value '{} <JWT>'".format(header_name,header_type)
-                raise InvalidHeaderError(status_code=422,message=msg)
+            if not re.match(r"{}\s".format(header_type), auth) or len(parts) != 2:
+                msg = "Bad {} header. Expected value '{} <JWT>'".format(
+                    header_name, header_type
+                )
+                raise InvalidHeaderError(status_code=422, message=msg)
             self._token = parts[1]
 
     def _get_jwt_identifier(self) -> str:
         return str(uuid.uuid4())
 
-    def _get_int_from_datetime(self,value: datetime) -> int:
+    def _get_int_from_datetime(self, value: datetime) -> int:
         """
         :param value: datetime with or without timezone, if don't contains timezone
                       it will managed as it is UTC
         :return: Seconds since the Epoch
         """
         if not isinstance(value, datetime):  # pragma: no cover
-            raise TypeError('a datetime is required')
+            raise TypeError("a datetime is required")
         return int(value.timestamp())
 
     def _get_secret_key(self, algorithm: str, process: str) -> str:
         """
         Get key with a different algorithm
 
         :param algorithm: algorithm for decode and encode token
         :param process: for indicating get key for encode or decode token
 
         :return: plain text or RSA depends on algorithm
         """
-        symmetric_algorithms, asymmetric_algorithms = {"HS256","HS384","HS512"}, requires_cryptography
-
-        if algorithm not in symmetric_algorithms and algorithm not in asymmetric_algorithms:
+        symmetric_algorithms, asymmetric_algorithms = {
+            "HS256",
+            "HS384",
+            "HS512",
+        }, requires_cryptography
+
+        if (
+            algorithm not in symmetric_algorithms
+            and algorithm not in asymmetric_algorithms
+        ):
             raise ValueError("Algorithm {} could not be found".format(algorithm))
 
         if algorithm in symmetric_algorithms:
             if not self._secret_key:
                 raise RuntimeError(
-                    "authjwt_secret_key must be set when using symmetric algorithm {}".format(algorithm)
+                    "authjwt_secret_key must be set when using symmetric algorithm {}".format(
+                        algorithm
+                    )
                 )
 
             return self._secret_key
 
         if algorithm in asymmetric_algorithms and not has_crypto:
             raise RuntimeError(
                 "Missing dependencies for using asymmetric algorithms. run 'pip install fastapi-jwt-auth[asymmetric]'"
             )
 
         if process == "encode":
             if not self._private_key:
                 raise RuntimeError(
-                    "authjwt_private_key must be set when using asymmetric algorithm {}".format(algorithm)
+                    "authjwt_private_key must be set when using asymmetric algorithm {}".format(
+                        algorithm
+                    )
                 )
 
             return self._private_key
 
         if process == "decode":
             if not self._public_key:
                 raise RuntimeError(
-                    "authjwt_public_key must be set when using asymmetric algorithm {}".format(algorithm)
+                    "authjwt_public_key must be set when using asymmetric algorithm {}".format(
+                        algorithm
+                    )
                 )
 
             return self._public_key
 
     def _create_token(
         self,
-        subject: Union[str,int],
+        subject: Union[str, int],
         type_token: str,
         exp_time: Optional[int],
         fresh: Optional[bool] = False,
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
         issuer: Optional[str] = None,
-        audience: Optional[Union[str,Sequence[str]]] = None,
-        user_claims: Optional[Dict] = {}
+        audience: Optional[Union[str, Sequence[str]]] = None,
+        user_claims: Optional[Dict] = {},
     ) -> str:
         """
         Create token for access_token and refresh_token (utf-8)
 
         :param subject: Identifier for who this token is for example id or username from database.
         :param type_token: indicate token is access_token or refresh_token
         :param exp_time: Set the duration of the JWT
@@ -140,15 +157,15 @@
         :param issuer: expected issuer in the JWT
         :param audience: expected audience in the JWT
         :param user_claims: Custom claims to include in this token. This data must be dictionary
 
         :return: Encoded token
         """
         # Validation type data
-        if not isinstance(subject, (str,int)):
+        if not isinstance(subject, (str, int)):
             raise TypeError("subject must be a string or integer")
         if not isinstance(fresh, bool):
             raise TypeError("fresh must be a boolean")
         if audience and not isinstance(audience, (str, list, tuple, set, frozenset)):
             raise TypeError("audience must be a string or sequence")
         if algorithm and not isinstance(algorithm, str):
             raise TypeError("algorithm must be a string")
@@ -156,521 +173,556 @@
             raise TypeError("user_claims must be a dictionary")
 
         # Data section
         reserved_claims = {
             "sub": subject,
             "iat": self._get_int_from_datetime(datetime.now(timezone.utc)),
             "nbf": self._get_int_from_datetime(datetime.now(timezone.utc)),
-            "jti": self._get_jwt_identifier()
+            "jti": self._get_jwt_identifier(),
         }
 
         custom_claims = {"type": type_token}
 
         # for access_token only fresh needed
-        if type_token == 'access':
-            custom_claims['fresh'] = fresh
+        if type_token == "access":
+            custom_claims["fresh"] = fresh
         # if cookie in token location and csrf protection enabled
         if self.jwt_in_cookies and self._cookie_csrf_protect:
-            custom_claims['csrf'] = self._get_jwt_identifier()
+            custom_claims["csrf"] = self._get_jwt_identifier()
 
         if exp_time:
-            reserved_claims['exp'] = exp_time
+            reserved_claims["exp"] = exp_time
         if issuer:
-            reserved_claims['iss'] = issuer
+            reserved_claims["iss"] = issuer
         if audience:
-            reserved_claims['aud'] = audience
+            reserved_claims["aud"] = audience
 
         algorithm = algorithm or self._algorithm
 
         try:
-            secret_key = self._get_secret_key(algorithm,"encode")
+            secret_key = self._get_secret_key(algorithm, "encode")
         except Exception:
             raise
 
         return jwt.encode(
             {**reserved_claims, **custom_claims, **user_claims},
             secret_key,
             algorithm=algorithm,
-            headers=headers
+            headers=headers,
         )
 
     def _has_token_in_denylist_callback(self) -> bool:
         """
         Return True if token denylist callback set
         """
         return self._token_in_denylist_callback is not None
 
-    def _check_token_is_revoked(self, raw_token: Dict[str,Union[str,int,bool]]) -> None:
+    def _check_token_is_revoked(
+        self, raw_token: Dict[str, Union[str, int, bool]]
+    ) -> None:
         """
         Ensure that AUTHJWT_DENYLIST_ENABLED is true and callback regulated, and then
         call function denylist callback with passing decode JWT, if true
         raise exception Token has been revoked
         """
         if not self._denylist_enabled:
             return
 
         if not self._has_token_in_denylist_callback():
-            raise RuntimeError("A token_in_denylist_callback must be provided via "
+            raise RuntimeError(
+                "A token_in_denylist_callback must be provided via "
                 "the '@AuthJWT.token_in_denylist_loader' if "
-                "authjwt_denylist_enabled is 'True'")
+                "authjwt_denylist_enabled is 'True'"
+            )
 
         if self._token_in_denylist_callback.__func__(raw_token):
-            raise RevokedTokenError(status_code=401,message="Token has been revoked")
+            raise RevokedTokenError(status_code=401, message="Token has been revoked")
 
     def _get_expired_time(
         self,
         type_token: str,
-        expires_time: Optional[Union[timedelta,int,bool]] = None
-    ) -> Union[None,int]:
+        expires_time: Optional[Union[timedelta, int, bool]] = None,
+    ) -> Union[None, int]:
         """
         Dynamic token expired, if expires_time is False exp claim not created
 
         :param type_token: indicate token is access_token or refresh_token
         :param expires_time: duration expired jwt
 
         :return: duration exp claim jwt
         """
-        if expires_time and not isinstance(expires_time, (timedelta,int,bool)):
+        if expires_time and not isinstance(expires_time, (timedelta, int, bool)):
             raise TypeError("expires_time must be between timedelta, int, bool")
 
         if expires_time is not False:
-            if type_token == 'access':
+            if type_token == "access":
                 expires_time = expires_time or self._access_token_expires
-            if type_token == 'refresh':
+            if type_token == "refresh":
                 expires_time = expires_time or self._refresh_token_expires
 
         if expires_time is not False:
             if isinstance(expires_time, bool):
-                if type_token == 'access':
+                if type_token == "access":
                     expires_time = self._access_token_expires
-                if type_token == 'refresh':
+                if type_token == "refresh":
                     expires_time = self._refresh_token_expires
             if isinstance(expires_time, timedelta):
                 expires_time = int(expires_time.total_seconds())
 
-            return self._get_int_from_datetime(datetime.now(timezone.utc)) + expires_time
+            return (
+                self._get_int_from_datetime(datetime.now(timezone.utc)) + expires_time
+            )
         else:
             return None
 
     def create_access_token(
         self,
-        subject: Union[str,int],
+        subject: Union[str, int],
         fresh: Optional[bool] = False,
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
-        expires_time: Optional[Union[timedelta,int,bool]] = None,
-        audience: Optional[Union[str,Sequence[str]]] = None,
-        user_claims: Optional[Dict] = {}
+        expires_time: Optional[Union[timedelta, int, bool]] = None,
+        audience: Optional[Union[str, Sequence[str]]] = None,
+        user_claims: Optional[Dict] = {},
     ) -> str:
         """
         Create a access token with 15 minutes for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
         return self._create_token(
             subject=subject,
             type_token="access",
-            exp_time=self._get_expired_time("access",expires_time),
+            exp_time=self._get_expired_time("access", expires_time),
             fresh=fresh,
             algorithm=algorithm,
             headers=headers,
             audience=audience,
             user_claims=user_claims,
-            issuer=self._encode_issuer
+            issuer=self._encode_issuer,
         )
 
     def create_refresh_token(
         self,
-        subject: Union[str,int],
+        subject: Union[str, int],
         algorithm: Optional[str] = None,
         headers: Optional[Dict] = None,
-        expires_time: Optional[Union[timedelta,int,bool]] = None,
-        audience: Optional[Union[str,Sequence[str]]] = None,
-        user_claims: Optional[Dict] = {}
+        expires_time: Optional[Union[timedelta, int, bool]] = None,
+        audience: Optional[Union[str, Sequence[str]]] = None,
+        user_claims: Optional[Dict] = {},
     ) -> str:
         """
         Create a refresh token with 30 days for expired time (default),
         info for param and return check to function create token
 
         :return: hash token
         """
         return self._create_token(
             subject=subject,
             type_token="refresh",
-            exp_time=self._get_expired_time("refresh",expires_time),
+            exp_time=self._get_expired_time("refresh", expires_time),
             algorithm=algorithm,
             headers=headers,
             audience=audience,
-            user_claims=user_claims
+            user_claims=user_claims,
         )
 
-    def _get_csrf_token(self,encoded_token: str) -> str:
+    def _get_csrf_token(self, encoded_token: str) -> str:
         """
         Returns the CSRF double submit token from an encoded JWT.
 
         :param encoded_token: The encoded JWT
         :return: The CSRF double submit token
         """
-        return self._verified_token(encoded_token)['csrf']
+        return self._verified_token(encoded_token)["csrf"]
 
     def set_access_cookies(
         self,
         encoded_access_token: str,
         response: Optional[Response] = None,
-        max_age: Optional[int] = None
+        max_age: Optional[int] = None,
     ) -> None:
         """
         Configures the response to set access token in a cookie.
         this will also set the CSRF double submit values in a separate cookie
 
         :param encoded_access_token: The encoded access token to set in the cookies
         :param response: The FastAPI response object to set the access cookies in
         :param max_age: The max age of the cookie value should be the number of seconds (integer)
         """
         if not self.jwt_in_cookies:
             raise RuntimeWarning(
                 "set_access_cookies() called without 'authjwt_token_location' configured to use cookies"
             )
 
-        if max_age and not isinstance(max_age,int):
+        if max_age and not isinstance(max_age, int):
             raise TypeError("max_age must be a integer")
-        if response and not isinstance(response,Response):
+        if response and not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
 
         response = response or self._response
 
         # Set the access JWT in the cookie
         response.set_cookie(
             self._access_cookie_key,
             encoded_access_token,
             max_age=max_age or self._cookie_max_age,
             path=self._access_cookie_path,
             domain=self._cookie_domain,
             secure=self._cookie_secure,
             httponly=True,
-            samesite=self._cookie_samesite
+            samesite=self._cookie_samesite,
         )
 
         # If enabled, set the csrf double submit access cookie
         if self._cookie_csrf_protect:
             response.set_cookie(
                 self._access_csrf_cookie_key,
                 self._get_csrf_token(encoded_access_token),
                 max_age=max_age or self._cookie_max_age,
                 path=self._access_csrf_cookie_path,
                 domain=self._cookie_domain,
                 secure=self._cookie_secure,
                 httponly=False,
-                samesite=self._cookie_samesite
+                samesite=self._cookie_samesite,
             )
 
     def set_refresh_cookies(
         self,
         encoded_refresh_token: str,
         response: Optional[Response] = None,
-        max_age: Optional[int] = None
+        max_age: Optional[int] = None,
     ) -> None:
         """
         Configures the response to set refresh token in a cookie.
         this will also set the CSRF double submit values in a separate cookie
 
         :param encoded_refresh_token: The encoded refresh token to set in the cookies
         :param response: The FastAPI response object to set the refresh cookies in
         :param max_age: The max age of the cookie value should be the number of seconds (integer)
         """
         if not self.jwt_in_cookies:
             raise RuntimeWarning(
                 "set_refresh_cookies() called without 'authjwt_token_location' configured to use cookies"
             )
 
-        if max_age and not isinstance(max_age,int):
+        if max_age and not isinstance(max_age, int):
             raise TypeError("max_age must be a integer")
-        if response and not isinstance(response,Response):
+        if response and not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
 
         response = response or self._response
 
         # Set the refresh JWT in the cookie
         response.set_cookie(
             self._refresh_cookie_key,
             encoded_refresh_token,
             max_age=max_age or self._cookie_max_age,
             path=self._refresh_cookie_path,
             domain=self._cookie_domain,
             secure=self._cookie_secure,
             httponly=True,
-            samesite=self._cookie_samesite
+            samesite=self._cookie_samesite,
         )
 
         # If enabled, set the csrf double submit refresh cookie
         if self._cookie_csrf_protect:
             response.set_cookie(
                 self._refresh_csrf_cookie_key,
                 self._get_csrf_token(encoded_refresh_token),
                 max_age=max_age or self._cookie_max_age,
                 path=self._refresh_csrf_cookie_path,
                 domain=self._cookie_domain,
                 secure=self._cookie_secure,
                 httponly=False,
-                samesite=self._cookie_samesite
+                samesite=self._cookie_samesite,
             )
 
-    def unset_jwt_cookies(self,response: Optional[Response] = None) -> None:
+    def unset_jwt_cookies(self, response: Optional[Response] = None) -> None:
         """
         Unset (delete) all jwt stored in a cookie
 
         :param response: The FastAPI response object to delete the JWT cookies in.
         """
         self.unset_access_cookies(response)
         self.unset_refresh_cookies(response)
 
-    def unset_access_cookies(self,response: Optional[Response] = None) -> None:
+    def unset_access_cookies(self, response: Optional[Response] = None) -> None:
         """
         Remove access token and access CSRF double submit from the response cookies
 
         :param response: The FastAPI response object to delete the access cookies in.
         """
         if not self.jwt_in_cookies:
             raise RuntimeWarning(
                 "unset_access_cookies() called without 'authjwt_token_location' configured to use cookies"
             )
 
-        if response and not isinstance(response,Response):
+        if response and not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
 
         response = response or self._response
 
         response.delete_cookie(
             self._access_cookie_key,
             path=self._access_cookie_path,
-            domain=self._cookie_domain
+            domain=self._cookie_domain,
         )
 
         if self._cookie_csrf_protect:
             response.delete_cookie(
                 self._access_csrf_cookie_key,
                 path=self._access_csrf_cookie_path,
-                domain=self._cookie_domain
+                domain=self._cookie_domain,
             )
 
-    def unset_refresh_cookies(self,response: Optional[Response] = None) -> None:
+    def unset_refresh_cookies(self, response: Optional[Response] = None) -> None:
         """
         Remove refresh token and refresh CSRF double submit from the response cookies
 
         :param response: The FastAPI response object to delete the refresh cookies in.
         """
         if not self.jwt_in_cookies:
             raise RuntimeWarning(
                 "unset_refresh_cookies() called without 'authjwt_token_location' configured to use cookies"
             )
 
-        if response and not isinstance(response,Response):
+        if response and not isinstance(response, Response):
             raise TypeError("The response must be an object response FastAPI")
 
         response = response or self._response
 
         response.delete_cookie(
             self._refresh_cookie_key,
             path=self._refresh_cookie_path,
-            domain=self._cookie_domain
+            domain=self._cookie_domain,
         )
 
         if self._cookie_csrf_protect:
             response.delete_cookie(
                 self._refresh_csrf_cookie_key,
                 path=self._refresh_csrf_cookie_path,
-                domain=self._cookie_domain
+                domain=self._cookie_domain,
             )
 
     def _verify_and_get_jwt_optional_in_cookies(
         self,
-        request: Union[Request,WebSocket],
+        request: Union[Request, WebSocket],
         csrf_token: Optional[str] = None,
     ) -> "AuthJWT":
         """
         Optionally check if cookies have a valid access token. if an access token present in
         cookies, self._token will set. raises exception error when an access token is invalid
         or doesn't match with CSRF token double submit
 
         :param request: for identity get cookies from HTTP or WebSocket
         :param csrf_token: the CSRF double submit token
         """
-        if not isinstance(request,(Request,WebSocket)):
+        if not isinstance(request, (Request, WebSocket)):
             raise TypeError("request must be an instance of 'Request' or 'WebSocket'")
 
         cookie_key = self._access_cookie_key
         cookie = request.cookies.get(cookie_key)
         if not isinstance(request, WebSocket):
             csrf_token = request.headers.get(self._access_csrf_header_name)
 
         if cookie and self._cookie_csrf_protect and not csrf_token:
             if isinstance(request, WebSocket) or request.method in self._csrf_methods:
-                raise CSRFError(status_code=401,message="Missing CSRF Token")
+                raise CSRFError(status_code=401, message="Missing CSRF Token")
 
         # set token from cookie and verify jwt
         self._token = cookie
         self._verify_jwt_optional_in_request(self._token)
 
         decoded_token = self.get_raw_jwt()
 
         if decoded_token and self._cookie_csrf_protect and csrf_token:
             if isinstance(request, WebSocket) or request.method in self._csrf_methods:
-                if 'csrf' not in decoded_token:
-                    raise JWTDecodeError(status_code=422,message="Missing claim: csrf")
-                if not hmac.compare_digest(csrf_token,decoded_token['csrf']):
-                    raise CSRFError(status_code=401,message="CSRF double submit tokens do not match")
+                if "csrf" not in decoded_token:
+                    raise JWTDecodeError(status_code=422, message="Missing claim: csrf")
+                if not hmac.compare_digest(csrf_token, decoded_token["csrf"]):
+                    raise CSRFError(
+                        status_code=401,
+                        message="CSRF double submit tokens do not match",
+                    )
 
     def _verify_and_get_jwt_in_cookies(
         self,
         type_token: str,
-        request: Union[Request,WebSocket],
+        request: Union[Request, WebSocket],
         csrf_token: Optional[str] = None,
         fresh: Optional[bool] = False,
     ) -> "AuthJWT":
         """
         Check if cookies have a valid access or refresh token. if an token present in
         cookies, self._token will set. raises exception error when an access or refresh token
         is invalid or doesn't match with CSRF token double submit
 
         :param type_token: indicate token is access or refresh token
         :param request: for identity get cookies from HTTP or WebSocket
         :param csrf_token: the CSRF double submit token
         :param fresh: check freshness token if True
         """
-        if type_token not in ['access','refresh']:
+        if type_token not in ["access", "refresh"]:
             raise ValueError("type_token must be between 'access' or 'refresh'")
-        if not isinstance(request,(Request,WebSocket)):
+        if not isinstance(request, (Request, WebSocket)):
             raise TypeError("request must be an instance of 'Request' or 'WebSocket'")
 
-        if type_token == 'access':
+        if type_token == "access":
             cookie_key = self._access_cookie_key
             cookie = request.cookies.get(cookie_key)
             if not isinstance(request, WebSocket):
                 csrf_token = request.headers.get(self._access_csrf_header_name)
-        if type_token == 'refresh':
+        if type_token == "refresh":
             cookie_key = self._refresh_cookie_key
             cookie = request.cookies.get(cookie_key)
             if not isinstance(request, WebSocket):
                 csrf_token = request.headers.get(self._refresh_csrf_header_name)
 
         if not cookie:
-            raise MissingTokenError(status_code=401,message="Missing cookie {}".format(cookie_key))
+            raise MissingTokenError(
+                status_code=401, message="Missing cookie {}".format(cookie_key)
+            )
 
         if self._cookie_csrf_protect and not csrf_token:
             if isinstance(request, WebSocket) or request.method in self._csrf_methods:
-                raise CSRFError(status_code=401,message="Missing CSRF Token")
+                raise CSRFError(status_code=401, message="Missing CSRF Token")
 
         # set token from cookie and verify jwt
         self._token = cookie
-        self._verify_jwt_in_request(self._token,type_token,'cookies',fresh)
+        self._verify_jwt_in_request(self._token, type_token, "cookies", fresh)
 
         decoded_token = self.get_raw_jwt()
 
         if self._cookie_csrf_protect and csrf_token:
             if isinstance(request, WebSocket) or request.method in self._csrf_methods:
-                if 'csrf' not in decoded_token:
-                    raise JWTDecodeError(status_code=422,message="Missing claim: csrf")
-                if not hmac.compare_digest(csrf_token,decoded_token['csrf']):
-                    raise CSRFError(status_code=401,message="CSRF double submit tokens do not match")
+                if "csrf" not in decoded_token:
+                    raise JWTDecodeError(status_code=422, message="Missing claim: csrf")
+                if not hmac.compare_digest(csrf_token, decoded_token["csrf"]):
+                    raise CSRFError(
+                        status_code=401,
+                        message="CSRF double submit tokens do not match",
+                    )
 
-    def _verify_jwt_optional_in_request(self,token: str) -> None:
+    def _verify_jwt_optional_in_request(self, token: str) -> None:
         """
         Optionally check if this request has a valid access token
 
         :param token: The encoded JWT
         """
-        if token: self._verifying_token(token)
+        if token:
+            self._verifying_token(token)
 
-        if token and self.get_raw_jwt(token)['type'] != 'access':
-            raise AccessTokenRequired(status_code=422,message="Only access tokens are allowed")
+        if token and self.get_raw_jwt(token)["type"] != "access":
+            raise AccessTokenRequired(
+                status_code=422, message="Only access tokens are allowed"
+            )
 
     def _verify_jwt_in_request(
         self,
         token: str,
         type_token: str,
         token_from: str,
-        fresh: Optional[bool] = False
+        fresh: Optional[bool] = False,
     ) -> None:
         """
         Ensure that the requester has a valid token. this also check the freshness of the access token
 
         :param token: The encoded JWT
         :param type_token: indicate token is access or refresh token
         :param token_from: indicate token from headers cookies, websocket
         :param fresh: check freshness token if True
         """
-        if type_token not in ['access','refresh']:
+        if type_token not in ["access", "refresh"]:
             raise ValueError("type_token must be between 'access' or 'refresh'")
-        if token_from not in ['headers','cookies','websocket']:
-            raise ValueError("token_from must be between 'headers', 'cookies', 'websocket'")
+        if token_from not in ["headers", "cookies", "websocket"]:
+            raise ValueError(
+                "token_from must be between 'headers', 'cookies', 'websocket'"
+            )
 
         if not token:
-            if token_from == 'headers':
-                raise MissingTokenError(status_code=401,message="Missing {} Header".format(self._header_name))
-            if token_from == 'websocket':
-                raise MissingTokenError(status_code=1008,message="Missing {} token from Query or Path".format(type_token))
+            if token_from == "headers":
+                raise MissingTokenError(
+                    status_code=401,
+                    message="Missing {} Header".format(self._header_name),
+                )
+            if token_from == "websocket":
+                raise MissingTokenError(
+                    status_code=1008,
+                    message="Missing {} token from Query or Path".format(type_token),
+                )
 
         # verify jwt
-        issuer = self._decode_issuer if type_token == 'access' else None
-        self._verifying_token(token,issuer)
+        issuer = self._decode_issuer if type_token == "access" else None
+        self._verifying_token(token, issuer)
 
-        if self.get_raw_jwt(token)['type'] != type_token:
+        if self.get_raw_jwt(token)["type"] != type_token:
             msg = "Only {} tokens are allowed".format(type_token)
-            if type_token == 'access':
-                raise AccessTokenRequired(status_code=422,message=msg)
-            if type_token == 'refresh':
-                raise RefreshTokenRequired(status_code=422,message=msg)
+            if type_token == "access":
+                raise AccessTokenRequired(status_code=422, message=msg)
+            if type_token == "refresh":
+                raise RefreshTokenRequired(status_code=422, message=msg)
+
+        if fresh and not self.get_raw_jwt(token)["fresh"]:
+            raise FreshTokenRequired(status_code=401, message="Fresh token required")
 
-        if fresh and not self.get_raw_jwt(token)['fresh']:
-            raise FreshTokenRequired(status_code=401,message="Fresh token required")
+        self._token = token
 
-    def _verifying_token(self,encoded_token: str, issuer: Optional[str] = None) -> None:
+    def _verifying_token(
+        self, encoded_token: str, issuer: Optional[str] = None
+    ) -> None:
         """
         Verified token and check if token is revoked
 
         :param encoded_token: token hash
         :param issuer: expected issuer in the JWT
         """
-        raw_token = self._verified_token(encoded_token,issuer)
-        if raw_token['type'] in self._denylist_token_checks:
+        raw_token = self._verified_token(encoded_token, issuer)
+        if raw_token["type"] in self._denylist_token_checks:
             self._check_token_is_revoked(raw_token)
 
-    def _verified_token(self,encoded_token: str, issuer: Optional[str] = None) -> Dict[str,Union[str,int,bool]]:
+    def _verified_token(
+        self, encoded_token: str, issuer: Optional[str] = None
+    ) -> Dict[str, Union[str, int, bool]]:
         """
         Verified token and catch all error from jwt package and return decode token
 
         :param encoded_token: token hash
         :param issuer: expected issuer in the JWT
 
         :return: raw data from the hash token in the form of a dictionary
         """
         algorithms = self._decode_algorithms or [self._algorithm]
 
         try:
             unverified_headers = self.get_unverified_jwt_headers(encoded_token)
         except Exception as err:
-            raise InvalidHeaderError(status_code=422,message=str(err))
+            raise InvalidHeaderError(status_code=422, message=str(err))
 
         try:
-            secret_key = self._get_secret_key(unverified_headers['alg'],"decode")
+            secret_key = self._get_secret_key(unverified_headers["alg"], "decode")
         except Exception:
             raise
 
         try:
             return jwt.decode(
                 encoded_token,
                 secret_key,
                 issuer=issuer,
                 audience=self._decode_audience,
                 leeway=self._decode_leeway,
-                algorithms=algorithms
+                algorithms=algorithms,
             )
         except Exception as err:
-            raise JWTDecodeError(status_code=422,message=str(err))
+            raise JWTDecodeError(
+                status_code=422,
+                message=str(err),
+                _error_code=self._get_error_code_from_exception(err),
+            )
 
     def jwt_required(
         self,
         auth_from: str = "request",
         token: Optional[str] = None,
         websocket: Optional[WebSocket] = None,
         csrf_token: Optional[str] = None,
@@ -682,28 +734,30 @@
         :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to
                       authorization and get token from Query Url or Path
         :param websocket: an instance of WebSocket, it's required if protected endpoint use a cookie to authorization
         :param csrf_token: the CSRF double submit token. since WebSocket cannot add specifying additional headers
                            its must be passing csrf_token manually and can achieve by Query Url or Path
         """
         if auth_from == "websocket":
-            if websocket: self._verify_and_get_jwt_in_cookies('access',websocket,csrf_token)
-            else: self._verify_jwt_in_request(token,'access','websocket')
+            if websocket:
+                self._verify_and_get_jwt_in_cookies("access", websocket, csrf_token)
+            else:
+                self._verify_jwt_in_request(token, "access", "websocket")
 
         if auth_from == "request":
             if len(self._token_location) == 2:
                 if self._token and self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'access','headers')
+                    self._verify_jwt_in_request(self._token, "access", "headers")
                 if not self._token and self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('access',self._request)
+                    self._verify_and_get_jwt_in_cookies("access", self._request)
             else:
                 if self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'access','headers')
+                    self._verify_jwt_in_request(self._token, "access", "headers")
                 if self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('access',self._request)
+                    self._verify_and_get_jwt_in_cookies("access", self._request)
 
     def jwt_optional(
         self,
         auth_from: str = "request",
         token: Optional[str] = None,
         websocket: Optional[WebSocket] = None,
         csrf_token: Optional[str] = None,
@@ -717,16 +771,18 @@
         :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to
                       authorization and get token from Query Url or Path
         :param websocket: an instance of WebSocket, it's required if protected endpoint use a cookie to authorization
         :param csrf_token: the CSRF double submit token. since WebSocket cannot add specifying additional headers
                            its must be passing csrf_token manually and can achieve by Query Url or Path
         """
         if auth_from == "websocket":
-            if websocket: self._verify_and_get_jwt_optional_in_cookies(websocket,csrf_token)
-            else: self._verify_jwt_optional_in_request(token)
+            if websocket:
+                self._verify_and_get_jwt_optional_in_cookies(websocket, csrf_token)
+            else:
+                self._verify_jwt_optional_in_request(token)
 
         if auth_from == "request":
             if len(self._token_location) == 2:
                 if self._token and self.jwt_in_headers:
                     self._verify_jwt_optional_in_request(self._token)
                 if not self._token and self.jwt_in_cookies:
                     self._verify_and_get_jwt_optional_in_cookies(self._request)
@@ -750,28 +806,30 @@
         :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to
                       authorization and get token from Query Url or Path
         :param websocket: an instance of WebSocket, it's required if protected endpoint use a cookie to authorization
         :param csrf_token: the CSRF double submit token. since WebSocket cannot add specifying additional headers
                            its must be passing csrf_token manually and can achieve by Query Url or Path
         """
         if auth_from == "websocket":
-            if websocket: self._verify_and_get_jwt_in_cookies('refresh',websocket,csrf_token)
-            else: self._verify_jwt_in_request(token,'refresh','websocket')
+            if websocket:
+                self._verify_and_get_jwt_in_cookies("refresh", websocket, csrf_token)
+            else:
+                self._verify_jwt_in_request(token, "refresh", "websocket")
 
         if auth_from == "request":
             if len(self._token_location) == 2:
                 if self._token and self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'refresh','headers')
+                    self._verify_jwt_in_request(self._token, "refresh", "headers")
                 if not self._token and self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('refresh',self._request)
+                    self._verify_and_get_jwt_in_cookies("refresh", self._request)
             else:
                 if self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'refresh','headers')
+                    self._verify_jwt_in_request(self._token, "refresh", "headers")
                 if self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('refresh',self._request)
+                    self._verify_and_get_jwt_in_cookies("refresh", self._request)
 
     def fresh_jwt_required(
         self,
         auth_from: str = "request",
         token: Optional[str] = None,
         websocket: Optional[WebSocket] = None,
         csrf_token: Optional[str] = None,
@@ -783,66 +841,87 @@
         :param token: the encoded JWT, it's required if the protected endpoint use WebSocket to
                       authorization and get token from Query Url or Path
         :param websocket: an instance of WebSocket, it's required if protected endpoint use a cookie to authorization
         :param csrf_token: the CSRF double submit token. since WebSocket cannot add specifying additional headers
                            its must be passing csrf_token manually and can achieve by Query Url or Path
         """
         if auth_from == "websocket":
-            if websocket: self._verify_and_get_jwt_in_cookies('access',websocket,csrf_token,True)
-            else: self._verify_jwt_in_request(token,'access','websocket',True)
+            if websocket:
+                self._verify_and_get_jwt_in_cookies(
+                    "access", websocket, csrf_token, True
+                )
+            else:
+                self._verify_jwt_in_request(token, "access", "websocket", True)
 
         if auth_from == "request":
             if len(self._token_location) == 2:
                 if self._token and self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'access','headers',True)
+                    self._verify_jwt_in_request(self._token, "access", "headers", True)
                 if not self._token and self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('access',self._request,fresh=True)
+                    self._verify_and_get_jwt_in_cookies(
+                        "access", self._request, fresh=True
+                    )
             else:
                 if self.jwt_in_headers:
-                    self._verify_jwt_in_request(self._token,'access','headers',True)
+                    self._verify_jwt_in_request(self._token, "access", "headers", True)
                 if self.jwt_in_cookies:
-                    self._verify_and_get_jwt_in_cookies('access',self._request,fresh=True)
-
-    def get_raw_jwt(self,encoded_token: Optional[str] = None) -> Optional[Dict[str,Union[str,int,bool]]]:
+                    self._verify_and_get_jwt_in_cookies(
+                        "access", self._request, fresh=True
+                    )
+
+    def get_raw_jwt(
+        self, encoded_token: Optional[str] = None
+    ) -> Optional[Dict[str, Union[str, int, bool]]]:
         """
         this will return the python dictionary which has all of the claims of the JWT that is accessing the endpoint.
         If no JWT is currently present, return None instead
 
         :param encoded_token: The encoded JWT from parameter
         :return: claims of JWT
         """
         token = encoded_token or self._token
 
         if token:
             return self._verified_token(token)
         return None
 
-    def get_jti(self,encoded_token: str) -> str:
+    def get_jti(self, encoded_token: str) -> str:
         """
         Returns the JTI (unique identifier) of an encoded JWT
 
         :param encoded_token: The encoded JWT from parameter
         :return: string of JTI
         """
-        return self._verified_token(encoded_token)['jti']
+        return self._verified_token(encoded_token)["jti"]
 
-    def get_jwt_subject(self) -> Optional[Union[str,int]]:
+    def get_jwt_subject(self) -> Optional[Union[str, int]]:
         """
         this will return the subject of the JWT that is accessing this endpoint.
         If no JWT is present, `None` is returned instead.
 
         :return: sub of JWT
         """
         if self._token:
-            return self._verified_token(self._token)['sub']
+            return self._verified_token(self._token)["sub"]
         return None
 
-    def get_unverified_jwt_headers(self,encoded_token: Optional[str] = None) -> dict:
+    def get_unverified_jwt_headers(self, encoded_token: Optional[str] = None) -> dict:
         """
         Returns the Headers of an encoded JWT without verifying the actual signature of JWT
 
         :param encoded_token: The encoded JWT to get the Header from
         :return: JWT header parameters as a dictionary
         """
         encoded_token = encoded_token or self._token
 
         return jwt.get_unverified_header(encoded_token)
+
+    @staticmethod
+    def _get_error_code_from_exception(exception: jwt.exceptions.PyJWTError) -> str:
+        """
+        Generates an error code from an exception name
+
+        :param exception: The exception to generate an error code
+        :return: Generated error code from exception's name
+        """
+        class_name = exception.__class__.__name__.removesuffix("Error")
+        return re.sub(r"(?<!^)(?=[A-Z])", "_", class_name).lower()
```

## ichi_auth/config.py

```diff
@@ -1,34 +1,33 @@
 from datetime import timedelta
 from typing import Optional, Union, Sequence, List
-from pydantic import (
-    BaseModel,
-    validator,
-    StrictBool,
-    StrictInt,
-    StrictStr
-)
+from pydantic import BaseModel, validator, StrictBool, StrictInt, StrictStr
+
 
 class LoadConfig(BaseModel):
-    authjwt_token_location: Optional[Sequence[StrictStr]] = {'headers'}
+    authjwt_token_location: Optional[Sequence[StrictStr]] = {"headers"}
     authjwt_secret_key: Optional[StrictStr] = None
     authjwt_public_key: Optional[StrictStr] = None
     authjwt_private_key: Optional[StrictStr] = None
     authjwt_algorithm: Optional[StrictStr] = "HS256"
     authjwt_decode_algorithms: Optional[List[StrictStr]] = None
-    authjwt_decode_leeway: Optional[Union[StrictInt,timedelta]] = 0
+    authjwt_decode_leeway: Optional[Union[StrictInt, timedelta]] = 0
     authjwt_encode_issuer: Optional[StrictStr] = None
     authjwt_decode_issuer: Optional[StrictStr] = None
-    authjwt_decode_audience: Optional[Union[StrictStr,Sequence[StrictStr]]] = None
+    authjwt_decode_audience: Optional[Union[StrictStr, Sequence[StrictStr]]] = None
     authjwt_denylist_enabled: Optional[StrictBool] = False
-    authjwt_denylist_token_checks: Optional[Sequence[StrictStr]] = {'access','refresh'}
+    authjwt_denylist_token_checks: Optional[Sequence[StrictStr]] = {"access", "refresh"}
     authjwt_header_name: Optional[StrictStr] = "Authorization"
     authjwt_header_type: Optional[StrictStr] = "Bearer"
-    authjwt_access_token_expires: Optional[Union[StrictBool,StrictInt,timedelta]] = timedelta(minutes=15)
-    authjwt_refresh_token_expires: Optional[Union[StrictBool,StrictInt,timedelta]] = timedelta(days=30)
+    authjwt_access_token_expires: Optional[
+        Union[StrictBool, StrictInt, timedelta]
+    ] = timedelta(minutes=15)
+    authjwt_refresh_token_expires: Optional[
+        Union[StrictBool, StrictInt, timedelta]
+    ] = timedelta(days=30)
     # option for create cookies
     authjwt_access_cookie_key: Optional[StrictStr] = "access_token_cookie"
     authjwt_refresh_cookie_key: Optional[StrictStr] = "refresh_token_cookie"
     authjwt_access_cookie_path: Optional[StrictStr] = "/"
     authjwt_refresh_cookie_path: Optional[StrictStr] = "/"
     authjwt_cookie_max_age: Optional[StrictInt] = None
     authjwt_cookie_domain: Optional[StrictStr] = None
@@ -38,48 +37,65 @@
     authjwt_cookie_csrf_protect: Optional[StrictBool] = True
     authjwt_access_csrf_cookie_key: Optional[StrictStr] = "csrf_access_token"
     authjwt_refresh_csrf_cookie_key: Optional[StrictStr] = "csrf_refresh_token"
     authjwt_access_csrf_cookie_path: Optional[StrictStr] = "/"
     authjwt_refresh_csrf_cookie_path: Optional[StrictStr] = "/"
     authjwt_access_csrf_header_name: Optional[StrictStr] = "X-CSRF-Token"
     authjwt_refresh_csrf_header_name: Optional[StrictStr] = "X-CSRF-Token"
-    authjwt_csrf_methods: Optional[Sequence[StrictStr]] = {'POST','PUT','PATCH','DELETE'}
+    authjwt_csrf_methods: Optional[Sequence[StrictStr]] = {
+        "POST",
+        "PUT",
+        "PATCH",
+        "DELETE",
+    }
 
-    @validator('authjwt_access_token_expires')
+    @validator("authjwt_access_token_expires")
     def validate_access_token_expires(cls, v):
         if v is True:
-            raise ValueError("The 'authjwt_access_token_expires' only accept value False (bool)")
+            raise ValueError(
+                "The 'authjwt_access_token_expires' only accept value False (bool)"
+            )
         return v
 
-    @validator('authjwt_refresh_token_expires')
+    @validator("authjwt_refresh_token_expires")
     def validate_refresh_token_expires(cls, v):
         if v is True:
-            raise ValueError("The 'authjwt_refresh_token_expires' only accept value False (bool)")
+            raise ValueError(
+                "The 'authjwt_refresh_token_expires' only accept value False (bool)"
+            )
         return v
 
-    @validator('authjwt_denylist_token_checks', each_item=True)
+    @validator("authjwt_denylist_token_checks", each_item=True)
     def validate_denylist_token_checks(cls, v):
-        if v not in ['access','refresh']:
-            raise ValueError("The 'authjwt_denylist_token_checks' must be between 'access' or 'refresh'")
+        if v not in ["access", "refresh"]:
+            raise ValueError(
+                "The 'authjwt_denylist_token_checks' must be between 'access' or 'refresh'"
+            )
         return v
 
-    @validator('authjwt_token_location', each_item=True)
+    @validator("authjwt_token_location", each_item=True)
     def validate_token_location(cls, v):
-        if v not in ['headers','cookies']:
-            raise ValueError("The 'authjwt_token_location' must be between 'headers' or 'cookies'")
+        if v not in ["headers", "cookies"]:
+            raise ValueError(
+                "The 'authjwt_token_location' must be between 'headers' or 'cookies'"
+            )
         return v
 
-    @validator('authjwt_cookie_samesite')
+    @validator("authjwt_cookie_samesite")
     def validate_cookie_samesite(cls, v):
-        if v not in ['strict','lax','none']:
-            raise ValueError("The 'authjwt_cookie_samesite' must be between 'strict', 'lax', 'none'")
+        if v not in ["strict", "lax", "none"]:
+            raise ValueError(
+                "The 'authjwt_cookie_samesite' must be between 'strict', 'lax', 'none'"
+            )
         return v
 
-    @validator('authjwt_csrf_methods', each_item=True)
+    @validator("authjwt_csrf_methods", each_item=True)
     def validate_csrf_methods(cls, v):
         if v.upper() not in {"GET", "HEAD", "POST", "PUT", "DELETE", "PATCH"}:
-            raise ValueError("The 'authjwt_csrf_methods' must be between http request methods")
+            raise ValueError(
+                "The 'authjwt_csrf_methods' must be between http request methods"
+            )
         return v.upper()
 
     class Config:
         min_anystr_length = 1
         anystr_strip_whitespace = True
```

## ichi_auth/exceptions.py

```diff
@@ -1,72 +1,77 @@
 class AuthJWTException(Exception):
     """
     Base except which all fastapi_jwt_auth errors extend
     """
-    pass
+
+    def __init__(self, status_code: int, message: str, _error_code: str = ""):
+        self.status_code = status_code
+        self.message = message
+        if _error_code:
+            self.error_code = _error_code
+
 
 class InvalidHeaderError(AuthJWTException):
     """
     An error getting jwt in header or jwt header information from a request
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "invalid_header"
+
 
 class JWTDecodeError(AuthJWTException):
     """
     An error decoding a JWT
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "token_decode_failed"
+
 
 class CSRFError(AuthJWTException):
     """
     An error with CSRF protection
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "csrf_error"
+
 
 class MissingTokenError(AuthJWTException):
     """
     Error raised when token not found
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "missing_token"
+
 
 class RevokedTokenError(AuthJWTException):
     """
     Error raised when a revoked token attempt to access a protected endpoint
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "revoked_token"
+
 
 class AccessTokenRequired(AuthJWTException):
     """
     Error raised when a valid, non-access JWT attempt to access an endpoint
     protected by jwt_required, jwt_optional, fresh_jwt_required
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "access_token_required"
+
 
 class RefreshTokenRequired(AuthJWTException):
     """
     Error raised when a valid, non-refresh JWT attempt to access an endpoint
     protected by jwt_refresh_token_required
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "refresh_token_required"
+
 
 class FreshTokenRequired(AuthJWTException):
     """
     Error raised when a valid, non-fresh JWT attempt to access an endpoint
     protected by fresh_jwt_required
     """
-    def __init__(self,status_code: int, message: str):
-        self.status_code = status_code
-        self.message = message
+
+    error_code = "fresh_token_required"
```

## Comparing `ichi_auth-1.0.post1.dist-info/LICENSE` & `ichi_auth-1.1.dist-info/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MIT License
 
 Copyright (c) 2020 Nyoman Pradipta Dewantara
-Copyright (c) 2022 Avery García
+Copyright (c) 2022-present aveeryy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `ichi_auth-1.0.post1.dist-info/METADATA` & `ichi_auth-1.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ichi-auth
-Version: 1.0.post1
+Version: 1.1
 Summary: FastAPI extension that provides JWT Auth support (secure, easy to use and lightweight)
-Author-email: Nyoman Pradipta Dewantara <nyomanpradipta120@gmail.com>, Avery García <aveeryy@protonmail.com>
+Author-email: Nyoman Pradipta Dewantara <nyomanpradipta120@gmail.com>, aveeryy <aveeryy@protonmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 Requires-Dist: mkdocs>=1.1.2,<2.0.0 ; extra == "doc"
 Requires-Dist: mkdocs-material>=5.5.0,<6.0.0 ; extra == "doc"
 Requires-Dist: markdown-include>=0.5.1,<0.6.0 ; extra == "doc"
 Requires-Dist: pytest==6.2.5 ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
 Requires-Dist: coveralls==3.3.1 ; extra == "test"
 Requires-Dist: httpx==0.23.0 ; extra == "test"
-Project-URL: Source, https://codeberg.org/ichi/auth
+Project-URL: Home, https://codeberg.org/ichi/auth
 Provides-Extra: asymmetric
 Provides-Extra: dev
 Provides-Extra: doc
 Provides-Extra: test
 
 <h1 align="left" style="margin-bottom: 20px; font-weight: 500; font-size: 50px; color: black;">
   ichi Auth
```

### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: ichi-auth Version: 1.0.post1 Summary: FastAPI
-extension that provides JWT Auth support (secure, easy to use and lightweight)
-Author-email: Nyoman Pradipta Dewantara
-gmail.com>, Avery GarcÃ­a
+Metadata-Version: 2.1 Name: ichi-auth Version: 1.1 Summary: FastAPI extension
+that provides JWT Auth support (secure, easy to use and lightweight) Author-
+email: Nyoman Pradipta Dewantara
+gmail.com>, aveeryy
 protonmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 MIT License Classifier: Operating System :: OS Independent Classifier: Topic ::
@@ -14,15 +14,15 @@
 Requires-Dist: PyJWT>=2.6.0 Requires-Dist: cryptography>=38.0.3 ; extra ==
 "asymmetric" Requires-Dist: cryptography>=38.0.3 ; extra == "dev" Requires-
 Dist: uvicorn>=0.19.0 ; extra == "dev" Requires-Dist: mkdocs>=1.1.2,<2.0.0 ;
 extra == "doc" Requires-Dist: mkdocs-material>=5.5.0,<6.0.0 ; extra == "doc"
 Requires-Dist: markdown-include>=0.5.1,<0.6.0 ; extra == "doc" Requires-Dist:
 pytest==6.2.5 ; extra == "test" Requires-Dist: pytest-cov==4.0.0 ; extra ==
 "test" Requires-Dist: coveralls==3.3.1 ; extra == "test" Requires-Dist:
-httpx==0.23.0 ; extra == "test" Project-URL: Source, https://codeberg.org/ichi/
+httpx==0.23.0 ; extra == "test" Project-URL: Home, https://codeberg.org/ichi/
 auth Provides-Extra: asymmetric Provides-Extra: dev Provides-Extra: doc
 Provides-Extra: test
 ****** ichi Auth ******
 A fork of [fastapi-jwt-auth]() with updated dependencies --- **Documentation**:
 https://indominusbyte.github.io/fastapi-jwt-auth **Source Code**: https://
 codeberg.org/ichi/ichi-auth --- ## Features FastAPI extension that provides JWT
 Auth support (secure, easy to use and lightweight), if you were familiar with
```

