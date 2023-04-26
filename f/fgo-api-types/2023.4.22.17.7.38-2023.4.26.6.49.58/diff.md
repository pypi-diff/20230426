# Comparing `tmp/fgo_api_types-2023.4.22.17.7.38.tar.gz` & `tmp/fgo_api_types-2023.4.26.6.49.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2023.4.22.17.7.38.tar", max compression
+gzip compressed data, was "fgo_api_types-2023.4.26.6.49.58.tar", max compression
```

## Comparing `fgo_api_types-2023.4.22.17.7.38.tar` & `fgo_api_types-2023.4.26.6.49.58.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2023-04-22 17:07:16.505451 fgo_api_types-2023.4.22.17.7.38/LICENSE
--rw-r--r--   0        0        0      449 2023-04-22 17:07:16.505451 fgo_api_types-2023.4.22.17.7.38/README.md
--rw-r--r--   0        0        0        0 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/base.py
--rw-r--r--   0        0        0     4195 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3631 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/common.py
--rw-r--r--   0        0        0    37431 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/enums.py
--rw-r--r--   0        0        0   155624 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    74299 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/nice.py
--rw-r--r--   0        0        0    49669 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4176 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    18464 2023-04-22 17:07:38.173727 fgo_api_types-2023.4.22.17.7.38/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2023-04-22 17:07:38.509731 fgo_api_types-2023.4.22.17.7.38/pyproject.toml
--rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.22.17.7.38/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-04-26 06:49:31.888901 fgo_api_types-2023.4.26.6.49.58/LICENSE
+-rw-r--r--   0        0        0      449 2023-04-26 06:49:31.888901 fgo_api_types-2023.4.26.6.49.58/README.md
+-rw-r--r--   0        0        0        0 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4195 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3631 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/common.py
+-rw-r--r--   0        0        0    37431 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   155885 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    74299 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    49669 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4176 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    18464 2023-04-26 06:49:58.889461 fgo_api_types-2023.4.26.6.49.58/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2023-04-26 06:49:59.281469 fgo_api_types-2023.4.26.6.49.58/pyproject.toml
+-rw-r--r--   0        0        0     1222 1970-01-01 00:00:00.000000 fgo_api_types-2023.4.26.6.49.58/PKG-INFO
```

### Comparing `fgo_api_types-2023.4.22.17.7.38/LICENSE` & `fgo_api_types-2023.4.26.6.49.58/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/basic.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/common.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/common.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/enums.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/gameenums.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/gameenums.py`

 * *Files 0% similar despite different names*

```diff
@@ -1710,14 +1710,15 @@
     EVENT_SVT_GET = 7
     QUEST_REWARD_ICON = 8
     COSTUME_RELEASE = 9
     COSTUME_GET = 10
     COMMAND_CODE = 11
     EVENT_POINT_BUFF = 12
     EVENT_BOARD_GAME_TOKEN = 13
+    EVENT_COMMAND_ASSIST = 14
 
 
 class NiceGiftType(StrEnum):
     """Gift Type Enum"""
 
     servant = "servant"
     item = "item"
@@ -1728,14 +1729,15 @@
     eventSvtGet = "eventSvtGet"
     questRewardIcon = "questRewardIcon"
     costumeRelease = "costumeRelease"
     costumeGet = "costumeGet"
     commandCode = "commandCode"
     eventPointBuff = "eventPointBuff"
     eventBoardGameToken = "eventBoardGameToken"
+    eventCommandAssist = "eventCommandAssist"
 
 
 GIFT_TYPE_NAME: dict[int, NiceGiftType] = {
     1: NiceGiftType.servant,
     2: NiceGiftType.item,
     3: NiceGiftType.friendship,
     4: NiceGiftType.userExp,
@@ -1744,14 +1746,15 @@
     7: NiceGiftType.eventSvtGet,
     8: NiceGiftType.questRewardIcon,
     9: NiceGiftType.costumeRelease,
     10: NiceGiftType.costumeGet,
     11: NiceGiftType.commandCode,
     12: NiceGiftType.eventPointBuff,
     13: NiceGiftType.eventBoardGameToken,
+    14: NiceGiftType.eventCommandAssist,
 }
 
 
 class ShopType(IntEnum):
     NONE = 0
     EVENT_ITEM = 1
     MANA = 2
@@ -2152,14 +2155,15 @@
     EVENT_TUTORIAL_FLAG_ON = 170
     EVENT_TUTORIAL_FLAG_OFF = 171
     EVENT_SUPER_BOSS_VALUE_EQUAL = 172
     NOT_EVENT_SUPER_BOSS_VALUE_EQUAL = 173
     ALL_SVT_TARGET_SKILL_LV_NUM = 174
     SUPER_BOSS_DAMAGE_ABOVE = 175
     SUPER_BOSS_DAMAGE_BELOW = 176
+    EVENT_MISSION_GROUP_ACHIEVE = 177
     NOT_WAR_CLEAR = 179
 
 
 class NiceCondType(StrEnum):
     """Condition Type Enum"""
 
     none = "none"
@@ -2332,14 +2336,15 @@
     eventTutorialFlagOn = "eventTutorialFlagOn"
     eventTutorialFlagOff = "eventTutorialFlagOff"
     eventSuperBossValueEqual = "eventSuperBossValueEqual"
     notEventSuperBossValueEqual = "notEventSuperBossValueEqual"
     allSvtTargetSkillLvNum = "allSvtTargetSkillLvNum"
     superBossDamageAbove = "superBossDamageAbove"
     superBossDamageBelow = "superBossDamageBelow"
+    eventMissionGroupAchieve = "eventMissionGroupAchieve"
     notWarClear = "notWarClear"
 
 
 COND_TYPE_NAME: dict[int, NiceCondType] = {
     0: NiceCondType.none,
     1: NiceCondType.questClear,
     2: NiceCondType.itemGet,
@@ -2510,14 +2515,15 @@
     170: NiceCondType.eventTutorialFlagOn,
     171: NiceCondType.eventTutorialFlagOff,
     172: NiceCondType.eventSuperBossValueEqual,
     173: NiceCondType.notEventSuperBossValueEqual,
     174: NiceCondType.allSvtTargetSkillLvNum,
     175: NiceCondType.superBossDamageAbove,
     176: NiceCondType.superBossDamageBelow,
+    177: NiceCondType.eventMissionGroupAchieve,
     179: NiceCondType.notWarClear,
 }
 
 
 class VoiceCondType(IntEnum):
     BIRTH_DAY = 1
     EVENT = 2
```

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/nice.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/nice.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/raw.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/rayshift.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/fgo_api_types/search.py` & `fgo_api_types-2023.4.26.6.49.58/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2023.4.22.17.7.38/pyproject.toml` & `fgo_api_types-2023.4.26.6.49.58/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2023.04.22.17.07.38"
+version = "2023.04.26.06.49.58"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2023.4.22.17.7.38/PKG-INFO` & `fgo_api_types-2023.4.26.6.49.58/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2023.4.22.17.7.38
+Version: 2023.4.26.6.49.58
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

