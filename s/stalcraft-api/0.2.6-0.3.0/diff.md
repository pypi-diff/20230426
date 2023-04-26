# Comparing `tmp/stalcraft_api-0.2.6.tar.gz` & `tmp/stalcraft_api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stalcraft_api-0.2.6.tar", max compression
+gzip compressed data, was "stalcraft_api-0.3.0.tar", max compression
```

## Comparing `stalcraft_api-0.2.6.tar` & `stalcraft_api-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 stalcraft_api-0.2.6/LICENSE
--rw-r--r--   0        0        0      409 2023-02-25 03:03:22.033108 stalcraft_api-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     6879 2023-02-23 09:30:39.987919 stalcraft_api-0.2.6/README.md
--rw-r--r--   0        0        0      298 2023-02-25 02:48:01.952910 stalcraft_api-0.2.6/stalcraft/__init__.py
--rw-r--r--   0        0        0     5401 2023-02-25 02:08:22.331185 stalcraft_api-0.2.6/stalcraft/api.py
--rw-r--r--   0        0        0     2539 2023-02-25 02:41:57.584275 stalcraft_api-0.2.6/stalcraft/auction.py
--rw-r--r--   0        0        0     3361 2023-02-25 02:30:24.009406 stalcraft_api-0.2.6/stalcraft/auth.py
--rw-r--r--   0        0        0     1287 2023-02-25 02:47:17.110836 stalcraft_api-0.2.6/stalcraft/clan.py
--rw-r--r--   0        0        0     6463 2023-02-25 02:47:56.401063 stalcraft_api-0.2.6/stalcraft/client.py
--rw-r--r--   0        0        0    94824 2023-02-23 06:28:27.723539 stalcraft_api-0.2.6/stalcraft/data/global/listing.json
--rw-r--r--   0        0        0   125939 2023-02-23 06:27:39.330539 stalcraft_api-0.2.6/stalcraft/data/ru/listing.json
--rw-r--r--   0        0        0     1045 2023-02-25 02:06:39.991922 stalcraft_api-0.2.6/stalcraft/enums.py
--rw-r--r--   0        0        0      491 2023-02-23 05:15:25.967229 stalcraft_api-0.2.6/stalcraft/exceptions.py
--rw-r--r--   0        0        0     3714 2023-02-25 02:50:17.626171 stalcraft_api-0.2.6/stalcraft/item.py
--rw-r--r--   0        0        0     5055 2023-02-25 02:53:15.666550 stalcraft_api-0.2.6/stalcraft/schemas.py
--rw-r--r--   0        0        0     7602 1970-01-01 00:00:00.000000 stalcraft_api-0.2.6/setup.py
--rw-r--r--   0        0        0     6960 1970-01-01 00:00:00.000000 stalcraft_api-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-01-22 13:34:34.609366 stalcraft_api-0.3.0/LICENSE
+-rw-r--r--   0        0        0      431 2023-04-26 09:32:06.330121 stalcraft_api-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3353 2023-04-26 09:29:26.774897 stalcraft_api-0.3.0/README.md
+-rw-r--r--   0        0        0      289 2023-04-26 09:05:23.436219 stalcraft_api-0.3.0/stalcraft/__init__.py
+-rw-r--r--   0        0        0     5399 2023-04-26 09:53:49.044276 stalcraft_api-0.3.0/stalcraft/api.py
+-rw-r--r--   0        0        0     2555 2023-04-26 08:59:28.501525 stalcraft_api-0.3.0/stalcraft/auction.py
+-rw-r--r--   0        0        0     3888 2023-04-26 09:05:30.070547 stalcraft_api-0.3.0/stalcraft/auth.py
+-rw-r--r--   0        0        0     1305 2023-04-26 08:59:34.363385 stalcraft_api-0.3.0/stalcraft/clan.py
+-rw-r--r--   0        0        0     6089 2023-04-26 09:02:32.651612 stalcraft_api-0.3.0/stalcraft/client.py
+-rw-r--r--   0        0        0   123829 2023-04-26 08:57:44.310351 stalcraft_api-0.3.0/stalcraft/data/global/listing.json
+-rw-r--r--   0        0        0   124333 2023-04-26 08:56:18.025262 stalcraft_api-0.3.0/stalcraft/data/ru/listing.json
+-rw-r--r--   0        0        0     1045 2023-02-25 02:06:39.991922 stalcraft_api-0.3.0/stalcraft/enums.py
+-rw-r--r--   0        0        0      491 2023-02-23 05:15:25.967229 stalcraft_api-0.3.0/stalcraft/exceptions.py
+-rw-r--r--   0        0        0     3712 2023-04-26 09:00:14.014452 stalcraft_api-0.3.0/stalcraft/item.py
+-rw-r--r--   0        0        0     4433 2023-04-26 09:53:08.796220 stalcraft_api-0.3.0/stalcraft/schemas.py
+-rw-r--r--   0        0        0     4092 1970-01-01 00:00:00.000000 stalcraft_api-0.3.0/setup.py
+-rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 stalcraft_api-0.3.0/PKG-INFO
```

### Comparing `stalcraft_api-0.2.6/LICENSE` & `stalcraft_api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stalcraft_api-0.2.6/stalcraft/api.py` & `stalcraft_api-0.3.0/stalcraft/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Any, Dict, Literal
-from dataclasses import dataclass
 from requests import Response
 from datetime import datetime
-import requests
-import base64
+from dataclasses import dataclass
 import pytz
 import json
+import base64
+import requests
 
 from . import BaseUrl
 from .enums import StatusCode
 
 from .exceptions import (
-    InvalidToken, StalcraftApiException, InvalidParameter, Unauthorised, NotFound, RateLimitException
+    InvalidToken, StalcraftApiException,
+    InvalidParameter, Unauthorised, NotFound, RateLimitException
 )
 
 
 @dataclass
 class RateLimit:
     limit: int
     remaining: int
@@ -48,29 +49,29 @@
 
     def _handle_response_status(self, response: Response, url: str, payload: Dict[str, Any]) -> Response:
         """
         Match response status_code
         """
 
         match response.status_code:
+            case StatusCode.OK.value:
+                return response
+
             case StatusCode.INVALID_PARAMETER.value:
                 raise InvalidParameter(f"One of parameters is invalid: url='{url}' payload={payload}")
 
             case StatusCode.UNAUTHORISED.value:
                 raise Unauthorised("Bad token or client_id and client_secret")
 
             case StatusCode.NOT_FOUND.value:
                 raise NotFound(f"Not Found: url='{url}' payload={payload}")
 
             case StatusCode.RATE_LIMIT.value:
                 raise RateLimitException(f"Too Many Requests: url='{url}' payload={payload}")
 
-            case StatusCode.OK.value:
-                return response
-
             case _:
                 raise StalcraftApiException(response)
 
     def _update_rate_limit(self, response):
         """
         Updates rate limit property
         """
@@ -90,15 +91,14 @@
     def _request(self, method: str, payload: Dict[str, Any]={}) -> Any:
         """
         Makes request to Stalcraft API
         """
 
         url = f"{self._base_url}/{method}"
 
-
         response = self._get_response(url, payload)
         response = self._handle_response_status(response, url, payload)
 
         self._update_rate_limit(response)
 
         return response.json()
 
@@ -106,15 +106,15 @@
         """
         Validate offset and limit values
         """
 
         assert offset >= 0, f"offset should be >= 0, got {offset}"
         assert limit in range(0, 101), f"limit should be between 0 and 100, got {limit}"
 
-    def __repr__(self):
+    def __str__(self):
         return f"base_url='{self._base_url}'"
 
 
 class TokenApi(BaseApi):
     def __init__(self, token: str, base_url: BaseUrl | str):
         super().__init__(base_url)
 
@@ -156,16 +156,16 @@
 
         if payload is False:
             raise InvalidToken(f"Invalid token provided: '{self.part_of_token}'")
 
         self.token_payload = payload
         return payload
 
-    def __repr__(self):
-        return f"{super().__repr__()} token='{self.part_of_token}'"
+    def __str__(self):
+        return f"{super().__str__()} token='{self.part_of_token}'"
 
 
 class SecretApi(BaseApi):
     def __init__(self, client_id: str, client_secret: str, base_url: BaseUrl | str):
         super().__init__(base_url)
 
         self.client_id = client_id
@@ -179,9 +179,9 @@
     def headers(self):
         return {
             "Client-Id": self.client_id,
             "Client-Secret": self.client_secret,
             "Content-Type": "application/json"
         }
 
-    def __repr__(self):
-        return f"{super().__repr__()} client_id='{self.client_id}' client_secret='{self.part_of_secret}'"
+    def __str__(self):
+        return f"{super().__str__()} client_id='{self.client_id}' client_secret='{self.part_of_secret}'"
```

### Comparing `stalcraft_api-0.2.6/stalcraft/auction.py` & `stalcraft_api-0.3.0/stalcraft/auction.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         payload = {"offset": offset, "limit": limit, "additional": additional}
         response = self._api._request(method, payload)
 
         if self.json is True:
             return response
 
         return [
-            schemas.Price(price)
+            schemas.Price.parse_obj(price)
             for price in response['prices']
         ]
 
     def lots(self, offset=0, limit=20, sort=Sort.TIME_CREATED, order=Order.ASCENDING, additional=False):
         """
         Returns list of currently active lots on the auction for the given item.
         Lots are sorted based on given parameter.
@@ -55,13 +55,13 @@
         payload = {"offset": offset, "limit": limit, "sort": sort.value, "order": order.value, "additional": additional}
         response = self._api._request(method, payload)
 
         if self.json is True:
             return response
 
         return [
-            schemas.Lot(lots)
-            for lots in response['lots']
+            schemas.Lot.parse_obj(lot)
+            for lot in response['lots']
         ]
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}> {self._api.__repr__()} item_id='{self.item_id}' region='{self.region}'"
+    def __str__(self):
+        return f"<{self.__class__.__name__}> {self._api.__str__()} item_id='{self.item_id}' region='{self.region}'"
```

### Comparing `stalcraft_api-0.2.6/stalcraft/auth.py` & `stalcraft_api-0.3.0/stalcraft/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 import requests
 
+from . import schemas
+
 
 class Authorization:
     AUTHORIZE_URL = "https://exbo.net/oauth/authorize"
     TOKEN_URL = "https://exbo.net/oauth/token"
     USER_URL = "https://exbo.net/oauth/user"
 
-    def __init__(self, client_id: str, client_secret: str, scope="", redirect_uri="http://localhost"):
+    def __init__(self, client_id: str, client_secret: str, scope="", redirect_uri="http://localhost", json=True):
         """
         Constructor for Authorization.
 
         Args:
             client_id: OAuth2 client ID
             client_secret: OAuth2 client secret
             scope (optional): Authorization scope requested by the client. Defaults to ""
             redirect_uri (optional): URI to redirect the user to after authorization. Defaults to "http://localhost"
+            json (optional): if True response returned in raw format. Defaults to True
         """
 
         self.client_id = client_id
         self.client_secret = client_secret
         self.scope = scope
         self.redirect_uri = redirect_uri
+        self.json = json
 
         self.code = ""
 
-    def get_user_code(self):
+    @property
+    def user_code_url(self):
         """
         Returns the URL that a user should visit to authorize the application.
         """
 
         return f"{self.AUTHORIZE_URL}?client_id={self.client_id}&redirect_uri={self.redirect_uri}&scope={self.scope}&response_type=code"
 
     def input_code(self):
@@ -47,33 +52,39 @@
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "code": self.code,
             "grant_type": "authorization_code",
             "redirect_uri": self.redirect_uri
         }
 
-        response = requests.post(self.TOKEN_URL, data=data)
+        response = requests.post(self.TOKEN_URL, data=data).json()
 
-        return response.json()
+        if self.json is True:
+            return response
+
+        return schemas.UserToken.parse_obj(response)
 
     def get_app_token(self):
         """
         Returns an OAuth2 token for the application, using the client credentials.
         """
 
         data = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "grant_type": "client_credentials",
             "scope": self.scope
         }
 
-        response = requests.post(self.TOKEN_URL, data=data)
+        response = requests.post(self.TOKEN_URL, data=data).json()
 
-        return response.json()
+        if self.json is True:
+            return response
+
+        return schemas.AppToken.parse_obj(response)
 
     def update_token(self, refresh_token: str):
         """
         Returns a new OAuth2 token using a refresh token.
 
         Args:
             refresh_token: The refresh token to use
@@ -85,27 +96,33 @@
             "grant_type": "refresh_token",
             "refresh_token": refresh_token,
             "scope": self.scope
         }
 
         response = requests.post(self.TOKEN_URL, data=data)
 
-        return response.json()
+        if self.json is True:
+            return response
+
+        return schemas.UserToken.parse_obj(response)
 
     def info(self, token: str):
         """
         Returns user information associated with the provided access token.
 
         Args:
             token: User access token
         """
 
         headers = {
             "Authorization": f"Bearer {token}"
         }
 
-        response = requests.get(self.USER_URL, headers=headers)
+        response = requests.get(self.USER_URL, headers=headers).json()
+
+        if self.json is True:
+            return response
 
-        return response.json()
+        return schemas.TokenInfo.parse_obj(response)
 
-    def __repr__(self):
-        return f"{super().__repr__()} client_id='{self.client_id}' redirect_uri='{self.redirect_uri}'"
+    def __str__(self):
+        return f"<{self.__class__.__name__}> client_id='{self.client_id}' redirect_uri='{self.redirect_uri}'"
```

### Comparing `stalcraft_api-0.2.6/stalcraft/clan.py` & `stalcraft_api-0.3.0/stalcraft/clan.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
         method = f"{self.region.value}/clan/{self.clan_id}/info"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
-        return schemas.ClanInfo(response)
+        return schemas.ClanInfo.parse_obj(response)
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}> {self._api.__repr__()} clan_id='{self.clan_id}' region='{self.region}'"
+    def __str__(self):
+        return f"<{self.__class__.__name__}> {self._api.__str__()} clan_id='{self.clan_id}' region='{self.region}'"
 
 
 class UserClan(Clan):
     def members(self):
         """
         Returns list of members in the given clan.
 
@@ -37,10 +37,10 @@
         method = f"{self.region.value}/clan/{self.clan_id}/members"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
         return [
-            schemas.ClanMember(member)
+            schemas.ClanMember.parse_obj(member)
             for member in response
         ]
```

### Comparing `stalcraft_api-0.2.6/stalcraft/client.py` & `stalcraft_api-0.3.0/stalcraft/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import Auction, BaseUrl, Clan, LocalItem, Region, SecretApi, TokenApi, UserClan, WebItem
+from . import TokenApi, SecretApi, Auction, Clan, UserClan, BaseUrl, Region, LocalItem, WebItem
 from . import schemas
 
 
 class Client:
     def __init__(
         self,
         token: str | None = None,
@@ -38,15 +38,15 @@
         method = "regions"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
         return [
-            schemas.RegionInfo(region)
+            schemas.RegionInfo.parse_obj(region)
             for region in response
         ]
 
     def emission(self, region=Region.RU):
         """
         Returns information about current emission, if any, and recorded time of the previous one.
 
@@ -56,15 +56,15 @@
 
         method = f"{region.value}/emission"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
-        return schemas.Emission(response)
+        return schemas.Emission.parse_obj(response)
 
     def clans(self, offset=0, limit=20, region=Region.RU):
         """
         Returns all clans which are currently registered in the game on specified region.
 
         Args:
             offset: Amount of clans in list to skip. Defaults to 0
@@ -78,15 +78,15 @@
         payload = {"offset": offset, "limit": limit}
         response = self._api._request(method, payload)
 
         if self.json is True:
             return response
 
         return [
-            schemas.ClanInfo(clan)
+            schemas.ClanInfo.parse_obj(clan)
             for clan in response['data']
         ]
 
     def auction(self, item_id: str | LocalItem | WebItem, region=Region.RU):
         """
         Factory method for working with auction.
 
@@ -109,71 +109,55 @@
 
         method = f"{region.value}/character/by-name/{character}/profile"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
-        return schemas.CharacterProfile(response)
+        return schemas.CharacterProfile.parse_obj(response)
 
-    def __repr__(self):
-        return f"<{self.__class__.__name__}> {self._api.__repr__()}"
+    def __str__(self):
+        return f"<{self.__class__.__name__}> {self._api.__str__()}"
 
 
 class AppClient(Client):
-    def __init__(
-        self,
-        token: str | None = None,
-        client_id: str | None = None,
-        client_secret: str | None = None,
-        base_url: BaseUrl | str = BaseUrl.PRODUCTION,
-        json = False
-    ):
-        """
-        App Client for working with the API.
-
-        Args:
-            token: App access token for authorization
-            client_id: Application ID for authorization
-            client_secret: Application secret for authorization
-            base_url (optional): API base URL. Defaults to PRODUCTION
-            json (optional): if True response returned in raw format. Defaults to False
-        """
-
-        super().__init__(token, client_id, client_secret, base_url, json)
+    """
+    App Client for working with the API.
 
+    Args:
+        token: App access token for authorization
+        client_id: Application ID for authorization
+        client_secret: Application secret for authorization
+        base_url (optional): API base URL. Defaults to PRODUCTION
+        json (optional): if True response returned in raw format. Defaults to False
+    """
 
     def clan(self, clan_id: str, region=Region.RU):
         """
         Factory method for working with clans.
 
         Args:
             clan_id: Clan ID. For example "647d6c53-b3d7-4d30-8d08-de874eb1d845"
             region: Stalcraft region. Defaults to RU
         """
 
         return Clan(self._api, clan_id, region, self.json)
 
 
 class UserClient(Client):
-    def __init__(
-        self,
-        token: str,
-        base_url: BaseUrl | str = BaseUrl.PRODUCTION,
-        json = False
-    ):
-        """
-        User Client for working with the API.
+    """
+    User Client for working with the API.
 
-        Args:
-            token: User access token for authorization
-            base_url (optional): API base URL. Defaults to PRODUCTION
-            json (optional): if True response returned in raw format. Defaults to False
-        """
+    Args:
+        token: User access token for authorization
+        base_url (optional): API base URL. Defaults to PRODUCTION
+        json (optional): if True response returned in raw format. Defaults to False
+    """
 
+    def __init__(self, token: str, base_url: BaseUrl | str = BaseUrl.PRODUCTION, json = False):
         super().__init__(token=token, base_url=base_url, json=json)
 
     def characters(self, region=Region.RU):
         """
         Returns list of characters created by the user by which used access token was provided.
 
         Args:
@@ -183,15 +167,15 @@
         method = f"{region.value}/characters"
         response = self._api._request(method)
 
         if self.json is True:
             return response
 
         return [
-            schemas.Character(character)
+            schemas.Character.parse_obj(character)
             for character in response
         ]
 
     def friends(self, character: str, region=Region.RU):
         """
         Returns list of character names who are friend with specified character.
```

### Comparing `stalcraft_api-0.2.6/stalcraft/data/global/listing.json` & `stalcraft_api-0.3.0/stalcraft/data/global/listing.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7135152284263959%*

 * *Differences: {"'00959'": "{'en': 'devils nettle'}",*

 * * "'0r52r'": "OrderedDict([('ru', 'ветка рябины'), ('en', 'rowan branch')])",*

 * * "'0r631'": "OrderedDict([('ru', 'камуфляж спектр - почва'), ('en', 'specterdirt camouflage')])",*

 * * "'0r6jk'": "OrderedDict([('ru', 'оружейная краска розовая'), ('en', 'pink weapon paint')])",*

 * * "'0r6pd'": "OrderedDict([('ru', 'камуфляж volumehex dune'), ('en', 'volumehex dune camouflage')])",*

 * * "'0r6vd'": "OrderedDict([('ru', 'камуфляж erdl arvn sv'), ('en', 'erdl arvn sv camouflage')])",*

 * * "'0rp […]*

```diff
@@ -1,10 +1,10 @@
 {
     "00959": {
-        "en": "devil\u2019s nettle",
+        "en": "devils nettle",
         "ru": "\u0434\u044c\u044f\u0432\u043e\u043b\u044c\u0441\u043a\u0430\u044f \u043a\u0440\u0430\u043f\u0438\u0432\u0430"
     },
     "009n9": {
         "en": "burning crappite",
         "ru": "\u043f\u043e\u043b\u044b\u0445\u0430\u044e\u0449\u0438\u0439 \u0441\u0440\u0430\u0447\u043d\u0438\u043a"
     },
     "009o9": {
@@ -15,18 +15,14 @@
         "en": "game bag",
         "ru": "\u044f\u0433\u0434\u0442\u0430\u0448"
     },
     "0o01": {
         "en": "gauss rifle charger",
         "ru": "\u0430\u043a\u043a\u0443\u043c\u0443\u043b\u044f\u0442\u043e\u0440 \u0434\u043b\u044f \u0433\u0430\u0443\u0441\u0441-\u043f\u0443\u0448\u043a\u0438"
     },
-    "0o9d": {
-        "en": "5.56 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "0or1": {
         "en": "12 caliber live ammo",
         "ru": "\u0431\u043e\u0435\u0432\u0430\u044f \u043f\u0443\u043b\u044f 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "0r211": {
         "en": "crye precision six12",
         "ru": "crye precision six12"
@@ -51,33 +47,53 @@
         "en": "worn ah-3 seeker suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "0r4q9": {
         "en": "mis-113 iolite",
         "ru": "\u043a\u0438\u043c-113 \u0438\u043e\u043b\u0438\u0442"
     },
+    "0r52r": {
+        "en": "rowan branch",
+        "ru": "\u0432\u0435\u0442\u043a\u0430 \u0440\u044f\u0431\u0438\u043d\u044b"
+    },
+    "0r631": {
+        "en": "specterdirt camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440 - \u043f\u043e\u0447\u0432\u0430"
+    },
+    "0r6jk": {
+        "en": "pink weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0440\u043e\u0437\u043e\u0432\u0430\u044f"
+    },
+    "0r6pd": {
+        "en": "volumehex dune camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex dune"
+    },
+    "0r6vd": {
+        "en": "erdl arvn sv camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn sv"
+    },
     "0rdld": {
         "en": "3rd class thermoblock",
         "ru": "\u0442\u0435\u0440\u043c\u043e\u0431\u0430\u0440\u044c\u0435\u0440 \u0442\u0440\u0435\u0442\u044c\u0435\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "0rn7d": {
         "en": "vanguard armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u0432\u0430\u043d\u0433\u0430\u0440\u0434"
     },
     "0rnw1": {
         "en": "mis-102 zircon",
         "ru": "\u043a\u0438\u043c-102 \u0446\u0438\u0440\u043a\u043e\u043d"
     },
     "0rp3y": {
-        "en": "5.56 pufgun clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 pufgun, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 pufgun clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 pufgun \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "0rpqy": {
-        "en": "7.62 plastic clip",
-        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62"
+        "en": "762 plastic clip",
+        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762"
     },
     "0rq2k": {
         "en": "ice pick",
         "ru": "\u043b\u0435\u0434\u043e\u0440\u0443\u0431"
     },
     "0rqkk": {
         "en": "fiery greeting",
@@ -95,14 +111,38 @@
         "en": "b-21m handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-21\u043c"
     },
     "0rv99": {
         "en": "springfield m1a pacs stock",
         "ru": "\u043b\u043e\u0436\u0435 springfield m1a pacs"
     },
+    "0rydr": {
+        "en": "chaplain",
+        "ru": "\u043a\u0430\u043f\u0435\u043b\u043b\u0430\u043d"
+    },
+    "0ryly": {
+        "en": "specterdirt camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440 - \u043f\u043e\u0447\u0432\u0430"
+    },
+    "0rymk": {
+        "en": "erdl arvn sv camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn sv"
+    },
+    "0ryor": {
+        "en": "martyr",
+        "ru": "\u043c\u0443\u0447\u0435\u043d\u0438\u043a"
+    },
+    "0ryw9": {
+        "en": "manly pink armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043c\u0443\u0436\u0435\u0441\u0442\u0432\u0435\u043d\u043d\u044b\u0439 \u0440\u043e\u0437\u043e\u0432\u044b\u0439"
+    },
+    "0ryyk": {
+        "en": "volumehex dune camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex dune"
+    },
     "12dq": {
         "en": "m381 grenade round",
         "ru": "\u0432\u044b\u0441\u0442\u0440\u0435\u043b \u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442\u043d\u044b\u0439 m381"
     },
     "12r1": {
         "en": "mbss backpack",
         "ru": "\u0440\u044e\u043a\u0437\u0430\u043a mbss"
@@ -139,69 +179,93 @@
         "en": "crystal thorn",
         "ru": "\u043a\u0440\u0438\u0441\u0442\u0430\u043b\u044c\u043d\u0430\u044f \u043a\u043e\u043b\u044e\u0447\u043a\u0430"
     },
     "1kv2": {
         "en": "gravi",
         "ru": "\u0433\u0440\u0430\u0432\u0438"
     },
-    "1n16": {
-        "en": "12 caliber silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "1n91": {
-        "en": "7.62 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c"
+        "en": "762 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c"
     },
     "1nr1": {
         "en": "9 mm armor-piercing ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "1p2r": {
         "en": "kzs-3u",
         "ru": "\u043a\u0437\u0441-3\u0443"
     },
     "1r1j6": {
         "en": "m203",
         "ru": "m203"
     },
     "1r2l6": {
-        "en": "\u201castrixin\u201d",
+        "en": "astrixin",
         "ru": "\u0430\u0441\u0442\u0440\u0438\u043a\u0446\u0438\u043d"
     },
     "1r2o6": {
         "en": "scientific first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u043d\u0430\u0443\u0447\u043d\u0430\u044f"
     },
     "1r351": {
         "en": "ris bracket-rail",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d-\u043f\u043b\u0430\u043d\u043a\u0430 ris"
     },
     "1r362": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "1r39q": {
-        "en": "akademia t\u2019ma flash suppressor",
+        "en": "akademia tma flash suppressor",
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c akademia \u0442\u044c\u043c\u0430"
     },
     "1r3j2": {
-        "en": "7.62x39 drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62x39"
+        "en": "762x39 drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762x39"
     },
     "1r3rq": {
         "en": "diamondhead compensator",
         "ru": "diamondhead compensator"
     },
     "1r3vr": {
-        "en": "protective rail, khaki",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0445\u0430\u043a\u0438"
+        "en": "protective rail khaki",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0445\u0430\u043a\u0438"
+    },
+    "1r62q": {
+        "en": "dead anarchist",
+        "ru": "\u043c\u0435\u0440\u0442\u0432\u044b\u0439 \u0430\u043d\u0430\u0440\u0445\u0438\u0441\u0442"
+    },
+    "1r66r": {
+        "en": "dpm oj camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm oj"
+    },
+    "1r6dr": {
+        "en": "m90 threat camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 threat"
+    },
+    "1r6l2": {
+        "en": "tempest camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0440\u044f"
+    },
+    "1r6mr": {
+        "en": "a-tacs au camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs au"
+    },
+    "1r6o2": {
+        "en": "bhutancliff edge camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043a\u0430\u043b\u0438\u0441\u0442\u044b\u0439 \u0431\u0435\u0440\u0435\u0433"
+    },
+    "1r6pq": {
+        "en": "prototype",
+        "ru": "\u043f\u0440\u043e\u0442\u043e\u0442\u0438\u043f"
     },
     "1r731": {
-        "en": "kbk wz. 88 tantal",
-        "ru": "kbk wz. 88 tantal"
+        "en": "kbk wz 88 tantal",
+        "ru": "kbk wz 88 tantal"
     },
     "1r742": {
         "en": "bm-16",
         "ru": "\u0431\u043c-16"
     },
     "1r756": {
         "en": "viper",
@@ -220,47 +284,55 @@
         "ru": "\u043f\u043c"
     },
     "1r7g1": {
         "en": "steyr aug a3",
         "ru": "steyr aug a3"
     },
     "1r7rg": {
-        "en": "mosin\u2019s carbine",
+        "en": "mosins carbine",
         "ru": "\u043a\u0430\u0440\u0430\u0431\u0438\u043d \u043c\u043e\u0441\u0438\u043d\u0430"
     },
     "1r7v1": {
         "en": "imi mini uzi",
         "ru": "imi mini uzi"
     },
     "1rd56": {
         "en": "aks-74",
         "ru": "\u0430\u043a\u0441-74"
     },
+    "1rd6r": {
+        "en": "hellish inferno",
+        "ru": "\u0430\u0434\u0441\u043a\u043e\u0435 \u043f\u0435\u043a\u043b\u043e"
+    },
+    "1rddr": {
+        "en": "otl-3 thug",
+        "ru": "\u0433\u043e\u043b\u043e\u0432\u043e\u0440\u0435\u0437 \u043e\u0442\u043b-3"
+    },
     "1rdg6": {
         "en": "hk mp5",
         "ru": "hk mp5"
     },
     "1rdnq": {
         "en": "dp",
         "ru": "\u0434\u043f"
     },
     "1rj7r": {
         "en": "project 6x4",
         "ru": "\u0438\u0437\u0434\u0435\u043b\u0438\u0435 6\u04454"
     },
     "1rj9g": {
-        "en": "eternal novice\u2019s pm",
+        "en": "eternal novices pm",
         "ru": "\u043f\u043c \u0432\u0435\u0447\u043d\u043e\u0433\u043e \u043d\u043e\u0432\u0438\u0447\u043a\u0430"
     },
     "1rjjr": {
         "en": "old sickle",
         "ru": "\u0441\u0442\u0430\u0440\u044b\u0439 \u0441\u0435\u0440\u043f"
     },
     "1rjqr": {
-        "en": "butcher\u2019s hook",
+        "en": "butchers hook",
         "ru": "\u043c\u044f\u0441\u043d\u0438\u0446\u043a\u0438\u0439 \u043a\u0440\u044e\u043a"
     },
     "1rk6g": {
         "en": "coat with face covering",
         "ru": "\u043a\u0443\u0440\u0442\u043a\u0430 \u0441 \u043f\u043e\u0432\u044f\u0437\u043a\u043e\u0439"
     },
     "1rk7g": {
@@ -283,18 +355,26 @@
         "en": "worn psz-10",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043f\u0441\u0437-10"
     },
     "1rkz2": {
         "en": "brigand armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u0440\u043c\u0430\u0439"
     },
+    "1rmwg": {
+        "en": "red armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043a\u0440\u0430\u0441\u043d\u0430\u044f"
+    },
     "1rp4q": {
         "en": "night-vision goggles",
         "ru": "\u043f\u0440\u0438\u0431\u043e\u0440 \u043d\u043e\u0447\u043d\u043e\u0433\u043e \u0432\u0438\u0434\u0435\u043d\u0438\u044f"
     },
+    "1rpl6": {
+        "en": "granite super-heavy armored suit",
+        "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u0440\u0430\u043d\u0438\u0442"
+    },
     "1rvg1": {
         "en": "eotech collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 eotech"
     },
     "1rvlg": {
         "en": "ris m4a1 handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 ris m4a1"
@@ -307,17 +387,41 @@
         "en": "leupold optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 leupold"
     },
     "1rwg2": {
         "en": "mobile camp",
         "ru": "\u043c\u043e\u0431\u0438\u043b\u044c\u043d\u044b\u0439 \u043b\u0430\u0433\u0435\u0440\u044c"
     },
+    "1ry36": {
+        "en": "dpm oj camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm oj"
+    },
+    "1ry4r": {
+        "en": "red weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u043a\u0440\u0430\u0441\u043d\u0430\u044f"
+    },
+    "1ry71": {
+        "en": "tempest camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0440\u044f"
+    },
+    "1ryd1": {
+        "en": "bhutancliff edge camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043a\u0430\u043b\u0438\u0441\u0442\u044b\u0439 \u0431\u0435\u0440\u0435\u0433"
+    },
+    "1ryv6": {
+        "en": "a-tacs au camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs au"
+    },
+    "1ryz6": {
+        "en": "m90 threat camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 threat"
+    },
     "1rz9q": {
-        "en": "fab defense ag-47 grip, black",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "fab defense ag-47 grip black",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "21365": {
         "en": "lim",
         "ru": "\u043b\u0438\u043c"
     },
     "21g9l": {
         "en": "infernal coal",
@@ -332,29 +436,45 @@
         "ru": "\u043c\u0430\u044f\u0447\u043e\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0431\u0435\u0442\u0430"
     },
     "29dm": {
         "en": "f-1",
         "ru": "\u0444-1"
     },
     "2o2wl": {
-        "en": "val/vss receiver cover",
-        "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u0432\u0430\u043b/\u0432\u0441\u0441"
+        "en": "valvss receiver cover",
+        "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u0432\u0430\u043b\u0432\u0441\u0441"
     },
     "2o2y6": {
         "en": "rusak collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u0440\u0443\u0441\u0430\u043a"
     },
+    "2o405": {
+        "en": "palm amoeba camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u0430\u043b\u044c\u043c\u043e\u0432\u0430\u044f \u0430\u043c\u0435\u0431\u0430"
+    },
+    "2o49m": {
+        "en": "agent",
+        "ru": "\u0430\u0433\u0435\u043d\u0442"
+    },
+    "2o4mv": {
+        "en": "erdl woodland camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl woodland"
+    },
     "2o7l5": {
         "en": "ots-14 extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043e\u0446-14"
     },
     "2o7q6": {
         "en": "picatinny rail for svt",
         "ru": "\u043f\u043b\u0430\u043d\u043a\u0430 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438 \u0434\u043b\u044f \u0441\u0432\u0442"
     },
+    "2od4v": {
+        "en": "test prototype ots-33",
+        "ru": "\u0442\u0435\u0441\u0442\u043e\u0432\u044b\u0439 \u043e\u0431\u0440\u0430\u0437\u0435\u0446 \u043e\u0446-33"
+    },
     "2ollv": {
         "en": "classic m9",
         "ru": "\u043a\u043b\u0430\u0441\u0441\u0438\u0447\u0435\u0441\u043a\u0438\u0439 m9"
     },
     "2olnv": {
         "en": "bat with nails",
         "ru": "\u0431\u0438\u0442\u0430 \u0441 \u0433\u0432\u043e\u0437\u0434\u044f\u043c\u0438"
@@ -367,18 +487,14 @@
         "en": "rpk-16",
         "ru": "\u0440\u043f\u043a-16"
     },
     "2opw0": {
         "en": "premium for 30 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 30 \u0434\u043d\u0435\u0439"
     },
-    "2oq55": {
-        "en": "nord-22 group assault trooper",
-        "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u0438\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "2oqdl": {
         "en": "fleece protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0440\u0441\u0430"
     },
     "2oqll": {
         "en": "jaeger exoarmor",
         "ru": "\u044d\u043a\u0437\u043e\u0431\u0440\u043e\u043d\u044f \u0435\u0433\u0435\u0440\u044c"
@@ -387,17 +503,25 @@
         "en": "ah-1 drifter suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-1 \u0431\u0440\u043e\u0434\u044f\u0433\u0430"
     },
     "2ovr0": {
         "en": "saturn suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0441\u0430\u0442\u0443\u0440\u043d"
     },
+    "2ow70": {
+        "en": "erdl woodland camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl woodland"
+    },
+    "2own6": {
+        "en": "palm amoeba camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u0430\u043b\u044c\u043c\u043e\u0432\u0430\u044f \u0430\u043c\u0435\u0431\u0430"
+    },
     "2p16": {
-        "en": "5.56 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
+        "en": "556 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "2pr6": {
         "en": "tank of combustible mixture",
         "ru": "\u0431\u0430\u043b\u043b\u043e\u043d \u0441 \u0433\u043e\u0440\u044e\u0447\u0435\u0439 \u0441\u043c\u0435\u0441\u044c\u044e"
     },
     "2vvv": {
         "en": "kzs-3",
@@ -423,74 +547,102 @@
         "en": "kzs-5y",
         "ru": "\u043a\u0437\u0441-5\u0443"
     },
     "3g1qz": {
         "en": "vodka",
         "ru": "\u0432\u043e\u0434\u043a\u0430"
     },
+    "3g2ng": {
+        "en": "northern slope camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0435\u0432\u0435\u0440\u043d\u044b\u0439 \u0441\u043a\u043b\u043e\u043d"
+    },
+    "3g2pz": {
+        "en": "multicam camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 multicam"
+    },
+    "3g2yz": {
+        "en": "captured erbsenmuster camouflage",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erbsenmuster"
+    },
     "3g69l": {
         "en": "skat-9b armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043a\u0430\u0442-9\u0431"
     },
     "3g6nl": {
         "en": "currant ghillie suit",
         "ru": "\u043c\u0430\u0441\u043a\u0438\u0440\u043e\u0432\u043e\u0447\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043c\u043e\u0440\u043e\u0434\u0438\u043d\u0430"
     },
     "3g6rl": {
         "en": "hoplite armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u043e\u043f\u043b\u0438\u0442"
     },
-    "3g6y5": {
-        "en": "nord-22 group exoskeleton",
-        "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "3g7wg": {
         "en": "dm collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 dm"
     },
     "3g991": {
-        "en": "butcher\u2019s knife",
+        "en": "butchers knife",
         "ru": "\u043c\u044f\u0441\u043d\u0438\u0446\u043a\u0438\u0439 \u043d\u043e\u0436"
     },
     "3g9n1": {
         "en": "aluminum club",
         "ru": "\u0430\u043b\u044e\u043c\u0438\u043d\u0438\u0435\u0432\u0430\u044f \u0431\u0438\u0442\u0430"
     },
     "3gdoz": {
         "en": "worn saturn suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0441\u0430\u0442\u0443\u0440\u043d"
     },
+    "3gk1k": {
+        "en": "odin",
+        "ru": "\u043e\u0434\u0438\u043d"
+    },
+    "3gkk1": {
+        "en": "captured erbsenmuster camouflage",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erbsenmuster"
+    },
+    "3gkm1": {
+        "en": "multicam camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 multicam"
+    },
+    "3gkq5": {
+        "en": "northern slope camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0435\u0432\u0435\u0440\u043d\u044b\u0439 \u0441\u043a\u043b\u043e\u043d"
+    },
     "3gn5g": {
         "en": "tkb-0146m",
         "ru": "\u0442\u043a\u0431-0146\u043c"
     },
     "3gp95": {
         "en": "mts-558 extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0434\u043b\u044f \u043c\u0446-558"
     },
+    "3grk1": {
+        "en": "test prototype rmo-93",
+        "ru": "\u0442\u0435\u0441\u0442\u043e\u0432\u044b\u0439 \u043e\u0431\u0440\u0430\u0437\u0435\u0446 \u0440\u043c\u043e-93"
+    },
+    "3gv2z": {
+        "en": "premium for 90 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 90 \u0434\u043d\u0435\u0439"
+    },
     "3v4g": {
-        "en": "5.56 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "556 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "3vog": {
-        "en": "12.7x55 ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c"
+        "en": "127x55 ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c"
     },
     "49dj": {
         "en": "berloga-6u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-6\u0443"
     },
     "49gj": {
         "en": "kzs-4",
         "ru": "\u043a\u0437\u0441-4"
     },
-    "4d5p": {
-        "en": "12.7x55 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "4dkn": {
         "en": "9x39 mm sp-6 ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u043f-6"
     },
     "4k3qo": {
         "en": "concentrated limboplasma",
         "ru": "\u043a\u043e\u043d\u0446\u0435\u043d\u0442\u0440\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u0430\u044f \u043b\u0438\u043c\u0431\u043e\u043f\u043b\u0430\u0437\u043c\u0430"
@@ -519,14 +671,22 @@
         "en": "moonlight",
         "ru": "\u043b\u0443\u043d\u043d\u044b\u0439 \u0441\u0432\u0435\u0442"
     },
     "4lml": {
         "en": "firefly",
         "ru": "\u0441\u0432\u0435\u0442\u043b\u044f\u043a"
     },
+    "4q00j": {
+        "en": "toxin",
+        "ru": "\u0442\u043e\u043a\u0441\u0438\u043d"
+    },
+    "4q02j": {
+        "en": "red autumn",
+        "ru": "red autumn"
+    },
     "4q09p": {
         "en": "hk g3a1",
         "ru": "hk g3a1"
     },
     "4q0lp": {
         "en": "smg-2000",
         "ru": "\u043f\u043f-2000"
@@ -539,26 +699,82 @@
         "en": "shiv",
         "ru": "\u043d\u043e\u0436 \u0438\u0437 \u0448\u0438\u043f\u0430"
     },
     "4q1nj": {
         "en": "kukri",
         "ru": "\u043a\u0443\u043a\u0440\u0438"
     },
+    "4q20j": {
+        "en": "hexcam bx camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam bx"
+    },
+    "4q22j": {
+        "en": "dpm woodland b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm woodland b"
+    },
+    "4q25o": {
+        "en": "drop camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0430\u0434"
+    },
+    "4q27o": {
+        "en": "flora camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0444\u043b\u043e\u0440\u0430"
+    },
+    "4q29l": {
+        "en": "peace",
+        "ru": "\u043c\u0438\u0440"
+    },
+    "4q2dl": {
+        "en": "iii-b",
+        "ru": "iii-b"
+    },
+    "4q2gl": {
+        "en": "outlaw",
+        "ru": "\u0438\u0437\u0433\u043e\u0439"
+    },
+    "4q2mj": {
+        "en": "belgian jigsaw desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 belgian jigsaw desert"
+    },
     "4q7pl": {
         "en": "advanced tools",
         "ru": "\u043f\u0440\u043e\u0434\u0432\u0438\u043d\u0443\u0442\u044b\u0435 \u0438\u043d\u0441\u0442\u0440\u0443\u043c\u0435\u043d\u0442\u044b"
     },
     "4q9op": {
         "en": "worn beast slayer",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0437\u0432\u0435\u0440\u043e\u0431\u043e\u0439"
     },
     "4qgop": {
         "en": "3rd class antirad",
         "ru": "\u0430\u043d\u0442\u0438\u0440\u0430\u0434 \u0442\u0440\u0435\u0442\u044c\u0435\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
+    "4qj0n": {
+        "en": "flora camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0444\u043b\u043e\u0440\u0430"
+    },
+    "4qj3j": {
+        "en": "purple weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u0430\u044f"
+    },
+    "4qjnn": {
+        "en": "drop camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0430\u0434"
+    },
+    "4qjpp": {
+        "en": "dpm woodland b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm woodland b"
+    },
+    "4qjvp": {
+        "en": "belgian jigsaw desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 belgian jigsaw desert"
+    },
+    "4qjwp": {
+        "en": "hexcam bx camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam bx"
+    },
     "4ql0r": {
         "en": "cloak",
         "ru": "\u043f\u043b\u0430\u0449"
     },
     "4ql1r": {
         "en": "centurion armored exoskeleton",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u0441\u043a\u0435\u043b\u0435\u0442 \u0446\u0435\u043d\u0442\u0443\u0440\u0438\u043e\u043d"
@@ -575,14 +791,18 @@
         "en": "mis-99 malachite",
         "ru": "\u043a\u0438\u043c-99\u043c \u043c\u0430\u043b\u0430\u0445\u0438\u0442"
     },
     "4qlvo": {
         "en": "worn centurion",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0446\u0435\u043d\u0442\u0443\u0440\u0438\u043e\u043d"
     },
+    "4qmrr": {
+        "en": "purple armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0444\u0438\u043e\u043b\u0435\u0442\u043e\u0432\u0430\u044f"
+    },
     "4qn2o": {
         "en": "protecta",
         "ru": "protecta"
     },
     "4qn6j": {
         "en": "ots-33 pernach",
         "ru": "\u043e\u0446-33 \u043f\u0435\u0440\u043d\u0430\u0447"
@@ -600,28 +820,28 @@
         "ru": "\u043e\u0446-14\u043c \u0448\u0442\u043e\u0440\u043c"
     },
     "4qnyn": {
         "en": "ptrd-m",
         "ru": "\u043f\u0442\u0440\u0434-\u043c"
     },
     "4qp0o": {
-        "en": "5.56 nato drum clip, black",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 nato drum clip black",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "4qp1o": {
-        "en": "5.45 drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "4qp4n": {
         "en": "clamp with 3 ris rails",
         "ru": "\u0445\u043e\u043c\u0443\u0442 \u0441 \u0442\u0440\u0435\u043c\u044f \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 ris"
     },
     "4qp7l": {
-        "en": "psuzv-11tm.12 imkas",
-        "ru": "i\u043c\u043a\u0430\u0441 \u043f\u0441\u0443\u0437\u0432\u201311\u0442\u043c.12"
+        "en": "psuzv-11tm12 imkas",
+        "ru": "i\u043c\u043a\u0430\u0441 \u043f\u0441\u0443\u0437\u043211\u0442\u043c12"
     },
     "4qpjr": {
         "en": "aps stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0430\u043f\u0441"
     },
     "4qpkl": {
         "en": "ash-12 standard barrel",
@@ -652,20 +872,16 @@
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0441\u043e"
     },
     "4qvyn": {
         "en": "valday collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u0432\u0430\u043b\u0434\u0430\u0439"
     },
     "5250": {
-        "en": "7.62 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
-    },
-    "526g": {
-        "en": "7.62 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "762 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "52l0": {
         "en": "9 mm sbp ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0431\u043f"
     },
     "553qq": {
         "en": "nuclear gelatin",
@@ -675,38 +891,78 @@
         "en": "army battery",
         "ru": "\u0430\u0440\u043c\u0435\u0439\u0441\u043a\u0438\u0439 \u0430\u043a\u043a\u0443\u043c\u0443\u043b\u044f\u0442\u043e\u0440"
     },
     "556z1": {
         "en": "alpha data fragment",
         "ru": "\u0444\u0440\u0430\u0433\u043c\u0435\u043d\u0442 \u0434\u0430\u043d\u043d\u044b\u0445 \u0430\u043b\u044c\u0444\u0430"
     },
+    "5l0m1": {
+        "en": "green armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0437\u0435\u043b\u0435\u043d\u0430\u044f"
+    },
     "5l134": {
         "en": "nvd-11 export",
         "ru": "nvd-11 export"
     },
     "5l1q0": {
         "en": "modified exoskeleton",
         "ru": "\u043c\u043e\u0434\u0438\u0444\u0438\u0446\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u044b\u0439 \u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442"
     },
     "5l1yg": {
         "en": "raps ah-6 nomad",
         "ru": "\u0443\u043a\u0430\u0437 \u0430\u043e-6 \u043a\u043e\u0447\u0435\u0432\u043d\u0438\u043a"
     },
     "5l4o4": {
-        "en": "fab defense agr-43 grip, khaki",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0445\u0430\u043a\u0438"
+        "en": "fab defense agr-43 grip khaki",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0445\u0430\u043a\u0438"
     },
     "5l6gg": {
         "en": "fn eglm grenade launcher",
         "ru": "\u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442 fn eglm"
     },
+    "5l70o": {
+        "en": "digital-a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 digital-a"
+    },
+    "5l714": {
+        "en": "half-life",
+        "ru": "\u043f\u043e\u043b\u0443\u0440\u0430\u0441\u043f\u0430\u0434"
+    },
+    "5l76q": {
+        "en": "field camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u043e\u043b\u0435"
+    },
+    "5l77o": {
+        "en": "dpm red desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm red desert"
+    },
+    "5l7do": {
+        "en": "volumehex flake camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flake"
+    },
+    "5l7oq": {
+        "en": "surpaturban noise camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442 - \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0448\u0443\u043c"
+    },
+    "5l7z4": {
+        "en": "one-eyed joe",
+        "ru": "\u043e\u0434\u043d\u043e\u0433\u043b\u0430\u0437\u044b\u0439 \u0434\u0436\u043e"
+    },
     "5ld1g": {
         "en": "ots-14 groza",
         "ru": "\u043e\u0446-14 \u0433\u0440\u043e\u0437\u0430"
     },
+    "5ld7o": {
+        "en": "collector",
+        "ru": "\u043a\u043e\u043b\u043b\u0435\u043a\u0446\u0438\u043e\u043d\u0435\u0440"
+    },
+    "5lddo": {
+        "en": "ots-33 frost tigor",
+        "ru": "\u043c\u043e\u0440\u043e\u0437\u043d\u044b\u0439 tigor \u043e\u0446-33"
+    },
     "5ldkg": {
         "en": "akm",
         "ru": "\u0430\u043a\u043c"
     },
     "5ldm4": {
         "en": "worn rpd",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0440\u043f\u0434"
@@ -723,14 +979,38 @@
         "en": "fire razor",
         "ru": "\u043e\u0433\u043d\u0435\u043d\u043d\u0430\u044f \u0431\u0440\u0438\u0442\u0432\u0430"
     },
     "5lgno": {
         "en": "glock feldmesser 78",
         "ru": "glock feldmesser 78"
     },
+    "5lj3o": {
+        "en": "green weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0437\u0435\u043b\u0435\u043d\u0430\u044f"
+    },
+    "5lj4g": {
+        "en": "volumehex flake camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flake"
+    },
+    "5ljd0": {
+        "en": "surpaturban noise camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442 - \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0448\u0443\u043c"
+    },
+    "5ljn0": {
+        "en": "field camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u043e\u043b\u0435"
+    },
+    "5ljpg": {
+        "en": "dpm red desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm red desert"
+    },
+    "5ljvg": {
+        "en": "digital-a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 digital-a"
+    },
     "5ln0q": {
         "en": "shorty 590",
         "ru": "shorty 590"
     },
     "5ln40": {
         "en": "lr-300",
         "ru": "lr-300"
@@ -780,20 +1060,20 @@
         "ru": "\u0434\u0442\u043a-1"
     },
     "5lp61": {
         "en": "m4 paddle stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434-\u0432\u0435\u0441\u043b\u043e m4"
     },
     "5lpdq": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "5lpgq": {
-        "en": "5.45 bakelite clip",
-        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 bakelite clip",
+        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "5lpj1": {
         "en": "wooden skeleton stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u044b\u0439 \u0440\u0430\u043c\u043e\u0447\u043d\u044b\u0439"
     },
     "5lpk0": {
         "en": "ris xm8 rail",
@@ -804,16 +1084,16 @@
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c lonewolf"
     },
     "5lpo4": {
         "en": "pbs-4",
         "ru": "\u043f\u0431\u0441-4"
     },
     "5lpvo": {
-        "en": "compact protective rail, khaki",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0445\u0430\u043a\u0438"
+        "en": "compact protective rail khaki",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0445\u0430\u043a\u0438"
     },
     "5lpy4": {
         "en": "scar-sd silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c scar-sd"
     },
     "5lr1o": {
         "en": "reinforced cloak",
@@ -840,28 +1120,28 @@
         "ru": "t\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0441\u0445\u043e\u0434"
     },
     "5lrvq": {
         "en": "damaged jaeger",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u0435\u0433\u0435\u0440\u044c"
     },
     "5lv31": {
-        "en": "akm wooden handguard, black",
-        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u043e\u0435 \u0430\u043a\u043c, \u0447\u0435\u0440\u043d\u043e\u0435"
+        "en": "akm wooden handguard black",
+        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u043e\u0435 \u0430\u043a\u043c \u0447\u0435\u0440\u043d\u043e\u0435"
     },
     "5lv7q": {
-        "en": "reg fab defense tactical grip, gray",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence, \u0441\u0435\u0440\u044b\u0439"
+        "en": "reg fab defense tactical grip gray",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence \u0441\u0435\u0440\u044b\u0439"
     },
     "5lv9o": {
         "en": "sig sauer optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 sig sauer"
     },
     "5lvmg": {
-        "en": "an/peq 15 tactical unit, khaki",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0445\u0430\u043a\u0438"
+        "en": "anpeq 15 tactical unit khaki",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0445\u0430\u043a\u0438"
     },
     "5lvo1": {
         "en": "ris p90 handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 ris p90"
     },
     "5lvpo": {
         "en": "1p77 optical sight",
@@ -916,20 +1196,20 @@
         "ru": "\u043a\u043e\u0440\u043a\u0430"
     },
     "5wd1": {
         "en": "sn-2 leg",
         "ru": "\u0441\u043d-2 \u043d\u043e\u0433\u0430"
     },
     "63oy": {
-        "en": "5.56 sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0431\u043f"
+        "en": "556 sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0441\u0431\u043f"
     },
     "63yy": {
-        "en": "12.7x55 mm sniper ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
+        "en": "127x55 mm sniper ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
     },
     "65r6": {
         "en": "vog-25 grenade round",
         "ru": "\u0432\u044b\u0441\u0442\u0440\u0435\u043b \u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442\u043d\u044b\u0439 \u0432\u043e\u0433-25"
     },
     "6o7m0": {
         "en": "lambda data fragment",
@@ -951,26 +1231,62 @@
         "en": "worn trapper suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0442\u0440\u0430\u043f\u043f\u0435\u0440"
     },
     "6w0zp": {
         "en": "trump exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u043c\u0430\u0441\u0442\u044c"
     },
+    "6w22n": {
+        "en": "captured sumpfmuster camouflage 1943 model",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440 1943 \u0433"
+    },
+    "6w236": {
+        "en": "raider",
+        "ru": "\u0440\u0435\u0439\u0434\u0435\u0440"
+    },
+    "6w256": {
+        "en": "lancelot",
+        "ru": "\u043b\u0430\u043d\u0446\u0435\u043b\u043e\u0442"
+    },
+    "6w290": {
+        "en": "flakes camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u043b\u043e\u043f\u044c\u044f"
+    },
+    "6w2dn": {
+        "en": "dpm iranian guard camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm iranian guard"
+    },
     "6w59j": {
-        "en": "\u201cstrike\u201d",
+        "en": "strike",
         "ru": "\u0443\u0434\u0430\u0440"
     },
     "6w64y": {
-        "en": "grizzly 8.5",
-        "ru": "grizzly 8.5"
+        "en": "grizzly 85",
+        "ru": "grizzly 85"
+    },
+    "6wj6y": {
+        "en": "flakes camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u043b\u043e\u043f\u044c\u044f"
+    },
+    "6wjkj": {
+        "en": "captured sumpfmuster camouflage 1943 model",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440 1943 \u0433"
+    },
+    "6wjpj": {
+        "en": "dpm iranian guard camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm iranian guard"
     },
     "6wpo6": {
         "en": "d-eagle barrel extension",
         "ru": "\u0443\u0434\u043b\u0438\u043d\u0435\u043d\u043d\u044b\u0439 \u0441\u0442\u0432\u043e\u043b d-eagle"
     },
+    "6wr2n": {
+        "en": "test prototype rpk-16",
+        "ru": "\u0442\u0435\u0441\u0442\u043e\u0432\u044b\u0439 \u043e\u0431\u0440\u0430\u0437\u0435\u0446 \u0440\u043f\u043a-16"
+    },
     "6wvqy": {
         "en": "panorama collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u0430\u043d\u043e\u0440\u0430\u043c\u0430"
     },
     "6wz1n": {
         "en": "fluorite",
         "ru": "\u0444\u043b\u044e\u043e\u0440\u0438\u0442"
@@ -992,20 +1308,40 @@
         "ru": "\u043a\u0432\u0430\u043d\u0442\u043e\u0432\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "77oy6": {
         "en": "remains of a signal processor",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u0441\u0438\u0433\u043d\u0430\u043b\u044c\u043d\u043e\u0433\u043e \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0440\u0430"
     },
     "7977": {
-        "en": "5.56 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
+        "en": "556 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "79w7": {
-        "en": "12.7x55 smg ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u043f\u043f"
+        "en": "127x55 smg ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c \u043f\u043f"
+    },
+    "7l209": {
+        "en": "dpm desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm desert"
+    },
+    "7l21j": {
+        "en": "snowdrift camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u0443\u0440\u0442\u043e\u0432\u0438\u043d\u0430"
+    },
+    "7l229": {
+        "en": "captured luft splinter camouflage",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 luft splinter"
+    },
+    "7l29r": {
+        "en": "thug",
+        "ru": "\u0433\u043e\u043b\u043e\u0432\u043e\u0440\u0435\u0437"
+    },
+    "7l2yr": {
+        "en": "archangel",
+        "ru": "\u0430\u0440\u0445\u0430\u043d\u0433\u0435\u043b"
     },
     "7l559": {
         "en": "reverse-grip knife",
         "ru": "\u043d\u043e\u0436 \u0441 \u043e\u0431\u0440\u0430\u0442\u043d\u044b\u043c \u0445\u0432\u0430\u0442\u043e\u043c"
     },
     "7l5g9": {
         "en": "endgame",
@@ -1015,48 +1351,64 @@
         "en": "hatchet",
         "ru": "\u0442\u0435\u0441\u0430\u043a"
     },
     "7l6j7": {
         "en": "kobra collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043a\u043e\u0431\u0440\u0430"
     },
+    "7l9d3": {
+        "en": "premium for 180 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 180 \u0434\u043d\u0435\u0439"
+    },
+    "7ldn7": {
+        "en": "snowdrift camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u0443\u0440\u0442\u043e\u0432\u0438\u043d\u0430"
+    },
+    "7ldp3": {
+        "en": "dpm desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm desert"
+    },
+    "7ldq3": {
+        "en": "captured luft splinter camouflage",
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 luft splinter"
+    },
     "7lm56": {
         "en": "exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442"
     },
     "7lmn6": {
         "en": "houndmaster protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043f\u0441\u0430\u0440\u044c"
     },
-    "7lmqj": {
-        "en": "nord-22 group blizzard-bound",
-        "ru": "\u0438\u0434\u0443\u0449\u0438\u0439 \u0432 \u043c\u0435\u0442\u0435\u043b\u0438 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "7lmr6": {
         "en": "trapper suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0442\u0440\u0430\u043f\u043f\u0435\u0440"
     },
     "7lnk7": {
         "en": "mts-116m",
         "ru": "\u043c\u0446-116\u043c"
     },
     "7lp5j": {
         "en": "psg1 extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d psg1"
     },
+    "7lr29": {
+        "en": "test prototype tkb-0146m",
+        "ru": "\u0442\u0435\u0441\u0442\u043e\u0432\u044b\u0439 \u043e\u0431\u0440\u0430\u0437\u0435\u0446 \u0442\u043a\u0431-0146\u043c"
+    },
     "7lrz3": {
         "en": "ak-103",
         "ru": "\u0430\u043a-103"
     },
     "7lwvj": {
         "en": "iou from shaman",
         "ru": "\u0440\u0430\u0441\u043f\u0438\u0441\u043a\u0430 \u043e\u0442 \u0448\u0430\u043c\u0430\u043d\u0430"
     },
     "7ly13": {
-        "en": "guide\u2019s first-aid kit",
+        "en": "guides first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u043f\u0440\u043e\u0432\u043e\u0434\u043d\u0438\u043a\u0430"
     },
     "7lzw3": {
         "en": "damaged saturn suit",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0441\u0430\u0442\u0443\u0440\u043d"
     },
     "7yl7": {
@@ -1071,14 +1423,50 @@
         "en": "v40 mini-grenade",
         "ru": "v40 mini-grenade"
     },
     "94mw": {
         "en": "vog-25 podkidysh grenade round",
         "ru": "\u0432\u044b\u0441\u0442\u0440\u0435\u043b \u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442\u043d\u044b\u0439 \u0432\u043e\u0433-25\u043f \u043f\u043e\u0434\u043a\u0438\u0434\u044b\u0448"
     },
+    "9607l": {
+        "en": "pure gold skin",
+        "ru": "\u0441\u043a\u0438\u043d \u0447\u0438\u0441\u0442\u043e\u0435 \u0437\u043e\u043b\u043e\u0442\u043e"
+    },
+    "9620q": {
+        "en": "a-tacs fg camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs fg"
+    },
+    "9622q": {
+        "en": "dpm kuwaiti police camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm kuwaiti police"
+    },
+    "9623y": {
+        "en": "bhutan camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d"
+    },
+    "9624w": {
+        "en": "carrie",
+        "ru": "\u043a\u044d\u0440\u0440\u0438"
+    },
+    "962gw": {
+        "en": "frost fighter",
+        "ru": "\u043c\u043e\u0440\u043e\u0437\u043e\u0431\u043e\u0440\u0435\u0446"
+    },
+    "962mq": {
+        "en": "hexagon-c camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-c"
+    },
+    "962yw": {
+        "en": "bulldozer",
+        "ru": "\u0431\u0443\u043b\u044c\u0434\u043e\u0437\u0435\u0440"
+    },
+    "962zy": {
+        "en": "bhutansnow camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043d\u0435\u0433"
+    },
     "96430": {
         "en": "personal first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u0438\u043d\u0434\u0438\u0432\u0438\u0434\u0443\u0430\u043b\u044c\u043d\u0430\u044f"
     },
     "9696l": {
         "en": "worn sks",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0441\u043a\u0441"
@@ -1107,14 +1495,18 @@
         "en": "gp-25 kostyor",
         "ru": "\u0433\u043f-25 \u043a\u043e\u0441\u0442\u0435\u0440"
     },
     "96ldw": {
         "en": "rk-3 grip",
         "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c \u0440\u043a-3"
     },
+    "96m2q": {
+        "en": "treasure of the oasis",
+        "ru": "\u0434\u0440\u0430\u0433\u043e\u0446\u0435\u043d\u043d\u043e\u0441\u0442\u044c \u043e\u0430\u0437\u0438\u0441\u0430"
+    },
     "96mj0": {
         "en": "smg-91 kedr",
         "ru": "\u043f\u043f-91 \u043a\u0435\u0434\u0440"
     },
     "96my0": {
         "en": "alk-22 dragonfly",
         "ru": "\u0430\u043b\u043a-22 \u0441\u0442\u0440\u0435\u043a\u043e\u0437\u0430"
@@ -1143,33 +1535,57 @@
         "en": "worn ah-2 nomad",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043e-2 \u0441\u0442\u0440\u0430\u043d\u043d\u0438\u043a"
     },
     "96nrq": {
         "en": "stylish jacket",
         "ru": "\u043c\u043e\u0434\u043d\u0430\u044f \u043a\u0443\u0440\u0442\u043a\u0430"
     },
+    "96o1q": {
+        "en": "gold weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0437\u043e\u043b\u043e\u0442\u0430\u044f"
+    },
+    "96o9z": {
+        "en": "bhutansnow camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043d\u0435\u0433"
+    },
+    "96ol0": {
+        "en": "hexagon-c camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-c"
+    },
+    "96omz": {
+        "en": "bhutan camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d"
+    },
+    "96op0": {
+        "en": "dpm kuwaiti police camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm kuwaiti police"
+    },
+    "96ov0": {
+        "en": "a-tacs fg camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs fg"
+    },
     "96p2y": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "96p6w": {
         "en": "noveske kx3 flash suppressor",
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c noveske kx3"
     },
     "96pkl": {
         "en": "mossberg stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 mossberg"
     },
     "96prz": {
         "en": "bm barrel mount",
         "ru": "\u043d\u0430\u0434\u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0435 \u043a\u0440\u0435\u043f\u043b\u0435\u043d\u0438\u0435 \u0431\u043c"
     },
     "96pvq": {
-        "en": "protective rail, olive",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u043e\u043b\u0438\u0432\u0430"
+        "en": "protective rail olive",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u043e\u043b\u0438\u0432\u0430"
     },
     "96pwy": {
         "en": "30-round clip for ak-308",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0430\u043a-308"
     },
     "96v0y": {
         "en": "magpul afg tactical grip",
@@ -1188,25 +1604,29 @@
         "ru": "\u0446\u0435\u0432\u044c\u0435 ris l85"
     },
     "96w5q": {
         "en": "grabber",
         "ru": "\u0440\u0432\u0430\u0447"
     },
     "96w9q": {
-        "en": "hunter\u2019s knife",
+        "en": "hunters knife",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043d\u043e\u0436"
     },
     "96wwq": {
         "en": "piece of pipe",
         "ru": "\u043a\u0443\u0441\u043e\u043a \u0442\u0440\u0443\u0431\u044b"
     },
     "96y1w": {
         "en": "home-made nvg",
         "ru": "\u043a\u0443\u0441\u0442\u0430\u0440\u043d\u044b\u0439 \u043f\u043d\u0432"
     },
+    "96yz0": {
+        "en": "reiter super-heavy armored suit",
+        "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0440\u0435\u0439\u0442\u0430\u0440"
+    },
     "9d1qy": {
         "en": "anomalous battery",
         "ru": "\u0430\u043d\u043e\u043c\u0430\u043b\u044c\u043d\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "9dk7l": {
         "en": "anomalous serum",
         "ru": "\u0430\u043d\u043e\u043c\u0430\u043b\u044c\u043d\u0430\u044f \u0441\u044b\u0432\u043e\u0440\u043e\u0442\u043a\u0430"
@@ -1223,18 +1643,14 @@
         "en": "swamp stone",
         "ru": "\u0431\u043e\u043b\u043e\u0442\u043d\u044b\u0439 \u043a\u0430\u043c\u0435\u043d\u044c"
     },
     "9g6z": {
         "en": "9 mm ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c"
     },
-    "9gk0": {
-        "en": "9 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "9j0l": {
         "en": "candle short range detector",
         "ru": "\u0434\u0435\u0442\u0435\u043a\u0442\u043e\u0440 \u0443\u0437\u043a\u043e\u0433\u043e \u0434\u0438\u0430\u043f\u0430\u0437\u043e\u043d\u0430 \u0441\u0432\u0435\u0447\u0430"
     },
     "9n1w": {
         "en": "stone blood",
         "ru": "\u043a\u0440\u043e\u0432\u044c \u043a\u0430\u043c\u043d\u044f"
@@ -1251,60 +1667,76 @@
         "en": "thorn",
         "ru": "\u043a\u043e\u043b\u044e\u0447\u043a\u0430"
     },
     "9nvy": {
         "en": "quirk",
         "ru": "\u0432\u044b\u0432\u0435\u0440\u0442"
     },
+    "9rkw": {
+        "en": "sak-1 wide range detector",
+        "ru": "\u0434\u0435\u0442\u0435\u043a\u0442\u043e\u0440 \u0448\u0438\u0440\u043e\u043a\u043e\u0433\u043e \u0434\u0438\u0430\u043f\u0430\u0437\u043e\u043d\u0430 \u0441\u0430\u043a-1"
+    },
     "9yyq": {
         "en": "kzs-1 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0437\u0441-1"
     },
     "d1mn": {
-        "en": "5.56 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c"
+        "en": "556 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c"
     },
     "dkq9": {
         "en": "rgd-5",
         "ru": "\u0440\u0433\u0434-5"
     },
     "dm09j": {
         "en": "ots-14 tactical grip",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u043d\u0430\u043a\u043b\u0430\u0434\u043a\u0430 \u043e\u0446-14"
     },
     "dm0dn": {
-        "en": "pk-01(t/z) collimator sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01(\u0442/\u0437)"
+        "en": "pk-01tz collimator sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01\u0442\u0437"
     },
     "dm195": {
         "en": "premium for 14 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 14 \u0434\u043d\u0435\u0439"
     },
     "dm27n": {
         "en": "increasing ris-rail",
         "ru": "\u043f\u043e\u0432\u044b\u0448\u0430\u044e\u0449\u0430\u044f ris-\u043f\u043b\u0430\u043d\u043a\u0430"
     },
     "dm2q2": {
         "en": "40-ammo emag clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 40-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 emag"
     },
     "dm2v2": {
-        "en": "30-round clip for vss/val",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441/\u0432\u0430\u043b"
+        "en": "30-round clip for vssval",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441\u0432\u0430\u043b"
+    },
+    "dm925": {
+        "en": "erdl uscm camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl uscm"
+    },
+    "dm9qn": {
+        "en": "amoeba camouflage 1942 model",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440 1942 \u0433"
+    },
+    "dm9w5": {
+        "en": "flecktarn frost camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn frost"
     },
     "dmg02": {
         "en": "worn kleptomaniac",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043b\u0435\u043f\u0442\u043e\u043c\u0430\u043d"
     },
     "dmgjj": {
         "en": "healing berill",
         "ru": "\u043b\u0435\u0447\u0435\u0431\u043d\u044b\u0439 \u0431\u0435\u0440\u0438\u043b\u043b"
     },
     "dmgqj": {
-        "en": "hunter\u2019s cloak",
+        "en": "hunters cloak",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043f\u043b\u0430\u0449"
     },
     "dmgvj": {
         "en": "osh protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043e\u0448"
     },
     "dmgw2": {
@@ -1316,45 +1748,73 @@
         "ru": "\u0430\u043a-308"
     },
     "dmjwn": {
         "en": "hk416",
         "ru": "hk416"
     },
     "dmky5": {
-        "en": "\u201cclearmind+\u201d",
-        "ru": "clearmind+"
+        "en": "clearmind",
+        "ru": "clearmind"
+    },
+    "dmqzg": {
+        "en": "deterioration",
+        "ru": "\u0438\u0437\u043d\u043e\u0441"
     },
     "dmvjg": {
         "en": "telescopic baton",
         "ru": "\u0442\u0435\u043b\u0435\u0441\u043a\u043e\u043f\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0434\u0443\u0431\u0438\u043d\u043a\u0430"
     },
     "dmvog": {
         "en": "ka-bar bkr3 tactical knife",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043d\u043e\u0436 ka-bar bkr3"
     },
     "dmvvg": {
-        "en": "swamp dweller\u2019s friend",
+        "en": "swamp dwellers friend",
         "ru": "\u0434\u0440\u0443\u0433 \u0431\u043e\u043b\u043e\u0442\u043d\u0438\u043a\u0430"
     },
+    "dmz19": {
+        "en": "arctic",
+        "ru": "\u0430\u0440\u043a\u0442\u0438\u043a\u0430"
+    },
+    "dmz4g": {
+        "en": "erdl uscm camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl uscm"
+    },
+    "dmzk9": {
+        "en": "sinner",
+        "ru": "\u0433\u0440\u0435\u0448\u043d\u0438\u043a"
+    },
+    "dmzy2": {
+        "en": "amoeba camouflage 1942 model",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440 1942 \u0433"
+    },
+    "dmzzg": {
+        "en": "flecktarn frost camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn frost"
+    },
     "dr61j": {
         "en": "beta data block",
         "ru": "\u0431\u043b\u043e\u043a \u0434\u0430\u043d\u043d\u044b\u0445 \u0431\u0435\u0442\u0430"
     },
     "dr6nj": {
         "en": "red fern",
         "ru": "\u0440\u044b\u0436\u0438\u0439 \u043f\u0430\u043f\u043e\u0440\u043e\u0442\u043d\u0438\u043a"
     },
     "g35n": {
-        "en": "bear\u2019s den \u2014 6 container",
+        "en": "bears den  6 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-6"
     },
     "g3ln": {
         "en": "fridge container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0445\u043e\u043b\u043e\u0434\u0438\u043b\u044c\u043d\u0438\u043a"
     },
+    "g400n": {
+        "en": "ots-62 thug",
+        "ru": "\u0433\u043e\u043b\u043e\u0432\u043e\u0440\u0435\u0437 \u043e\u0446-62"
+    },
     "g405g": {
         "en": "rpk-74",
         "ru": "\u0440\u043f\u043a-74"
     },
     "g4060": {
         "en": "l85a1",
         "ru": "l85a1"
@@ -1363,46 +1823,54 @@
         "en": "l86a1",
         "ru": "l86a1"
     },
     "g40d0": {
         "en": "imi uzi",
         "ru": "imi uzi"
     },
+    "g40wn": {
+        "en": "legend",
+        "ru": "\u043b\u0435\u0433\u0435\u043d\u0434\u0430"
+    },
     "g40y0": {
         "en": "worn an-94 abakan",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043d-94 \u0430\u0431\u0430\u043a\u0430\u043d"
     },
     "g424g": {
         "en": "resistance armament compensator",
         "ru": "resistance armament compensator"
     },
     "g426p": {
         "en": "picatinny rail and base",
         "ru": "\u043f\u043b\u0430\u043d\u043a\u0430 \u0441 \u0431\u0430\u0437\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "g42gn": {
-        "en": "protective rail, black",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "protective rail black",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "g42kg": {
         "en": "js silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c js"
     },
     "g42ng": {
         "en": "kosoi mbc",
         "ru": "\u0434\u0442\u043a \u043a\u043e\u0441\u043e\u0439"
     },
     "g42w5": {
-        "en": "5.56 nato pmag clip, khaki",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato pmag, \u0445\u0430\u043a\u0438"
+        "en": "556 nato pmag clip khaki",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato pmag \u0445\u0430\u043a\u0438"
     },
     "g42z6": {
         "en": "izhmash wooden stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0438\u0436\u043c\u0430\u0448 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u044b\u0439"
     },
+    "g4310": {
+        "en": "chieftain super-heavy armored suit",
+        "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0436\u0434\u044c"
+    },
     "g43k0": {
         "en": "mule exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u043c\u0443\u043b"
     },
     "g43pg": {
         "en": "2nd generation nvg",
         "ru": "\u043f\u043d\u0432 2-\u0433\u043e \u043f\u043e\u043a\u043e\u043b\u0435\u043d\u0438\u044f"
@@ -1435,28 +1903,32 @@
         "en": "elcan optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 elcan"
     },
     "g4gyp": {
         "en": "obzor collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043e\u0431\u0437\u043e\u0440"
     },
+    "g4j76": {
+        "en": "orange armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
+    },
     "g4l10": {
         "en": "atlas anabolic steroid",
         "ru": "\u0430\u043d\u0430\u0431\u043e\u043b\u0438\u043a atlas"
     },
     "g4lk0": {
         "en": "army first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u0430\u0440\u043c\u0435\u0439\u0441\u043a\u0430\u044f"
     },
     "g4m0n": {
         "en": "tt",
         "ru": "\u0442\u0442"
     },
     "g4m2p": {
-        "en": "mosin\u2019s rifle",
+        "en": "mosins rifle",
         "ru": "\u0432\u0438\u043d\u0442\u043e\u0432\u043a\u0430 \u043c\u043e\u0441\u0438\u043d\u0430"
     },
     "g4m46": {
         "en": "sks",
         "ru": "\u0441\u043a\u0441"
     },
     "g4mdp": {
@@ -1488,37 +1960,65 @@
         "ru": "beretta 92fs"
     },
     "g4mz5": {
         "en": "toz-34",
         "ru": "\u0442\u043e\u0437-34"
     },
     "g4q1g": {
-        "en": "fab defense agr-43 grip, black",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "fab defense agr-43 grip black",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "g4qng": {
-        "en": "fab defense ag-47 grip, green",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
+        "en": "fab defense ag-47 grip green",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
     },
     "g4vj5": {
         "en": "rg-6",
         "ru": "\u0440\u0433-6"
     },
     "g4vk6": {
         "en": "dream",
         "ru": "\u043c\u0435\u0447\u0442\u0430"
     },
     "g4vmn": {
         "en": "crowbar",
         "ru": "\u043c\u043e\u043d\u0442\u0438\u0440\u043e\u0432\u043a\u0430"
     },
     "g4vvn": {
-        "en": "new year\u2019s shovel",
+        "en": "new years shovel",
         "ru": "\u043d\u043e\u0432\u043e\u0433\u043e\u0434\u043d\u044f\u044f \u043b\u043e\u043f\u0430\u0442\u0430"
     },
+    "g4w0n": {
+        "en": "m90 winter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 winter"
+    },
+    "g4w15": {
+        "en": "belarusian digital camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u043b\u043e\u0440\u0443\u0441\u0441\u043a\u0430\u044f \u0446\u0438\u0444\u0440\u0430"
+    },
+    "g4w3g": {
+        "en": "firefighter",
+        "ru": "\u043f\u043e\u0436\u0430\u0440\u043d\u044b\u0439"
+    },
+    "g4wjn": {
+        "en": "hexagon-a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-a"
+    },
+    "g4wk5": {
+        "en": "birch tree camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430"
+    },
+    "g4wlg": {
+        "en": "liquidator",
+        "ru": "\u043b\u0438\u043a\u0432\u0438\u0434\u0430\u0442\u043e\u0440"
+    },
+    "g4wwn": {
+        "en": "dpm oman camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm oman"
+    },
     "g4y06": {
         "en": "worn striker armored suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u0442\u0440\u0430\u0439\u043a\u0435\u0440"
     },
     "g4y3n": {
         "en": "cd-1 suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u043a\u0437-1"
@@ -1543,25 +2043,45 @@
         "en": "grenadier exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u0433\u0440\u0435\u043d\u0430\u0434\u0435\u0440"
     },
     "g4yw6": {
         "en": "bandit coat",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0430\u044f \u043a\u0443\u0440\u0442\u043a\u0430"
     },
+    "g4z0p": {
+        "en": "birch tree camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430"
+    },
+    "g4z20": {
+        "en": "dpm oman camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm oman"
+    },
+    "g4zg0": {
+        "en": "hexagon-a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-a"
+    },
+    "g4zmp": {
+        "en": "belarusian digital camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u043b\u043e\u0440\u0443\u0441\u0441\u043a\u0430\u044f \u0446\u0438\u0444\u0440\u0430"
+    },
+    "g4zpn": {
+        "en": "orange weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
+    },
+    "g4zq0": {
+        "en": "m90 winter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 winter"
+    },
     "g54p": {
         "en": "9 mm expanding ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
-    "g590": {
-        "en": "5.45 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "g5np": {
-        "en": "7.62 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
+        "en": "762 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "gd06": {
         "en": "sn-1 pancake",
         "ru": "\u0441\u043d-1 \u0431\u043b\u0438\u043d"
     },
     "gdj6": {
         "en": "elbrus short range detector",
@@ -1647,58 +2167,82 @@
         "en": "smc container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0441\u043c"
     },
     "j456": {
         "en": "12 caliber canister shot",
         "ru": "\u043a\u0430\u0440\u0442\u0435\u0447\u044c 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
-    "j4z7": {
-        "en": "9 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "j52lg": {
-        "en": "7.62 nato pmag clip, khaki",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62 nato pmag, \u0445\u0430\u043a\u0438"
+        "en": "762 nato pmag clip khaki",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 762 nato pmag \u0445\u0430\u043a\u0438"
     },
     "j52q4": {
         "en": "mts-558 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u043c\u0446-558"
     },
     "j52vg": {
         "en": "smg-91 clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043f-91"
     },
     "j561l": {
         "en": "bars optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u0430\u0440\u0441"
     },
     "j562l": {
-        "en": "pilad 3.5x20 optical sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0438\u043b\u0430\u0434 3.5\u044520"
+        "en": "pilad 35x20 optical sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0438\u043b\u0430\u0434 35\u044520"
     },
     "j569g": {
         "en": "fma dark earth fire transfer grip",
         "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c \u043f\u0435\u0440\u0435\u043d\u043e\u0441\u0430 \u043e\u0433\u043d\u044f fma dark earth"
     },
     "j56d6": {
         "en": "barska collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 barska"
     },
     "j56w0": {
         "en": "an-94 udav handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0443\u0434\u0430\u0432 \u0430\u043d-94"
     },
     "j56y7": {
-        "en": "an/peq 15 tactical unit, black (green laser)",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0447\u0435\u0440\u043d\u044b\u0439 (\u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "anpeq 15 tactical unit black green laser",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0447\u0435\u0440\u043d\u044b\u0439 \u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "j56z0": {
         "en": "m1a stock with picatinny rails",
         "ru": "\u043b\u043e\u0436\u0435 m1a \u0441 \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
+    "j5934": {
+        "en": "uss-01",
+        "ru": "uss-01"
+    },
+    "j5944": {
+        "en": "reborn",
+        "ru": "\u043f\u0435\u0440\u0435\u0440\u043e\u0436\u0434\u0435\u043d\u043d\u044b\u0439"
+    },
+    "j599l": {
+        "en": "hexcam opfor camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam opfor"
+    },
+    "j59jl": {
+        "en": "m90 desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 desert"
+    },
+    "j59m4": {
+        "en": "modification 47",
+        "ru": "\u043c\u043e\u0434\u0438\u0444\u0438\u043a\u0430\u0446\u0438\u044f 47"
+    },
+    "j59p0": {
+        "en": "khaki armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0445\u0430\u043a\u0438"
+    },
+    "j59qg": {
+        "en": "fissure camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0438\u0437\u043b\u043e\u043c"
+    },
     "j5k10": {
         "en": "worn seva suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0441\u0435\u0432\u0430"
     },
     "j5k6g": {
         "en": "worn emerald",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0438\u0437\u0443\u043c\u0440\u0443\u0434"
@@ -1752,17 +2296,33 @@
         "ru": "glock 18c"
     },
     "j5vol": {
         "en": "tanto with a ring",
         "ru": "\u0442\u0430\u043d\u0442\u043e \u0441 \u043a\u043e\u043b\u044c\u0446\u043e\u043c"
     },
     "j5vvl": {
-        "en": "military stalkers\u2019 hatchet",
+        "en": "military stalkers hatchet",
         "ru": "\u0442\u0435\u0441\u0430\u043a \u0432\u043e\u0435\u043d\u0441\u0442\u0430\u043b\u043e\u0432"
     },
+    "j5w27": {
+        "en": "hexcam opfor camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam opfor"
+    },
+    "j5w67": {
+        "en": "m90 desert camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 desert"
+    },
+    "j5wgl": {
+        "en": "khaki weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0445\u0430\u043a\u0438"
+    },
+    "j5wl6": {
+        "en": "fissure camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0438\u0437\u043b\u043e\u043c"
+    },
     "jkj4": {
         "en": "pellicle",
         "ru": "\u043f\u043b\u0435\u043d\u043a\u0430"
     },
     "jkml": {
         "en": "eye of the storm",
         "ru": "\u0433\u043b\u0430\u0437 \u0431\u0443\u0440\u0438"
@@ -1783,14 +2343,66 @@
         "en": "frost shot",
         "ru": "\u043c\u043e\u0440\u043e\u0437\u043d\u044b\u0439 \u0432\u044b\u0441\u0442\u0440\u0435\u043b"
     },
     "kkrv": {
         "en": "9x39 mm bp ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0431\u043f"
     },
+    "kn11j": {
+        "en": "hexcam arid camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam arid"
+    },
+    "kn133": {
+        "en": "\u0430bs380",
+        "ru": "\u0430bs380"
+    },
+    "kn15p": {
+        "en": "spruce camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0435\u043b\u044c\u043d\u0438\u043a"
+    },
+    "kn1jj": {
+        "en": "m90 camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90"
+    },
+    "kn1k3": {
+        "en": "special machinery",
+        "ru": "\u0441\u043f\u0435\u0446\u0442\u0435\u0445\u043d\u0438\u043a\u0430"
+    },
+    "kn1o3": {
+        "en": "forsaken",
+        "ru": "\u043e\u0442\u0440\u0435\u043a\u0448\u0438\u0439\u0441\u044f"
+    },
+    "kn1pp": {
+        "en": "dune camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0434\u044e\u043d\u0430"
+    },
+    "kn1yy": {
+        "en": "black armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0447\u0435\u0440\u043d\u0430\u044f"
+    },
+    "kn290": {
+        "en": "hexcam arid camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam arid"
+    },
+    "kn2lv": {
+        "en": "dune camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0434\u044e\u043d\u0430"
+    },
+    "kn2mv": {
+        "en": "spruce camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0435\u043b\u044c\u043d\u0438\u043a"
+    },
+    "kn2w0": {
+        "en": "m90 camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90"
+    },
+    "kn2zj": {
+        "en": "black weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0447\u0435\u0440\u043d\u0430\u044f"
+    },
     "kn360": {
         "en": "worn mule",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043c\u0443\u043b"
     },
     "kn3yv": {
         "en": "rigel suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0440\u0438\u0433\u0435\u043b\u044c"
@@ -1808,15 +2420,15 @@
         "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0434\u043b\u044f \u043f\u043c"
     },
     "knl30": {
         "en": "fn f2000 tactical",
         "ru": "fn f2000 tactical"
     },
     "knl70": {
-        "en": "cleaner\u2019s aks",
+        "en": "cleaners aks",
         "ru": "\u0430\u043a\u0441 \u0447\u0438\u0441\u0442\u0438\u043b\u044c\u0449\u0438\u043a\u0430"
     },
     "knlgv": {
         "en": "lim",
         "ru": "\u043b\u0438\u043c"
     },
     "knlq0": {
@@ -1837,15 +2449,15 @@
     },
     "knmgj": {
         "en": "colt python",
         "ru": "colt python"
     },
     "knmpy": {
         "en": "worn vss vintorez",
-        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \"\u0432\u0441\u0441 \u0432\u0438\u043d\u0442\u043e\u0440\u0435\u0437\""
+        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0432\u0441\u0441 \u0432\u0438\u043d\u0442\u043e\u0440\u0435\u0437"
     },
     "kno60": {
         "en": "2nd class psy-blocker",
         "ru": "\u043f\u0441\u0438-\u0431\u043b\u043e\u043a\u0430\u0434\u0430 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "knp93": {
         "en": "special tools",
@@ -1860,15 +2472,15 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u0438\u043c-99 \u044f\u043d\u0442\u0430\u0440\u044c"
     },
     "knqkv": {
         "en": "albatross scout armored exoskeleton",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u0441\u043a\u0435\u043b\u0435\u0442 \u0430\u043b\u044c\u0431\u0430\u0442\u0440\u043e\u0441-\u0440\u0430\u0437\u0432\u0435\u0434\u0447\u0438\u043a"
     },
     "knqly": {
-        "en": "reporter\u2019s armor",
+        "en": "reporters armor",
         "ru": "\u0431\u0440\u043e\u043d\u044f \u0440\u0435\u043f\u043e\u0440\u0442\u0435\u0440\u0430"
     },
     "knqmy": {
         "en": "bandit cloak",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043f\u043b\u0430\u0449"
     },
     "knqvy": {
@@ -1884,16 +2496,16 @@
         "ru": "jagdkommando"
     },
     "knvvj": {
         "en": "icy kukri",
         "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043a\u0443\u043a\u0440\u0438"
     },
     "knw1p": {
-        "en": "fortis shift vertical tactical grip, orange",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical, \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
+        "en": "fortis shift vertical tactical grip orange",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
     },
     "knw2y": {
         "en": "pkp receiver cover with picatinny rail",
         "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u043f\u043a\u043f \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "knw5y": {
         "en": "handguard with guiding ris for sig sg 550",
@@ -1960,20 +2572,16 @@
         "ru": "\u0440\u044e\u043a\u0437\u0430\u043a hellboy"
     },
     "l3n2": {
         "en": "berloga-4u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-4\u0443"
     },
     "l601": {
-        "en": "7.62 mm sniper ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
-    },
-    "l69j": {
-        "en": "12 caliber silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "762 mm sniper ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
     },
     "l6y1": {
         "en": "12 caliber buckshot",
         "ru": "\u0434\u0440\u043e\u0431\u044c 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "ljpq": {
         "en": "polyhedron",
@@ -1988,16 +2596,16 @@
         "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u043e\u0439 \u0440\u044e\u043a\u0437\u0430\u043a tri-zip"
     },
     "ly1kq": {
         "en": "surefire socom556-rc2 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c surefire socom556-rc2"
     },
     "ly1lo": {
-        "en": "7.62 nato pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62 nato pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "762 nato pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 762 nato pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "ly1vo": {
         "en": "kobra extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043a\u043e\u0431\u0440\u0430"
     },
     "ly29k": {
         "en": "worn l96a1",
@@ -2028,33 +2636,57 @@
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fma td grip"
     },
     "ly4ok": {
         "en": "handguard for saiga-12k",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u043b\u044f \u0441\u0430\u0439\u0433\u0430-12\u043a"
     },
     "ly4qj": {
-        "en": "hq issue mini laser sight (green laser)",
-        "ru": "hq issue mini laser sight (\u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "hq issue mini laser sight green laser",
+        "ru": "hq issue mini laser sight \u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "ly4z2": {
         "en": "acecare optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 acecare"
     },
+    "lyg3q": {
+        "en": "legend",
+        "ru": "\u043b\u0435\u0433\u0435\u043d\u0434\u0430"
+    },
+    "lyg6q": {
+        "en": "lich",
+        "ru": "\u043b\u0438\u0447"
+    },
+    "lygg2": {
+        "en": "hexcam mist camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam mist"
+    },
+    "lygnq": {
+        "en": "guardian",
+        "ru": "\u0445\u0440\u0430\u043d\u0438\u0442\u0435\u043b\u044c"
+    },
+    "lygp2": {
+        "en": "m90 urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 urban"
+    },
+    "lygro": {
+        "en": "shear camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043a\u043e\u043b"
+    },
+    "lygwk": {
+        "en": "olive armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043e\u043b\u0438\u0432\u043a\u043e\u0432\u0430\u044f"
+    },
     "lyj2k": {
         "en": "zarya-b suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0437\u0430\u0440\u044f-\u0431"
     },
     "lyj4o": {
         "en": "worn amethyst",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043c\u0435\u0442\u0438\u0441\u0442"
     },
-    "lyjmo": {
-        "en": "nord group assault trooper",
-        "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u0438\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434"
-    },
     "lyjvk": {
         "en": "ah-3 seeker suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "lyjzk": {
         "en": "worn reaper suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0436\u043d\u0435\u0446"
@@ -2063,32 +2695,52 @@
         "en": "ash-12",
         "ru": "\u0430\u0448-12"
     },
     "lyl7j": {
         "en": "worn m16a2",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u0430\u044f m16a2"
     },
+    "lylg2": {
+        "en": "handmade",
+        "ru": "\u0441\u0430\u043c\u043e\u0434\u0435\u043b"
+    },
     "lyljj": {
         "en": "m4 lb",
         "ru": "m4 lb"
     },
     "lynkj": {
         "en": "jiden extra energy drink",
         "ru": "\u044d\u043d\u0435\u0440\u0433\u0435\u0442\u0438\u043a \u0436\u0438\u0434\u0435\u043d\u044c extra"
     },
     "lynrj": {
         "en": "3rd class antidote",
         "ru": "\u0430\u043d\u0442\u0438\u0434\u043e\u0442 \u0442\u0440\u0435\u0442\u044c\u0435\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
+    "lyo1j": {
+        "en": "hexcam mist camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam mist"
+    },
+    "lyo4j": {
+        "en": "m90 urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 urban"
+    },
+    "lyo52": {
+        "en": "olive weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u043e\u043b\u0438\u0432\u043a\u043e\u0432\u0430\u044f"
+    },
+    "lyol1": {
+        "en": "shear camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043a\u043e\u043b"
+    },
     "lyr3k": {
         "en": "strange crate",
         "ru": "\u0441\u0442\u0440\u0430\u043d\u043d\u044b\u0439 \u044f\u0449\u0438\u043a"
     },
     "lyv22": {
-        "en": "hunter\u2019s machete",
+        "en": "hunters machete",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043c\u0430\u0447\u0435\u0442\u0435"
     },
     "lyvv2": {
         "en": "twitcher",
         "ru": "\u0442\u0432\u0438\u0447\u0435\u0440"
     },
     "m023j": {
@@ -2111,73 +2763,113 @@
         "en": "skat-10 armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043a\u0430\u0442-10"
     },
     "m06my": {
         "en": "bandit suit with gas mask",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441 \u043f\u0440\u043e\u0442\u0438\u0432\u043e\u0433\u0430\u0437\u043e\u043c"
     },
-    "m06o2": {
-        "en": "khors group zivcas",
-        "ru": "zivcas \u0433\u0440\u0443\u043f\u043f\u044b \u0445\u043e\u0440\u0441"
-    },
     "m06vy": {
         "en": "mis-116 emerald",
         "ru": "\u043a\u0438\u043c-116 \u0438\u0437\u0443\u043c\u0440\u0443\u0434"
     },
     "m0g22": {
         "en": "browning extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d browning"
     },
     "m0g77": {
         "en": "kochetov mount for patriot with picatinny rail",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u043a\u043e\u0447\u0435\u0442\u043e\u0432\u0430 \u043f\u0430\u0442\u0440\u0438\u043e\u0442 \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "m0gv2": {
-        "en": "7.62 bakelite clip",
-        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62"
+        "en": "762 bakelite clip",
+        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762"
+    },
+    "m0jyj": {
+        "en": "premium for 1 day",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 1 \u0434\u0435\u043d\u044c"
     },
     "m0kd7": {
         "en": "vortex collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 vortex"
     },
     "m0kny": {
-        "en": "b-10m handguard (bottom rail)",
-        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-10\u043c (\u043d\u0438\u0436\u043d\u044f\u044f \u043f\u043b\u0430\u043d\u043a\u0430)"
+        "en": "b-10m handguard bottom rail",
+        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-10\u043c \u043d\u0438\u0436\u043d\u044f\u044f \u043f\u043b\u0430\u043d\u043a\u0430"
+    },
+    "m0lmr": {
+        "en": "upsilon data",
+        "ru": "\u0438\u043f\u0441\u0438\u043b\u043e\u043d \u0434\u0430\u043d\u043d\u044b\u0435"
     },
     "m0m7j": {
         "en": "smg nut",
         "ru": "\u043f\u043f \u043e\u0440\u0435\u0445"
     },
     "m0mo7": {
         "en": "vsk-94",
         "ru": "\u0432\u0441\u043a-94"
     },
+    "m0n27": {
+        "en": "geleteika camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0435\u043b\u0435\u0442\u0435\u0439\u043a\u0430"
+    },
+    "m0ngj": {
+        "en": "volumehex wave camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex wave"
+    },
+    "m0nkj": {
+        "en": "erdl arvn yellow camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn yellow"
+    },
+    "m0nyk": {
+        "en": "gray weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0441\u0435\u0440\u0430\u044f"
+    },
     "m0pqj": {
         "en": "1st class psy-blocker",
         "ru": "\u043f\u0441\u0438-\u0431\u043b\u043e\u043a\u0430\u0434\u0430 \u043f\u0435\u0440\u0432\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "m0v5k": {
         "en": "bone knife",
         "ru": "\u043a\u043e\u0441\u0442\u044f\u043d\u043e\u0439 \u043d\u043e\u0436"
     },
     "m0vmk": {
         "en": "ax",
         "ru": "\u0442\u043e\u043f\u043e\u0440"
     },
+    "m0z9k": {
+        "en": "erdl arvn yellow camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn yellow"
+    },
+    "m0zjr": {
+        "en": "oasis guardian",
+        "ru": "\u0445\u0440\u0430\u043d\u0438\u0442\u0435\u043b\u044c \u043e\u0430\u0437\u0438\u0441\u0430"
+    },
+    "m0zpr": {
+        "en": "burst of color",
+        "ru": "\u0432\u0437\u0440\u044b\u0432 \u043a\u0440\u0430\u0441\u043e\u043a"
+    },
+    "m0zq2": {
+        "en": "geleteika camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0435\u043b\u0435\u0442\u0435\u0439\u043a\u0430"
+    },
+    "m0zwy": {
+        "en": "gray armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0441\u0435\u0440\u0430\u044f"
+    },
+    "m0zzk": {
+        "en": "volumehex wave camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex wave"
+    },
     "m3pk": {
         "en": "freezer container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u043e\u043b\u043e\u0442\u0443\u043d"
     },
     "mj07": {
-        "en": "5.45 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c"
-    },
-    "mj1j": {
-        "en": "7.62 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "545 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c"
     },
     "mr13y": {
         "en": "red fly agaric",
         "ru": "\u0440\u0436\u0430\u0432\u044b\u0439 \u043c\u0443\u0445\u043e\u043c\u043e\u0440"
     },
     "mr1jy": {
         "en": "remains of scientific equipment",
@@ -2203,22 +2895,58 @@
         "en": "emches machete",
         "ru": "\u043c\u0430\u0447\u0435\u0442\u0435 \u044d\u043c\u0447\u0435\u0441"
     },
     "n42y9": {
         "en": "steel tiger karambit",
         "ru": "\u043a\u0435\u0440\u0430\u043c\u0431\u0438\u0442 steel tiger"
     },
+    "n4519": {
+        "en": "erdl stinger camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl stinger"
+    },
+    "n4559": {
+        "en": "flecktarn camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn"
+    },
+    "n45lw": {
+        "en": "secureops",
+        "ru": "\u0441\u043f\u0435\u0446\u043e\u0445\u0440\u0430\u043d\u0430"
+    },
+    "n45vw": {
+        "en": "psycho",
+        "ru": "\u043f\u0441\u0438\u0445"
+    },
+    "n45w2": {
+        "en": "russian digital camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0440\u0443\u0441\u0441\u043a\u0430\u044f \u0446\u0438\u0444\u0440\u0430"
+    },
+    "n4lo6": {
+        "en": "premium for 3 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 3 \u0434\u043d\u044f"
+    },
     "n4m93": {
         "en": "\u043c\u0440-412",
         "ru": "\u043c\u0440-412"
     },
     "n4md3": {
         "en": "hk xm8s",
         "ru": "hk xm8s"
     },
+    "n4o96": {
+        "en": "flecktarn camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn"
+    },
+    "n4op3": {
+        "en": "russian digital camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0440\u0443\u0441\u0441\u043a\u0430\u044f \u0446\u0438\u0444\u0440\u0430"
+    },
+    "n4oz6": {
+        "en": "erdl stinger camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl stinger"
+    },
     "n4qd3": {
         "en": "trijicon collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 trijicon"
     },
     "n4r21": {
         "en": "mis-x atlas",
         "ru": "\u043a\u0438\u043c-\u0445 \u0430\u0442\u043b\u0430\u0441"
@@ -2232,41 +2960,37 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u043f\u0435\u0440\u0435\u0441\u043c\u0435\u0448\u043d\u0438\u043a"
     },
     "n4ry1": {
         "en": "worn osh protective suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043e\u0448"
     },
     "n4z22": {
-        "en": "pm/pb extended clip",
-        "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043c/\u043f\u0431"
+        "en": "pmpb extended clip",
+        "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043c\u043f\u0431"
     },
     "n4zp2": {
         "en": "beretta extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d beretta"
     },
     "nkgl1": {
         "en": "formaldehyde",
         "ru": "\u0444\u043e\u0440\u043c\u0430\u043b\u0438\u043d"
     },
     "nkgv1": {
         "en": "piece of infernal coal",
         "ru": "\u043a\u0443\u0441\u043e\u043a \u0430\u0434\u0441\u043a\u043e\u0433\u043e \u0443\u0433\u043b\u044f"
     },
     "nl43": {
-        "en": "5.45 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "545 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "nlk3": {
         "en": "10 mm ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 10 \u043c\u043c"
     },
-    "nln6": {
-        "en": "large-caliber silver ammo",
-        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
-    },
     "nv43": {
         "en": "npa backpack",
         "ru": "\u0440\u044e\u043a\u0437\u0430\u043a npa"
     },
     "nvpw": {
         "en": "flare grenade",
         "ru": "\u0441\u0437\u0433 \u0432\u0441\u043f\u044b\u0448\u043a\u0430"
@@ -2275,18 +2999,14 @@
         "en": "kzs-2u",
         "ru": "\u043a\u0437\u0441-2\u0443"
     },
     "odq0": {
         "en": "sports bag",
         "ru": "\u0441\u043f\u043e\u0440\u0442\u0438\u0432\u043d\u0430\u044f \u0441\u0443\u043c\u043a\u0430"
     },
-    "ok01m": {
-        "en": "khors group tank",
-        "ru": "\u0442\u0430\u043d\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0445\u043e\u0440\u0441"
-    },
     "ok096": {
         "en": "mis-122 amethyst",
         "ru": "\u043a\u0438\u043c-122 \u0430\u043c\u0435\u0442\u0438\u0441\u0442"
     },
     "ok0m6": {
         "en": "bandit suit with gas tanks",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441 \u0431\u0430\u043b\u043b\u043e\u043d\u0430\u043c\u0438"
@@ -2300,21 +3020,33 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u0440\u043e\u043c\u0438\u043b\u0430"
     },
     "ok570": {
         "en": "ris rail for smg-91 kedr",
         "ru": "\u043f\u043b\u0430\u043d\u043a\u0430 ris \u043d\u0430 \u043f\u043f-91 \u043a\u0435\u0434\u0440"
     },
     "ok59m": {
-        "en": "5.45 pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45 pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "545 pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 545 pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "ok5vm": {
         "en": "colt extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d colt"
     },
+    "ok65o": {
+        "en": "volumehex pink camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex pink"
+    },
+    "ok6jo": {
+        "en": "erdl red camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl red"
+    },
+    "ok6v0": {
+        "en": "urban quadricolor camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0447\u0435\u0442\u044b\u0440\u0435\u0445\u0446\u0432\u0435\u0442\u043d\u044b\u0439"
+    },
     "ok995": {
         "en": "diversion knife",
         "ru": "\u0434\u0438\u0432\u0435\u0440\u0441\u0438\u043e\u043d\u043d\u044b\u0439 \u043d\u043e\u0436"
     },
     "ok9m5": {
         "en": "hammer",
         "ru": "\u043c\u043e\u043b\u043e\u0442\u043e\u043a"
@@ -2335,54 +3067,70 @@
         "en": "steyr aug 9 mm",
         "ru": "steyr aug 9mm"
     },
     "okm20": {
         "en": "hk psg1",
         "ru": "hk psg1"
     },
+    "okrno": {
+        "en": "premium for 2 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 2 \u0434\u043d\u044f"
+    },
     "okv0o": {
         "en": "m16a2",
         "ru": "m16a2"
     },
+    "okyd4": {
+        "en": "stove",
+        "ru": "\u043f\u0435\u0447\u044c"
+    },
+    "okyg5": {
+        "en": "erdl red camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl red"
+    },
+    "okypm": {
+        "en": "urban quadricolor camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0447\u0435\u0442\u044b\u0440\u0435\u0445\u0446\u0432\u0435\u0442\u043d\u044b\u0439"
+    },
+    "okyy5": {
+        "en": "volumehex pink camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex pink"
+    },
     "olz36": {
         "en": "spool of copper wire",
         "ru": "\u043c\u043e\u0442\u043e\u043a \u043c\u0435\u0434\u043d\u043e\u0439 \u043f\u0440\u043e\u0432\u043e\u043b\u043e\u043a\u0438"
     },
     "olzo6": {
         "en": "delta data block",
         "ru": "\u0431\u043b\u043e\u043a \u0434\u0430\u043d\u043d\u044b\u0445 \u0434\u0435\u043b\u044c\u0442\u0430"
     },
     "olzr6": {
         "en": "beta data fragment",
         "ru": "\u0444\u0440\u0430\u0433\u043c\u0435\u043d\u0442 \u0434\u0430\u043d\u043d\u044b\u0445 \u0431\u0435\u0442\u0430"
     },
     "ork0": {
-        "en": "5.45 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
-    },
-    "orzo": {
-        "en": "9x39 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "545 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "p062": {
-        "en": "5.45 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
+        "en": "545 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "p0j2": {
         "en": "10 mm incendiary ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 10 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
-    "p0n6": {
-        "en": "12.7x55 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "p2r5": {
         "en": "m84",
         "ru": "m84"
     },
+    "p60o6": {
+        "en": "premium for 5 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 5 \u0434\u043d\u0435\u0439"
+    },
     "p611d": {
         "en": "spiked club",
         "ru": "\u0448\u0438\u043f\u0430\u0441\u0442\u0430\u044f \u0434\u0443\u0431\u0438\u043d\u043a\u0430"
     },
     "p613d": {
         "en": "m9 bayonet knife",
         "ru": "\u0448\u0442\u044b\u043a-\u043d\u043e\u0436 m9"
@@ -2423,33 +3171,65 @@
         "en": "ratcatcher exoarmor",
         "ru": "\u044d\u043a\u0437\u043e\u0431\u0440\u043e\u043d\u044f \u043a\u0440\u044b\u0441\u043e\u043b\u043e\u0432"
     },
     "p6mrw": {
         "en": "worn fleece protective suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0440\u0441\u0430"
     },
+    "p6og6": {
+        "en": "flecktarn suburban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn suburban"
+    },
+    "p6or2": {
+        "en": "gravel camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0440\u0430\u0432\u0438\u0439"
+    },
+    "p6oy6": {
+        "en": "erdl streetfighter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl streetfighter"
+    },
     "p6qz2": {
         "en": "black regalia",
         "ru": "\u0447\u0435\u0440\u043d\u044b\u0439 \u0440\u0435\u0433\u0430\u043b\u0438\u0439"
     },
     "p6r26": {
         "en": "fn f2000",
         "ru": "fn f2000"
     },
+    "p6w05": {
+        "en": "secureops",
+        "ru": "\u0441\u043f\u0435\u0446\u043e\u0445\u0440\u0430\u043d\u0430"
+    },
+    "p6w25": {
+        "en": "habolog",
+        "ru": "habolog"
+    },
+    "p6wq4": {
+        "en": "gravel camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0440\u0430\u0432\u0438\u0439"
+    },
+    "p6wwd": {
+        "en": "flecktarn suburban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn suburban"
+    },
+    "p6wzd": {
+        "en": "erdl streetfighter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl streetfighter"
+    },
     "p6y14": {
         "en": "fort-12 extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0444\u043e\u0440\u0442-12"
     },
     "p6y72": {
         "en": "adaptive ris rail for dp",
         "ru": "\u0430\u0434\u0430\u043f\u0442\u0438\u0432\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 ris \u0434\u043b\u044f \u0434\u043f"
     },
     "p6yr4": {
-        "en": "g3/m1a drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d g3/m1a"
+        "en": "g3m1a drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d g3m1a"
     },
     "p92d": {
         "en": "hive container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0443\u043b\u0435\u0439"
     },
     "p99d": {
         "en": "iu-2 container",
@@ -2495,24 +3275,52 @@
         "en": "fn scar ssr",
         "ru": "fn scar ssr"
     },
     "qj2zk": {
         "en": "aa-12",
         "ru": "aa-12"
     },
+    "qj419": {
+        "en": "full metal",
+        "ru": "\u0446\u0435\u043b\u044c\u043d\u043e\u043c\u0435\u0442\u0430\u043b\u043b\u0438\u0447\u0435\u0441\u043a\u0438\u0439"
+    },
+    "qj444": {
+        "en": "hexcam jungle camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam jungle"
+    },
+    "qj454": {
+        "en": "m90 night camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 night"
+    },
+    "qj499": {
+        "en": "anarchist",
+        "ru": "\u0430\u043d\u0430\u0440\u0445\u0438\u0441\u0442"
+    },
+    "qj4lj": {
+        "en": "white armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0431\u0435\u043b\u0430\u044f"
+    },
+    "qj4m9": {
+        "en": "steel hunter",
+        "ru": "\u0441\u0442\u0430\u043b\u044c\u043d\u043e\u0439 \u043e\u0445\u043e\u0442\u043d\u0438\u043a"
+    },
+    "qj4q3": {
+        "en": "wave camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0432\u043e\u043b\u043d\u0430"
+    },
     "qj9q6": {
         "en": "3rd class psy-blocker",
         "ru": "\u043f\u0441\u0438-\u0431\u043b\u043e\u043a\u0430\u0434\u0430 \u0442\u0440\u0435\u0442\u044c\u0435\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "qj9y6": {
         "en": "2nd class antidote",
         "ru": "\u0430\u043d\u0442\u0438\u0434\u043e\u0442 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "qjg24": {
-        "en": "sapper\u2019s shovel",
+        "en": "sappers shovel",
         "ru": "\u0441\u0430\u043f\u0435\u0440\u043d\u0430\u044f \u043b\u043e\u043f\u0430\u0442\u0430"
     },
     "qjgg4": {
         "en": "frozen ice pick",
         "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043b\u0435\u0434\u043e\u0440\u0443\u0431"
     },
     "qjo2j": {
@@ -2535,25 +3343,41 @@
         "en": "worn iolite",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0438\u043e\u043b\u0438\u0442"
     },
     "qjoz3": {
         "en": "bear exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u043c\u0435\u0434\u0432\u0435\u0434\u044c"
     },
+    "qjpn4": {
+        "en": "white weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0431\u0435\u043b\u0430\u044f"
+    },
+    "qjpr6": {
+        "en": "m90 night camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 night"
+    },
+    "qjpvk": {
+        "en": "wave camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0432\u043e\u043b\u043d\u0430"
+    },
+    "qjpw6": {
+        "en": "hexcam jungle camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam jungle"
+    },
     "qjqw9": {
         "en": "standard tools",
         "ru": "\u0441\u0442\u0430\u043d\u0434\u0430\u0440\u0442\u043d\u044b\u0435 \u0438\u043d\u0441\u0442\u0440\u0443\u043c\u0435\u043d\u0442\u044b"
     },
     "qjr3j": {
         "en": "m1a with picatinny rail handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 m1a \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "qjr43": {
-        "en": "fortis shift vertical tactical grip, black",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical, \u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "fortis shift vertical tactical grip black",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical \u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "qjrk4": {
         "en": "elcan optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 elcan"
     },
     "qjrw4": {
         "en": "tulip optical sight",
@@ -2568,24 +3392,24 @@
         "ru": "spectre m4"
     },
     "qjw5j": {
         "en": "ots-33 stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u043e\u0446-33"
     },
     "qjw7k": {
-        "en": "sks bracket\u2014dovetail joint",
+        "en": "sks bracketdovetail joint",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u0441\u043a\u0441 - \u043b\u0430\u0441\u0442\u043e\u0447\u043a\u0438\u043d \u0445\u0432\u043e\u0441\u0442"
     },
     "qjwg3": {
-        "en": "ergonomic clip for vss/val",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u044d\u0440\u0433\u043e\u043d\u043e\u043c\u0438\u0447\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441/\u0432\u0430\u043b"
+        "en": "ergonomic clip for vssval",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u044d\u0440\u0433\u043e\u043d\u043e\u043c\u0438\u0447\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441\u0432\u0430\u043b"
     },
     "qjwq9": {
-        "en": "ash-12/mts-558 silencer",
-        "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0448-12/\u043c\u0446-558"
+        "en": "ash-12mts-558 silencer",
+        "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0448-12\u043c\u0446-558"
     },
     "qjwv3": {
         "en": "aa-12 drum clip",
         "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d aa-12"
     },
     "qm0k": {
         "en": "large-caliber ammo",
@@ -2619,25 +3443,21 @@
         "en": "pieces of copper wire",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u043c\u0435\u0434\u043d\u043e\u0439 \u043f\u0440\u043e\u0432\u043e\u043b\u043e\u043a\u0438"
     },
     "rj6ov": {
         "en": "chlorinex",
         "ru": "\u0445\u043b\u043e\u0440\u043d\u0438\u043a"
     },
-    "ro6g": {
-        "en": "5.45 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "row5": {
         "en": "12 caliber hunting round",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u044c\u044f \u043f\u0443\u043b\u044f 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "rw03g": {
-        "en": "hq issue low-profile laser sight (red laser)",
-        "ru": "hq issue low-profile laser sight (\u043a\u0440\u0430\u0441\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "hq issue low-profile laser sight red laser",
+        "ru": "hq issue low-profile laser sight \u043a\u0440\u0430\u0441\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "rw06v": {
         "en": "fab defense g3-rs handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 fab defence g3-rs"
     },
     "rw09v": {
         "en": "sks tactical grip",
@@ -2648,15 +3468,15 @@
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 bering optics"
     },
     "rw0ky": {
         "en": "tapco vertical grip",
         "ru": "\u0432\u0435\u0440\u0442\u0438\u043a\u0430\u043b\u044c\u043d\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 tapco"
     },
     "rw1mg": {
-        "en": "\u201chercules\u201d",
+        "en": "hercules",
         "ru": "\u0433\u0435\u0440\u043a\u0443\u043b\u0435\u0441"
     },
     "rw1vg": {
         "en": "1st class thermoblock",
         "ru": "\u0442\u0435\u0440\u043c\u043e\u0431\u0430\u0440\u044c\u0435\u0440 \u043f\u0435\u0440\u0432\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "rw23l": {
@@ -2675,38 +3495,78 @@
         "en": "rapier",
         "ru": "\u0440\u0430\u043f\u0438\u0440\u0430"
     },
     "rw2d5": {
         "en": "mcmillan cs5",
         "ru": "mcmillan cs5"
     },
+    "rw32l": {
+        "en": "ice shard",
+        "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043e\u0441\u043a\u043e\u043b\u043e\u043a"
+    },
     "rw4ry": {
-        "en": "5.56 nato emag drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato emag"
+        "en": "556 nato emag drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato emag"
     },
     "rw4zy": {
         "en": "smg-2000 clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043f-2000"
     },
+    "rw90g": {
+        "en": "erdl arvn red camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn red"
+    },
+    "rw94g": {
+        "en": "volumehex flora camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flora"
+    },
+    "rw9pz": {
+        "en": "brown weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u0430\u044f"
+    },
+    "rw9r5": {
+        "en": "specter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440"
+    },
     "rwgl5": {
         "en": "mis-100 garnet",
         "ru": "\u043a\u0438\u043c-100 \u0433\u0440\u0430\u043d\u0430\u0442"
     },
     "rwgmg": {
         "en": "hounds exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u043e\u043d\u0447\u0438\u0439"
     },
+    "rwk1l": {
+        "en": "magma",
+        "ru": "\u043c\u0430\u0433\u043c\u0430"
+    },
+    "rwkkz": {
+        "en": "volumehex flora camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flora"
+    },
+    "rwklv": {
+        "en": "brown armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043a\u043e\u0440\u0438\u0447\u043d\u0435\u0432\u0430\u044f"
+    },
+    "rwkol": {
+        "en": "forest sprite",
+        "ru": "\u043b\u0435\u0448\u0438\u0439"
+    },
+    "rwkvy": {
+        "en": "specter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440"
+    },
+    "rwkyz": {
+        "en": "erdl arvn red camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn red"
+    },
     "rwn2v": {
         "en": "tourist suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0442\u0443\u0440\u0438\u0441\u0442"
     },
-    "rwn5y": {
-        "en": "nord group exoskeleton",
-        "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434"
-    },
     "rwnqv": {
         "en": "damaged ah-3 seeker suit",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "rwnrv": {
         "en": "gorka-3 suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u043e\u0440\u043a\u0430-3"
@@ -2715,14 +3575,18 @@
         "en": "mis-105 topaz",
         "ru": "\u043a\u0438\u043c-105 \u0442\u043e\u043f\u0430\u0437"
     },
     "rwrgg": {
         "en": "old hk g3a1",
         "ru": "\u0441\u0442\u0430\u0440\u0430\u044f hk g3a1"
     },
+    "rwrkz": {
+        "en": "incandescent",
+        "ru": "\u043d\u0430\u043a\u0430\u043b"
+    },
     "rwrng": {
         "en": "an-94 abakan",
         "ru": "\u0430\u043d-94 \u0430\u0431\u0430\u043a\u0430\u043d"
     },
     "rwz2z": {
         "en": "russian bayonet",
         "ru": "\u0440\u0443\u0441\u0441\u043a\u0438\u0439 \u0448\u0442\u044b\u043a"
@@ -2736,16 +3600,16 @@
         "ru": "\u0440\u0438\u0442\u0443\u0430\u043b\u044c\u043d\u044b\u0439 \u0442\u043e\u043f\u043e\u0440"
     },
     "rwzzz": {
         "en": "6h9 knife",
         "ru": "\u043d\u043e\u0436 6\u04459"
     },
     "vdjd": {
-        "en": "5.45 mm sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0431\u043f"
+        "en": "545 mm sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0441\u0431\u043f"
     },
     "vdnd": {
         "en": "tank of combustible mixture",
         "ru": "\u0431\u0430\u043b\u043b\u043e\u043d \u0441 \u0433\u043e\u0440\u044e\u0447\u0435\u0439 \u0441\u043c\u0435\u0441\u044c\u044e"
     },
     "vj12r": {
         "en": "worm armored suit",
@@ -2771,33 +3635,69 @@
         "en": "m48 tomahawk",
         "ru": "m48 tomahawk"
     },
     "vj497": {
         "en": "cossack shashka",
         "ru": "\u043a\u0430\u0437\u0430\u0447\u044c\u044f \u0448\u0430\u0448\u043a\u0430"
     },
+    "vj5kn": {
+        "en": "flecktarn forest camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn forest"
+    },
+    "vj5ln": {
+        "en": "erdl urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl urban"
+    },
+    "vj5rd": {
+        "en": "birch tree camouflage 1943 model",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440 1943 \u0433"
+    },
     "vjd5n": {
         "en": "premium for 7 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 7 \u0434\u043d\u0435\u0439"
     },
     "vjl4p": {
-        "en": "mp-133/mp-153 clip extender",
-        "ru": "\u0443\u0434\u043b\u0438\u043d\u0438\u0442\u0435\u043b\u044c \u043c\u0430\u0433\u0430\u0437\u0438\u043d\u0430 \u043c\u0440-133/\u043c\u0440-153"
+        "en": "mp-133mp-153 clip extender",
+        "ru": "\u0443\u0434\u043b\u0438\u043d\u0438\u0442\u0435\u043b\u044c \u043c\u0430\u0433\u0430\u0437\u0438\u043d\u0430 \u043c\u0440-133\u043c\u0440-153"
     },
     "vjl7d": {
         "en": "sight mount for m16a2",
         "ru": "\u043a\u0440\u0435\u043f\u043b\u0435\u043d\u0438\u0435 \u043f\u0440\u0438\u0446\u0435\u043b\u0430 \u0434\u043b\u044f m16a2"
     },
+    "vjm3p": {
+        "en": "birch tree camouflage 1943 model",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440 1943 \u0433"
+    },
+    "vjmdg": {
+        "en": "prophet",
+        "ru": "\u043f\u0440\u043e\u0440\u043e\u043a"
+    },
+    "vjmm7": {
+        "en": "flecktarn forest camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn forest"
+    },
+    "vjmv7": {
+        "en": "erdl urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl urban"
+    },
+    "vjmyg": {
+        "en": "spectre",
+        "ru": "spectre"
+    },
     "vjp5r": {
         "en": "tactical stock for sks",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u043e\u0435 \u043b\u043e\u0436\u0435 \u0434\u043b\u044f \u0441\u043a\u0441"
     },
     "vjpzd": {
-        "en": "pk-01(t) collimator sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01(\u0442)"
+        "en": "pk-01t collimator sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01\u0442"
+    },
+    "vjrm7": {
+        "en": "uz",
+        "ru": "\u0443\u0437"
     },
     "vjy3n": {
         "en": "epinephrine",
         "ru": "\u044d\u043f\u0438\u043d\u0435\u0444\u0440\u0438\u043d"
     },
     "vn0dr": {
         "en": "hard drives",
@@ -2811,18 +3711,14 @@
         "en": "remains of a radio transmitter",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u0440\u0430\u0434\u0438\u043e\u043f\u0435\u0440\u0435\u0434\u0430\u0442\u0447\u0438\u043a\u0430"
     },
     "vyrg": {
         "en": "m84 qd",
         "ru": "m84 qd"
     },
-    "w20p": {
-        "en": "large-caliber silver ammo",
-        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
-    },
     "w23o": {
         "en": "9x39 mm sp-5 ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u043f-5"
     },
     "w3022": {
         "en": "gamma group tracker",
         "ru": "\u043c\u0430\u044f\u0447\u043e\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0433\u0430\u043c\u043c\u0430"
@@ -2836,15 +3732,15 @@
         "ru": "\u0431\u0435\u043b\u0438\u0447\u044c\u0438 \u0434\u0440\u043e\u0436\u0436\u0438"
     },
     "w3zj3": {
         "en": "modified anomalous battery",
         "ru": "\u043c\u043e\u0434\u0438\u0444\u0438\u0446\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u0430\u044f \u0430\u043d\u043e\u043c\u0430\u043b\u044c\u043d\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "w4wz": {
-        "en": "bear\u2019s den \u2014 4 container",
+        "en": "bears den  4 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-4"
     },
     "wg3p": {
         "en": "disintegrator",
         "ru": "\u0434\u0435\u0437\u0438\u043d\u0442\u0435\u0433\u0440\u0430\u0442\u043e\u0440"
     },
     "wg53": {
@@ -2852,15 +3748,15 @@
         "ru": "\u0430\u0442\u043e\u043c"
     },
     "wg62": {
         "en": "night star",
         "ru": "\u043d\u043e\u0447\u043d\u0430\u044f \u0437\u0432\u0435\u0437\u0434\u0430"
     },
     "wglp": {
-        "en": "mama\u2019s beads",
+        "en": "mamas beads",
         "ru": "\u043c\u0430\u043c\u0438\u043d\u044b \u0431\u0443\u0441\u044b"
     },
     "wgr3": {
         "en": "black crystal",
         "ru": "\u0447\u0435\u0440\u043d\u044b\u0439 \u043a\u0440\u0438\u0441\u0442\u0430\u043b\u043b"
     },
     "wgvd": {
@@ -2959,14 +3855,46 @@
         "en": "mis-85d",
         "ru": "\u043a\u0438\u043c-85\u0434"
     },
     "wjlrd": {
         "en": "cheap tools",
         "ru": "\u0434\u0435\u0448\u0435\u0432\u044b\u0435 \u0438\u043d\u0441\u0442\u0440\u0443\u043c\u0435\u043d\u0442\u044b"
     },
+    "wjm03": {
+        "en": "digital tiger camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0446\u0438\u0444\u0440\u043e\u0432\u043e\u0439 \u0442\u0438\u0433\u0440"
+    },
+    "wjm2d": {
+        "en": "supersonic",
+        "ru": "\u0441\u0432\u0435\u0440\u0445\u0437\u0432\u0443\u043a\u043e\u0432\u043e\u0439"
+    },
+    "wjm4d": {
+        "en": "metal scrap",
+        "ru": "\u0436\u0435\u043b\u0435\u0437\u044f\u043a\u0430"
+    },
+    "wjml3": {
+        "en": "toadwhite camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430 - \u0431\u0435\u043b\u044b\u0439"
+    },
+    "wjmmz": {
+        "en": "dpm woodland a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm woodland a"
+    },
+    "wjmoz": {
+        "en": "a-tacs wn camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs wn"
+    },
+    "wjmvz": {
+        "en": "belgian jigsaw camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 belgian jigsaw"
+    },
+    "wjmwd": {
+        "en": "rune master",
+        "ru": "\u043c\u0430\u0433\u0438\u0441\u0442\u0440 \u0440\u0443\u043d"
+    },
     "wjo4p": {
         "en": "a-545",
         "ru": "\u0430-545"
     },
     "wjo5p": {
         "en": "worn aks-74u",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043a\u0441-74\u0443"
@@ -2975,14 +3903,22 @@
         "en": "worn aks-74",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043a\u0441-74"
     },
     "wjogp": {
         "en": "sig sg 550",
         "ru": "sig sg 550"
     },
+    "wjomz": {
+        "en": "rasta man",
+        "ru": "\u0440\u0430\u0441\u0442\u0430\u043c\u0430\u043d"
+    },
+    "wjooz": {
+        "en": "hellfire",
+        "ru": "\u0445\u0440\u0435\u043d\u043e\u0441\u0442\u0440\u0435\u043b"
+    },
     "wjp1z": {
         "en": "trijicon acog optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 trijicon acog"
     },
     "wjp5o": {
         "en": "bsa reflex collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 bsa reflex"
@@ -3000,16 +3936,16 @@
         "ru": "\u0446\u0435\u0432\u044c\u0435 caa rs-21"
     },
     "wjr3d": {
         "en": "9 mm barrel extension",
         "ru": "\u0443\u0434\u043b\u0438\u043d\u0435\u043d\u043d\u044b\u0439 \u0441\u0442\u0432\u043e\u043b 9 \u043c\u043c"
     },
     "wjr63": {
-        "en": "5.45 clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "wjr9d": {
         "en": "salvo 12 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c salvo 12"
     },
     "wjrdo": {
         "en": "clamp with ris rail",
@@ -3020,25 +3956,53 @@
         "ru": "vg6 epsilon 556 muzzle brake"
     },
     "wjrld": {
         "en": "silencer for ots-14 groza",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0434\u043b\u044f \u043e\u0446-14 \u0433\u0440\u043e\u0437\u0430"
     },
     "wjro3": {
-        "en": "5.56 nato drum clip, khaki",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato, \u0445\u0430\u043a\u0438"
+        "en": "556 nato drum clip khaki",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato \u0445\u0430\u043a\u0438"
     },
     "wjry2": {
         "en": "zm high standard ak stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 zm high standard ak"
     },
+    "wjvk2": {
+        "en": "blue armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0441\u0438\u043d\u044f\u044f"
+    },
     "wjw9p": {
         "en": "2nd class antirad",
         "ru": "\u0430\u043d\u0442\u0438\u0440\u0430\u0434 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
+    "wjy7o": {
+        "en": "digital tiger camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0446\u0438\u0444\u0440\u043e\u0432\u043e\u0439 \u0442\u0438\u0433\u0440"
+    },
+    "wjyoo": {
+        "en": "toadwhite camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430 - \u0431\u0435\u043b\u044b\u0439"
+    },
+    "wjypp": {
+        "en": "belgian jigsaw camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 belgian jigsaw"
+    },
+    "wjyqp": {
+        "en": "a-tacs wn camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs wn"
+    },
+    "wjyrp": {
+        "en": "dpm woodland a camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm woodland a"
+    },
+    "wjyzz": {
+        "en": "blue weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0441\u0438\u043d\u044f\u044f"
+    },
     "y32gk": {
         "en": "worn m40a5",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u0430\u044f m40a5"
     },
     "y32j0": {
         "en": "beretta 93r",
         "ru": "beretta 93r"
@@ -3091,22 +4055,54 @@
         "en": "worn jaeger",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0435\u0433\u0435\u0440\u044c"
     },
     "y35q0": {
         "en": "coat and hat",
         "ru": "\u043f\u0430\u043b\u044c\u0442\u043e \u0441\u043e \u0448\u043b\u044f\u043f\u043e\u0439"
     },
+    "y362o": {
+        "en": "ridge camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0440\u044f\u0434\u0430"
+    },
+    "y367o": {
+        "en": "toad camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430"
+    },
+    "y36lz": {
+        "en": "dpm white camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm white"
+    },
+    "y36mz": {
+        "en": "dpm urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm urban"
+    },
+    "y36pz": {
+        "en": "digital-b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 digital-b"
+    },
+    "y36y0": {
+        "en": "light blue weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0433\u043e\u043b\u0443\u0431\u0430\u044f"
+    },
     "y375z": {
         "en": "as val",
         "ru": "\u0430\u0441 \u0432\u0430\u043b"
     },
+    "y3770": {
+        "en": "hellbringer",
+        "ru": "\u0445\u0440\u0435\u043d\u043e\u0440\u0435\u0437\u043a\u0430"
+    },
     "y37dz": {
         "en": "smg-19-01 vityaz",
         "ru": "\u043f\u043f-19-01 \u0432\u0438\u0442\u044f\u0437\u044c"
     },
+    "y37o0": {
+        "en": "pine",
+        "ru": "\u0441\u043e\u0441\u043d\u0430"
+    },
     "y37qz": {
         "en": "tdi kriss vector",
         "ru": "tdi kriss vector"
     },
     "y37wz": {
         "en": "walther mpk",
         "ru": "walther mpk"
@@ -3128,64 +4124,92 @@
         "ru": "\u043e\u0431\u043b\u0435\u0433\u0447\u0435\u043d\u043d\u044b\u0439 \u043f\u0440\u0438\u043a\u043b\u0430\u0434 m4"
     },
     "y3m3w": {
         "en": "3 port mini compensator",
         "ru": "3 port mini compensator"
     },
     "y3m4w": {
-        "en": "citadel 5.45 mbc",
-        "ru": "\u0434\u0442\u043a \u0446\u0438\u0442\u0430\u0434\u0435\u043b\u044c 5.45"
+        "en": "citadel 545 mbc",
+        "ru": "\u0434\u0442\u043a \u0446\u0438\u0442\u0430\u0434\u0435\u043b\u044c 545"
     },
     "y3m6k": {
         "en": "m4 buttstock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 m4 buttstock"
     },
     "y3m73": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "y3mdo": {
         "en": "guiding ris for shotgun",
         "ru": "\u043d\u0430\u043f\u0440\u0430\u0432\u043b\u044f\u044e\u0449\u0430\u044f ris \u0434\u043b\u044f \u0434\u0440\u043e\u0431\u043e\u0432\u0438\u043a\u043e\u0432"
     },
     "y3mgw": {
         "en": "fa556 mini silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c fa556 mini"
     },
     "y3mj3": {
-        "en": "5.45 plastic clip",
-        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 plastic clip",
+        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "y3mnw": {
         "en": "atg silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0442\u0433"
     },
     "y3mp0": {
-        "en": "compact protective rail, black",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430,\u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "compact protective rail black",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430\u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "y3nmw": {
         "en": "spare parts",
         "ru": "\u0437\u0430\u043f\u0430\u0441\u043d\u044b\u0435 \u0434\u0435\u0442\u0430\u043b\u0438"
     },
+    "y3o03": {
+        "en": "ridge camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0433\u0440\u044f\u0434\u0430"
+    },
+    "y3o70": {
+        "en": "dpm white camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm white"
+    },
+    "y3okw": {
+        "en": "mercury",
+        "ru": "\u043c\u0435\u0440\u043a\u0443\u0440\u0438\u0439"
+    },
+    "y3on3": {
+        "en": "toad camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430"
+    },
+    "y3oo0": {
+        "en": "dpm urban camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm urban"
+    },
+    "y3oqw": {
+        "en": "mark v",
+        "ru": "mark v"
+    },
+    "y3ov0": {
+        "en": "digital-b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 digital-b"
+    },
     "y3pm0": {
         "en": "posp optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u043e\u0441\u043f"
     },
     "y3pnk": {
         "en": "fal quad rail",
         "ru": "fal quad rail"
     },
     "y3po3": {
         "en": "grip for ots-14 groza",
         "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 \u0434\u043b\u044f \u043e\u0446-14 \u0433\u0440\u043e\u0437\u0430"
     },
     "y3prz": {
-        "en": "an/peq 15 tactical unit, black",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "anpeq 15 tactical unit black",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "y3pwo": {
         "en": "okp-7 collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043e\u043a\u043f-7"
     },
     "y3pyk": {
         "en": "fab defense ak handguard",
@@ -3203,14 +4227,18 @@
         "en": "worn ah-6 nomad",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043e-6 \u043a\u043e\u0447\u0435\u0432\u043d\u0438\u043a"
     },
     "y3qyw": {
         "en": "nvg o1m",
         "ru": "\u043f\u043d\u0432 \u043e1\u043c"
     },
+    "y3vrk": {
+        "en": "light blue armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0433\u043e\u043b\u0443\u0431\u0430\u044f"
+    },
     "y405k": {
         "en": "seeds",
         "ru": "\u0441\u0435\u043c\u0435\u0447\u043a\u0438"
     },
     "y409k": {
         "en": "gamma data block",
         "ru": "\u0431\u043b\u043e\u043a \u0434\u0430\u043d\u043d\u044b\u0445 \u0433\u0430\u043c\u043c\u0430"
@@ -3255,49 +4283,41 @@
         "en": "prism",
         "ru": "\u043f\u0440\u0438\u0437\u043c\u0430"
     },
     "y5yw": {
         "en": "spring",
         "ru": "\u043f\u0440\u0443\u0436\u0438\u043d\u0430"
     },
-    "y90z": {
-        "en": "9x39 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "y94o": {
-        "en": "7.62 mm sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0431\u043f"
+        "en": "762 mm sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0441\u0431\u043f"
     },
     "yqq0": {
         "en": "kzs-1u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0437\u0441-1\u0443"
     },
     "yw7k": {
         "en": "sn-2u leglet",
         "ru": "\u0441\u043d-2\u0443 \u043d\u043e\u0436\u043a\u0430"
     },
-    "z102": {
-        "en": "5.56 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "z13n": {
-        "en": "7.62 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "762 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "z1zn": {
         "en": "9 mm incendiary ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "z301y": {
         "en": "flowering northern moss",
         "ru": "\u0446\u0432\u0435\u0442\u0443\u0449\u0438\u0439 \u0441\u0435\u0432\u0435\u0440\u043d\u044b\u0439 \u043c\u043e\u0445"
     },
     "z30mm": {
-        "en": "notes of major d.",
-        "ru": "\u0437\u0430\u043f\u0438\u0441\u0438 \u043c\u0430\u0439\u043e\u0440\u0430 \u0434."
+        "en": "notes of major d",
+        "ru": "\u0437\u0430\u043f\u0438\u0441\u0438 \u043c\u0430\u0439\u043e\u0440\u0430 \u0434"
     },
     "z30my": {
         "en": "flowering red fern",
         "ru": "\u0446\u0432\u0435\u0442\u0443\u0449\u0438\u0439 \u0440\u044b\u0436\u0438\u0439 \u043f\u0430\u043f\u043e\u0440\u043e\u0442\u043d\u0438\u043a"
     },
     "z30qy": {
         "en": "blue yeast",
@@ -3403,18 +4423,50 @@
         "en": "franchi spas-12",
         "ru": "franchi spas-12"
     },
     "zz2wy": {
         "en": "m1a fa",
         "ru": "m1a fa"
     },
+    "zz66k": {
+        "en": "dpm pecoc camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm pecoc"
+    },
+    "zz67k": {
+        "en": "erdl winter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl winter"
+    },
+    "zz6j9": {
+        "en": "mechatronics",
+        "ru": "\u043c\u0435\u0445\u0430\u0442\u0440\u043e\u043d\u0438\u043a\u0430"
+    },
+    "zz6km": {
+        "en": "surpat camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442"
+    },
+    "zz6q9": {
+        "en": "hell rider",
+        "ru": "hell rider"
+    },
+    "zz6vk": {
+        "en": "hexagon-b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-b"
+    },
+    "zz6wm": {
+        "en": "kazakhstan digital camouflage",
+        "ru": "\u0446\u0438\u0444\u0440\u043e\u0432\u043e\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043a\u0430\u0437\u0430\u0445\u0441\u0442\u0430\u043d\u0430"
+    },
     "zz742": {
         "en": "aek-919k kashtan",
         "ru": "\u0430\u0435\u043a-919\u043a \u043a\u0430\u0448\u0442\u0430\u043d"
     },
+    "zz76k": {
+        "en": "black rose",
+        "ru": "\u0447\u0435\u0440\u043d\u0430\u044f \u0440\u043e\u0437\u0430"
+    },
     "zz7d2": {
         "en": "smg-19 bizon-2-01",
         "ru": "\u043f\u043f-19 \u0431\u0438\u0437\u043e\u043d-2-01"
     },
     "zz7j2": {
         "en": "hk g36c",
         "ru": "hk g36c"
@@ -3432,32 +4484,32 @@
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 mp5 \u043d\u0435\u0441\u043a\u043b\u0430\u0434\u043d\u043e\u0439"
     },
     "zz939": {
         "en": "whirlwind mbc",
         "ru": "\u0434\u0442\u043a \u0432\u0438\u0445\u0440\u044c"
     },
     "zz96m": {
-        "en": "5.56 nato pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 nato pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "zz9dn": {
         "en": "side bracket with picatinny rail",
         "ru": "\u0431\u043e\u043a\u043e\u0432\u043e\u0439 \u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "zz9k9": {
         "en": "osprey silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c osprey"
     },
     "zz9ny": {
         "en": "izhmash plastic stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0438\u0436\u043c\u0430\u0448 \u043f\u043e\u043b\u0438\u043c\u0435\u0440\u043d\u044b\u0439"
     },
     "zz9pk": {
-        "en": "compact protective rail, olive",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u043e\u043b\u0438\u0432\u0430"
+        "en": "compact protective rail olive",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u043e\u043b\u0438\u0432\u0430"
     },
     "zz9z9": {
         "en": "hera arms cc compensator",
         "ru": "hera arms cc compensator"
     },
     "zzjgn": {
         "en": "albatross infiltrator armored exoskeleton",
@@ -3483,14 +4535,38 @@
         "en": "razor",
         "ru": "\u0431\u0440\u0438\u0442\u0432\u0430"
     },
     "zzlvm": {
         "en": "flamethrower",
         "ru": "\u043e\u0433\u043d\u0435\u043c\u0435\u0442"
     },
+    "zzn2n": {
+        "en": "kazakhstan digital camouflage",
+        "ru": "\u0446\u0438\u0444\u0440\u043e\u0432\u043e\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043a\u0430\u0437\u0430\u0445\u0441\u0442\u0430\u043d\u0430"
+    },
+    "zzn7n": {
+        "en": "surpat camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442"
+    },
+    "zzn92": {
+        "en": "dpm pecoc camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm pecoc"
+    },
+    "zznok": {
+        "en": "yellow weapon paint",
+        "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0436\u0435\u043b\u0442\u0430\u044f"
+    },
+    "zznp2": {
+        "en": "hexagon-b camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-b"
+    },
+    "zznr2": {
+        "en": "erdl winter camouflage",
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl winter"
+    },
     "zzp4n": {
         "en": "trijicon collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 trijicon"
     },
     "zzp5k": {
         "en": "trijicon acog optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 trijicon acog"
@@ -3504,36 +4580,40 @@
         "ru": "\u043b\u0430\u0437\u0435\u0440\u043d\u044b\u0439 \u0446\u0435\u043b\u0435\u0443\u043a\u0430\u0437\u0430\u0442\u0435\u043b\u044c \u043a\u043b\u0435\u0449-2\u043f\u0441"
     },
     "zzpoy": {
         "en": "b-11 handguard with upper rail",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-11 \u0441 \u0432\u0435\u0440\u0445\u043d\u0435\u0439 \u043f\u043b\u0430\u043d\u043a\u043e\u0439"
     },
     "zzpvm": {
-        "en": "reg fab defense tactical grip, khaki",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence, \u0445\u0430\u043a\u0438"
+        "en": "reg fab defense tactical grip khaki",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence \u0445\u0430\u043a\u0438"
     },
     "zzpwy": {
         "en": "mp5 with picatinny rail handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 mp5 \u0441 \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "zzpyn": {
         "en": "kobra collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043a\u043e\u0431\u0440\u0430"
     },
     "zzqk2": {
         "en": "bandage",
         "ru": "\u0431\u0438\u043d\u0442"
     },
     "zzr39": {
-        "en": "fab defense ag-47 grip, khaki",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0445\u0430\u043a\u0438"
+        "en": "fab defense ag-47 grip khaki",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0445\u0430\u043a\u0438"
     },
     "zzrw9": {
-        "en": "fab defense agr-43 grip, green",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
+        "en": "fab defense agr-43 grip green",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
+    },
+    "zzvmy": {
+        "en": "yellow armor paint",
+        "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0436\u0435\u043b\u0442\u0430\u044f"
     },
     "zzy1n": {
         "en": "altyn set",
         "ru": "\u043a\u043e\u043c\u043f\u043b\u0435\u043a\u0442 \u0430\u043b\u0442\u044b\u043d"
     },
     "zzy2y": {
         "en": "reaper suit",
```

### Comparing `stalcraft_api-0.2.6/stalcraft/data/ru/listing.json` & `stalcraft_api-0.3.0/stalcraft/data/ru/listing.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9450757575757576%*

 * *Differences: {"'00959'": "{'en': 'devils nettle'}",*

 * * "'0r52r'": "OrderedDict([('ru', 'ветка рябины'), ('en', 'rowan branch')])",*

 * * "'0r631'": "{'en': 'specterdirt camouflage'}",*

 * * "'0rp3y'": "{'ru': 'магазин 556 pufgun черный', 'en': '556 pufgun clip black'}",*

 * * "'0rpqy'": "{'ru': 'пластиковый магазин 762', 'en': '762 plastic clip'}",*

 * * "'0ryly'": "{'en': 'specterdirt camouflage'}",*

 * * "'1n91'": "{'ru': 'патрон 762 мм', 'en': '762 mm ammo'}",*

 * * "'1r2l6'": "{'en': 'astrixin'}",*

 * * "'1r362'": "{'ru': 'магазин 556 nato stanag', 'en […]*

```diff
@@ -1,10 +1,10 @@
 {
     "00959": {
-        "en": "devil\u2019s nettle",
+        "en": "devils nettle",
         "ru": "\u0434\u044c\u044f\u0432\u043e\u043b\u044c\u0441\u043a\u0430\u044f \u043a\u0440\u0430\u043f\u0438\u0432\u0430"
     },
     "009n9": {
         "en": "burning crappite",
         "ru": "\u043f\u043e\u043b\u044b\u0445\u0430\u044e\u0449\u0438\u0439 \u0441\u0440\u0430\u0447\u043d\u0438\u043a"
     },
     "009o9": {
@@ -15,18 +15,14 @@
         "en": "game bag",
         "ru": "\u044f\u0433\u0434\u0442\u0430\u0448"
     },
     "0o01": {
         "en": "gauss rifle charger",
         "ru": "\u0430\u043a\u043a\u0443\u043c\u0443\u043b\u044f\u0442\u043e\u0440 \u0434\u043b\u044f \u0433\u0430\u0443\u0441\u0441-\u043f\u0443\u0448\u043a\u0438"
     },
-    "0o9d": {
-        "en": "5.56 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "0or1": {
         "en": "12 caliber live ammo",
         "ru": "\u0431\u043e\u0435\u0432\u0430\u044f \u043f\u0443\u043b\u044f 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "0r211": {
         "en": "crye precision six12",
         "ru": "crye precision six12"
@@ -51,16 +47,20 @@
         "en": "worn ah-3 seeker suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "0r4q9": {
         "en": "mis-113 iolite",
         "ru": "\u043a\u0438\u043c-113 \u0438\u043e\u043b\u0438\u0442"
     },
+    "0r52r": {
+        "en": "rowan branch",
+        "ru": "\u0432\u0435\u0442\u043a\u0430 \u0440\u044f\u0431\u0438\u043d\u044b"
+    },
     "0r631": {
-        "en": "specter\u2014dirt camouflage",
+        "en": "specterdirt camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440 - \u043f\u043e\u0447\u0432\u0430"
     },
     "0r6jk": {
         "en": "pink weapon paint",
         "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0440\u043e\u0437\u043e\u0432\u0430\u044f"
     },
     "0r6pd": {
@@ -80,20 +80,20 @@
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u0432\u0430\u043d\u0433\u0430\u0440\u0434"
     },
     "0rnw1": {
         "en": "mis-102 zircon",
         "ru": "\u043a\u0438\u043c-102 \u0446\u0438\u0440\u043a\u043e\u043d"
     },
     "0rp3y": {
-        "en": "5.56 pufgun clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 pufgun, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 pufgun clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 pufgun \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "0rpqy": {
-        "en": "7.62 plastic clip",
-        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62"
+        "en": "762 plastic clip",
+        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762"
     },
     "0rq2k": {
         "en": "ice pick",
         "ru": "\u043b\u0435\u0434\u043e\u0440\u0443\u0431"
     },
     "0rqkk": {
         "en": "fiery greeting",
@@ -116,15 +116,15 @@
         "ru": "\u043b\u043e\u0436\u0435 springfield m1a pacs"
     },
     "0rydr": {
         "en": "chaplain",
         "ru": "\u043a\u0430\u043f\u0435\u043b\u043b\u0430\u043d"
     },
     "0ryly": {
-        "en": "specter\u2014dirt camouflage",
+        "en": "specterdirt camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043f\u0435\u043a\u0442\u0440 - \u043f\u043e\u0447\u0432\u0430"
     },
     "0rymk": {
         "en": "erdl arvn sv camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn sv"
     },
     "0ryor": {
@@ -179,65 +179,61 @@
         "en": "crystal thorn",
         "ru": "\u043a\u0440\u0438\u0441\u0442\u0430\u043b\u044c\u043d\u0430\u044f \u043a\u043e\u043b\u044e\u0447\u043a\u0430"
     },
     "1kv2": {
         "en": "gravi",
         "ru": "\u0433\u0440\u0430\u0432\u0438"
     },
-    "1n16": {
-        "en": "12 caliber silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "1n91": {
-        "en": "7.62 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c"
+        "en": "762 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c"
     },
     "1nr1": {
         "en": "9 mm armor-piercing ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "1p2r": {
         "en": "kzs-3u",
         "ru": "\u043a\u0437\u0441-3\u0443"
     },
     "1r1j6": {
         "en": "m203",
         "ru": "m203"
     },
     "1r2l6": {
-        "en": "\u201castrixin\u201d",
+        "en": "astrixin",
         "ru": "\u0430\u0441\u0442\u0440\u0438\u043a\u0446\u0438\u043d"
     },
     "1r2o6": {
         "en": "scientific first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u043d\u0430\u0443\u0447\u043d\u0430\u044f"
     },
     "1r351": {
         "en": "ris bracket-rail",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d-\u043f\u043b\u0430\u043d\u043a\u0430 ris"
     },
     "1r362": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "1r39q": {
-        "en": "akademia t\u2019ma flash suppressor",
+        "en": "akademia tma flash suppressor",
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c akademia \u0442\u044c\u043c\u0430"
     },
     "1r3j2": {
-        "en": "7.62x39 drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62x39"
+        "en": "762x39 drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762x39"
     },
     "1r3rq": {
         "en": "diamondhead compensator",
         "ru": "diamondhead compensator"
     },
     "1r3vr": {
-        "en": "protective rail, khaki",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0445\u0430\u043a\u0438"
+        "en": "protective rail khaki",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0445\u0430\u043a\u0438"
     },
     "1r62q": {
         "en": "dead anarchist",
         "ru": "\u043c\u0435\u0440\u0442\u0432\u044b\u0439 \u0430\u043d\u0430\u0440\u0445\u0438\u0441\u0442"
     },
     "1r66r": {
         "en": "dpm oj camouflage",
@@ -252,24 +248,24 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0440\u044f"
     },
     "1r6mr": {
         "en": "a-tacs au camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs au"
     },
     "1r6o2": {
-        "en": "bhutan\u2014cliff edge camouflage",
+        "en": "bhutancliff edge camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043a\u0430\u043b\u0438\u0441\u0442\u044b\u0439 \u0431\u0435\u0440\u0435\u0433"
     },
     "1r6pq": {
         "en": "prototype",
         "ru": "\u043f\u0440\u043e\u0442\u043e\u0442\u0438\u043f"
     },
     "1r731": {
-        "en": "kbk wz. 88 tantal",
-        "ru": "kbk wz. 88 tantal"
+        "en": "kbk wz 88 tantal",
+        "ru": "kbk wz 88 tantal"
     },
     "1r742": {
         "en": "bm-16",
         "ru": "\u0431\u043c-16"
     },
     "1r756": {
         "en": "viper",
@@ -288,15 +284,15 @@
         "ru": "\u043f\u043c"
     },
     "1r7g1": {
         "en": "steyr aug a3",
         "ru": "steyr aug a3"
     },
     "1r7rg": {
-        "en": "mosin\u2019s carbine",
+        "en": "mosins carbine",
         "ru": "\u043a\u0430\u0440\u0430\u0431\u0438\u043d \u043c\u043e\u0441\u0438\u043d\u0430"
     },
     "1r7v1": {
         "en": "imi mini uzi",
         "ru": "imi mini uzi"
     },
     "1rd56": {
@@ -320,23 +316,23 @@
         "ru": "\u0434\u043f"
     },
     "1rj7r": {
         "en": "project 6x4",
         "ru": "\u0438\u0437\u0434\u0435\u043b\u0438\u0435 6\u04454"
     },
     "1rj9g": {
-        "en": "eternal novice\u2019s pm",
+        "en": "eternal novices pm",
         "ru": "\u043f\u043c \u0432\u0435\u0447\u043d\u043e\u0433\u043e \u043d\u043e\u0432\u0438\u0447\u043a\u0430"
     },
     "1rjjr": {
         "en": "old sickle",
         "ru": "\u0441\u0442\u0430\u0440\u044b\u0439 \u0441\u0435\u0440\u043f"
     },
     "1rjqr": {
-        "en": "butcher\u2019s hook",
+        "en": "butchers hook",
         "ru": "\u043c\u044f\u0441\u043d\u0438\u0446\u043a\u0438\u0439 \u043a\u0440\u044e\u043a"
     },
     "1rk6g": {
         "en": "coat with face covering",
         "ru": "\u043a\u0443\u0440\u0442\u043a\u0430 \u0441 \u043f\u043e\u0432\u044f\u0437\u043a\u043e\u0439"
     },
     "1rk7g": {
@@ -368,15 +364,15 @@
         "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043a\u0440\u0430\u0441\u043d\u0430\u044f"
     },
     "1rp4q": {
         "en": "night-vision goggles",
         "ru": "\u043f\u0440\u0438\u0431\u043e\u0440 \u043d\u043e\u0447\u043d\u043e\u0433\u043e \u0432\u0438\u0434\u0435\u043d\u0438\u044f"
     },
     "1rpl6": {
-        "en": "item.arm.granite.name",
+        "en": "granite super-heavy armored suit",
         "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u0440\u0430\u043d\u0438\u0442"
     },
     "1rvg1": {
         "en": "eotech collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 eotech"
     },
     "1rvlg": {
@@ -404,28 +400,28 @@
         "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u043a\u0440\u0430\u0441\u043d\u0430\u044f"
     },
     "1ry71": {
         "en": "tempest camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0440\u044f"
     },
     "1ryd1": {
-        "en": "bhutan\u2014cliff edge camouflage",
+        "en": "bhutancliff edge camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043a\u0430\u043b\u0438\u0441\u0442\u044b\u0439 \u0431\u0435\u0440\u0435\u0433"
     },
     "1ryv6": {
         "en": "a-tacs au camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs au"
     },
     "1ryz6": {
         "en": "m90 threat camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 threat"
     },
     "1rz9q": {
-        "en": "fab defense ag-47 grip, black",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "fab defense ag-47 grip black",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "21365": {
         "en": "lim",
         "ru": "\u043b\u0438\u043c"
     },
     "21g9l": {
         "en": "infernal coal",
@@ -440,16 +436,16 @@
         "ru": "\u043c\u0430\u044f\u0447\u043e\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0431\u0435\u0442\u0430"
     },
     "29dm": {
         "en": "f-1",
         "ru": "\u0444-1"
     },
     "2o2wl": {
-        "en": "val/vss receiver cover",
-        "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u0432\u0430\u043b/\u0432\u0441\u0441"
+        "en": "valvss receiver cover",
+        "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u0432\u0430\u043b\u0432\u0441\u0441"
     },
     "2o2y6": {
         "en": "rusak collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u0440\u0443\u0441\u0430\u043a"
     },
     "2o405": {
         "en": "palm amoeba camouflage",
@@ -491,22 +487,22 @@
         "en": "rpk-16",
         "ru": "\u0440\u043f\u043a-16"
     },
     "2opw0": {
         "en": "premium for 30 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 30 \u0434\u043d\u0435\u0439"
     },
-    "2oq55": {
-        "en": "nord-22 group assault trooper",
-        "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u0438\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "2oqdl": {
         "en": "fleece protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0440\u0441\u0430"
     },
+    "2oqjl": {
+        "en": "oracles berill",
+        "ru": "\u0431\u0435\u0440\u0438\u043b\u043b \u043e\u0440\u0430\u043a\u0443\u043b\u0430"
+    },
     "2oqll": {
         "en": "jaeger exoarmor",
         "ru": "\u044d\u043a\u0437\u043e\u0431\u0440\u043e\u043d\u044f \u0435\u0433\u0435\u0440\u044c"
     },
     "2oqnl": {
         "en": "ah-1 drifter suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-1 \u0431\u0440\u043e\u0434\u044f\u0433\u0430"
@@ -520,16 +516,16 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl woodland"
     },
     "2own6": {
         "en": "palm amoeba camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u0430\u043b\u044c\u043c\u043e\u0432\u0430\u044f \u0430\u043c\u0435\u0431\u0430"
     },
     "2p16": {
-        "en": "5.56 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
+        "en": "556 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "2pr6": {
         "en": "tank of combustible mixture",
         "ru": "\u0431\u0430\u043b\u043b\u043e\u043d \u0441 \u0433\u043e\u0440\u044e\u0447\u0435\u0439 \u0441\u043c\u0435\u0441\u044c\u044e"
     },
     "2vvv": {
         "en": "kzs-3",
@@ -571,32 +567,32 @@
         "en": "captured erbsenmuster camouflage",
         "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erbsenmuster"
     },
     "3g69l": {
         "en": "skat-9b armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043a\u0430\u0442-9\u0431"
     },
+    "3g6ll": {
+        "en": "oracles worm",
+        "ru": "\u0447\u0435\u0440\u0432\u044c \u043e\u0440\u0430\u043a\u0443\u043b\u0430"
+    },
     "3g6nl": {
         "en": "currant ghillie suit",
         "ru": "\u043c\u0430\u0441\u043a\u0438\u0440\u043e\u0432\u043e\u0447\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043c\u043e\u0440\u043e\u0434\u0438\u043d\u0430"
     },
     "3g6rl": {
         "en": "hoplite armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u043e\u043f\u043b\u0438\u0442"
     },
-    "3g6y5": {
-        "en": "nord-22 group exoskeleton",
-        "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "3g7wg": {
         "en": "dm collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 dm"
     },
     "3g991": {
-        "en": "butcher\u2019s knife",
+        "en": "butchers knife",
         "ru": "\u043c\u044f\u0441\u043d\u0438\u0446\u043a\u0438\u0439 \u043d\u043e\u0436"
     },
     "3g9n1": {
         "en": "aluminum club",
         "ru": "\u0430\u043b\u044e\u043c\u0438\u043d\u0438\u0435\u0432\u0430\u044f \u0431\u0438\u0442\u0430"
     },
     "3gdoz": {
@@ -627,34 +623,34 @@
         "en": "mts-558 extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0434\u043b\u044f \u043c\u0446-558"
     },
     "3grk1": {
         "en": "test prototype rmo-93",
         "ru": "\u0442\u0435\u0441\u0442\u043e\u0432\u044b\u0439 \u043e\u0431\u0440\u0430\u0437\u0435\u0446 \u0440\u043c\u043e-93"
     },
+    "3gv2z": {
+        "en": "premium for 90 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 90 \u0434\u043d\u0435\u0439"
+    },
     "3v4g": {
-        "en": "5.56 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "556 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "3vog": {
-        "en": "12.7x55 ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c"
+        "en": "127x55 ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c"
     },
     "49dj": {
         "en": "berloga-6u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-6\u0443"
     },
     "49gj": {
         "en": "kzs-4",
         "ru": "\u043a\u0437\u0441-4"
     },
-    "4d5p": {
-        "en": "12.7x55 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "4dkn": {
         "en": "9x39 mm sp-6 ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u043f-6"
     },
     "4k3qo": {
         "en": "concentrated limboplasma",
         "ru": "\u043a\u043e\u043d\u0446\u0435\u043d\u0442\u0440\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u0430\u044f \u043b\u0438\u043c\u0431\u043e\u043f\u043b\u0430\u0437\u043c\u0430"
@@ -832,28 +828,28 @@
         "ru": "\u043e\u0446-14\u043c \u0448\u0442\u043e\u0440\u043c"
     },
     "4qnyn": {
         "en": "ptrd-m",
         "ru": "\u043f\u0442\u0440\u0434-\u043c"
     },
     "4qp0o": {
-        "en": "5.56 nato drum clip, black",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 nato drum clip black",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "4qp1o": {
-        "en": "5.45 drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "4qp4n": {
         "en": "clamp with 3 ris rails",
         "ru": "\u0445\u043e\u043c\u0443\u0442 \u0441 \u0442\u0440\u0435\u043c\u044f \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 ris"
     },
     "4qp7l": {
-        "en": "psuzv-11tm.12 imkas",
-        "ru": "i\u043c\u043a\u0430\u0441 \u043f\u0441\u0443\u0437\u0432\u201311\u0442\u043c.12"
+        "en": "psuzv-11tm12 imkas",
+        "ru": "i\u043c\u043a\u0430\u0441 \u043f\u0441\u0443\u0437\u043211\u0442\u043c12"
     },
     "4qpjr": {
         "en": "aps stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0430\u043f\u0441"
     },
     "4qpkl": {
         "en": "ash-12 standard barrel",
@@ -884,20 +880,16 @@
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0441\u043e"
     },
     "4qvyn": {
         "en": "valday collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u0432\u0430\u043b\u0434\u0430\u0439"
     },
     "5250": {
-        "en": "7.62 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
-    },
-    "526g": {
-        "en": "7.62 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "762 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "52l0": {
         "en": "9 mm sbp ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0431\u043f"
     },
     "553qq": {
         "en": "nuclear gelatin",
@@ -924,16 +916,16 @@
         "ru": "\u043c\u043e\u0434\u0438\u0444\u0438\u0446\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u044b\u0439 \u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442"
     },
     "5l1yg": {
         "en": "raps ah-6 nomad",
         "ru": "\u0443\u043a\u0430\u0437 \u0430\u043e-6 \u043a\u043e\u0447\u0435\u0432\u043d\u0438\u043a"
     },
     "5l4o4": {
-        "en": "fab defense agr-43 grip, khaki",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0445\u0430\u043a\u0438"
+        "en": "fab defense agr-43 grip khaki",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0445\u0430\u043a\u0438"
     },
     "5l6gg": {
         "en": "fn eglm grenade launcher",
         "ru": "\u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442 fn eglm"
     },
     "5l70o": {
         "en": "digital-a camouflage",
@@ -952,15 +944,15 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm red desert"
     },
     "5l7do": {
         "en": "volumehex flake camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flake"
     },
     "5l7oq": {
-        "en": "surpat\u2014urban noise camouflage",
+        "en": "surpaturban noise camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442 - \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0448\u0443\u043c"
     },
     "5l7z4": {
         "en": "one-eyed joe",
         "ru": "\u043e\u0434\u043d\u043e\u0433\u043b\u0430\u0437\u044b\u0439 \u0434\u0436\u043e"
     },
     "5ld1g": {
@@ -1004,15 +996,15 @@
         "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0437\u0435\u043b\u0435\u043d\u0430\u044f"
     },
     "5lj4g": {
         "en": "volumehex flake camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex flake"
     },
     "5ljd0": {
-        "en": "surpat\u2014urban noise camouflage",
+        "en": "surpaturban noise camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u0443\u0440\u043f\u0430\u0442 - \u0433\u043e\u0440\u043e\u0434\u0441\u043a\u043e\u0439 \u0448\u0443\u043c"
     },
     "5ljn0": {
         "en": "field camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u043f\u043e\u043b\u0435"
     },
     "5ljpg": {
@@ -1076,20 +1068,20 @@
         "ru": "\u0434\u0442\u043a-1"
     },
     "5lp61": {
         "en": "m4 paddle stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434-\u0432\u0435\u0441\u043b\u043e m4"
     },
     "5lpdq": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "5lpgq": {
-        "en": "5.45 bakelite clip",
-        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 bakelite clip",
+        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "5lpj1": {
         "en": "wooden skeleton stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u044b\u0439 \u0440\u0430\u043c\u043e\u0447\u043d\u044b\u0439"
     },
     "5lpk0": {
         "en": "ris xm8 rail",
@@ -1100,16 +1092,16 @@
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c lonewolf"
     },
     "5lpo4": {
         "en": "pbs-4",
         "ru": "\u043f\u0431\u0441-4"
     },
     "5lpvo": {
-        "en": "compact protective rail, khaki",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0445\u0430\u043a\u0438"
+        "en": "compact protective rail khaki",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0445\u0430\u043a\u0438"
     },
     "5lpy4": {
         "en": "scar-sd silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c scar-sd"
     },
     "5lr1o": {
         "en": "reinforced cloak",
@@ -1136,28 +1128,28 @@
         "ru": "t\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0441\u0445\u043e\u0434"
     },
     "5lrvq": {
         "en": "damaged jaeger",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u0435\u0433\u0435\u0440\u044c"
     },
     "5lv31": {
-        "en": "akm wooden handguard, black",
-        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u043e\u0435 \u0430\u043a\u043c, \u0447\u0435\u0440\u043d\u043e\u0435"
+        "en": "akm wooden handguard black",
+        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u043e\u0435 \u0430\u043a\u043c \u0447\u0435\u0440\u043d\u043e\u0435"
     },
     "5lv7q": {
-        "en": "reg fab defense tactical grip, gray",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence, \u0441\u0435\u0440\u044b\u0439"
+        "en": "reg fab defense tactical grip gray",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence \u0441\u0435\u0440\u044b\u0439"
     },
     "5lv9o": {
         "en": "sig sauer optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 sig sauer"
     },
     "5lvmg": {
-        "en": "an/peq 15 tactical unit, khaki",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0445\u0430\u043a\u0438"
+        "en": "anpeq 15 tactical unit khaki",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0445\u0430\u043a\u0438"
     },
     "5lvo1": {
         "en": "ris p90 handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 ris p90"
     },
     "5lvpo": {
         "en": "1p77 optical sight",
@@ -1212,20 +1204,20 @@
         "ru": "\u043a\u043e\u0440\u043a\u0430"
     },
     "5wd1": {
         "en": "sn-2 leg",
         "ru": "\u0441\u043d-2 \u043d\u043e\u0433\u0430"
     },
     "63oy": {
-        "en": "5.56 sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0431\u043f"
+        "en": "556 sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0441\u0431\u043f"
     },
     "63yy": {
-        "en": "12.7x55 mm sniper ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
+        "en": "127x55 mm sniper ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
     },
     "65r6": {
         "en": "vog-25 grenade round",
         "ru": "\u0432\u044b\u0441\u0442\u0440\u0435\u043b \u0433\u0440\u0430\u043d\u0430\u0442\u043e\u043c\u0435\u0442\u043d\u044b\u0439 \u0432\u043e\u0433-25"
     },
     "6o7m0": {
         "en": "lambda data fragment",
@@ -1249,15 +1241,15 @@
     },
     "6w0zp": {
         "en": "trump exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u043c\u0430\u0441\u0442\u044c"
     },
     "6w22n": {
         "en": "captured sumpfmuster camouflage 1943 model",
-        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440. 1943 \u0433."
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440 1943 \u0433"
     },
     "6w236": {
         "en": "raider",
         "ru": "\u0440\u0435\u0439\u0434\u0435\u0440"
     },
     "6w256": {
         "en": "lancelot",
@@ -1268,28 +1260,28 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u043b\u043e\u043f\u044c\u044f"
     },
     "6w2dn": {
         "en": "dpm iranian guard camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm iranian guard"
     },
     "6w59j": {
-        "en": "\u201cstrike\u201d",
+        "en": "strike",
         "ru": "\u0443\u0434\u0430\u0440"
     },
     "6w64y": {
-        "en": "grizzly 8.5",
-        "ru": "grizzly 8.5"
+        "en": "grizzly 85",
+        "ru": "grizzly 85"
     },
     "6wj6y": {
         "en": "flakes camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u043b\u043e\u043f\u044c\u044f"
     },
     "6wjkj": {
         "en": "captured sumpfmuster camouflage 1943 model",
-        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440. 1943 \u0433."
+        "ru": "\u0442\u0440\u043e\u0444\u0435\u0439\u043d\u044b\u0439 \u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 sumpfmuster \u043e\u0431\u0440 1943 \u0433"
     },
     "6wjpj": {
         "en": "dpm iranian guard camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm iranian guard"
     },
     "6wpo6": {
         "en": "d-eagle barrel extension",
@@ -1324,20 +1316,20 @@
         "ru": "\u043a\u0432\u0430\u043d\u0442\u043e\u0432\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "77oy6": {
         "en": "remains of a signal processor",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u0441\u0438\u0433\u043d\u0430\u043b\u044c\u043d\u043e\u0433\u043e \u043f\u0440\u043e\u0446\u0435\u0441\u0441\u043e\u0440\u0430"
     },
     "7977": {
-        "en": "5.56 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
+        "en": "556 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "79w7": {
-        "en": "12.7x55 smg ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u043f\u043f"
+        "en": "127x55 smg ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 127x55 \u043c\u043c \u043f\u043f"
     },
     "7l209": {
         "en": "dpm desert camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm desert"
     },
     "7l21j": {
         "en": "snowdrift camouflage",
@@ -1367,14 +1359,18 @@
         "en": "hatchet",
         "ru": "\u0442\u0435\u0441\u0430\u043a"
     },
     "7l6j7": {
         "en": "kobra collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043a\u043e\u0431\u0440\u0430"
     },
+    "7l9d3": {
+        "en": "premium for 180 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 180 \u0434\u043d\u0435\u0439"
+    },
     "7ldn7": {
         "en": "snowdrift camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0445\u0443\u0440\u0442\u043e\u0432\u0438\u043d\u0430"
     },
     "7ldp3": {
         "en": "dpm desert camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm desert"
@@ -1387,18 +1383,14 @@
         "en": "exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442"
     },
     "7lmn6": {
         "en": "houndmaster protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043f\u0441\u0430\u0440\u044c"
     },
-    "7lmqj": {
-        "en": "nord-22 group blizzard-bound",
-        "ru": "\u0438\u0434\u0443\u0449\u0438\u0439 \u0432 \u043c\u0435\u0442\u0435\u043b\u0438 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434-22"
-    },
     "7lmr6": {
         "en": "trapper suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0442\u0440\u0430\u043f\u043f\u0435\u0440"
     },
     "7lnk7": {
         "en": "mts-116m",
         "ru": "\u043c\u0446-116\u043c"
@@ -1416,15 +1408,15 @@
         "ru": "\u0430\u043a-103"
     },
     "7lwvj": {
         "en": "iou from shaman",
         "ru": "\u0440\u0430\u0441\u043f\u0438\u0441\u043a\u0430 \u043e\u0442 \u0448\u0430\u043c\u0430\u043d\u0430"
     },
     "7ly13": {
-        "en": "guide\u2019s first-aid kit",
+        "en": "guides first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u043f\u0440\u043e\u0432\u043e\u0434\u043d\u0438\u043a\u0430"
     },
     "7lzw3": {
         "en": "damaged saturn suit",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0441\u0430\u0442\u0443\u0440\u043d"
     },
     "7yl7": {
@@ -1472,15 +1464,15 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-c"
     },
     "962yw": {
         "en": "bulldozer",
         "ru": "\u0431\u0443\u043b\u044c\u0434\u043e\u0437\u0435\u0440"
     },
     "962zy": {
-        "en": "bhutan\u2014snow camouflage",
+        "en": "bhutansnow camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043d\u0435\u0433"
     },
     "96430": {
         "en": "personal first-aid kit",
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u0438\u043d\u0434\u0438\u0432\u0438\u0434\u0443\u0430\u043b\u044c\u043d\u0430\u044f"
     },
     "9696l": {
@@ -1556,15 +1548,15 @@
         "ru": "\u043c\u043e\u0434\u043d\u0430\u044f \u043a\u0443\u0440\u0442\u043a\u0430"
     },
     "96o1q": {
         "en": "gold weapon paint",
         "ru": "\u043e\u0440\u0443\u0436\u0435\u0439\u043d\u0430\u044f \u043a\u0440\u0430\u0441\u043a\u0430 \u0437\u043e\u043b\u043e\u0442\u0430\u044f"
     },
     "96o9z": {
-        "en": "bhutan\u2014snow camouflage",
+        "en": "bhutansnow camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0443\u0442\u0430\u043d - \u0441\u043d\u0435\u0433"
     },
     "96ol0": {
         "en": "hexagon-c camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexagon-c"
     },
     "96omz": {
@@ -1576,32 +1568,32 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm kuwaiti police"
     },
     "96ov0": {
         "en": "a-tacs fg camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 a-tacs fg"
     },
     "96p2y": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "96p6w": {
         "en": "noveske kx3 flash suppressor",
         "ru": "\u043f\u043b\u0430\u043c\u0435\u0433\u0430\u0441\u0438\u0442\u0435\u043b\u044c noveske kx3"
     },
     "96pkl": {
         "en": "mossberg stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 mossberg"
     },
     "96prz": {
         "en": "bm barrel mount",
         "ru": "\u043d\u0430\u0434\u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0435 \u043a\u0440\u0435\u043f\u043b\u0435\u043d\u0438\u0435 \u0431\u043c"
     },
     "96pvq": {
-        "en": "protective rail, olive",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u043e\u043b\u0438\u0432\u0430"
+        "en": "protective rail olive",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u043e\u043b\u0438\u0432\u0430"
     },
     "96pwy": {
         "en": "30-round clip for ak-308",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0430\u043a-308"
     },
     "96v0y": {
         "en": "magpul afg tactical grip",
@@ -1620,27 +1612,27 @@
         "ru": "\u0446\u0435\u0432\u044c\u0435 ris l85"
     },
     "96w5q": {
         "en": "grabber",
         "ru": "\u0440\u0432\u0430\u0447"
     },
     "96w9q": {
-        "en": "hunter\u2019s knife",
+        "en": "hunters knife",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043d\u043e\u0436"
     },
     "96wwq": {
         "en": "piece of pipe",
         "ru": "\u043a\u0443\u0441\u043e\u043a \u0442\u0440\u0443\u0431\u044b"
     },
     "96y1w": {
         "en": "home-made nvg",
         "ru": "\u043a\u0443\u0441\u0442\u0430\u0440\u043d\u044b\u0439 \u043f\u043d\u0432"
     },
     "96yz0": {
-        "en": "item.arm.reiter.name",
+        "en": "reiter super-heavy armored suit",
         "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0440\u0435\u0439\u0442\u0430\u0440"
     },
     "9d1qy": {
         "en": "anomalous battery",
         "ru": "\u0430\u043d\u043e\u043c\u0430\u043b\u044c\u043d\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "9dk7l": {
@@ -1659,18 +1651,14 @@
         "en": "swamp stone",
         "ru": "\u0431\u043e\u043b\u043e\u0442\u043d\u044b\u0439 \u043a\u0430\u043c\u0435\u043d\u044c"
     },
     "9g6z": {
         "en": "9 mm ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c"
     },
-    "9gk0": {
-        "en": "9 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "9j0l": {
         "en": "candle short range detector",
         "ru": "\u0434\u0435\u0442\u0435\u043a\u0442\u043e\u0440 \u0443\u0437\u043a\u043e\u0433\u043e \u0434\u0438\u0430\u043f\u0430\u0437\u043e\u043d\u0430 \u0441\u0432\u0435\u0447\u0430"
     },
     "9n1w": {
         "en": "stone blood",
         "ru": "\u043a\u0440\u043e\u0432\u044c \u043a\u0430\u043c\u043d\u044f"
@@ -1687,72 +1675,76 @@
         "en": "thorn",
         "ru": "\u043a\u043e\u043b\u044e\u0447\u043a\u0430"
     },
     "9nvy": {
         "en": "quirk",
         "ru": "\u0432\u044b\u0432\u0435\u0440\u0442"
     },
+    "9rkw": {
+        "en": "sak-1 wide range detector",
+        "ru": "\u0434\u0435\u0442\u0435\u043a\u0442\u043e\u0440 \u0448\u0438\u0440\u043e\u043a\u043e\u0433\u043e \u0434\u0438\u0430\u043f\u0430\u0437\u043e\u043d\u0430 \u0441\u0430\u043a-1"
+    },
     "9yyq": {
         "en": "kzs-1 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0437\u0441-1"
     },
     "d1mn": {
-        "en": "5.56 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c"
+        "en": "556 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 556 \u043c\u043c"
     },
     "dkq9": {
         "en": "rgd-5",
         "ru": "\u0440\u0433\u0434-5"
     },
     "dm09j": {
         "en": "ots-14 tactical grip",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u043d\u0430\u043a\u043b\u0430\u0434\u043a\u0430 \u043e\u0446-14"
     },
     "dm0dn": {
-        "en": "pk-01(t/z) collimator sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01(\u0442/\u0437)"
+        "en": "pk-01tz collimator sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01\u0442\u0437"
     },
     "dm195": {
         "en": "premium for 14 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 14 \u0434\u043d\u0435\u0439"
     },
     "dm27n": {
         "en": "increasing ris-rail",
         "ru": "\u043f\u043e\u0432\u044b\u0448\u0430\u044e\u0449\u0430\u044f ris-\u043f\u043b\u0430\u043d\u043a\u0430"
     },
     "dm2q2": {
         "en": "40-ammo emag clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 40-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 emag"
     },
     "dm2v2": {
-        "en": "30-round clip for vss/val",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441/\u0432\u0430\u043b"
+        "en": "30-round clip for vssval",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 30-\u043f\u0430\u0442\u0440\u043e\u043d\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441\u0432\u0430\u043b"
     },
     "dm925": {
         "en": "erdl uscm camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl uscm"
     },
     "dm9qn": {
         "en": "amoeba camouflage 1942 model",
-        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440. 1942 \u0433."
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440 1942 \u0433"
     },
     "dm9w5": {
         "en": "flecktarn frost camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn frost"
     },
     "dmg02": {
         "en": "worn kleptomaniac",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043b\u0435\u043f\u0442\u043e\u043c\u0430\u043d"
     },
     "dmgjj": {
         "en": "healing berill",
         "ru": "\u043b\u0435\u0447\u0435\u0431\u043d\u044b\u0439 \u0431\u0435\u0440\u0438\u043b\u043b"
     },
     "dmgqj": {
-        "en": "hunter\u2019s cloak",
+        "en": "hunters cloak",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043f\u043b\u0430\u0449"
     },
     "dmgvj": {
         "en": "osh protective suit",
         "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043e\u0448"
     },
     "dmgw2": {
@@ -1764,31 +1756,31 @@
         "ru": "\u0430\u043a-308"
     },
     "dmjwn": {
         "en": "hk416",
         "ru": "hk416"
     },
     "dmky5": {
-        "en": "\u201cclearmind+\u201d",
-        "ru": "clearmind+"
+        "en": "clearmind",
+        "ru": "clearmind"
     },
     "dmqzg": {
         "en": "deterioration",
         "ru": "\u0438\u0437\u043d\u043e\u0441"
     },
     "dmvjg": {
         "en": "telescopic baton",
         "ru": "\u0442\u0435\u043b\u0435\u0441\u043a\u043e\u043f\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0434\u0443\u0431\u0438\u043d\u043a\u0430"
     },
     "dmvog": {
         "en": "ka-bar bkr3 tactical knife",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043d\u043e\u0436 ka-bar bkr3"
     },
     "dmvvg": {
-        "en": "swamp dweller\u2019s friend",
+        "en": "swamp dwellers friend",
         "ru": "\u0434\u0440\u0443\u0433 \u0431\u043e\u043b\u043e\u0442\u043d\u0438\u043a\u0430"
     },
     "dmz19": {
         "en": "arctic",
         "ru": "\u0430\u0440\u043a\u0442\u0438\u043a\u0430"
     },
     "dmz4g": {
@@ -1797,30 +1789,30 @@
     },
     "dmzk9": {
         "en": "sinner",
         "ru": "\u0433\u0440\u0435\u0448\u043d\u0438\u043a"
     },
     "dmzy2": {
         "en": "amoeba camouflage 1942 model",
-        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440. 1942 \u0433."
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0430\u043c\u0435\u0431\u0430 \u043e\u0431\u0440 1942 \u0433"
     },
     "dmzzg": {
         "en": "flecktarn frost camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 flecktarn frost"
     },
     "dr61j": {
         "en": "beta data block",
         "ru": "\u0431\u043b\u043e\u043a \u0434\u0430\u043d\u043d\u044b\u0445 \u0431\u0435\u0442\u0430"
     },
     "dr6nj": {
         "en": "red fern",
         "ru": "\u0440\u044b\u0436\u0438\u0439 \u043f\u0430\u043f\u043e\u0440\u043e\u0442\u043d\u0438\u043a"
     },
     "g35n": {
-        "en": "bear\u2019s den \u2014 6 container",
+        "en": "bears den  6 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-6"
     },
     "g3ln": {
         "en": "fridge container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0445\u043e\u043b\u043e\u0434\u0438\u043b\u044c\u043d\u0438\u043a"
     },
     "g400n": {
@@ -1856,35 +1848,35 @@
         "ru": "resistance armament compensator"
     },
     "g426p": {
         "en": "picatinny rail and base",
         "ru": "\u043f\u043b\u0430\u043d\u043a\u0430 \u0441 \u0431\u0430\u0437\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "g42gn": {
-        "en": "protective rail, black",
-        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "protective rail black",
+        "ru": "\u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "g42kg": {
         "en": "js silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c js"
     },
     "g42ng": {
         "en": "kosoi mbc",
         "ru": "\u0434\u0442\u043a \u043a\u043e\u0441\u043e\u0439"
     },
     "g42w5": {
-        "en": "5.56 nato pmag clip, khaki",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato pmag, \u0445\u0430\u043a\u0438"
+        "en": "556 nato pmag clip khaki",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato pmag \u0445\u0430\u043a\u0438"
     },
     "g42z6": {
         "en": "izhmash wooden stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0438\u0436\u043c\u0430\u0448 \u0434\u0435\u0440\u0435\u0432\u044f\u043d\u043d\u044b\u0439"
     },
     "g4310": {
-        "en": "item.arm.chieftain.name",
+        "en": "chieftain super-heavy armored suit",
         "ru": "\u0441\u0432\u0435\u0440\u0445\u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0432\u043e\u0436\u0434\u044c"
     },
     "g43k0": {
         "en": "mule exoskeleton",
         "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u043c\u0443\u043b"
     },
     "g43pg": {
@@ -1936,15 +1928,15 @@
         "ru": "\u0430\u043f\u0442\u0435\u0447\u043a\u0430 \u0430\u0440\u043c\u0435\u0439\u0441\u043a\u0430\u044f"
     },
     "g4m0n": {
         "en": "tt",
         "ru": "\u0442\u0442"
     },
     "g4m2p": {
-        "en": "mosin\u2019s rifle",
+        "en": "mosins rifle",
         "ru": "\u0432\u0438\u043d\u0442\u043e\u0432\u043a\u0430 \u043c\u043e\u0441\u0438\u043d\u0430"
     },
     "g4m46": {
         "en": "sks",
         "ru": "\u0441\u043a\u0441"
     },
     "g4mdp": {
@@ -1976,35 +1968,35 @@
         "ru": "beretta 92fs"
     },
     "g4mz5": {
         "en": "toz-34",
         "ru": "\u0442\u043e\u0437-34"
     },
     "g4q1g": {
-        "en": "fab defense agr-43 grip, black",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "fab defense agr-43 grip black",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "g4qng": {
-        "en": "fab defense ag-47 grip, green",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
+        "en": "fab defense ag-47 grip green",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
     },
     "g4vj5": {
         "en": "rg-6",
         "ru": "\u0440\u0433-6"
     },
     "g4vk6": {
         "en": "dream",
         "ru": "\u043c\u0435\u0447\u0442\u0430"
     },
     "g4vmn": {
         "en": "crowbar",
         "ru": "\u043c\u043e\u043d\u0442\u0438\u0440\u043e\u0432\u043a\u0430"
     },
     "g4vvn": {
-        "en": "new year\u2019s shovel",
+        "en": "new years shovel",
         "ru": "\u043d\u043e\u0432\u043e\u0433\u043e\u0434\u043d\u044f\u044f \u043b\u043e\u043f\u0430\u0442\u0430"
     },
     "g4w0n": {
         "en": "m90 winter camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 winter"
     },
     "g4w15": {
@@ -2087,21 +2079,17 @@
         "en": "m90 winter camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 m90 winter"
     },
     "g54p": {
         "en": "9 mm expanding ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
-    "g590": {
-        "en": "5.45 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "g5np": {
-        "en": "7.62 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
+        "en": "762 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "gd06": {
         "en": "sn-1 pancake",
         "ru": "\u0441\u043d-1 \u0431\u043b\u0438\u043d"
     },
     "gdj6": {
         "en": "elbrus short range detector",
@@ -2187,53 +2175,49 @@
         "en": "smc container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0441\u043c"
     },
     "j456": {
         "en": "12 caliber canister shot",
         "ru": "\u043a\u0430\u0440\u0442\u0435\u0447\u044c 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
-    "j4z7": {
-        "en": "9 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "j52lg": {
-        "en": "7.62 nato pmag clip, khaki",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62 nato pmag, \u0445\u0430\u043a\u0438"
+        "en": "762 nato pmag clip khaki",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 762 nato pmag \u0445\u0430\u043a\u0438"
     },
     "j52q4": {
         "en": "mts-558 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u043c\u0446-558"
     },
     "j52vg": {
         "en": "smg-91 clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043f-91"
     },
     "j561l": {
         "en": "bars optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u0430\u0440\u0441"
     },
     "j562l": {
-        "en": "pilad 3.5x20 optical sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0438\u043b\u0430\u0434 3.5\u044520"
+        "en": "pilad 35x20 optical sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043f\u0438\u043b\u0430\u0434 35\u044520"
     },
     "j569g": {
         "en": "fma dark earth fire transfer grip",
         "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c \u043f\u0435\u0440\u0435\u043d\u043e\u0441\u0430 \u043e\u0433\u043d\u044f fma dark earth"
     },
     "j56d6": {
         "en": "barska collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 barska"
     },
     "j56w0": {
         "en": "an-94 udav handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0443\u0434\u0430\u0432 \u0430\u043d-94"
     },
     "j56y7": {
-        "en": "an/peq 15 tactical unit, black (green laser)",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0447\u0435\u0440\u043d\u044b\u0439 (\u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "anpeq 15 tactical unit black green laser",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0447\u0435\u0440\u043d\u044b\u0439 \u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "j56z0": {
         "en": "m1a stock with picatinny rails",
         "ru": "\u043b\u043e\u0436\u0435 m1a \u0441 \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "j5934": {
         "en": "uss-01",
@@ -2320,15 +2304,15 @@
         "ru": "glock 18c"
     },
     "j5vol": {
         "en": "tanto with a ring",
         "ru": "\u0442\u0430\u043d\u0442\u043e \u0441 \u043a\u043e\u043b\u044c\u0446\u043e\u043c"
     },
     "j5vvl": {
-        "en": "military stalkers\u2019 hatchet",
+        "en": "military stalkers hatchet",
         "ru": "\u0442\u0435\u0441\u0430\u043a \u0432\u043e\u0435\u043d\u0441\u0442\u0430\u043b\u043e\u0432"
     },
     "j5w27": {
         "en": "hexcam opfor camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 hexcam opfor"
     },
     "j5w67": {
@@ -2444,15 +2428,15 @@
         "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0434\u043b\u044f \u043f\u043c"
     },
     "knl30": {
         "en": "fn f2000 tactical",
         "ru": "fn f2000 tactical"
     },
     "knl70": {
-        "en": "cleaner\u2019s aks",
+        "en": "cleaners aks",
         "ru": "\u0430\u043a\u0441 \u0447\u0438\u0441\u0442\u0438\u043b\u044c\u0449\u0438\u043a\u0430"
     },
     "knlgv": {
         "en": "lim",
         "ru": "\u043b\u0438\u043c"
     },
     "knlq0": {
@@ -2473,15 +2457,15 @@
     },
     "knmgj": {
         "en": "colt python",
         "ru": "colt python"
     },
     "knmpy": {
         "en": "worn vss vintorez",
-        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \"\u0432\u0441\u0441 \u0432\u0438\u043d\u0442\u043e\u0440\u0435\u0437\""
+        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0432\u0441\u0441 \u0432\u0438\u043d\u0442\u043e\u0440\u0435\u0437"
     },
     "kno60": {
         "en": "2nd class psy-blocker",
         "ru": "\u043f\u0441\u0438-\u0431\u043b\u043e\u043a\u0430\u0434\u0430 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "knp93": {
         "en": "special tools",
@@ -2496,15 +2480,15 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u0438\u043c-99 \u044f\u043d\u0442\u0430\u0440\u044c"
     },
     "knqkv": {
         "en": "albatross scout armored exoskeleton",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u0441\u043a\u0435\u043b\u0435\u0442 \u0430\u043b\u044c\u0431\u0430\u0442\u0440\u043e\u0441-\u0440\u0430\u0437\u0432\u0435\u0434\u0447\u0438\u043a"
     },
     "knqly": {
-        "en": "reporter\u2019s armor",
+        "en": "reporters armor",
         "ru": "\u0431\u0440\u043e\u043d\u044f \u0440\u0435\u043f\u043e\u0440\u0442\u0435\u0440\u0430"
     },
     "knqmy": {
         "en": "bandit cloak",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043f\u043b\u0430\u0449"
     },
     "knqvy": {
@@ -2520,16 +2504,16 @@
         "ru": "jagdkommando"
     },
     "knvvj": {
         "en": "icy kukri",
         "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043a\u0443\u043a\u0440\u0438"
     },
     "knw1p": {
-        "en": "fortis shift vertical tactical grip, orange",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical, \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
+        "en": "fortis shift vertical tactical grip orange",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical \u043e\u0440\u0430\u043d\u0436\u0435\u0432\u0430\u044f"
     },
     "knw2y": {
         "en": "pkp receiver cover with picatinny rail",
         "ru": "\u043a\u0440\u044b\u0448\u043a\u0430 \u0441\u0442\u0432\u043e\u043b\u044c\u043d\u043e\u0439 \u043a\u043e\u0440\u043e\u0431\u043a\u0438 \u043f\u043a\u043f \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "knw5y": {
         "en": "handguard with guiding ris for sig sg 550",
@@ -2596,44 +2580,44 @@
         "ru": "\u0440\u044e\u043a\u0437\u0430\u043a hellboy"
     },
     "l3n2": {
         "en": "berloga-4u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-4\u0443"
     },
     "l601": {
-        "en": "7.62 mm sniper ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
-    },
-    "l69j": {
-        "en": "12 caliber silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "762 mm sniper ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0441\u043d\u0430\u0439\u043f\u0435\u0440\u0441\u043a\u0438\u0439"
     },
     "l6y1": {
         "en": "12 caliber buckshot",
         "ru": "\u0434\u0440\u043e\u0431\u044c 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "ljpq": {
         "en": "polyhedron",
         "ru": "\u043c\u043d\u043e\u0433\u043e\u0433\u0440\u0430\u043d\u043d\u0438\u043a"
     },
+    "ljrj": {
+        "en": "radiator",
+        "ru": "\u0440\u0430\u0434\u0438\u0430\u0442\u043e\u0440"
+    },
     "lngq": {
         "en": "rgo",
         "ru": "\u0440\u0433\u043e"
     },
     "lny1": {
         "en": "tri-zip assault backpack",
         "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u043e\u0439 \u0440\u044e\u043a\u0437\u0430\u043a tri-zip"
     },
     "ly1kq": {
         "en": "surefire socom556-rc2 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c surefire socom556-rc2"
     },
     "ly1lo": {
-        "en": "7.62 nato pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62 nato pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "762 nato pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 762 nato pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "ly1vo": {
         "en": "kobra extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043a\u043e\u0431\u0440\u0430"
     },
     "ly29k": {
         "en": "worn l96a1",
@@ -2664,16 +2648,16 @@
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fma td grip"
     },
     "ly4ok": {
         "en": "handguard for saiga-12k",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0434\u043b\u044f \u0441\u0430\u0439\u0433\u0430-12\u043a"
     },
     "ly4qj": {
-        "en": "hq issue mini laser sight (green laser)",
-        "ru": "hq issue mini laser sight (\u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "hq issue mini laser sight green laser",
+        "ru": "hq issue mini laser sight \u0437\u0435\u043b\u0435\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "ly4z2": {
         "en": "acecare optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 acecare"
     },
     "lyg3q": {
         "en": "legend",
@@ -2703,22 +2687,14 @@
         "en": "olive armor paint",
         "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u043e\u043b\u0438\u0432\u043a\u043e\u0432\u0430\u044f"
     },
     "lyj2k": {
         "en": "zarya-b suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0437\u0430\u0440\u044f-\u0431"
     },
-    "lyj4o": {
-        "en": "worn amethyst",
-        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0430\u043c\u0435\u0442\u0438\u0441\u0442"
-    },
-    "lyjmo": {
-        "en": "nord group assault trooper",
-        "ru": "\u0448\u0442\u0443\u0440\u043c\u043e\u0432\u0438\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434"
-    },
     "lyjvk": {
         "en": "ah-3 seeker suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "lyjzk": {
         "en": "worn reaper suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0436\u043d\u0435\u0446"
@@ -2764,15 +2740,15 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0441\u043a\u043e\u043b"
     },
     "lyr3k": {
         "en": "strange crate",
         "ru": "\u0441\u0442\u0440\u0430\u043d\u043d\u044b\u0439 \u044f\u0449\u0438\u043a"
     },
     "lyv22": {
-        "en": "hunter\u2019s machete",
+        "en": "hunters machete",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u0438\u0439 \u043c\u0430\u0447\u0435\u0442\u0435"
     },
     "lyvv2": {
         "en": "twitcher",
         "ru": "\u0442\u0432\u0438\u0447\u0435\u0440"
     },
     "m023j": {
@@ -2795,41 +2771,45 @@
         "en": "skat-10 armored suit",
         "ru": "\u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043a\u0430\u0442-10"
     },
     "m06my": {
         "en": "bandit suit with gas mask",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441 \u043f\u0440\u043e\u0442\u0438\u0432\u043e\u0433\u0430\u0437\u043e\u043c"
     },
-    "m06o2": {
-        "en": "khors group zivcas",
-        "ru": "zivcas \u0433\u0440\u0443\u043f\u043f\u044b \u0445\u043e\u0440\u0441"
-    },
     "m06vy": {
         "en": "mis-116 emerald",
         "ru": "\u043a\u0438\u043c-116 \u0438\u0437\u0443\u043c\u0440\u0443\u0434"
     },
     "m0g22": {
         "en": "browning extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d browning"
     },
     "m0g77": {
         "en": "kochetov mount for patriot with picatinny rail",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u043a\u043e\u0447\u0435\u0442\u043e\u0432\u0430 \u043f\u0430\u0442\u0440\u0438\u043e\u0442 \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "m0gv2": {
-        "en": "7.62 bakelite clip",
-        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 7.62"
+        "en": "762 bakelite clip",
+        "ru": "\u0431\u0430\u043a\u0435\u043b\u0438\u0442\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 762"
+    },
+    "m0jyj": {
+        "en": "premium for 1 day",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 1 \u0434\u0435\u043d\u044c"
     },
     "m0kd7": {
         "en": "vortex collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 vortex"
     },
     "m0kny": {
-        "en": "b-10m handguard (bottom rail)",
-        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-10\u043c (\u043d\u0438\u0436\u043d\u044f\u044f \u043f\u043b\u0430\u043d\u043a\u0430)"
+        "en": "b-10m handguard bottom rail",
+        "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-10\u043c \u043d\u0438\u0436\u043d\u044f\u044f \u043f\u043b\u0430\u043d\u043a\u0430"
+    },
+    "m0lmr": {
+        "en": "upsilon data",
+        "ru": "\u0438\u043f\u0441\u0438\u043b\u043e\u043d \u0434\u0430\u043d\u043d\u044b\u0435"
     },
     "m0m7j": {
         "en": "smg nut",
         "ru": "\u043f\u043f \u043e\u0440\u0435\u0445"
     },
     "m0mo7": {
         "en": "vsk-94",
@@ -2888,20 +2868,16 @@
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 volumehex wave"
     },
     "m3pk": {
         "en": "freezer container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u043e\u043b\u043e\u0442\u0443\u043d"
     },
     "mj07": {
-        "en": "5.45 mm ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c"
-    },
-    "mj1j": {
-        "en": "7.62 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "545 mm ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c"
     },
     "mr13y": {
         "en": "red fly agaric",
         "ru": "\u0440\u0436\u0430\u0432\u044b\u0439 \u043c\u0443\u0445\u043e\u043c\u043e\u0440"
     },
     "mr1jy": {
         "en": "remains of scientific equipment",
@@ -2947,14 +2923,18 @@
         "en": "psycho",
         "ru": "\u043f\u0441\u0438\u0445"
     },
     "n45w2": {
         "en": "russian digital camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0440\u0443\u0441\u0441\u043a\u0430\u044f \u0446\u0438\u0444\u0440\u0430"
     },
+    "n4lo6": {
+        "en": "premium for 3 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 3 \u0434\u043d\u044f"
+    },
     "n4m93": {
         "en": "\u043c\u0440-412",
         "ru": "\u043c\u0440-412"
     },
     "n4md3": {
         "en": "hk xm8s",
         "ru": "hk xm8s"
@@ -2988,41 +2968,37 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u043f\u0435\u0440\u0435\u0441\u043c\u0435\u0448\u043d\u0438\u043a"
     },
     "n4ry1": {
         "en": "worn osh protective suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0437\u0430\u0449\u0438\u0442\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u043e\u0448"
     },
     "n4z22": {
-        "en": "pm/pb extended clip",
-        "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043c/\u043f\u0431"
+        "en": "pmpb extended clip",
+        "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043c\u043f\u0431"
     },
     "n4zp2": {
         "en": "beretta extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d beretta"
     },
     "nkgl1": {
         "en": "formaldehyde",
         "ru": "\u0444\u043e\u0440\u043c\u0430\u043b\u0438\u043d"
     },
     "nkgv1": {
         "en": "piece of infernal coal",
         "ru": "\u043a\u0443\u0441\u043e\u043a \u0430\u0434\u0441\u043a\u043e\u0433\u043e \u0443\u0433\u043b\u044f"
     },
     "nl43": {
-        "en": "5.45 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "545 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "nlk3": {
         "en": "10 mm ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 10 \u043c\u043c"
     },
-    "nln6": {
-        "en": "large-caliber silver ammo",
-        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
-    },
     "nv43": {
         "en": "npa backpack",
         "ru": "\u0440\u044e\u043a\u0437\u0430\u043a npa"
     },
     "nvpw": {
         "en": "flare grenade",
         "ru": "\u0441\u0437\u0433 \u0432\u0441\u043f\u044b\u0448\u043a\u0430"
@@ -3031,22 +3007,22 @@
         "en": "kzs-2u",
         "ru": "\u043a\u0437\u0441-2\u0443"
     },
     "odq0": {
         "en": "sports bag",
         "ru": "\u0441\u043f\u043e\u0440\u0442\u0438\u0432\u043d\u0430\u044f \u0441\u0443\u043c\u043a\u0430"
     },
-    "ok01m": {
-        "en": "khors group tank",
-        "ru": "\u0442\u0430\u043d\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0445\u043e\u0440\u0441"
-    },
     "ok096": {
         "en": "mis-122 amethyst",
         "ru": "\u043a\u0438\u043c-122 \u0430\u043c\u0435\u0442\u0438\u0441\u0442"
     },
+    "ok0jm": {
+        "en": "worn skat-9b",
+        "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0441\u043a\u0430\u0442-9\u0431"
+    },
     "ok0m6": {
         "en": "bandit suit with gas tanks",
         "ru": "\u0431\u0430\u043d\u0434\u0438\u0442\u0441\u043a\u0438\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0441 \u0431\u0430\u043b\u043b\u043e\u043d\u0430\u043c\u0438"
     },
     "ok0v6": {
         "en": "worn hawk armored suit",
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0441\u043e\u043a\u043e\u043b"
@@ -3056,16 +3032,16 @@
         "ru": "\u043f\u043e\u043d\u043e\u0448\u0435\u043d\u043d\u044b\u0439 \u0442\u044f\u0436\u0435\u043b\u044b\u0439 \u0431\u0440\u043e\u043d\u0435\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u0440\u043e\u043c\u0438\u043b\u0430"
     },
     "ok570": {
         "en": "ris rail for smg-91 kedr",
         "ru": "\u043f\u043b\u0430\u043d\u043a\u0430 ris \u043d\u0430 \u043f\u043f-91 \u043a\u0435\u0434\u0440"
     },
     "ok59m": {
-        "en": "5.45 pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45 pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "545 pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 545 pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "ok5vm": {
         "en": "colt extended clip",
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d colt"
     },
     "ok65o": {
         "en": "volumehex pink camouflage",
@@ -3103,18 +3079,26 @@
         "en": "steyr aug 9 mm",
         "ru": "steyr aug 9mm"
     },
     "okm20": {
         "en": "hk psg1",
         "ru": "hk psg1"
     },
+    "okrno": {
+        "en": "premium for 2 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 2 \u0434\u043d\u044f"
+    },
     "okv0o": {
         "en": "m16a2",
         "ru": "m16a2"
     },
+    "okv7o": {
+        "en": "itemwpnabakan-05name",
+        "ru": "\u0430\u043d-94 \u0430\u0431\u0430\u043a\u0430\u043d"
+    },
     "okyd4": {
         "en": "stove",
         "ru": "\u043f\u0435\u0447\u044c"
     },
     "okyg5": {
         "en": "erdl red camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl red"
@@ -3136,37 +3120,33 @@
         "ru": "\u0431\u043b\u043e\u043a \u0434\u0430\u043d\u043d\u044b\u0445 \u0434\u0435\u043b\u044c\u0442\u0430"
     },
     "olzr6": {
         "en": "beta data fragment",
         "ru": "\u0444\u0440\u0430\u0433\u043c\u0435\u043d\u0442 \u0434\u0430\u043d\u043d\u044b\u0445 \u0431\u0435\u0442\u0430"
     },
     "ork0": {
-        "en": "5.45 mm armor-piercing ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
-    },
-    "orzo": {
-        "en": "9x39 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
+        "en": "545 mm armor-piercing ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0431\u0440\u043e\u043d\u0435\u0431\u043e\u0439\u043d\u044b\u0439"
     },
     "p062": {
-        "en": "5.45 mm incendiary ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
+        "en": "545 mm incendiary ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "p0j2": {
         "en": "10 mm incendiary ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 10 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
-    "p0n6": {
-        "en": "12.7x55 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 12.7x55 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "p2r5": {
         "en": "m84",
         "ru": "m84"
     },
+    "p60o6": {
+        "en": "premium for 5 days",
+        "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 5 \u0434\u043d\u0435\u0439"
+    },
     "p611d": {
         "en": "spiked club",
         "ru": "\u0448\u0438\u043f\u0430\u0441\u0442\u0430\u044f \u0434\u0443\u0431\u0438\u043d\u043a\u0430"
     },
     "p613d": {
         "en": "m9 bayonet knife",
         "ru": "\u0448\u0442\u044b\u043a-\u043d\u043e\u0436 m9"
@@ -3256,16 +3236,16 @@
         "ru": "\u0443\u0432\u0435\u043b\u0438\u0447\u0435\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d \u0444\u043e\u0440\u0442-12"
     },
     "p6y72": {
         "en": "adaptive ris rail for dp",
         "ru": "\u0430\u0434\u0430\u043f\u0442\u0438\u0432\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 ris \u0434\u043b\u044f \u0434\u043f"
     },
     "p6yr4": {
-        "en": "g3/m1a drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d g3/m1a"
+        "en": "g3m1a drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d g3m1a"
     },
     "p92d": {
         "en": "hive container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0443\u043b\u0435\u0439"
     },
     "p99d": {
         "en": "iu-2 container",
@@ -3348,15 +3328,15 @@
         "ru": "\u043f\u0441\u0438-\u0431\u043b\u043e\u043a\u0430\u0434\u0430 \u0442\u0440\u0435\u0442\u044c\u0435\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "qj9y6": {
         "en": "2nd class antidote",
         "ru": "\u0430\u043d\u0442\u0438\u0434\u043e\u0442 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "qjg24": {
-        "en": "sapper\u2019s shovel",
+        "en": "sappers shovel",
         "ru": "\u0441\u0430\u043f\u0435\u0440\u043d\u0430\u044f \u043b\u043e\u043f\u0430\u0442\u0430"
     },
     "qjgg4": {
         "en": "frozen ice pick",
         "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043b\u0435\u0434\u043e\u0440\u0443\u0431"
     },
     "qjo2j": {
@@ -3404,16 +3384,16 @@
         "ru": "\u0441\u0442\u0430\u043d\u0434\u0430\u0440\u0442\u043d\u044b\u0435 \u0438\u043d\u0441\u0442\u0440\u0443\u043c\u0435\u043d\u0442\u044b"
     },
     "qjr3j": {
         "en": "m1a with picatinny rail handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 m1a \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "qjr43": {
-        "en": "fortis shift vertical tactical grip, black",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical, \u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "fortis shift vertical tactical grip black",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 fortis shift vertical \u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "qjrk4": {
         "en": "elcan optical sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043e\u043f\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 elcan"
     },
     "qjrw4": {
         "en": "tulip optical sight",
@@ -3428,37 +3408,41 @@
         "ru": "spectre m4"
     },
     "qjw5j": {
         "en": "ots-33 stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u043e\u0446-33"
     },
     "qjw7k": {
-        "en": "sks bracket\u2014dovetail joint",
+        "en": "sks bracketdovetail joint",
         "ru": "\u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u0441\u043a\u0441 - \u043b\u0430\u0441\u0442\u043e\u0447\u043a\u0438\u043d \u0445\u0432\u043e\u0441\u0442"
     },
     "qjwg3": {
-        "en": "ergonomic clip for vss/val",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u044d\u0440\u0433\u043e\u043d\u043e\u043c\u0438\u0447\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441/\u0432\u0430\u043b"
+        "en": "ergonomic clip for vssval",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u044d\u0440\u0433\u043e\u043d\u043e\u043c\u0438\u0447\u043d\u044b\u0439 \u0434\u043b\u044f \u0432\u0441\u0441\u0432\u0430\u043b"
     },
     "qjwq9": {
-        "en": "ash-12/mts-558 silencer",
-        "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0448-12/\u043c\u0446-558"
+        "en": "ash-12mts-558 silencer",
+        "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0448-12\u043c\u0446-558"
     },
     "qjwv3": {
         "en": "aa-12 drum clip",
         "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d aa-12"
     },
     "qm0k": {
         "en": "large-caliber ammo",
-        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
+        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u0441\u0430\u043c\u043e\u0434\u0435\u043b\u044c\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
     },
     "qmjk": {
         "en": "12 caliber incendiary",
         "ru": "\u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0435 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
+    "qo06": {
+        "en": "transformer",
+        "ru": "\u0442\u0440\u0430\u043d\u0441\u0444\u043e\u0440\u043c\u0430\u0442\u043e\u0440"
+    },
     "qo59": {
         "en": "bubble",
         "ru": "\u043f\u0443\u0437\u044b\u0440\u044c"
     },
     "qo94": {
         "en": "chicken god",
         "ru": "\u043a\u0443\u0440\u0438\u043d\u044b\u0439 \u0431\u043e\u0433"
@@ -3479,25 +3463,21 @@
         "en": "pieces of copper wire",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u043c\u0435\u0434\u043d\u043e\u0439 \u043f\u0440\u043e\u0432\u043e\u043b\u043e\u043a\u0438"
     },
     "rj6ov": {
         "en": "chlorinex",
         "ru": "\u0445\u043b\u043e\u0440\u043d\u0438\u043a"
     },
-    "ro6g": {
-        "en": "5.45 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "row5": {
         "en": "12 caliber hunting round",
         "ru": "\u043e\u0445\u043e\u0442\u043d\u0438\u0447\u044c\u044f \u043f\u0443\u043b\u044f 12 \u043a\u0430\u043b\u0438\u0431\u0440\u0430"
     },
     "rw03g": {
-        "en": "hq issue low-profile laser sight (red laser)",
-        "ru": "hq issue low-profile laser sight (\u043a\u0440\u0430\u0441\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440)"
+        "en": "hq issue low-profile laser sight red laser",
+        "ru": "hq issue low-profile laser sight \u043a\u0440\u0430\u0441\u043d\u044b\u0439 \u043b\u0430\u0437\u0435\u0440"
     },
     "rw06v": {
         "en": "fab defense g3-rs handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 fab defence g3-rs"
     },
     "rw09v": {
         "en": "sks tactical grip",
@@ -3508,15 +3488,15 @@
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 bering optics"
     },
     "rw0ky": {
         "en": "tapco vertical grip",
         "ru": "\u0432\u0435\u0440\u0442\u0438\u043a\u0430\u043b\u044c\u043d\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 tapco"
     },
     "rw1mg": {
-        "en": "\u201chercules\u201d",
+        "en": "hercules",
         "ru": "\u0433\u0435\u0440\u043a\u0443\u043b\u0435\u0441"
     },
     "rw1vg": {
         "en": "1st class thermoblock",
         "ru": "\u0442\u0435\u0440\u043c\u043e\u0431\u0430\u0440\u044c\u0435\u0440 \u043f\u0435\u0440\u0432\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "rw23l": {
@@ -3535,17 +3515,21 @@
         "en": "rapier",
         "ru": "\u0440\u0430\u043f\u0438\u0440\u0430"
     },
     "rw2d5": {
         "en": "mcmillan cs5",
         "ru": "mcmillan cs5"
     },
+    "rw32l": {
+        "en": "ice shard",
+        "ru": "\u043b\u0435\u0434\u044f\u043d\u043e\u0439 \u043e\u0441\u043a\u043e\u043b\u043e\u043a"
+    },
     "rw4ry": {
-        "en": "5.56 nato emag drum clip",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato emag"
+        "en": "556 nato emag drum clip",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato emag"
     },
     "rw4zy": {
         "en": "smg-2000 clip",
         "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d \u043f\u043f-2000"
     },
     "rw90g": {
         "en": "erdl arvn red camouflage",
@@ -3595,18 +3579,14 @@
         "en": "erdl arvn red camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl arvn red"
     },
     "rwn2v": {
         "en": "tourist suit",
         "ru": "\u043a\u043e\u043c\u0431\u0438\u043d\u0435\u0437\u043e\u043d \u0442\u0443\u0440\u0438\u0441\u0442"
     },
-    "rwn5y": {
-        "en": "nord group exoskeleton",
-        "ru": "\u044d\u043a\u0437\u043e\u0441\u043a\u0435\u043b\u0435\u0442 \u0433\u0440\u0443\u043f\u043f\u044b \u043d\u043e\u0440\u0434"
-    },
     "rwnqv": {
         "en": "damaged ah-3 seeker suit",
         "ru": "\u043f\u043e\u0432\u0440\u0435\u0436\u0434\u0435\u043d\u043d\u044b\u0439 \u043a\u043e\u0441\u0442\u044e\u043c \u0430\u043e-3 \u0438\u0441\u043a\u0430\u0442\u0435\u043b\u044c"
     },
     "rwnrv": {
         "en": "gorka-3 suit",
         "ru": "\u043a\u043e\u0441\u0442\u044e\u043c \u0433\u043e\u0440\u043a\u0430-3"
@@ -3621,15 +3601,15 @@
     },
     "rwrkz": {
         "en": "incandescent",
         "ru": "\u043d\u0430\u043a\u0430\u043b"
     },
     "rwrng": {
         "en": "an-94 abakan",
-        "ru": "\u0430\u043d-94 \u0430\u0431\u0430\u043a\u0430\u043d"
+        "ru": "\u0430\u043d-94\u043c \u0430\u0431\u0430\u043a\u0430\u043d"
     },
     "rwz2z": {
         "en": "russian bayonet",
         "ru": "\u0440\u0443\u0441\u0441\u043a\u0438\u0439 \u0448\u0442\u044b\u043a"
     },
     "rwzmv": {
         "en": "bee",
@@ -3640,16 +3620,16 @@
         "ru": "\u0440\u0438\u0442\u0443\u0430\u043b\u044c\u043d\u044b\u0439 \u0442\u043e\u043f\u043e\u0440"
     },
     "rwzzz": {
         "en": "6h9 knife",
         "ru": "\u043d\u043e\u0436 6\u04459"
     },
     "vdjd": {
-        "en": "5.45 mm sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.45 \u043c\u043c \u0441\u0431\u043f"
+        "en": "545 mm sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 545 \u043c\u043c \u0441\u0431\u043f"
     },
     "vdnd": {
         "en": "tank of combustible mixture",
         "ru": "\u0431\u0430\u043b\u043b\u043e\u043d \u0441 \u0433\u043e\u0440\u044e\u0447\u0435\u0439 \u0441\u043c\u0435\u0441\u044c\u044e"
     },
     "vj12r": {
         "en": "worm armored suit",
@@ -3685,31 +3665,31 @@
     },
     "vj5ln": {
         "en": "erdl urban camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 erdl urban"
     },
     "vj5rd": {
         "en": "birch tree camouflage 1943 model",
-        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440. 1943 \u0433."
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440 1943 \u0433"
     },
     "vjd5n": {
         "en": "premium for 7 days",
         "ru": "\u043f\u0440\u0435\u043c\u0438\u0443\u043c \u043d\u0430 7 \u0434\u043d\u0435\u0439"
     },
     "vjl4p": {
-        "en": "mp-133/mp-153 clip extender",
-        "ru": "\u0443\u0434\u043b\u0438\u043d\u0438\u0442\u0435\u043b\u044c \u043c\u0430\u0433\u0430\u0437\u0438\u043d\u0430 \u043c\u0440-133/\u043c\u0440-153"
+        "en": "mp-133mp-153 clip extender",
+        "ru": "\u0443\u0434\u043b\u0438\u043d\u0438\u0442\u0435\u043b\u044c \u043c\u0430\u0433\u0430\u0437\u0438\u043d\u0430 \u043c\u0440-133\u043c\u0440-153"
     },
     "vjl7d": {
         "en": "sight mount for m16a2",
         "ru": "\u043a\u0440\u0435\u043f\u043b\u0435\u043d\u0438\u0435 \u043f\u0440\u0438\u0446\u0435\u043b\u0430 \u0434\u043b\u044f m16a2"
     },
     "vjm3p": {
         "en": "birch tree camouflage 1943 model",
-        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440. 1943 \u0433."
+        "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0431\u0435\u0440\u0435\u0437\u043a\u0430 \u043e\u0431\u0440 1943 \u0433"
     },
     "vjmdg": {
         "en": "prophet",
         "ru": "\u043f\u0440\u043e\u0440\u043e\u043a"
     },
     "vjmm7": {
         "en": "flecktarn forest camouflage",
@@ -3724,16 +3704,16 @@
         "ru": "spectre"
     },
     "vjp5r": {
         "en": "tactical stock for sks",
         "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u043e\u0435 \u043b\u043e\u0436\u0435 \u0434\u043b\u044f \u0441\u043a\u0441"
     },
     "vjpzd": {
-        "en": "pk-01(t) collimator sight",
-        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01(\u0442)"
+        "en": "pk-01t collimator sight",
+        "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043f\u043a-01\u0442"
     },
     "vjrm7": {
         "en": "uz",
         "ru": "\u0443\u0437"
     },
     "vjy3n": {
         "en": "epinephrine",
@@ -3751,18 +3731,14 @@
         "en": "remains of a radio transmitter",
         "ru": "\u043e\u0441\u0442\u0430\u0442\u043a\u0438 \u0440\u0430\u0434\u0438\u043e\u043f\u0435\u0440\u0435\u0434\u0430\u0442\u0447\u0438\u043a\u0430"
     },
     "vyrg": {
         "en": "m84 qd",
         "ru": "m84 qd"
     },
-    "w20p": {
-        "en": "large-caliber silver ammo",
-        "ru": "\u043a\u0440\u0443\u043f\u043d\u043e\u043a\u0430\u043b\u0438\u0431\u0435\u0440\u043d\u044b\u0439 \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439 \u043f\u0430\u0442\u0440\u043e\u043d"
-    },
     "w23o": {
         "en": "9x39 mm sp-5 ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u043f-5"
     },
     "w3022": {
         "en": "gamma group tracker",
         "ru": "\u043c\u0430\u044f\u0447\u043e\u043a \u0433\u0440\u0443\u043f\u043f\u044b \u0433\u0430\u043c\u043c\u0430"
@@ -3776,15 +3752,15 @@
         "ru": "\u0431\u0435\u043b\u0438\u0447\u044c\u0438 \u0434\u0440\u043e\u0436\u0436\u0438"
     },
     "w3zj3": {
         "en": "modified anomalous battery",
         "ru": "\u043c\u043e\u0434\u0438\u0444\u0438\u0446\u0438\u0440\u043e\u0432\u0430\u043d\u043d\u0430\u044f \u0430\u043d\u043e\u043c\u0430\u043b\u044c\u043d\u0430\u044f \u0431\u0430\u0442\u0430\u0440\u0435\u044f"
     },
     "w4wz": {
-        "en": "bear\u2019s den \u2014 4 container",
+        "en": "bears den  4 container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u0431\u0435\u0440\u043b\u043e\u0433\u0430-4"
     },
     "wg3p": {
         "en": "disintegrator",
         "ru": "\u0434\u0435\u0437\u0438\u043d\u0442\u0435\u0433\u0440\u0430\u0442\u043e\u0440"
     },
     "wg53": {
@@ -3792,15 +3768,15 @@
         "ru": "\u0430\u0442\u043e\u043c"
     },
     "wg62": {
         "en": "night star",
         "ru": "\u043d\u043e\u0447\u043d\u0430\u044f \u0437\u0432\u0435\u0437\u0434\u0430"
     },
     "wglp": {
-        "en": "mama\u2019s beads",
+        "en": "mamas beads",
         "ru": "\u043c\u0430\u043c\u0438\u043d\u044b \u0431\u0443\u0441\u044b"
     },
     "wgr3": {
         "en": "black crystal",
         "ru": "\u0447\u0435\u0440\u043d\u044b\u0439 \u043a\u0440\u0438\u0441\u0442\u0430\u043b\u043b"
     },
     "wgvd": {
@@ -3912,15 +3888,15 @@
         "ru": "\u0441\u0432\u0435\u0440\u0445\u0437\u0432\u0443\u043a\u043e\u0432\u043e\u0439"
     },
     "wjm4d": {
         "en": "metal scrap",
         "ru": "\u0436\u0435\u043b\u0435\u0437\u044f\u043a\u0430"
     },
     "wjml3": {
-        "en": "toad\u2014white camouflage",
+        "en": "toadwhite camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430 - \u0431\u0435\u043b\u044b\u0439"
     },
     "wjmmz": {
         "en": "dpm woodland a camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 dpm woodland a"
     },
     "wjmoz": {
@@ -3980,16 +3956,16 @@
         "ru": "\u0446\u0435\u0432\u044c\u0435 caa rs-21"
     },
     "wjr3d": {
         "en": "9 mm barrel extension",
         "ru": "\u0443\u0434\u043b\u0438\u043d\u0435\u043d\u043d\u044b\u0439 \u0441\u0442\u0432\u043e\u043b 9 \u043c\u043c"
     },
     "wjr63": {
-        "en": "5.45 clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "wjr9d": {
         "en": "salvo 12 silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c salvo 12"
     },
     "wjrdo": {
         "en": "clamp with ris rail",
@@ -4000,16 +3976,16 @@
         "ru": "vg6 epsilon 556 muzzle brake"
     },
     "wjrld": {
         "en": "silencer for ots-14 groza",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0434\u043b\u044f \u043e\u0446-14 \u0433\u0440\u043e\u0437\u0430"
     },
     "wjro3": {
-        "en": "5.56 nato drum clip, khaki",
-        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato, \u0445\u0430\u043a\u0438"
+        "en": "556 nato drum clip khaki",
+        "ru": "\u0431\u0430\u0440\u0430\u0431\u0430\u043d\u043d\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato \u0445\u0430\u043a\u0438"
     },
     "wjry2": {
         "en": "zm high standard ak stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 zm high standard ak"
     },
     "wjvk2": {
         "en": "blue armor paint",
@@ -4020,15 +3996,15 @@
         "ru": "\u0430\u043d\u0442\u0438\u0440\u0430\u0434 \u0432\u0442\u043e\u0440\u043e\u0433\u043e \u043a\u043b\u0430\u0441\u0441\u0430"
     },
     "wjy7o": {
         "en": "digital tiger camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0446\u0438\u0444\u0440\u043e\u0432\u043e\u0439 \u0442\u0438\u0433\u0440"
     },
     "wjyoo": {
-        "en": "toad\u2014white camouflage",
+        "en": "toadwhite camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 \u0436\u0430\u0431\u0430 - \u0431\u0435\u043b\u044b\u0439"
     },
     "wjypp": {
         "en": "belgian jigsaw camouflage",
         "ru": "\u043a\u0430\u043c\u0443\u0444\u043b\u044f\u0436 belgian jigsaw"
     },
     "wjyqp": {
@@ -4168,44 +4144,44 @@
         "ru": "\u043e\u0431\u043b\u0435\u0433\u0447\u0435\u043d\u043d\u044b\u0439 \u043f\u0440\u0438\u043a\u043b\u0430\u0434 m4"
     },
     "y3m3w": {
         "en": "3 port mini compensator",
         "ru": "3 port mini compensator"
     },
     "y3m4w": {
-        "en": "citadel 5.45 mbc",
-        "ru": "\u0434\u0442\u043a \u0446\u0438\u0442\u0430\u0434\u0435\u043b\u044c 5.45"
+        "en": "citadel 545 mbc",
+        "ru": "\u0434\u0442\u043a \u0446\u0438\u0442\u0430\u0434\u0435\u043b\u044c 545"
     },
     "y3m6k": {
         "en": "m4 buttstock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 m4 buttstock"
     },
     "y3m73": {
-        "en": "5.56 nato stanag clip",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato stanag"
+        "en": "556 nato stanag clip",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato stanag"
     },
     "y3mdo": {
         "en": "guiding ris for shotgun",
         "ru": "\u043d\u0430\u043f\u0440\u0430\u0432\u043b\u044f\u044e\u0449\u0430\u044f ris \u0434\u043b\u044f \u0434\u0440\u043e\u0431\u043e\u0432\u0438\u043a\u043e\u0432"
     },
     "y3mgw": {
         "en": "fa556 mini silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c fa556 mini"
     },
     "y3mj3": {
-        "en": "5.45 plastic clip",
-        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.45"
+        "en": "545 plastic clip",
+        "ru": "\u043f\u043b\u0430\u0441\u0442\u0438\u043a\u043e\u0432\u044b\u0439 \u043c\u0430\u0433\u0430\u0437\u0438\u043d 545"
     },
     "y3mnw": {
         "en": "atg silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c \u0430\u0442\u0433"
     },
     "y3mp0": {
-        "en": "compact protective rail, black",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430,\u0447\u0435\u0440\u043d\u0430\u044f"
+        "en": "compact protective rail black",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430\u0447\u0435\u0440\u043d\u0430\u044f"
     },
     "y3nmw": {
         "en": "spare parts",
         "ru": "\u0437\u0430\u043f\u0430\u0441\u043d\u044b\u0435 \u0434\u0435\u0442\u0430\u043b\u0438"
     },
     "y3o03": {
         "en": "ridge camouflage",
@@ -4244,16 +4220,16 @@
         "ru": "fal quad rail"
     },
     "y3po3": {
         "en": "grip for ots-14 groza",
         "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 \u0434\u043b\u044f \u043e\u0446-14 \u0433\u0440\u043e\u0437\u0430"
     },
     "y3prz": {
-        "en": "an/peq 15 tactical unit, black",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a an/peq 15, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "anpeq 15 tactical unit black",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u0431\u043b\u043e\u043a anpeq 15 \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "y3pwo": {
         "en": "okp-7 collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043e\u043a\u043f-7"
     },
     "y3pyk": {
         "en": "fab defense ak handguard",
@@ -4327,49 +4303,41 @@
         "en": "prism",
         "ru": "\u043f\u0440\u0438\u0437\u043c\u0430"
     },
     "y5yw": {
         "en": "spring",
         "ru": "\u043f\u0440\u0443\u0436\u0438\u043d\u0430"
     },
-    "y90z": {
-        "en": "9x39 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9x39 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "y94o": {
-        "en": "7.62 mm sbp ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u0441\u0431\u043f"
+        "en": "762 mm sbp ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u0441\u0431\u043f"
     },
     "yqq0": {
         "en": "kzs-1u container",
         "ru": "\u043a\u043e\u043d\u0442\u0435\u0439\u043d\u0435\u0440 \u043a\u0437\u0441-1\u0443"
     },
     "yw7k": {
         "en": "sn-2u leglet",
         "ru": "\u0441\u043d-2\u0443 \u043d\u043e\u0436\u043a\u0430"
     },
-    "z102": {
-        "en": "5.56 mm silver ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 5.56 \u043c\u043c \u0441\u0435\u0440\u0435\u0431\u0440\u0435\u043d\u044b\u0439"
-    },
     "z13n": {
-        "en": "7.62 mm expanding ammo",
-        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 7.62 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
+        "en": "762 mm expanding ammo",
+        "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 762 \u043c\u043c \u044d\u043a\u0441\u043f\u0430\u043d\u0441\u0438\u0432\u043d\u044b\u0439"
     },
     "z1zn": {
         "en": "9 mm incendiary ammo",
         "ru": "\u043f\u0430\u0442\u0440\u043e\u043d 9 \u043c\u043c \u0437\u0430\u0436\u0438\u0433\u0430\u0442\u0435\u043b\u044c\u043d\u044b\u0439"
     },
     "z301y": {
         "en": "flowering northern moss",
         "ru": "\u0446\u0432\u0435\u0442\u0443\u0449\u0438\u0439 \u0441\u0435\u0432\u0435\u0440\u043d\u044b\u0439 \u043c\u043e\u0445"
     },
     "z30mm": {
-        "en": "notes of major d.",
-        "ru": "\u0437\u0430\u043f\u0438\u0441\u0438 \u043c\u0430\u0439\u043e\u0440\u0430 \u0434."
+        "en": "notes of major d",
+        "ru": "\u0437\u0430\u043f\u0438\u0441\u0438 \u043c\u0430\u0439\u043e\u0440\u0430 \u0434"
     },
     "z30my": {
         "en": "flowering red fern",
         "ru": "\u0446\u0432\u0435\u0442\u0443\u0449\u0438\u0439 \u0440\u044b\u0436\u0438\u0439 \u043f\u0430\u043f\u043e\u0440\u043e\u0442\u043d\u0438\u043a"
     },
     "z30qy": {
         "en": "blue yeast",
@@ -4536,32 +4504,32 @@
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 mp5 \u043d\u0435\u0441\u043a\u043b\u0430\u0434\u043d\u043e\u0439"
     },
     "zz939": {
         "en": "whirlwind mbc",
         "ru": "\u0434\u0442\u043a \u0432\u0438\u0445\u0440\u044c"
     },
     "zz96m": {
-        "en": "5.56 nato pmag clip, black",
-        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 5.56 nato pmag, \u0447\u0435\u0440\u043d\u044b\u0439"
+        "en": "556 nato pmag clip black",
+        "ru": "\u043c\u0430\u0433\u0430\u0437\u0438\u043d 556 nato pmag \u0447\u0435\u0440\u043d\u044b\u0439"
     },
     "zz9dn": {
         "en": "side bracket with picatinny rail",
         "ru": "\u0431\u043e\u043a\u043e\u0432\u043e\u0439 \u043a\u0440\u043e\u043d\u0448\u0442\u0435\u0439\u043d \u0441 \u043f\u043b\u0430\u043d\u043a\u043e\u0439 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "zz9k9": {
         "en": "osprey silencer",
         "ru": "\u0433\u043b\u0443\u0448\u0438\u0442\u0435\u043b\u044c osprey"
     },
     "zz9ny": {
         "en": "izhmash plastic stock",
         "ru": "\u043f\u0440\u0438\u043a\u043b\u0430\u0434 \u0438\u0436\u043c\u0430\u0448 \u043f\u043e\u043b\u0438\u043c\u0435\u0440\u043d\u044b\u0439"
     },
     "zz9pk": {
-        "en": "compact protective rail, olive",
-        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430, \u043e\u043b\u0438\u0432\u0430"
+        "en": "compact protective rail olive",
+        "ru": "\u043a\u043e\u043c\u043f\u0430\u043a\u0442\u043d\u0430\u044f \u0437\u0430\u0449\u0438\u0442\u043d\u0430\u044f \u043f\u043b\u0430\u043d\u043a\u0430 \u043e\u043b\u0438\u0432\u0430"
     },
     "zz9z9": {
         "en": "hera arms cc compensator",
         "ru": "hera arms cc compensator"
     },
     "zzjgn": {
         "en": "albatross infiltrator armored exoskeleton",
@@ -4632,36 +4600,36 @@
         "ru": "\u043b\u0430\u0437\u0435\u0440\u043d\u044b\u0439 \u0446\u0435\u043b\u0435\u0443\u043a\u0430\u0437\u0430\u0442\u0435\u043b\u044c \u043a\u043b\u0435\u0449-2\u043f\u0441"
     },
     "zzpoy": {
         "en": "b-11 handguard with upper rail",
         "ru": "\u0446\u0435\u0432\u044c\u0435 \u0431-11 \u0441 \u0432\u0435\u0440\u0445\u043d\u0435\u0439 \u043f\u043b\u0430\u043d\u043a\u043e\u0439"
     },
     "zzpvm": {
-        "en": "reg fab defense tactical grip, khaki",
-        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence, \u0445\u0430\u043a\u0438"
+        "en": "reg fab defense tactical grip khaki",
+        "ru": "\u0442\u0430\u043a\u0442\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u0440\u0443\u043a\u043e\u044f\u0442\u043a\u0430 reg fab defence \u0445\u0430\u043a\u0438"
     },
     "zzpwy": {
         "en": "mp5 with picatinny rail handguard",
         "ru": "\u0446\u0435\u0432\u044c\u0435 mp5 \u0441 \u043f\u043b\u0430\u043d\u043a\u0430\u043c\u0438 \u043f\u0438\u043a\u0430\u0442\u0438\u043d\u043d\u0438"
     },
     "zzpyn": {
         "en": "kobra collimator sight",
         "ru": "\u043f\u0440\u0438\u0446\u0435\u043b \u043a\u043e\u043b\u043b\u0438\u043c\u0430\u0442\u043e\u0440\u043d\u044b\u0439 \u043a\u043e\u0431\u0440\u0430"
     },
     "zzqk2": {
         "en": "bandage",
         "ru": "\u0431\u0438\u043d\u0442"
     },
     "zzr39": {
-        "en": "fab defense ag-47 grip, khaki",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47, \u0445\u0430\u043a\u0438"
+        "en": "fab defense ag-47 grip khaki",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence ag-47 \u0445\u0430\u043a\u0438"
     },
     "zzrw9": {
-        "en": "fab defense agr-43 grip, green",
-        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43, \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
+        "en": "fab defense agr-43 grip green",
+        "ru": "\u0440\u0443\u043a\u043e\u044f\u0442\u044c fab defence agr-43 \u0437\u0435\u043b\u0435\u043d\u044b\u0439"
     },
     "zzvmy": {
         "en": "yellow armor paint",
         "ru": "\u043a\u0440\u0430\u0441\u043a\u0430 \u0434\u043b\u044f \u0431\u0440\u043e\u043d\u0438 \u0436\u0435\u043b\u0442\u0430\u044f"
     },
     "zzy1n": {
         "en": "altyn set",
```

### Comparing `stalcraft_api-0.2.6/stalcraft/enums.py` & `stalcraft_api-0.3.0/stalcraft/enums.py`

 * *Files identical despite different names*

### Comparing `stalcraft_api-0.2.6/stalcraft/item.py` & `stalcraft_api-0.3.0/stalcraft/item.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     def __str__(self):
         return self.item_id
 
     def __repr__(self):
         return f"<{self.__class__.__name__}> name='{self.name}' item_id='{self.item_id}'"
 
 
-
 class LocalItem(Item):
     def __init__(self, name: str, path="", encoding="utf-8", folder=ItemFolder.RU):
         """
         Search for Item ID by name in file
 
         name: Name of item (without quotes)
         path: Path to the file. Defaults to built-in items.json
```

