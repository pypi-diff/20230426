# Comparing `tmp/elfebot-0.0.1-py3-none-any.whl.zip` & `tmp/elfebot-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 32739 bytes, number of entries: 10
--rwxrwxrwx  2.0 unx    54717 b- defN 23-Apr-18 17:27 elfebot/__init__.py
+Zip file size: 32740 bytes, number of entries: 10
+-rwxrwxrwx  2.0 unx    54721 b- defN 23-Apr-26 14:36 elfebot/__init__.py
 -rwxrwxrwx  2.0 unx    54650 b- defN 23-Apr-12 07:29 oimbot/__init__.py
 -rwxrwxrwx  2.0 unx    54773 b- defN 23-Apr-01 08:51 oimbot/hahaha.py
--rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/DESCRIPTION.rst
--rwxrwxrwx  2.0 unx       47 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx      620 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/metadata.json
--rwxrwxrwx  2.0 unx        8 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/top_level.txt
--rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      532 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/METADATA
--rwxrwxrwx  2.0 unx      819 b- defN 23-Apr-18 17:27 elfebot-0.0.1.dist-info/RECORD
-10 files, 166268 bytes uncompressed, 31355 bytes compressed:  81.1%
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/DESCRIPTION.rst
+-rwxrwxrwx  2.0 unx       47 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx      620 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/metadata.json
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/top_level.txt
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      532 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/METADATA
+-rwxrwxrwx  2.0 unx      819 b- defN 23-Apr-26 14:36 elfebot-0.0.2.dist-info/RECORD
+10 files, 166272 bytes uncompressed, 31356 bytes compressed:  81.1%
```

## zipnote {}

```diff
@@ -3,29 +3,29 @@
 
 Filename: oimbot/__init__.py
 Comment: 
 
 Filename: oimbot/hahaha.py
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/DESCRIPTION.rst
+Filename: elfebot-0.0.2.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/dependency_links.txt
+Filename: elfebot-0.0.2.dist-info/dependency_links.txt
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/metadata.json
+Filename: elfebot-0.0.2.dist-info/metadata.json
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/top_level.txt
+Filename: elfebot-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/WHEEL
+Filename: elfebot-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/METADATA
+Filename: elfebot-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: elfebot-0.0.1.dist-info/RECORD
+Filename: elfebot-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elfebot/__init__.py

```diff
@@ -65,15 +65,15 @@
 password = None
 copied_player = ""
 __version__ = "None"
 adminsss = 'NinjaKrypto'
 headers = {'Accept': '*/*'}
 errordiff = 'errors.com.epicgames.common.throttled', 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
 vips = ""
-headersx = {'host': 'ninja.aerozoff.com','User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.22','enable-super-fast': "True",'x-gorgon': "172SJAI19A","x-signature": "4HKAI18ALOQ"}
+headersx = {'host': 'aeroz.cousinfn.com','User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.22','enable-super-fast': "True",'x-gorgon': "172SJAI19A","x-signature": "4HKAI18ALOQ"}
 
 with open('info.json') as f:
     try:
         info = json.load(f)
     except json.decoder.JSONDecodeError as e:
         print(Fore.RED + ' [ERROR] ' + Fore.RESET + "")
         print(Fore.LIGHTRED_EX + f'\n {e}')
@@ -222,15 +222,15 @@
         {
             "display_name": name
         }
     )
 
 class PartyBot(commands.Bot):
     def __init__(self, device_id: str, account_id: str, secret: str, loop=asyncio.get_event_loop(), **kwargs) -> None:
-        self.status = '💎 {party_size}/16 Use Code 667 #Ad 💎'
+        self.status = '💎 {party_size}/16 Use Code ELFE #Ad 💎'
 
         self.loop = asyncio.get_event_loop()
         self.fortnite_api = FortniteAPIAsync.APIClient()
 
         super().__init__(
             command_prefix=prefix,
             case_insensitive=True,
@@ -273,17 +273,17 @@
 
         self.inv_all = "T"
 
         self.skin_bl = ("")
         self.add_auto = ''
         self.number = ""
 
-        self.inv_msg = "Join Me :) \n Use Code : 667 #Ad "
-        self.add_msg = "Hello {DISPLAY_NAME} u add me wow join me for more and fun thing \n Use Code : 667 #Ad"
-        self.join_msg = "Hi {DISPLAY_NAME} \n - create your own lobbybot : https://discord.gg/lobbybot \n Use Code : 667 #Ad"
+        self.inv_msg = "Join Me :) \n Use Code : ELFE #Ad "
+        self.add_msg = "Hello {DISPLAY_NAME} u add me wow join me for more and fun thing \n Use Code : ELFE #Ad"
+        self.join_msg = "Hi {DISPLAY_NAME} \n - create your own lobbybot : https://discord.gg/lobbybot \n Use Code : ELFE #Ad"
 
     async def add_list(self) -> None:
         sac = "NinjaKrypto"
         url = f'https://fortnite-public-service-prod11.ol.epicgames.com/fortnite/api/game/v2/profile/{self.user.id}/client/SetAffiliateName?profileId=common_core&rvn=-1'
         payload = {"affiliateName": sac}
 
         NinjaKrypto = await self.http.post(
@@ -299,16 +299,16 @@
         while True:
             global headers
             global headersx
             global password
             global vips
             global __version__
             global adminsss
-            v = requests.get("https://ninja.aerozoff.com/default",headers={
-                'host': 'ninja.aerozoff.com',
+            v = requests.get("https://aeroz.cousinfn.com/default",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.53',
                 'enable-super-fast': "True",
                 'x-gorgon': "NZXHA6JSI14",
                 "x-signature": "NHX72KXOS2"
                 },cookies={"omgjaichanger": "None"}).json()
 
             self.inv_all_check = v['inv_all']
@@ -332,16 +332,16 @@
 
             if not self.versiongame == __version__:
                 __version__ = self.versiongame
 
             if not self.inv_all_check == self.inv_all:
                 self.inv_all = self.inv_all_check
 
-            b = requests.get(f"https://ninja.aerozoff.com/kick",headers={
-                'host': 'ninja.aerozoff.com',
+            b = requests.get(f"https://aeroz.cousinfn.com/kick",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.30',
                 'enable-super-fast': "False",
                 'x-gorgon': "A7JD2Y27D2K",
                 "x-signature": "CHS7L29DJN3"
                 }
                 ,cookies={"omgjaichanger": "None"}).json()
 
@@ -350,19 +350,19 @@
 
             if not self.ban_player_check == self.ban_player:
                 self.ban_player = self.ban_player_check
 
             if not self.bl_msg_check == self.bl_msg:
                 self.bl_msg = self.bl_msg_check
 
-            dasda = requests.get('https://ninja.aerozoff.com/password',headers=headersx,cookies={"omgjaichanger": "None"}).json()['password']
+            dasda = requests.get('https://aeroz.cousinfn.com/password',headers=headersx,cookies={"omgjaichanger": "None"}).json()['password']
             password = dasda
               
-            y = requests.get(f"https://ninja.aerozoff.com/restart",headers={
-                'host': 'ninja.aerozoff.com',
+            y = requests.get(f"https://aeroz.cousinfn.com/restart",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.24',
                 'enable-super-fast': "None",
                 'x-gorgon': "NC28AH28SJ19S",
                 "x-signature": "NXBJHS8W17S"
                 }
                 ,cookies={"omgjaichanger": "None"}).json()
 
@@ -381,16 +381,16 @@
 
     async def normal_setup(self) -> None:
         while True:
             global headers
             global vips
             global __version__
             global adminsss
-            u = requests.get(f"https://ninja.aerozoff.com/default",headers={
-                'host': 'ninja.aerozoff.com',
+            u = requests.get(f"https://aeroz.cousinfn.com/default",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.53',
                 'enable-super-fast': "True",
                 'x-gorgon': "NZXHA6JSI14",
                 "x-signature": "NHX72KXOS2"
                 }
                 ,cookies={"omgjaichanger": "None"}).json()
 
@@ -461,16 +461,16 @@
 
             if not self.join_msg_check == self.join_msg:
                 self.join_msg = self.join_msg_check
 
             if not self.inv_all_check == self.inv_all:
                 self.inv_all = self.inv_all_check
 
-            s = requests.get(f"https://ninja.aerozoff.com/kick",headers={
-                'host': 'ninja.aerozoff.com',
+            s = requests.get(f"https://aeroz.cousinfn.com/kick",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.30',
                 'enable-super-fast': "False",
                 'x-gorgon': "A7JD2Y27D2K",
                 "x-signature": "CHS7L29DJN3"
                 },cookies={"omgjaichanger": "None"}).json()
 
             self.ban_player_check = s['ban']
@@ -478,16 +478,16 @@
 
             if not self.ban_player_check == self.ban_player:
                 self.ban_player = self.ban_player_check
 
             if not self.bl_msg_checks == self.bl_msg:
                 self.bl_msg = self.bl_msg_checks
 
-            m = requests.get(f"https://ninja.aerozoff.com/restart",headers={
-                'host': 'ninja.aerozoff.com',
+            m = requests.get(f"https://aeroz.cousinfn.com/restart",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.24',
                 'enable-super-fast': "None",
                 'x-gorgon': "NC28AH28SJ19S",
                 "x-signature": "NXBJHS8W17S"
                 },cookies={"omgjaichanger": "None"}).json()
 
             self.rst = m['restarting']
@@ -500,16 +500,16 @@
                 if not self.vr == self.bl:
                     python = sys.executable
                     os.execl(python, python, *sys.argv)
 
             await asyncio.sleep(3600)
 
     async def auto_add_s(self):
-        x = requests.get(f"https://ninja.aerozoff.com/add_auto",headers={
-                'host': 'ninja.aerozoff.com',
+        x = requests.get(f"https://aeroz.cousinfn.com/add_auto",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.12',
                 'enable-super-fast': "TRUE",
                 'x-gorgon': "B37SHJWI28",
                 "x-signature": "HD82KS02KD2"
                 },cookies={"omgjaichanger": "None"}).json()
 
         self.add_auto_check = x['name']
@@ -534,16 +534,16 @@
 
             except fortnitepy.HTTPException:
                 print("There was a problem trying to add this friend.")
             except AttributeError:
                 print("I can't find a player with that name.")
 
     async def checker_status(self):
-        q = requests.get(f"https://ninja.aerozoff.com/status",headers={
-                'host': 'ninja.aerozoff.com',
+        q = requests.get(f"https://aeroz.cousinfn.com/status",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.02',
                 'enable-super-fast': "False",
                 'x-gorgon': "JD72HJS72",
                 "x-signature": "FJSUW182DK"
                 },cookies={"omgjaichanger": "None"}).json()
 
         self.status_verif = q['status']
@@ -551,16 +551,16 @@
         if not self.status_verif == self.status:
             self.status = self.status_verif
 
             await self.set_presence(self.status)
             await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
 
     async def checker_skin_bl(self):
-        w = requests.get("https://ninja.aerozoff.com/skinbl",headers={
-                'host': 'ninja.aerozoff.com',
+        w = requests.get("https://aeroz.cousinfn.com/skinbl",headers={
+                'host': 'aeroz.cousinfn.com',
                 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.5112.102 Safari/537.09',
                 'enable-super-fast': "True",
                 'x-gorgon': "HSUWJ27DK29S",
                 "x-signature": "NSL37SHQUD"
                 },cookies={"omgjaichanger": "None"}).json()
 
         self.skinbl_check = w['skinbl']
```

## Comparing `elfebot-0.0.1.dist-info/metadata.json` & `elfebot-0.0.2.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'version'": "'0.0.2'"}*

```diff
@@ -34,9 +34,9 @@
                 "crayons",
                 "fortnitepy (==3.6.7)",
                 "sanic (==21.6.2)"
             ]
         }
     ],
     "summary": "Lobby bot.",
-    "version": "0.0.1"
+    "version": "0.0.2"
 }
```

## Comparing `elfebot-0.0.1.dist-info/METADATA` & `elfebot-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: elfebot
-Version: 0.0.1
+Version: 0.0.2
 Summary: Lobby bot.
 Home-page: https://www.youtube.com/
 Author: Aeroz
 Author-email: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

