# Comparing `tmp/hoyo_daily_logins_helper-1.0.0-py3-none-any.whl.zip` & `tmp/hoyo_daily_logins_helper-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 6526 bytes, number of entries: 14
+Zip file size: 17947 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 21:37 src/__init__.py
 -rw-r--r--  2.0 unx       33 b- defN 23-Apr-25 21:37 src/__main__.py
--rw-r--r--  2.0 unx      663 b- defN 23-Apr-25 23:59 src/config.py
+-rw-r--r--  2.0 unx      474 b- defN 23-Apr-26 01:31 src/config.py
 -rw-r--r--  2.0 unx     1685 b- defN 23-Apr-26 00:00 src/http.py
 -rw-r--r--  2.0 unx     2134 b- defN 23-Apr-26 00:01 src/main.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-25 21:50 src/games/__init__.py
--rw-r--r--  2.0 unx      381 b- defN 23-Apr-25 23:57 src/games/genshin.py
--rw-r--r--  2.0 unx     2362 b- defN 23-Apr-26 00:05 src/games/hoyo_checkin.py
--rw-r--r--  2.0 unx      388 b- defN 23-Apr-26 00:02 src/games/starrail.py
--rw-r--r--  2.0 unx     1664 b- defN 23-Apr-26 00:35 hoyo_daily_logins_helper-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 00:35 hoyo_daily_logins_helper-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       59 b- defN 23-Apr-26 00:35 hoyo_daily_logins_helper-1.0.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 00:35 hoyo_daily_logins_helper-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1131 b- defN 23-Apr-26 00:35 hoyo_daily_logins_helper-1.0.0.dist-info/RECORD
-14 files, 10596 bytes uncompressed, 4630 bytes compressed:  56.3%
+-rw-r--r--  2.0 unx      200 b- defN 23-Apr-26 01:31 src/games/genshin.py
+-rw-r--r--  2.0 unx     2190 b- defN 23-Apr-26 01:41 src/games/hoyo_checkin.py
+-rw-r--r--  2.0 unx      207 b- defN 23-Apr-26 01:31 src/games/starrail.py
+-rw-r--r--  2.0 unx    34227 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1781 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       59 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        4 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1237 b- defN 23-Apr-26 03:09 hoyo_daily_logins_helper-1.0.1.dist-info/RECORD
+15 files, 44323 bytes uncompressed, 15879 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -21,23 +21,26 @@
 
 Filename: src/games/hoyo_checkin.py
 Comment: 
 
 Filename: src/games/starrail.py
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.0.dist-info/METADATA
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.0.dist-info/WHEEL
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.0.dist-info/entry_points.txt
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.0.dist-info/top_level.txt
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: hoyo_daily_logins_helper-1.0.0.dist-info/RECORD
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/top_level.txt
+Comment: 
+
+Filename: hoyo_daily_logins_helper-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## src/config.py

```diff
@@ -1,10 +1,9 @@
 import os
-from http.cookies import SimpleCookie
-from typing import Optional, Dict
+from typing import Optional
 
 _default_configs = {
     "USER_AGENT": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
                   "AppleWebKit/537.36 (KHTML, like Gecko) "
                   "Chrome/74.0.3729.169 Safari/537.36"
 }
 
@@ -14,12 +13,7 @@
 def get_config(key: str) -> Optional[str]:
     if key not in os.environ:
         if key in _default_configs:
             return _default_configs[key]
         return None
     return os.environ[key]
 
-
-def parse_cookie_string(cookie: str) -> Dict[str, str]:
-    c = SimpleCookie()
-    c.load(cookie)
-    return {k: v.value for k, v in c.items()}
```

## src/games/genshin.py

```diff
@@ -1,17 +1,9 @@
-from src.config import parse_cookie_string
 from src.games.hoyo_checkin import hoyo_checkin
 
 
 def run(cookie_str: str):
-    cookies = parse_cookie_string(cookie_str)
-
-    uid = cookies["account_id"]
-    token = cookies["ltoken"]
-
     hoyo_checkin(
         "https://hk4e-api-os.mihoyo.com/event/sol",
         "e202102251931481",
-        uid,
-        token,
         cookie_str,
     )
```

## src/games/hoyo_checkin.py

```diff
@@ -8,57 +8,50 @@
 
 RET_CODE_ALREADY_SIGNED_IN = -5003
 
 
 def hoyo_checkin(
     event_base_url: str,
     act_id: str,
-    uid: str,
-    token: str,
     cookie_str: str
 ):
     lang = "en-us"
     referer_url = "https://act.hoyolab.com/"
     reward_url = f"{event_base_url}/home?lang={lang}" \
                  f"&act_id={act_id}"
     info_url = f"{event_base_url}/info?lang={lang}" \
                f"&act_id={act_id}"
     sign_url = f"{event_base_url}/sign?lang={lang}"
 
-    if not token or not uid:
-        raise Exception("account_id and/or ltoken data is missing")
-
     headers = {
         "Referer": referer_url,
         "Accept-Encoding": "gzip, deflate, br",
         "Cookie": cookie_str,
     }
 
     info_list = http_get_json(info_url, headers=headers)
 
     today = info_list.get("data", {}).get("today")
     total_sign_in_day = info_list.get("data", {}).get("total_sign_day")
     already_signed_in = info_list.get("data", {}).get("is_sign")
     first_bind = info_list.get("data", {}).get("first_bind")
 
-    logging.debug(f"Today is {today}")
-
     if already_signed_in:
         logging.info("Already checked in today")
         return
 
     if first_bind:
         logging.info("Please check in manually once")
         return
 
     awards_data = http_get_json(reward_url)
 
     awards = awards_data.get("data", {}).get("awards")
 
-    logging.info(f"Checking in account {uid} for today...")
+    logging.info(f"Checking in account for {today}...")
 
     # a normal human can't instantly click, so we wait a bit
     sleep_time = random.uniform(2.0, 10.0)
     logging.debug(f"Sleep for {sleep_time}")
     time.sleep(sleep_time)
 
     request_data = json.dumps({
```

## src/games/starrail.py

```diff
@@ -1,17 +1,9 @@
-from src.config import parse_cookie_string
 from src.games.hoyo_checkin import hoyo_checkin
 
 
 def run(cookie_str: str):
-    cookies = parse_cookie_string(cookie_str)
-
-    uid = cookies["account_id"]
-    token = cookies["ltoken"]
-
     hoyo_checkin(
         "https://sg-public-api.hoyolab.com/event/luna/os",
         "e202303301540311",
-        uid,
-        token,
         cookie_str,
     )
```

## Comparing `hoyo_daily_logins_helper-1.0.0.dist-info/METADATA` & `hoyo_daily_logins_helper-1.0.1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hoyo-daily-logins-helper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Get hoyo daily login rewards automatically!
 Home-page: https://github.com/atomicptr/hoyo-daily-logins-helper
 Author: Christopher Kaster
 Author-email: me@atomicptr.de
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: certifi (==2022.12.7)
 Requires-Dist: charset-normalizer (==3.1.0)
 Requires-Dist: requests (==2.28.2)
 Requires-Dist: urllib3 (==1.26.15)
 
 # hoyo-daily-login-helper
 
@@ -39,7 +40,13 @@
 
 The command line options are also available via environment variables which
 allows you to easily run this script in Docker/Podman!
 
 ```bash
 $ docker run --rm --env GAME=starrail --env COOKIE="your cookie string" ghcr.io/atomicptr/hoyo-daily-logins-helper
 ```
+
+## License
+
+GNU General Public License v3
+
+![](https://www.gnu.org/graphics/gplv3-127x51.png)
```

## Comparing `hoyo_daily_logins_helper-1.0.0.dist-info/RECORD` & `hoyo_daily_logins_helper-1.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/__main__.py,sha256=PMTdGm21mzeJd45xL_OXHrls33P9jeAwQCR_OSijKfI,33
-src/config.py,sha256=7ndcz5eGQGwFNxoCLNslCud8n0RW6Fv37OH1Jzhfaa8,663
+src/config.py,sha256=QEMtjB0gQdH14PYjB0QXl_bHIhwFjJ3RJpGcXo7LZj0,474
 src/http.py,sha256=yhHjY5tBRgDcgLr3fO2kFxvNEPW8AQmlM-aEAJ25jWk,1685
 src/main.py,sha256=nrPWCqpLsIiaI3PKaCoJJ46uvlNjd9EcgQn8DCtbHXQ,2134
 src/games/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-src/games/genshin.py,sha256=fJQjKz1d65nSPmrr_ucwIWTPIhJu6yS_ioy7TvNGp2U,381
-src/games/hoyo_checkin.py,sha256=SOR_6MgdtKtHLbwQ-DfPrcsZ6V14YN4ru2HZQvpNAio,2362
-src/games/starrail.py,sha256=5_qQjR4cRd-JriJPZqx-JsK4ugBhP6Z5P0iD07XaQHo,388
-hoyo_daily_logins_helper-1.0.0.dist-info/METADATA,sha256=eNxMi-5AClEAWG15ZgPwcBHYhTbfxfGBl_bJWohajus,1664
-hoyo_daily_logins_helper-1.0.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-hoyo_daily_logins_helper-1.0.0.dist-info/entry_points.txt,sha256=RWkn_oFw-w5I2PPijySe7udmVaEUD3ew8wXMCQ9I3_g,59
-hoyo_daily_logins_helper-1.0.0.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
-hoyo_daily_logins_helper-1.0.0.dist-info/RECORD,,
+src/games/genshin.py,sha256=iwKd-NhdRVZXPgXR4y7O-GxfA1eKV9fM-zrBOXv-Gcc,200
+src/games/hoyo_checkin.py,sha256=ssUAyJyTuArYrMqq6Kkt7tSwnT7u1rsDNX0-q1Zkgwo,2190
+src/games/starrail.py,sha256=wtXQPrJGjUmW8A9PIZDTzB-hZiiSxmNHxWEbTUo_cXc,207
+hoyo_daily_logins_helper-1.0.1.dist-info/LICENSE,sha256=mYluISwUlRhyOocFBuQndyF5ZKqTzDtalcVTCKd34gE,34227
+hoyo_daily_logins_helper-1.0.1.dist-info/METADATA,sha256=CCnKvVrsekr0ikLHRJt_nHj_i7HWF6rL5Mu4dHl13bw,1781
+hoyo_daily_logins_helper-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+hoyo_daily_logins_helper-1.0.1.dist-info/entry_points.txt,sha256=RWkn_oFw-w5I2PPijySe7udmVaEUD3ew8wXMCQ9I3_g,59
+hoyo_daily_logins_helper-1.0.1.dist-info/top_level.txt,sha256=74rtVfumQlgAPzR5_2CgYN24MB0XARCg0t-gzk6gTrM,4
+hoyo_daily_logins_helper-1.0.1.dist-info/RECORD,,
```

