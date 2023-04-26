# Comparing `tmp/aqimon-0.3.0.tar.gz` & `tmp/aqimon-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqimon-0.3.0.tar", max compression
+gzip compressed data, was "aqimon-0.4.0.tar", max compression
```

## Comparing `aqimon-0.3.0.tar` & `aqimon-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1065 2023-04-23 23:22:03.569603 aqimon-0.3.0/LICENSE
--rw-r--r--   0        0        0     5828 2023-04-23 23:22:03.569603 aqimon-0.3.0/README.md
--rw-r--r--   0        0        0       45 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/__init__.py
--rw-r--r--   0        0        0     2449 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/aqi_common.py
--rw-r--r--   0        0        0     2372 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/config.py
--rw-r--r--   0        0        0     6988 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/database.py
--rw-r--r--   0        0        0      881 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/mock.py
--rw-r--r--   0        0        0     2113 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/novapm.py
--rw-r--r--   0        0        0    12441 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/constants.py
--rw-r--r--   0        0        0     1524 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/exceptions.py
--rw-r--r--   0        0        0     4082 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/read/sds011/responses.py
--rw-r--r--   0        0        0     7944 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/server.py
--rw-r--r--   0        0        0     6835 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/android-chrome-192x192.png
--rw-r--r--   0        0        0    20365 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/android-chrome-512x512.png
--rw-r--r--   0        0        0     6288 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/apple-touch-icon.png
--rw-r--r--   0        0        0   437308 2023-04-23 23:22:33.441220 aqimon-0.3.0/aqimon/static/elm.js
--rw-r--r--   0        0        0      351 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon-16x16.png
--rw-r--r--   0        0        0      754 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/favicon.ico
--rw-r--r--   0        0        0     1799 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/failing.png
--rw-r--r--   0        0        0     2418 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/idle.png
--rw-r--r--   0        0        0    24380 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/images/loading.gif
--rw-r--r--   0        0        0      696 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/static/index.html
--rw-r--r--   0        0        0     5587 2023-04-23 23:22:03.569603 aqimon-0.3.0/aqimon/templates/index.html
--rw-r--r--   0        0        0      968 2023-04-23 23:22:03.569603 aqimon-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 aqimon-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-26 04:51:03.327597 aqimon-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5828 2023-04-26 04:51:03.327597 aqimon-0.4.0/README.md
+-rw-r--r--   0        0        0       45 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/__init__.py
+-rw-r--r--   0        0        0     2633 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/aqi_common.py
+-rw-r--r--   0        0        0     2372 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/config.py
+-rw-r--r--   0        0        0     7030 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/database.py
+-rw-r--r--   0        0        0      881 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/__init__.py
+-rw-r--r--   0        0        0     1712 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/mock.py
+-rw-r--r--   0        0        0     2133 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/novapm.py
+-rw-r--r--   0        0        0    12441 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/constants.py
+-rw-r--r--   0        0        0     1524 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/exceptions.py
+-rw-r--r--   0        0        0     4082 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/read/sds011/responses.py
+-rw-r--r--   0        0        0     8437 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/server.py
+-rw-r--r--   0        0        0     6835 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/android-chrome-192x192.png
+-rw-r--r--   0        0        0    20365 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/android-chrome-512x512.png
+-rw-r--r--   0        0        0     6288 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/apple-touch-icon.png
+-rw-r--r--   0        0        0   452012 2023-04-26 04:51:29.004291 aqimon-0.4.0/aqimon/static/elm.js
+-rw-r--r--   0        0        0      351 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon-16x16.png
+-rw-r--r--   0        0        0      754 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/favicon.ico
+-rw-r--r--   0        0        0     1799 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/failing.png
+-rw-r--r--   0        0        0     2418 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/idle.png
+-rw-r--r--   0        0        0     6349 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/loading.gif
+-rw-r--r--   0        0        0    44088 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/images/warmingup.gif
+-rw-r--r--   0        0        0      696 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/static/index.html
+-rw-r--r--   0        0        0     5587 2023-04-26 04:51:03.327597 aqimon-0.4.0/aqimon/templates/index.html
+-rw-r--r--   0        0        0      968 2023-04-26 04:51:03.327597 aqimon-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6420 1970-01-01 00:00:00.000000 aqimon-0.4.0/PKG-INFO
```

### Comparing `aqimon-0.3.0/LICENSE` & `aqimon-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/README.md` & `aqimon-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/aqi_common.py` & `aqimon-0.4.0/aqimon/aqi_common.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,32 @@
 class Pollutant(Enum):
     """Enum of possible pollutans."""
 
     PM_25 = 0
     PM_10 = 1
 
 
+class EpaLevels(Enum):
+    """Enum of EPA levels."""
+
+    GOOD = 0
+    MODERATE = 1
+    UNHEALTHY_FOR_SENSITIVE = 2
+    UNHEALTHY = 3
+    VERY_UNHEALTHY = 4
+    HAZARDOUS = 5
+
+
 AQI: List[Tuple[int, int]] = [
     (0, 50),
     (51, 100),
     (101, 150),
     (151, 200),
     (201, 300),
-    (301, 400),
-    (401, 500),
+    (301, 500),
 ]
 PM_25: List[Tuple[float, float]] = [
     (0.0, 12.0),
     (12.1, 35.4),
     (35.5, 55.4),
     (55.5, 150.4),
     (150.5, 250.4),
@@ -59,19 +69,19 @@
 class EpaAqi:
     """An EPA AQI value, with the pollutant responsible for the value."""
 
     reading: float
     responsible_pollutant: Pollutant
 
 
-def get_level_from_pm25(pm25: float) -> int:
+def get_epa_level(epa_reading: float) -> EpaLevels:
     """Get the EPA level from a PM25 reading."""
-    for i, pair in enumerate(PM_25):
-        if pair[0] <= pm25 <= pair[1]:
-            return i
+    for i, pair in enumerate(AQI):
+        if pair[0] <= epa_reading <= pair[1]:
+            return EpaLevels(i)
     raise ValueError("Invalid PM value")
 
 
 def calculate_epa_aqi(readings: List[PollutantReading]) -> Optional[EpaAqi]:
     """Calculate the EPA AQI from a list of pollutant readings.
 
     The worst possible value will be reported.
```

### Comparing `aqimon-0.3.0/aqimon/config.py` & `aqimon-0.4.0/aqimon/config.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/database.py` & `aqimon-0.4.0/aqimon/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,17 @@
 
     Note that the lookback will include one additional value outside of the window if it exists.  This allows for us to
     ensure full coverage of the lookback window.
     """
     lookback = int(lookback_to.timestamp())
     result = await dbconn.fetch_one(
         "SELECT "
-        "AVG(pm25) as avg_pm25, AVG(pm10) as avg_pm10, COUNT(*) as count, MIN(event_time) as oldest_time "
+        "ROUND(AVG(pm25), 2) as avg_pm25, ROUND(AVG(pm10), 2) as avg_pm10, "
+        "COUNT(*) as count, "
+        "MIN(event_time) as oldest_time "
         "FROM read_log "
         "WHERE (event_time >= :lookback) OR "
         "(event_time = (SELECT MAX(event_time) FROM read_log WHERE event_time <= :lookback)) ORDER BY event_time ASC",
         values={"lookback": lookback},
     )
 
     if result is None:
```

### Comparing `aqimon-0.3.0/aqimon/read/__init__.py` & `aqimon-0.4.0/aqimon/read/__init__.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/read/mock.py` & `aqimon-0.4.0/aqimon/read/mock.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 import logging
 from aqimon.read import AqiRead, ReaderState, ReaderStatus
 
 
 class MockReader:
     """Mock reader class."""
 
-    def __init__(self, fake_sleep_secs=5, raise_error_odds=50):
+    def __init__(self, fake_sleep_secs=5, raise_error_odds=50, warm_up_secs=5):
         """Create a mock reader."""
         self.state = ReaderState(ReaderStatus.IDLE, None)
         self.fake_sleep_secs = fake_sleep_secs
         self.raise_error_odds = raise_error_odds
+        self.warm_up_secs = warm_up_secs
 
     async def read(self) -> AqiRead:
         """Read from the 'device'.
 
         Returns randomized data for the mock class.
 
         Also, randomly fails some percentage of the time.
         """
         try:
+            self.state = ReaderState(ReaderStatus.WARM_UP, None)
+            await asyncio.sleep(self.warm_up_secs)
             self.state = ReaderState(ReaderStatus.READING, None)
             raise_error_roll = random.randint(0, 100)
             if raise_error_roll < self.raise_error_odds:
                 raise Exception("Fake error from the reader.")
             pm25: float = round(random.uniform(0.0, 500.4), 2)
             pm10: float = round(random.uniform(0.0, 300.0), 2)
             result = AqiRead(pmtwofive=pm25, pmten=pm10)
```

### Comparing `aqimon-0.3.0/aqimon/read/novapm.py` & `aqimon-0.4.0/aqimon/read/novapm.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             for x in range(0, self.iterations):
                 await asyncio.sleep(self.sleep_time)
                 result = self.reader.query()
                 pm25_reads.append(result.pm25)
                 pm10_reads.append(result.pm10)
             self.reader.sleep()
             self.state = ReaderState(ReaderStatus.IDLE, None)
-            return AqiRead(pmtwofive=mean(pm25_reads), pmten=mean(pm10_reads))
+            return AqiRead(pmtwofive=round(mean(pm25_reads), 2), pmten=round(mean(pm10_reads), 2))
         except Exception as e:
             self.state = ReaderState(ReaderStatus.ERRORING, e)
             self.reader.sleep()
             raise e
 
     def get_state(self) -> ReaderState:
         """Get the current state of the reader."""
```

### Comparing `aqimon-0.3.0/aqimon/read/sds011/__init__.py` & `aqimon-0.4.0/aqimon/read/sds011/__init__.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/read/sds011/constants.py` & `aqimon-0.4.0/aqimon/read/sds011/constants.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/read/sds011/exceptions.py` & `aqimon-0.4.0/aqimon/read/sds011/exceptions.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/read/sds011/responses.py` & `aqimon-0.4.0/aqimon/read/sds011/responses.py`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/server.py` & `aqimon-0.4.0/aqimon/server.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import uvicorn
 import databases
 from pathlib import Path
 from datetime import datetime, timedelta
 from .database import (
     get_all_reads,
     get_all_epa_aqis,
+    get_latest_read,
+    get_latest_epa_aqi,
     add_read,
     add_epa_read,
     get_averaged_reads,
     create_tables,
     clean_old,
     ReadLogEntry,
     EpaAqiLogEntry,
@@ -211,14 +213,29 @@
     else:
         all_reads = await get_all_reads(database, None)
         all_epas = await get_all_epa_aqis(database, None)
     all_json = convert_all_to_view_dict(all_reads, all_epas)
     return all_json
 
 
+@app.get("/api/latest_data")
+async def latest_data(
+    database: databases.Database = Depends(get_database),
+):
+    """Retrieve most recent reads."""
+    latest_reads = await get_latest_read(database)
+    latest_epa = await get_latest_epa_aqi(database)
+    return {
+        "epa": latest_epa.epa_aqi,
+        "level": aqi_common.get_epa_level(latest_epa.epa_aqi).name,
+        "pm25": latest_reads.pm25,
+        "pm10": latest_reads.pm10,
+    }
+
+
 @app.get("/api/status")
 async def status(reader: ScheduledReader = Depends(get_reader)):
     """Get the system status."""
     last_exception = reader.reader.get_state().last_exception
 
     return {
         "reader_status": str(reader.reader.get_state().status.name),
```

### Comparing `aqimon-0.3.0/aqimon/static/android-chrome-192x192.png` & `aqimon-0.4.0/aqimon/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/android-chrome-512x512.png` & `aqimon-0.4.0/aqimon/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/apple-touch-icon.png` & `aqimon-0.4.0/aqimon/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/elm.js` & `aqimon-0.4.0/aqimon/static/elm.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -828,18 +828,18 @@
 
             case 11:
                 throw new Error('Cannot perform mod 0. Division by zero error.');
         }
     }
 
     function _Debug_regionToString(region) {
-        if (region.dD.aY === region.d0.aY) {
-            return 'on line ' + region.dD.aY;
+        if (region.dz.aY === region.d_.aY) {
+            return 'on line ' + region.dz.aY;
         }
-        return 'on lines ' + region.dD.aY + ' through ' + region.d0.aY;
+        return 'on lines ' + region.dz.aY + ' through ' + region.d_.aY;
     }
 
 
 
     // MATH
 
     var _Basics_add = F2(function(a, b) {
@@ -1822,17 +1822,17 @@
     // PROGRAMS
 
 
     var _Platform_worker = F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fN,
-            impl.gr,
-            impl.ga,
+            impl.fQ,
+            impl.gu,
+            impl.gd,
             function() {
                 return function() {}
             }
         );
     });
 
 
@@ -2622,17 +2622,17 @@
 
     var _VirtualDom_mapEventTuple = F2(function(func, tuple) {
         return _Utils_Tuple2(func(tuple.a), tuple.b);
     });
 
     var _VirtualDom_mapEventRecord = F2(function(func, record) {
         return {
-            aa: func(record.aa),
-            dF: record.dF,
-            $7: record.$7
+            ae: func(record.ae),
+            dB: record.dB,
+            dm: record.dm
         }
     });
 
 
 
     // ORGANIZE FACTS
 
@@ -2864,19 +2864,19 @@
 
             // 0 = Normal
             // 1 = MayStopPropagation
             // 2 = MayPreventDefault
             // 3 = Custom
 
             var value = result.a;
-            var message = !tag ? value : tag < 3 ? value.a : value.aa;
-            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dF;
+            var message = !tag ? value : tag < 3 ? value.a : value.ae;
+            var stopPropagation = tag == 1 ? value.b : tag == 3 && value.dB;
             var currentEventNode = (
                 stopPropagation && event.stopPropagation(),
-                (tag == 2 ? value.b : tag == 3 && value.$7) && event.preventDefault(),
+                (tag == 2 ? value.b : tag == 3 && value.dm) && event.preventDefault(),
                 eventNode
             );
             var tagger;
             var i;
             while (tagger = currentEventNode.j) {
                 if (typeof tagger == 'function') {
                     message = tagger(message);
@@ -3717,19 +3717,19 @@
 
     var _Debugger_element;
 
     var _Browser_element = _Debugger_element || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fN,
-            impl.gr,
-            impl.ga,
+            impl.fQ,
+            impl.gu,
+            impl.gd,
             function(sendToApp, initialModel) {
-                var view = impl.gt;
+                var view = impl.gw;
                 /**/
                 var domNode = args['node'];
                 //*/
                 /**_UNUSED/
                 var domNode = args && args['node'] ? args['node'] : _Debug_crash(0);
                 //*/
                 var currNode = _VirtualDom_virtualize(domNode);
@@ -3751,32 +3751,32 @@
 
     var _Debugger_document;
 
     var _Browser_document = _Debugger_document || F4(function(impl, flagDecoder, debugMetadata, args) {
         return _Platform_initialize(
             flagDecoder,
             args,
-            impl.fN,
-            impl.gr,
-            impl.ga,
+            impl.fQ,
+            impl.gu,
+            impl.gd,
             function(sendToApp, initialModel) {
-                var divertHrefToApp = impl.dw && impl.dw(sendToApp)
-                var view = impl.gt;
+                var divertHrefToApp = impl.ds && impl.ds(sendToApp)
+                var view = impl.gw;
                 var title = _VirtualDom_doc.title;
                 var bodyNode = _VirtualDom_doc.body;
                 var currNode = _VirtualDom_virtualize(bodyNode);
                 return _Browser_makeAnimator(initialModel, function(model) {
                     _VirtualDom_divertHrefToApp = divertHrefToApp;
                     var doc = view(model);
-                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.fp);
+                    var nextNode = _VirtualDom_node('body')(_List_Nil)(doc.fs);
                     var patches = _VirtualDom_diff(currNode, nextNode);
                     bodyNode = _VirtualDom_applyPatches(bodyNode, currNode, patches, sendToApp);
                     currNode = nextNode;
                     _VirtualDom_divertHrefToApp = 0;
-                    (title !== doc.gf) && (_VirtualDom_doc.title = title = doc.gf);
+                    (title !== doc.gi) && (_VirtualDom_doc.title = title = doc.gi);
                 });
             }
         );
     });
 
 
 
@@ -3825,50 +3825,50 @@
 
 
 
     // APPLICATION
 
 
     function _Browser_application(impl) {
-        var onUrlChange = impl.fX;
-        var onUrlRequest = impl.fY;
+        var onUrlChange = impl.f_;
+        var onUrlRequest = impl.f$;
         var key = function() {
             key.a(onUrlChange(_Browser_getUrl()));
         };
 
         return _Browser_document({
-            dw: function(sendToApp) {
+            ds: function(sendToApp) {
                 key.a = sendToApp;
                 _Browser_window.addEventListener('popstate', key);
                 _Browser_window.navigator.userAgent.indexOf('Trident') < 0 || _Browser_window.addEventListener('hashchange', key);
 
                 return F2(function(domNode, event) {
                     if (!event.ctrlKey && !event.metaKey && !event.shiftKey && event.button < 1 && !domNode.target && !domNode.hasAttribute('download')) {
                         event.preventDefault();
                         var href = domNode.href;
                         var curr = _Browser_getUrl();
                         var next = $elm$url$Url$fromString(href).a;
                         sendToApp(onUrlRequest(
                             (next &&
-                                curr.eK === next.eK &&
-                                curr.ec === next.ec &&
-                                curr.eF.a === next.eF.a
+                                curr.eM === next.eM &&
+                                curr.eb === next.eb &&
+                                curr.eH.a === next.eH.a
                             ) ?
                             $elm$browser$Browser$Internal(next) :
                             $elm$browser$Browser$External(href)
                         ));
                     }
                 });
             },
-            fN: function(flags) {
-                return A3(impl.fN, flags, _Browser_getUrl(), key);
+            fQ: function(flags) {
+                return A3(impl.fQ, flags, _Browser_getUrl(), key);
             },
-            gt: impl.gt,
-            gr: impl.gr,
-            ga: impl.ga
+            gw: impl.gw,
+            gu: impl.gu,
+            gd: impl.gd
         });
     }
 
     function _Browser_getUrl() {
         return $elm$url$Url$fromString(_VirtualDom_doc.location.href).a || _Debug_crash(1);
     }
 
@@ -3928,35 +3928,35 @@
 
     // PAGE VISIBILITY
 
 
     function _Browser_visibilityInfo() {
         return (typeof _VirtualDom_doc.hidden !== 'undefined') ?
             {
-                fG: 'hidden',
-                fr: 'visibilitychange'
+                fJ: 'hidden',
+                fu: 'visibilitychange'
             } :
             (typeof _VirtualDom_doc.mozHidden !== 'undefined') ?
             {
-                fG: 'mozHidden',
-                fr: 'mozvisibilitychange'
+                fJ: 'mozHidden',
+                fu: 'mozvisibilitychange'
             } :
             (typeof _VirtualDom_doc.msHidden !== 'undefined') ?
             {
-                fG: 'msHidden',
-                fr: 'msvisibilitychange'
+                fJ: 'msHidden',
+                fu: 'msvisibilitychange'
             } :
             (typeof _VirtualDom_doc.webkitHidden !== 'undefined') ?
             {
-                fG: 'webkitHidden',
-                fr: 'webkitvisibilitychange'
+                fJ: 'webkitHidden',
+                fu: 'webkitvisibilitychange'
             } :
             {
-                fG: 'hidden',
-                fr: 'visibilitychange'
+                fJ: 'hidden',
+                fu: 'visibilitychange'
             };
     }
 
 
 
     // ANIMATION FRAMES
 
@@ -4020,30 +4020,30 @@
 
 
     // WINDOW VIEWPORT
 
 
     function _Browser_getViewport() {
         return {
-            eV: _Browser_getScene(),
-            fc: {
-                fg: _Browser_window.pageXOffset,
-                fh: _Browser_window.pageYOffset,
-                ff: _Browser_doc.documentElement.clientWidth,
-                eb: _Browser_doc.documentElement.clientHeight
+            eZ: _Browser_getScene(),
+            ff: {
+                fj: _Browser_window.pageXOffset,
+                fk: _Browser_window.pageYOffset,
+                fi: _Browser_doc.documentElement.clientWidth,
+                ea: _Browser_doc.documentElement.clientHeight
             }
         };
     }
 
     function _Browser_getScene() {
         var body = _Browser_doc.body;
         var elem = _Browser_doc.documentElement;
         return {
-            ff: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
-            eb: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
+            fi: Math.max(body.scrollWidth, body.offsetWidth, elem.scrollWidth, elem.offsetWidth, elem.clientWidth),
+            ea: Math.max(body.scrollHeight, body.offsetHeight, elem.scrollHeight, elem.offsetHeight, elem.clientHeight)
         };
     }
 
     var _Browser_setViewport = F2(function(x, y) {
         return _Browser_withWindow(function() {
             _Browser_window.scroll(x, y);
             return _Utils_Tuple0;
@@ -4054,23 +4054,23 @@
 
     // ELEMENT VIEWPORT
 
 
     function _Browser_getViewportOf(id) {
         return _Browser_withNode(id, function(node) {
             return {
-                eV: {
-                    ff: node.scrollWidth,
-                    eb: node.scrollHeight
+                eZ: {
+                    fi: node.scrollWidth,
+                    ea: node.scrollHeight
                 },
-                fc: {
-                    fg: node.scrollLeft,
-                    fh: node.scrollTop,
-                    ff: node.clientWidth,
-                    eb: node.clientHeight
+                ff: {
+                    fj: node.scrollLeft,
+                    fk: node.scrollTop,
+                    fi: node.clientWidth,
+                    ea: node.clientHeight
                 }
             };
         });
     }
 
 
     var _Browser_setViewportOf = F3(function(id, x, y) {
@@ -4088,26 +4088,26 @@
 
     function _Browser_getElement(id) {
         return _Browser_withNode(id, function(node) {
             var rect = node.getBoundingClientRect();
             var x = _Browser_window.pageXOffset;
             var y = _Browser_window.pageYOffset;
             return {
-                eV: _Browser_getScene(),
-                fc: {
-                    fg: x,
-                    fh: y,
-                    ff: _Browser_doc.documentElement.clientWidth,
-                    eb: _Browser_doc.documentElement.clientHeight
+                eZ: _Browser_getScene(),
+                ff: {
+                    fj: x,
+                    fk: y,
+                    fi: _Browser_doc.documentElement.clientWidth,
+                    ea: _Browser_doc.documentElement.clientHeight
                 },
-                fB: {
-                    fg: x + rect.left,
-                    fh: y + rect.top,
-                    ff: rect.width,
-                    eb: rect.height
+                fE: {
+                    fj: x + rect.left,
+                    fk: y + rect.top,
+                    fi: rect.width,
+                    ea: rect.height
                 }
             };
         });
     }
 
 
 
@@ -4174,58 +4174,58 @@
 
 
     // SEND REQUEST
 
     var _Http_toTask = F3(function(router, toTask, request) {
         return _Scheduler_binding(function(callback) {
             function done(response) {
-                callback(toTask(request.d3.a(response)));
+                callback(toTask(request.cZ.a(response)));
             }
 
             var xhr = new XMLHttpRequest();
             xhr.addEventListener('error', function() {
                 done($elm$http$Http$NetworkError_);
             });
             xhr.addEventListener('timeout', function() {
                 done($elm$http$Http$Timeout_);
             });
             xhr.addEventListener('load', function() {
-                done(_Http_toResponse(request.d3.b, xhr));
+                done(_Http_toResponse(request.cZ.b, xhr));
             });
-            $elm$core$Maybe$isJust(request.e8) && _Http_track(router, xhr, request.e8.a);
+            $elm$core$Maybe$isJust(request.fc) && _Http_track(router, xhr, request.fc.a);
 
             try {
-                xhr.open(request.fU, request.fb, true);
+                xhr.open(request.fX, request.dF, true);
             } catch (e) {
-                return done($elm$http$Http$BadUrl_(request.fb));
+                return done($elm$http$Http$BadUrl_(request.dF));
             }
 
             _Http_configureRequest(xhr, request);
 
-            request.fp.a && xhr.setRequestHeader('Content-Type', request.fp.a);
-            xhr.send(request.fp.b);
+            request.fs.a && xhr.setRequestHeader('Content-Type', request.fs.a);
+            xhr.send(request.fs.b);
 
             return function() {
                 xhr.c = true;
                 xhr.abort();
             };
         });
     });
 
 
     // CONFIGURE
 
     function _Http_configureRequest(xhr, request) {
-        for (var headers = request.ea; headers.b; headers = headers.b) // WHILE_CONS
+        for (var headers = request.d9; headers.b; headers = headers.b) // WHILE_CONS
         {
             xhr.setRequestHeader(headers.a.a, headers.a.b);
         }
-        xhr.timeout = request.gd.a || 0;
-        xhr.responseType = request.d3.d;
-        xhr.withCredentials = request.fk;
+        xhr.timeout = request.gg.a || 0;
+        xhr.responseType = request.cZ.d;
+        xhr.withCredentials = request.fn;
     }
 
 
     // RESPONSES
 
     function _Http_toResponse(toBody, xhr) {
         return A2(
@@ -4236,18 +4236,18 @@
     }
 
 
     // METADATA
 
     function _Http_toMetadata(xhr) {
         return {
-            fb: xhr.responseURL,
-            f8: xhr.status,
-            f9: xhr.statusText,
-            ea: _Http_parseHeaders(xhr.getAllResponseHeaders())
+            dF: xhr.responseURL,
+            gb: xhr.status,
+            gc: xhr.statusText,
+            d9: _Http_parseHeaders(xhr.getAllResponseHeaders())
         };
     }
 
 
     // HEADERS
 
     function _Http_parseHeaders(rawHeaders) {
@@ -4338,25 +4338,25 @@
         // TODO check out lengthComputable on loadstart event
 
         xhr.upload.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Sending({
-                f5: event.loaded,
-                eZ: event.total
+                f8: event.loaded,
+                e1: event.total
             }))));
         });
         xhr.addEventListener('progress', function(event) {
             if (xhr.c) {
                 return;
             }
             _Scheduler_rawSpawn(A2($elm$core$Platform$sendToSelf, router, _Utils_Tuple2(tracker, $elm$http$Http$Receiving({
-                f0: event.loaded,
-                eZ: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
+                f3: event.loaded,
+                e1: event.lengthComputable ? $elm$core$Maybe$Just(event.total) : $elm$core$Maybe$Nothing
             }))));
         });
     }
 
 
     var _Bitwise_and = F2(function(a, b) {
         return a & b;
@@ -4926,20 +4926,20 @@
     };
     var $elm$browser$Browser$Dom$NotFound = $elm$core$Basics$identity;
     var $elm$url$Url$Http = 0;
     var $elm$url$Url$Https = 1;
     var $elm$url$Url$Url = F6(
         function(protocol, host, port_, path, query, fragment) {
             return {
-                d8: fragment,
-                ec: host,
-                eB: path,
-                eF: port_,
-                eK: protocol,
-                eL: query
+                d7: fragment,
+                eb: host,
+                eD: path,
+                eH: port_,
+                eM: protocol,
+                eN: query
             };
         });
     var $elm$core$String$contains = _String_contains;
     var $elm$core$String$length = _String_length;
     var $elm$core$String$slice = _String_slice;
     var $elm$core$String$dropLeft = F2(
         function(n, string) {
@@ -5210,22 +5210,30 @@
     var $elm$core$Task$command = _Platform_leaf('Task');
     var $elm$core$Task$perform = F2(
         function(toMessage, task) {
             return $elm$core$Task$command(
                 A2($elm$core$Task$map, toMessage, task));
         });
     var $elm$browser$Browser$element = _Browser_element;
+    var $author$project$Main$Epa = 0;
     var $author$project$Main$FetchData = function(a) {
         return {
             $: 0,
             a: a
         };
     };
+    var $author$project$Main$FetchLatest = function(a) {
+        return {
+            $: 1,
+            a: a
+        };
+    };
     var $author$project$Main$Hour = 1;
     var $author$project$DeviceStatus$Idle = 2;
+    var $elm$core$Platform$Cmd$batch = _Platform_batch;
     var $elm$time$Time$Name = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $elm$time$Time$Offset = function(a) {
@@ -5244,46 +5252,51 @@
         });
     var $elm$time$Time$customZone = $elm$time$Time$Zone;
     var $elm$time$Time$Posix = $elm$core$Basics$identity;
     var $elm$time$Time$millisToPosix = $elm$core$Basics$identity;
     var $elm$time$Time$now = _Time_now($elm$time$Time$millisToPosix);
     var $author$project$Main$init = function(_v0) {
         return _Utils_Tuple2({
+                bp: _List_Nil,
                 bq: _List_Nil,
-                br: _List_Nil,
-                dW: $elm$core$Maybe$Nothing,
-                dX: true,
-                T: {
-                    ak: '',
-                    al: '',
-                    an: false
+                aO: 0,
+                dU: $elm$core$Maybe$Nothing,
+                dV: true,
+                G: {
+                    U: '',
+                    V: '',
+                    W: false
                 },
+                bV: _List_Nil,
                 bW: _List_Nil,
-                bX: _List_Nil,
-                aE: {
-                    d1: 0.0,
-                    c_: 0,
-                    eD: 0.0,
-                    eE: 0.0,
-                    dq: 0
+                ad: {
+                    d$: $elm$core$Maybe$Nothing,
+                    d0: $elm$core$Maybe$Nothing,
+                    eF: $elm$core$Maybe$Nothing,
+                    eG: $elm$core$Maybe$Nothing
                 },
-                b$: $elm$core$Maybe$Nothing,
-                V: {
-                    dW: $elm$core$Maybe$Nothing,
+                b_: $elm$core$Maybe$Nothing,
+                Y: {
+                    dU: $elm$core$Maybe$Nothing,
                     eo: $elm$core$Maybe$Nothing,
-                    ey: $elm$core$Maybe$Nothing,
-                    a2: 2
+                    eA: $elm$core$Maybe$Nothing,
+                    a1: 2
                 },
-                ae: 1
+                ai: 1
             },
-            A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now));
+            $elm$core$Platform$Cmd$batch(
+                _List_fromArray(
+                    [
+                        A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now),
+                        A2($elm$core$Task$perform, $author$project$Main$FetchLatest, $elm$time$Time$now)
+                    ])));
     };
     var $author$project$Main$Tick = function(a) {
         return {
-            $: 7,
+            $: 9,
             a: a
         };
     };
     var $elm$core$Platform$Sub$batch = _Platform_batch;
     var $elm$time$Time$Every = F2(
         function(a, b) {
             return {
@@ -5291,16 +5304,16 @@
                 a: a,
                 b: b
             };
         });
     var $elm$time$Time$State = F2(
         function(taggers, processes) {
             return {
-                eJ: processes,
-                e0: taggers
+                eL: processes,
+                e4: taggers
             };
         });
     var $elm$core$Dict$RBEmpty_elm_builtin = {
         $: -2
     };
     var $elm$core$Dict$empty = $elm$core$Dict$RBEmpty_elm_builtin;
     var $elm$time$Time$init = $elm$core$Task$succeed(
@@ -5580,15 +5593,15 @@
                         A3($elm$core$Dict$insert, interval, id, processes));
                 };
                 return A2($elm$core$Task$andThen, spawnRest, spawnTimer);
             }
         });
     var $elm$time$Time$onEffects = F3(
         function(router, subs, _v0) {
-            var processes = _v0.eJ;
+            var processes = _v0.eL;
             var rightStep = F3(
                 function(_v6, id, _v7) {
                     var spawns = _v7.a;
                     var existing = _v7.b;
                     var kills = _v7.c;
                     return _Utils_Tuple3(
                         spawns,
@@ -5646,15 +5659,15 @@
                     function(_v2) {
                         return A3($elm$time$Time$spawnHelp, router, spawnList, existingDict);
                     },
                     killTask));
         });
     var $elm$time$Time$onSelfMsg = F3(
         function(router, interval, state) {
-            var _v0 = A2($elm$core$Dict$get, interval, state.e0);
+            var _v0 = A2($elm$core$Dict$get, interval, state.e4);
             if (_v0.$ === 1) {
                 return $elm$core$Task$succeed(state);
             } else {
                 var taggers = _v0.a;
                 var tellTaggers = function(time) {
                     return $elm$core$Task$sequence(
                         A2(
@@ -5697,23 +5710,25 @@
                 A2($elm$time$Time$Every, interval, tagger));
         });
     var $author$project$Main$subscriptions = function(model) {
         return $elm$core$Platform$Sub$batch(
             _List_fromArray(
                 [
                     A2($elm$time$Time$every, 5000, $author$project$Main$FetchData),
+                    A2($elm$time$Time$every, 5000, $author$project$Main$FetchLatest),
                     A2($elm$time$Time$every, 500, $author$project$Main$Tick)
                 ]));
     };
     var $author$project$Main$FetchStatus = function(a) {
         return {
-            $: 1,
+            $: 2,
             a: a
         };
     };
+    var $author$project$Main$ParticleMatter = 1;
     var $author$project$Main$errorToString = function(error) {
         switch (error.$) {
             case 0:
                 var url = error.a;
                 return 'The URL ' + (url + ' was invalid');
             case 1:
                 return 'Unable to reach the server, try again';
@@ -5731,47 +5746,47 @@
             default:
                 var errorMessage = error.a;
                 return errorMessage;
         }
     };
     var $author$project$Main$GotData = function(a) {
         return {
-            $: 2,
+            $: 3,
             a: a
         };
     };
     var $author$project$Main$AllData = F2(
         function(reads, epas) {
             return {
-                c$: epas,
-                dr: reads
+                d1: epas,
+                eQ: reads
             };
         });
     var $author$project$Main$EpaData = F2(
         function(time, epa) {
             return {
-                d1: epa,
-                cG: time
+                d$: epa,
+                cF: time
             };
         });
     var $elm$json$Json$Decode$field = _Json_decodeField;
     var $elm$json$Json$Decode$float = _Json_decodeFloat;
     var $elm$json$Json$Decode$list = _Json_decodeList;
     var $author$project$Main$epaDataDecoder = $elm$json$Json$Decode$list(
         A3(
             $elm$json$Json$Decode$map2,
             $author$project$Main$EpaData,
             A2($elm$json$Json$Decode$field, 't', $elm$json$Json$Decode$float),
             A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float)));
     var $author$project$Main$ReadData = F3(
         function(time, pm25, pm10) {
             return {
-                eD: pm10,
-                eE: pm25,
-                cG: time
+                eF: pm10,
+                eG: pm25,
+                cF: time
             };
         });
     var $elm$json$Json$Decode$map3 = _Json_map3;
     var $author$project$Main$readDataDecoder = $elm$json$Json$Decode$list(
         A4(
             $elm$json$Json$Decode$map3,
             $author$project$Main$ReadData,
@@ -6260,15 +6275,15 @@
                 case 1:
                     return $elm$core$Result$Err($elm$http$Http$Timeout);
                 case 2:
                     return $elm$core$Result$Err($elm$http$Http$NetworkError);
                 case 3:
                     var metadata = response.a;
                     return $elm$core$Result$Err(
-                        $elm$http$Http$BadStatus(metadata.f8));
+                        $elm$http$Http$BadStatus(metadata.gb));
                 default:
                     var body = response.b;
                     return A2(
                         $elm$core$Result$mapError,
                         $elm$http$Http$BadBody,
                         toResult(body));
             }
@@ -6292,16 +6307,16 @@
             $: 1,
             a: a
         };
     };
     var $elm$http$Http$State = F2(
         function(reqs, subs) {
             return {
-                eP: reqs,
-                e$: subs
+                eS: reqs,
+                e3: subs
             };
         });
     var $elm$http$Http$init = $elm$core$Task$succeed(
         A2($elm$http$Http$State, $elm$core$Dict$empty, _List_Nil));
     var $elm$http$Http$updateReqs = F3(
         function(router, cmds, reqs) {
             updateReqs: while (true) {
@@ -6335,15 +6350,15 @@
                                 $elm$core$Process$kill(pid));
                         }
                     } else {
                         var req = cmd.a;
                         return A2(
                             $elm$core$Task$andThen,
                             function(pid) {
-                                var _v4 = req.e8;
+                                var _v4 = req.fc;
                                 if (_v4.$ === 1) {
                                     return A3($elm$http$Http$updateReqs, router, otherCmds, reqs);
                                 } else {
                                     var tracker = _v4.a;
                                     return A3(
                                         $elm$http$Http$updateReqs,
                                         router,
@@ -6365,15 +6380,15 @@
         function(router, cmds, subs, state) {
             return A2(
                 $elm$core$Task$andThen,
                 function(reqs) {
                     return $elm$core$Task$succeed(
                         A2($elm$http$Http$State, reqs, subs));
                 },
-                A3($elm$http$Http$updateReqs, router, cmds, state.eP));
+                A3($elm$http$Http$updateReqs, router, cmds, state.eS));
         });
     var $elm$core$List$maybeCons = F3(
         function(f, mx, xs) {
             var _v0 = f(mx);
             if (!_v0.$) {
                 var x = _v0.a;
                 return A2($elm$core$List$cons, x, xs);
@@ -6408,15 +6423,15 @@
                 function(_v1) {
                     return $elm$core$Task$succeed(state);
                 },
                 $elm$core$Task$sequence(
                     A2(
                         $elm$core$List$filterMap,
                         A3($elm$http$Http$maybeSend, router, tracker, progress),
-                        state.e$)));
+                        state.e3)));
         });
     var $elm$http$Http$Cancel = function(a) {
         return {
             $: 0,
             a: a
         };
     };
@@ -6424,22 +6439,22 @@
         function(func, cmd) {
             if (!cmd.$) {
                 var tracker = cmd.a;
                 return $elm$http$Http$Cancel(tracker);
             } else {
                 var r = cmd.a;
                 return $elm$http$Http$Request({
-                    fk: r.fk,
-                    fp: r.fp,
-                    d3: A2(_Http_mapExpect, func, r.d3),
-                    ea: r.ea,
-                    fU: r.fU,
-                    gd: r.gd,
-                    e8: r.e8,
-                    fb: r.fb
+                    fn: r.fn,
+                    fs: r.fs,
+                    cZ: A2(_Http_mapExpect, func, r.cZ),
+                    d9: r.d9,
+                    fX: r.fX,
+                    gg: r.gg,
+                    fc: r.fc,
+                    dF: r.dF
                 });
             }
         });
     var $elm$http$Http$MySub = F2(
         function(a, b) {
             return {
                 $: 0,
@@ -6458,33 +6473,33 @@
         });
     _Platform_effectManagers['Http'] = _Platform_createManager($elm$http$Http$init, $elm$http$Http$onEffects, $elm$http$Http$onSelfMsg, $elm$http$Http$cmdMap, $elm$http$Http$subMap);
     var $elm$http$Http$command = _Platform_leaf('Http');
     var $elm$http$Http$subscription = _Platform_leaf('Http');
     var $elm$http$Http$request = function(r) {
         return $elm$http$Http$command(
             $elm$http$Http$Request({
-                fk: false,
-                fp: r.fp,
-                d3: r.d3,
-                ea: r.ea,
-                fU: r.fU,
-                gd: r.gd,
-                e8: r.e8,
-                fb: r.fb
+                fn: false,
+                fs: r.fs,
+                cZ: r.cZ,
+                d9: r.d9,
+                fX: r.fX,
+                gg: r.gg,
+                fc: r.fc,
+                dF: r.dF
             }));
     };
     var $elm$http$Http$get = function(r) {
         return $elm$http$Http$request({
-            fp: $elm$http$Http$emptyBody,
-            d3: r.d3,
-            ea: _List_Nil,
-            fU: 'GET',
-            gd: $elm$core$Maybe$Nothing,
-            e8: $elm$core$Maybe$Nothing,
-            fb: r.fb
+            fs: $elm$http$Http$emptyBody,
+            cZ: r.cZ,
+            d9: _List_Nil,
+            fX: 'GET',
+            gg: $elm$core$Maybe$Nothing,
+            fc: $elm$core$Maybe$Nothing,
+            dF: r.dF
         });
     };
     var $author$project$Main$getData = function(windowDuration) {
         var stringDuration = function() {
             switch (windowDuration) {
                 case 0:
                     return 'all';
@@ -6493,93 +6508,106 @@
                 case 2:
                     return 'day';
                 default:
                     return 'week';
             }
         }();
         return $elm$http$Http$get({
-            d3: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$allDataDecoder),
-            fb: '/api/sensor_data?window=' + stringDuration
+            cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotData, $author$project$Main$allDataDecoder),
+            dF: '/api/sensor_data?window=' + stringDuration
         });
     };
-    var $elm$core$List$head = function(list) {
-        if (list.b) {
-            var x = list.a;
-            var xs = list.b;
-            return $elm$core$Maybe$Just(x);
-        } else {
-            return $elm$core$Maybe$Nothing;
-        }
-    };
-    var $author$project$Main$getLastListItem = function(allData) {
-        var lastReads = function() {
-            var _v1 = $elm$core$List$head(
-                $elm$core$List$reverse(allData.dr));
-            if (!_v1.$) {
-                var a = _v1.a;
-                return a;
-            } else {
-                return {
-                    eD: 0,
-                    eE: 0,
-                    cG: 0
-                };
-            }
-        }();
-        var lastEpas = function() {
-            var _v0 = $elm$core$List$head(
-                $elm$core$List$reverse(allData.c$));
-            if (!_v0.$) {
-                var a = _v0.a;
-                return a;
-            } else {
-                return {
-                    d1: 0,
-                    cG: 0
-                };
-            }
-        }();
+    var $author$project$Main$GotLatest = function(a) {
         return {
-            d1: lastEpas.d1,
-            c_: lastEpas.cG,
-            eD: lastReads.eD,
-            eE: lastReads.eE,
-            dq: lastReads.cG
-        };
-    };
-    var $author$project$Main$GotStatus = function(a) {
-        return {
-            $: 3,
+            $: 4,
             a: a
         };
     };
-    var $author$project$Main$DeviceInfoResponse = F3(
-        function(readerStatus, readerException, nextSchedule) {
+    var $author$project$Main$LatestData = F4(
+        function(pm25, pm10, epa, epaLevel) {
             return {
-                ey: nextSchedule,
-                eM: readerException,
-                eN: readerStatus
+                d$: epa,
+                d0: epaLevel,
+                eF: pm10,
+                eG: pm25
             };
         });
-    var $elm$json$Json$Decode$int = _Json_decodeInt;
+    var $author$project$EpaCommon$Good = 5;
+    var $author$project$EpaCommon$Hazardous = 0;
+    var $author$project$EpaCommon$Moderate = 4;
+    var $author$project$EpaCommon$Unhealthy = 2;
+    var $author$project$EpaCommon$UnhealthyForSensitive = 3;
+    var $author$project$EpaCommon$VeryUnhealthy = 1;
+    var $elm$json$Json$Decode$andThen = _Json_andThen;
+    var $elm$json$Json$Decode$fail = _Json_fail;
+    var $elm$json$Json$Decode$string = _Json_decodeString;
+    var $author$project$Main$epaLevelDecoder = A2(
+        $elm$json$Json$Decode$andThen,
+        function(str) {
+            switch (str) {
+                case 'HAZARDOUS':
+                    return $elm$json$Json$Decode$succeed(0);
+                case 'VERY_UNHEALTHY':
+                    return $elm$json$Json$Decode$succeed(1);
+                case 'UNHEALTHY':
+                    return $elm$json$Json$Decode$succeed(2);
+                case 'UNHEALTHY_FOR_SENSITIVE':
+                    return $elm$json$Json$Decode$succeed(3);
+                case 'MODERATE':
+                    return $elm$json$Json$Decode$succeed(4);
+                case 'GOOD':
+                    return $elm$json$Json$Decode$succeed(5);
+                default:
+                    return $elm$json$Json$Decode$fail('Invalid Epa Level');
+            }
+        },
+        $elm$json$Json$Decode$string);
+    var $elm$json$Json$Decode$map4 = _Json_map4;
     var $elm$json$Json$Decode$oneOf = _Json_oneOf;
     var $elm$json$Json$Decode$maybe = function(decoder) {
         return $elm$json$Json$Decode$oneOf(
             _List_fromArray(
                 [
                     A2($elm$json$Json$Decode$map, $elm$core$Maybe$Just, decoder),
                     $elm$json$Json$Decode$succeed($elm$core$Maybe$Nothing)
                 ]));
     };
+    var $author$project$Main$latestDataDecoder = A5(
+        $elm$json$Json$Decode$map4,
+        $author$project$Main$LatestData,
+        $elm$json$Json$Decode$maybe(
+            A2($elm$json$Json$Decode$field, 'pm25', $elm$json$Json$Decode$float)),
+        $elm$json$Json$Decode$maybe(
+            A2($elm$json$Json$Decode$field, 'pm10', $elm$json$Json$Decode$float)),
+        $elm$json$Json$Decode$maybe(
+            A2($elm$json$Json$Decode$field, 'epa', $elm$json$Json$Decode$float)),
+        $elm$json$Json$Decode$maybe(
+            A2($elm$json$Json$Decode$field, 'level', $author$project$Main$epaLevelDecoder)));
+    var $author$project$Main$getLatest = $elm$http$Http$get({
+        cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotLatest, $author$project$Main$latestDataDecoder),
+        dF: '/api/latest_data'
+    });
+    var $author$project$Main$GotStatus = function(a) {
+        return {
+            $: 5,
+            a: a
+        };
+    };
+    var $author$project$Main$DeviceInfoResponse = F3(
+        function(readerStatus, readerException, nextSchedule) {
+            return {
+                eA: nextSchedule,
+                eO: readerException,
+                eP: readerStatus
+            };
+        });
+    var $elm$json$Json$Decode$int = _Json_decodeInt;
     var $author$project$DeviceStatus$Failing = 3;
     var $author$project$DeviceStatus$Reading = 0;
     var $author$project$DeviceStatus$WarmingUp = 1;
-    var $elm$json$Json$Decode$andThen = _Json_andThen;
-    var $elm$json$Json$Decode$fail = _Json_fail;
-    var $elm$json$Json$Decode$string = _Json_decodeString;
     var $author$project$Main$stateDecoder = A2(
         $elm$json$Json$Decode$andThen,
         function(str) {
             switch (str) {
                 case 'IDLE':
                     return $elm$json$Json$Decode$succeed(2);
                 case 'WARM_UP':
@@ -6598,28 +6626,27 @@
         $author$project$Main$DeviceInfoResponse,
         A2($elm$json$Json$Decode$field, 'reader_status', $author$project$Main$stateDecoder),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'reader_exception', $elm$json$Json$Decode$string)),
         $elm$json$Json$Decode$maybe(
             A2($elm$json$Json$Decode$field, 'next_schedule', $elm$json$Json$Decode$int)));
     var $author$project$Main$getStatus = $elm$http$Http$get({
-        d3: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
-        fb: '/api/status'
+        cZ: A2($elm$http$Http$expectJson, $author$project$Main$GotStatus, $author$project$Main$statusDecoder),
+        dF: '/api/status'
     });
     var $elm$core$Maybe$map = F2(
         function(f, maybe) {
             if (!maybe.$) {
                 var value = maybe.a;
                 return $elm$core$Maybe$Just(
                     f(value));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
         });
-    var $elm$core$Platform$Cmd$batch = _Platform_batch;
     var $elm$core$Platform$Cmd$none = $elm$core$Platform$Cmd$batch(_List_Nil);
     var $elm$time$Time$posixToMillis = function(_v0) {
         var millis = _v0;
         return millis;
     };
     var $author$project$Main$getDuration = F2(
         function(currentTime, scheduledTime) {
@@ -6657,167 +6684,226 @@
         function(model, currentTime) {
             var timeToNextRead = A2(
                 $elm$core$Maybe$withDefault,
                 1,
                 A3(
                     $elm$core$Maybe$map2,
                     $author$project$Main$getDuration,
-                    model.V.ey,
+                    model.Y.eA,
                     $elm$core$Maybe$Just(currentTime)));
             var maxTimeBetweenPolls = 15000;
             var timeSinceLastPoll = A2(
                 $elm$core$Maybe$withDefault,
                 maxTimeBetweenPolls + 1,
                 A3(
                     $elm$core$Maybe$map2,
                     $author$project$Main$getDuration,
-                    model.b$,
+                    model.b_,
                     $elm$core$Maybe$Just(currentTime)));
-            return ((!model.V.a2) || (model.V.a2 === 1)) || ((_Utils_cmp(timeSinceLastPoll, maxTimeBetweenPolls) > 0) || (_Utils_cmp(timeToNextRead, -1) > 0));
+            return ((!model.Y.a1) || (model.Y.a1 === 1)) || ((_Utils_cmp(timeSinceLastPoll, maxTimeBetweenPolls) > 0) || (_Utils_cmp(timeToNextRead, -1) > 0));
         });
     var $author$project$Main$update = F2(
         function(msg, model) {
             switch (msg.$) {
-                case 2:
+                case 3:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    bq: data.c$,
-                                    br: data.dr,
-                                    T: {
-                                        ak: '',
-                                        al: '',
-                                        an: false
-                                    },
-                                    aE: $author$project$Main$getLastListItem(data)
+                                    bp: data.d1,
+                                    bq: data.eQ,
+                                    G: {
+                                        U: '',
+                                        V: '',
+                                        W: false
+                                    }
                                 }),
                             $elm$core$Platform$Cmd$none);
                     } else {
                         var e = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    T: {
-                                        ak: $author$project$Main$errorToString(e),
-                                        al: 'Failed to retrieve read data',
-                                        an: true
+                                    G: {
+                                        U: $author$project$Main$errorToString(e),
+                                        V: 'Failed to retrieve read data',
+                                        W: true
                                     }
                                 }),
                             $elm$core$Platform$Cmd$none);
                     }
                 case 0:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dW: $elm$core$Maybe$Just(newTime)
+                                dU: $elm$core$Maybe$Just(newTime)
                             }),
-                        $author$project$Main$getData(model.ae));
-                case 3:
+                        $author$project$Main$getData(model.ai));
+                case 4:
+                    var result = msg.a;
+                    if (!result.$) {
+                        var data = result.a;
+                        return _Utils_Tuple2(
+                            _Utils_update(
+                                model, {
+                                    G: {
+                                        U: '',
+                                        V: '',
+                                        W: false
+                                    },
+                                    ad: data
+                                }),
+                            $elm$core$Platform$Cmd$none);
+                    } else {
+                        var e = result.a;
+                        return _Utils_Tuple2(
+                            _Utils_update(
+                                model, {
+                                    G: {
+                                        U: $author$project$Main$errorToString(e),
+                                        V: 'Failed to retrieve latest data',
+                                        W: true
+                                    }
+                                }),
+                            $elm$core$Platform$Cmd$none);
+                    }
+                case 1:
+                    var newTime = msg.a;
+                    return _Utils_Tuple2(
+                        _Utils_update(
+                            model, {
+                                dU: $elm$core$Maybe$Just(newTime)
+                            }),
+                        $author$project$Main$getLatest);
+                case 5:
                     var result = msg.a;
                     if (!result.$) {
                         var data = result.a;
                         var deviceInfo = {
-                            dW: model.dW,
-                            eo: data.eM,
-                            ey: A2($elm$core$Maybe$map, $elm$time$Time$millisToPosix, data.ey),
-                            a2: data.eN
+                            dU: model.dU,
+                            eo: data.eO,
+                            eA: A2($elm$core$Maybe$map, $elm$time$Time$millisToPosix, data.eA),
+                            a1: data.eP
                         };
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    T: {
-                                        ak: '',
-                                        al: '',
-                                        an: false
+                                    G: {
+                                        U: '',
+                                        V: '',
+                                        W: false
                                     },
-                                    V: deviceInfo
+                                    Y: deviceInfo
                                 }),
                             $elm$core$Platform$Cmd$none);
                     } else {
                         var e = result.a;
                         return _Utils_Tuple2(
                             _Utils_update(
                                 model, {
-                                    T: {
-                                        ak: $author$project$Main$errorToString(e),
-                                        al: 'Failed to retrieve device status',
-                                        an: true
+                                    G: {
+                                        U: $author$project$Main$errorToString(e),
+                                        V: 'Failed to retrieve device status',
+                                        W: true
                                     }
                                 }),
                             $elm$core$Platform$Cmd$none);
                     }
-                case 1:
+                case 2:
                     var newTime = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dW: $elm$core$Maybe$Just(newTime),
-                                b$: $elm$core$Maybe$Just(newTime)
+                                dU: $elm$core$Maybe$Just(newTime),
+                                b_: $elm$core$Maybe$Just(newTime)
                             }),
                         $author$project$Main$getStatus);
-                case 4:
+                case 6:
                     var window = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                ae: window
+                                ai: window
                             }),
                         A2($elm$core$Task$perform, $author$project$Main$FetchData, $elm$time$Time$now));
-                case 5:
+                case 7:
                     var hovering = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bX: hovering
+                                bW: hovering
                             }),
                         $elm$core$Platform$Cmd$none);
-                case 6:
+                case 8:
                     var hovering = msg.a;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                bW: hovering
+                                bV: hovering
                             }),
                         $elm$core$Platform$Cmd$none);
-                default:
+                case 9:
                     var newTime = msg.a;
-                    var readerState = model.V;
+                    var readerState = model.Y;
                     var updatedReaderState = _Utils_update(
                         readerState, {
-                            dW: $elm$core$Maybe$Just(newTime)
+                            dU: $elm$core$Maybe$Just(newTime)
                         });
                     var cmd = A2($author$project$Main$shouldFetchStatus, model, newTime) ? A2($elm$core$Task$perform, $author$project$Main$FetchStatus, $elm$time$Time$now) : $elm$core$Platform$Cmd$none;
                     return _Utils_Tuple2(
                         _Utils_update(
                             model, {
-                                dW: $elm$core$Maybe$Just(newTime),
-                                V: updatedReaderState
+                                dU: $elm$core$Maybe$Just(newTime),
+                                Y: updatedReaderState
                             }),
                         cmd);
+                default:
+                    var newView = msg.a;
+                    var newGraph = (newView === 'pm') ? 1 : 0;
+                    return _Utils_Tuple2(
+                        _Utils_update(
+                            model, {
+                                aO: newGraph
+                            }),
+                        $elm$core$Platform$Cmd$none);
             }
         });
     var $author$project$Main$All = 0;
+    var $author$project$Main$ChangeGraphView = function(a) {
+        return {
+            $: 10,
+            a: a
+        };
+    };
     var $author$project$Main$Day = 2;
     var $author$project$Main$OnEpaHover = function(a) {
         return {
-            $: 6,
+            $: 8,
             a: a
         };
     };
     var $author$project$Main$OnReadHover = function(a) {
         return {
-            $: 5,
+            $: 7,
             a: a
         };
     };
     var $author$project$Main$Week = 3;
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$Attrs = function(a) {
+        return {
+            $: 2,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$attrs = function(attrs_) {
+        return $rundis$elm_bootstrap$Bootstrap$ButtonGroup$Attrs(attrs_);
+    };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColAttrs = function(a) {
         return {
             $: 6,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs = function(attrs_) {
@@ -6833,16 +6919,16 @@
         return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowAttrs(attrs_);
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$Center = 1;
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$MD = 2;
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$HAlign = F2(
         function(screenSize, align) {
             return {
-                dO: align,
-                eW: screenSize
+                dL: align,
+                e_: screenSize
             };
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$RowHAlign = function(a) {
         return {
             $: 1,
             a: a
         };
@@ -6867,16 +6953,16 @@
             $: 0,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$col = F2(
         function(options, children) {
             return $rundis$elm_bootstrap$Bootstrap$Grid$Column({
-                dT: children,
-                dj: options
+                dR: children,
+                dh: options
             });
         });
     var $elm$html$Html$div = _VirtualDom_node('div');
     var $rundis$elm_bootstrap$Bootstrap$Grid$container = F2(
         function(attributes, children) {
             return A2(
                 $elm$html$Html$div,
@@ -6884,309 +6970,242 @@
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('container')
                         ]),
                     attributes),
                 children);
         });
-    var $author$project$DeviceStatus$deviceStatusColor = function(deviceStatus) {
-        switch (deviceStatus) {
+    var $elm$html$Html$a = _VirtualDom_node('a');
+    var $elm$core$String$fromFloat = _String_fromNumber;
+    var $author$project$EpaCommon$getColorForLevel = function(level) {
+        switch (level) {
             case 0:
-                return 'green';
+                return 'maroon';
             case 1:
-                return 'orange';
+                return 'purple';
             case 2:
-                return 'gray';
-            default:
                 return 'red';
-        }
-    };
-    var $author$project$DeviceStatus$deviceStatusImage = function(deviceStatus) {
-        switch (deviceStatus) {
-            case 0:
-                return '/static/images/loading.gif';
-            case 1:
-                return '/static/images/loading.gif';
-            case 2:
-                return '/static/images/idle.png';
-            default:
-                return '/static/images/failing.png';
-        }
-    };
-    var $author$project$DeviceStatus$deviceStatusToString = function(deviceStatus) {
-        switch (deviceStatus) {
-            case 0:
-                return 'Reading';
-            case 1:
-                return 'Warming Up';
-            case 2:
-                return 'Idle';
+            case 3:
+                return 'orange';
+            case 4:
+                return 'yellow';
             default:
-                return 'Failing';
+                return 'green';
         }
     };
-    var $elm$core$Basics$modBy = _Basics_modBy;
-    var $elm$core$String$cons = _String_cons;
-    var $elm$core$String$fromChar = function(_char) {
-        return A2($elm$core$String$cons, _char, '');
+    var $elm$html$Html$h1 = _VirtualDom_node('h1');
+    var $elm$html$Html$Attributes$href = function(url) {
+        return A2(
+            $elm$html$Html$Attributes$stringProperty,
+            'href',
+            _VirtualDom_noJavaScriptUri(url));
     };
-    var $elm$core$Bitwise$and = _Bitwise_and;
-    var $elm$core$Bitwise$shiftRightBy = _Bitwise_shiftRightBy;
-    var $elm$core$String$repeatHelp = F3(
-        function(n, chunk, result) {
-            return (n <= 0) ? result : A3(
-                $elm$core$String$repeatHelp,
-                n >> 1,
-                _Utils_ap(chunk, chunk),
-                (!(n & 1)) ? result : _Utils_ap(result, chunk));
-        });
-    var $elm$core$String$repeat = F2(
-        function(n, chunk) {
-            return A3($elm$core$String$repeatHelp, n, chunk, '');
-        });
-    var $elm$core$String$padLeft = F3(
-        function(n, _char, string) {
-            return _Utils_ap(
-                A2(
-                    $elm$core$String$repeat,
-                    n - $elm$core$String$length(string),
-                    $elm$core$String$fromChar(_char)),
-                string);
-        });
-    var $author$project$DeviceStatus$formatDuration = F2(
-        function(currentTime, scheduledTime) {
-            var durationMillis = $elm$time$Time$posixToMillis(scheduledTime) - $elm$time$Time$posixToMillis(currentTime);
-            var hour = (((((durationMillis / 1000) | 0) / 60) | 0) / 60) | 0;
-            var minute = A2($elm$core$Basics$modBy, 60, (((durationMillis / 1000) | 0) / 60) | 0);
-            var second = A2($elm$core$Basics$modBy, 60, (durationMillis / 1000) | 0);
-            return (durationMillis > 0) ? (A3(
-                $elm$core$String$padLeft,
-                2,
-                '0',
-                $elm$core$String$fromInt(hour)) + (':' + (A3(
-                $elm$core$String$padLeft,
-                2,
-                '0',
-                $elm$core$String$fromInt(minute)) + (':' + A3(
-                $elm$core$String$padLeft,
-                2,
-                '0',
-                $elm$core$String$fromInt(second)))))) : '00:00:00';
-        });
-    var $elm$html$Html$h5 = _VirtualDom_node('h5');
-    var $elm$virtual_dom$VirtualDom$text = _VirtualDom_text;
-    var $elm$html$Html$text = $elm$virtual_dom$VirtualDom$text;
-    var $author$project$DeviceStatus$htmlIf = F2(
-        function(el, cond) {
-            return cond ? el : $elm$html$Html$text('');
-        });
-    var $elm$html$Html$img = _VirtualDom_node('img');
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col = 0;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width = F2(
         function(screenSize, columnCount) {
             return {
-                dV: columnCount,
-                eW: screenSize
+                dT: columnCount,
+                e_: screenSize
             };
         });
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$XS = 0;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign = F2(
         function(align_, options) {
-            var _v0 = align_.eW;
+            var _v0 = align_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bp: $elm$core$Maybe$Just(align_)
+                            bo: $elm$core$Maybe$Just(align_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            bn: $elm$core$Maybe$Just(align_)
+                            bm: $elm$core$Maybe$Just(align_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bm: $elm$core$Maybe$Just(align_)
+                            bl: $elm$core$Maybe$Just(align_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            bl: $elm$core$Maybe$Just(align_)
+                            bk: $elm$core$Maybe$Just(align_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bo: $elm$core$Maybe$Just(align_)
+                            bn: $elm$core$Maybe$Just(align_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset = F2(
         function(offset_, options) {
-            var _v0 = offset_.eW;
+            var _v0 = offset_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            ca: $elm$core$Maybe$Just(offset_)
+                            b9: $elm$core$Maybe$Just(offset_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            b7: $elm$core$Maybe$Just(offset_)
+                            b6: $elm$core$Maybe$Just(offset_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            b6: $elm$core$Maybe$Just(offset_)
+                            b5: $elm$core$Maybe$Just(offset_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            b5: $elm$core$Maybe$Just(offset_)
+                            b4: $elm$core$Maybe$Just(offset_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            b9: $elm$core$Maybe$Just(offset_)
+                            b8: $elm$core$Maybe$Just(offset_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOrder = F2(
         function(order_, options) {
-            var _v0 = order_.eW;
+            var _v0 = order_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            ck: $elm$core$Maybe$Just(order_)
+                            cj: $elm$core$Maybe$Just(order_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            ci: $elm$core$Maybe$Just(order_)
+                            ch: $elm$core$Maybe$Just(order_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            ch: $elm$core$Maybe$Just(order_)
+                            cg: $elm$core$Maybe$Just(order_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cg: $elm$core$Maybe$Just(order_)
+                            cf: $elm$core$Maybe$Just(order_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            cj: $elm$core$Maybe$Just(order_)
+                            ci: $elm$core$Maybe$Just(order_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPull = F2(
         function(pull_, options) {
-            var _v0 = pull_.eW;
+            var _v0 = pull_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cq: $elm$core$Maybe$Just(pull_)
+                            cp: $elm$core$Maybe$Just(pull_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            co: $elm$core$Maybe$Just(pull_)
+                            cn: $elm$core$Maybe$Just(pull_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cn: $elm$core$Maybe$Just(pull_)
+                            cm: $elm$core$Maybe$Just(pull_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cm: $elm$core$Maybe$Just(pull_)
+                            cl: $elm$core$Maybe$Just(pull_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            cp: $elm$core$Maybe$Just(pull_)
+                            co: $elm$core$Maybe$Just(pull_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColPush = F2(
         function(push_, options) {
-            var _v0 = push_.eW;
+            var _v0 = push_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cv: $elm$core$Maybe$Just(push_)
+                            cu: $elm$core$Maybe$Just(push_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            ct: $elm$core$Maybe$Just(push_)
+                            cs: $elm$core$Maybe$Just(push_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cs: $elm$core$Maybe$Just(push_)
+                            cr: $elm$core$Maybe$Just(push_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cr: $elm$core$Maybe$Just(push_)
+                            cq: $elm$core$Maybe$Just(push_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            cu: $elm$core$Maybe$Just(push_)
+                            ct: $elm$core$Maybe$Just(push_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth = F2(
         function(width_, options) {
-            var _v0 = width_.eW;
+            var _v0 = width_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bd: $elm$core$Maybe$Just(width_)
+                            bc: $elm$core$Maybe$Just(width_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            bb: $elm$core$Maybe$Just(width_)
+                            ba: $elm$core$Maybe$Just(width_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            ba: $elm$core$Maybe$Just(width_)
+                            a9: $elm$core$Maybe$Just(width_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            a9: $elm$core$Maybe$Just(width_)
+                            a8: $elm$core$Maybe$Just(width_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bc: $elm$core$Maybe$Just(width_)
+                            bb: $elm$core$Maybe$Just(width_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 6:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bu: _Utils_ap(options.bu, attrs)
+                            bt: _Utils_ap(options.bt, attrs)
                         });
                 case 0:
                     var width_ = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColWidth, width_, options);
                 case 1:
                     var offset_ = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOffset, offset_, options);
@@ -7202,15 +7221,15 @@
                 case 5:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColAlign, align, options);
                 default:
                     var align = modifier.a;
                     return _Utils_update(
                         options, {
-                            cF: $elm$core$Maybe$Just(align)
+                            cE: $elm$core$Maybe$Just(align)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$columnCountOption = function(size) {
         switch (size) {
             case 0:
                 return $elm$core$Maybe$Nothing;
@@ -7253,16 +7272,16 @@
             case 3:
                 return $elm$core$Maybe$Just('lg');
             default:
                 return $elm$core$Maybe$Just('xl');
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthClass = function(_v0) {
-        var screenSize = _v0.eW;
-        var columnCount = _v0.dV;
+        var screenSize = _v0.e_;
+        var columnCount = _v0.dT;
         return $elm$html$Html$Attributes$class(
             'col' + (A2(
                 $elm$core$Maybe$withDefault,
                 '',
                 A2(
                     $elm$core$Maybe$map,
                     function(v) {
@@ -7284,46 +7303,46 @@
         };
         return A2(
             $elm$core$List$filterMap,
             $elm$core$Basics$identity,
             A2($elm$core$List$map, width_, widths));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions = {
+        bk: $elm$core$Maybe$Nothing,
         bl: $elm$core$Maybe$Nothing,
         bm: $elm$core$Maybe$Nothing,
         bn: $elm$core$Maybe$Nothing,
         bo: $elm$core$Maybe$Nothing,
-        bp: $elm$core$Maybe$Nothing,
-        bu: _List_Nil,
+        bt: _List_Nil,
+        b4: $elm$core$Maybe$Nothing,
         b5: $elm$core$Maybe$Nothing,
         b6: $elm$core$Maybe$Nothing,
-        b7: $elm$core$Maybe$Nothing,
+        b8: $elm$core$Maybe$Nothing,
         b9: $elm$core$Maybe$Nothing,
-        ca: $elm$core$Maybe$Nothing,
+        cf: $elm$core$Maybe$Nothing,
         cg: $elm$core$Maybe$Nothing,
         ch: $elm$core$Maybe$Nothing,
         ci: $elm$core$Maybe$Nothing,
         cj: $elm$core$Maybe$Nothing,
-        ck: $elm$core$Maybe$Nothing,
+        cl: $elm$core$Maybe$Nothing,
         cm: $elm$core$Maybe$Nothing,
         cn: $elm$core$Maybe$Nothing,
         co: $elm$core$Maybe$Nothing,
         cp: $elm$core$Maybe$Nothing,
         cq: $elm$core$Maybe$Nothing,
         cr: $elm$core$Maybe$Nothing,
         cs: $elm$core$Maybe$Nothing,
         ct: $elm$core$Maybe$Nothing,
         cu: $elm$core$Maybe$Nothing,
-        cv: $elm$core$Maybe$Nothing,
-        cF: $elm$core$Maybe$Nothing,
+        cE: $elm$core$Maybe$Nothing,
+        a8: $elm$core$Maybe$Nothing,
         a9: $elm$core$Maybe$Nothing,
         ba: $elm$core$Maybe$Nothing,
         bb: $elm$core$Maybe$Nothing,
-        bc: $elm$core$Maybe$Nothing,
-        bd: $elm$core$Maybe$Nothing
+        bc: $elm$core$Maybe$Nothing
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption = function(size) {
         switch (size) {
             case 0:
                 return '0';
             case 1:
                 return '1';
@@ -7355,16 +7374,16 @@
             var s = _v0.a;
             return '-' + (s + '-');
         } else {
             return '-';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass = function(_v0) {
-        var screenSize = _v0.eW;
-        var offsetCount = _v0.eA;
+        var screenSize = _v0.e_;
+        var offsetCount = _v0.eC;
         return $elm$html$Html$Attributes$class(
             'offset' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetCountOption(offsetCount)));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes = function(offsets) {
         var offset_ = function(m) {
             return A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetClass, m);
         };
@@ -7404,15 +7423,15 @@
             default:
                 return 'last';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes = function(orders) {
         var order_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.eW;
+                var screenSize = m.a.e_;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'order' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderColOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7451,15 +7470,15 @@
             default:
                 return '12';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes = function(pulls) {
         var pull_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.eW;
+                var screenSize = m.a.e_;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'pull' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7468,15 +7487,15 @@
             $elm$core$List$filterMap,
             $elm$core$Basics$identity,
             A2($elm$core$List$map, pull_, pulls));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes = function(pushes) {
         var push_ = function(m) {
             if (!m.$) {
-                var screenSize = m.a.eW;
+                var screenSize = m.a.e_;
                 var moveCount = m.a.aF;
                 return $elm$core$Maybe$Just(
                     $elm$html$Html$Attributes$class(
                         'push' + ($rundis$elm_bootstrap$Bootstrap$Grid$Internal$screenSizeToPartialString(screenSize) + $rundis$elm_bootstrap$Bootstrap$Grid$Internal$moveCountOption(moveCount))));
             } else {
                 return $elm$core$Maybe$Nothing;
             }
@@ -7493,16 +7512,16 @@
             case 0:
                 return 'left';
             default:
                 return 'right';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass = function(_v0) {
-        var dir = _v0.d_;
-        var size = _v0.eZ;
+        var dir = _v0.dY;
+        var size = _v0.e1;
         return $elm$html$Html$Attributes$class(
             'text' + (A2(
                 $elm$core$Maybe$withDefault,
                 '-',
                 A2(
                     $elm$core$Maybe$map,
                     function(s) {
@@ -7518,16 +7537,16 @@
                 return 'center';
             default:
                 return 'end';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignClass = F2(
         function(prefix, _v0) {
-            var align = _v0.dO;
-            var screenSize = _v0.eW;
+            var align = _v0.dL;
+            var screenSize = _v0.e_;
             return $elm$html$Html$Attributes$class(
                 _Utils_ap(
                     prefix,
                     _Utils_ap(
                         A2(
                             $elm$core$Maybe$withDefault,
                             '',
@@ -7555,181 +7574,181 @@
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes = function(modifiers) {
         var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyColOption, $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultColOptions, modifiers);
         var shouldAddDefaultXs = !$elm$core$List$length(
             A2(
                 $elm$core$List$filterMap,
                 $elm$core$Basics$identity,
                 _List_fromArray(
-                    [options.bd, options.bb, options.ba, options.a9, options.bc])));
+                    [options.bc, options.ba, options.a9, options.a8, options.bb])));
         return _Utils_ap(
             $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colWidthsToAttributes(
                 _List_fromArray(
                     [
                         shouldAddDefaultXs ? $elm$core$Maybe$Just(
-                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.bd,
-                        options.bb,
+                            A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, 0, 0)) : options.bc,
                         options.ba,
                         options.a9,
-                        options.bc
+                        options.a8,
+                        options.bb
                     ])),
             _Utils_ap(
                 $rundis$elm_bootstrap$Bootstrap$Grid$Internal$offsetsToAttributes(
                     _List_fromArray(
-                        [options.ca, options.b7, options.b6, options.b5, options.b9])),
+                        [options.b9, options.b6, options.b5, options.b4, options.b8])),
                 _Utils_ap(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pullsToAttributes(
                         _List_fromArray(
-                            [options.cq, options.co, options.cn, options.cm, options.cp])),
+                            [options.cp, options.cn, options.cm, options.cl, options.co])),
                     _Utils_ap(
                         $rundis$elm_bootstrap$Bootstrap$Grid$Internal$pushesToAttributes(
                             _List_fromArray(
-                                [options.cv, options.ct, options.cs, options.cr, options.cu])),
+                                [options.cu, options.cs, options.cr, options.cq, options.ct])),
                         _Utils_ap(
                             $rundis$elm_bootstrap$Bootstrap$Grid$Internal$orderToAttributes(
                                 _List_fromArray(
-                                    [options.ck, options.ci, options.ch, options.cg, options.cj])),
+                                    [options.cj, options.ch, options.cg, options.cf, options.ci])),
                             _Utils_ap(
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
                                     'align-self-',
                                     _List_fromArray(
-                                        [options.bp, options.bn, options.bm, options.bl, options.bo])),
+                                        [options.bo, options.bm, options.bl, options.bk, options.bn])),
                                 _Utils_ap(
                                     function() {
-                                        var _v0 = options.cF;
+                                        var _v0 = options.cE;
                                         if (!_v0.$) {
                                             var a = _v0.a;
                                             return _List_fromArray(
                                                 [
                                                     $rundis$elm_bootstrap$Bootstrap$Internal$Text$textAlignClass(a)
                                                 ]);
                                         } else {
                                             return _List_Nil;
                                         }
                                     }(),
-                                    options.bu)))))));
+                                    options.bt)))))));
     };
     var $elm$virtual_dom$VirtualDom$keyedNode = function(tag) {
         return _VirtualDom_keyedNode(
             _VirtualDom_noScript(tag));
     };
     var $elm$html$Html$Keyed$node = $elm$virtual_dom$VirtualDom$keyedNode;
     var $rundis$elm_bootstrap$Bootstrap$Grid$renderCol = function(column) {
         switch (column.$) {
             case 0:
-                var options = column.a.dj;
-                var children = column.a.dT;
+                var options = column.a.dh;
+                var children = column.a.dR;
                 return A2(
                     $elm$html$Html$div,
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
                     children);
             case 1:
                 var e = column.a;
                 return e;
             default:
-                var options = column.a.dj;
-                var children = column.a.dT;
+                var options = column.a.dh;
+                var children = column.a.dR;
                 return A3(
                     $elm$html$Html$Keyed$node,
                     'div',
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$colAttributes(options),
                     children);
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign = F2(
         function(align, options) {
-            var _v0 = align.eW;
+            var _v0 = align.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            bT: $elm$core$Maybe$Just(align)
+                            bS: $elm$core$Maybe$Just(align)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            bR: $elm$core$Maybe$Just(align)
+                            bQ: $elm$core$Maybe$Just(align)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bQ: $elm$core$Maybe$Just(align)
+                            bP: $elm$core$Maybe$Just(align)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            bP: $elm$core$Maybe$Just(align)
+                            bO: $elm$core$Maybe$Just(align)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            bS: $elm$core$Maybe$Just(align)
+                            bR: $elm$core$Maybe$Just(align)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign = F2(
         function(align_, options) {
-            var _v0 = align_.eW;
+            var _v0 = align_.e_;
             switch (_v0) {
                 case 0:
                     return _Utils_update(
                         options, {
-                            cP: $elm$core$Maybe$Just(align_)
+                            cO: $elm$core$Maybe$Just(align_)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cN: $elm$core$Maybe$Just(align_)
+                            cM: $elm$core$Maybe$Just(align_)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            cM: $elm$core$Maybe$Just(align_)
+                            cL: $elm$core$Maybe$Just(align_)
                         });
                 case 3:
                     return _Utils_update(
                         options, {
-                            cL: $elm$core$Maybe$Just(align_)
+                            cK: $elm$core$Maybe$Just(align_)
                         });
                 default:
                     return _Utils_update(
                         options, {
-                            cO: $elm$core$Maybe$Just(align_)
+                            cN: $elm$core$Maybe$Just(align_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowOption = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 2:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bu: _Utils_ap(options.bu, attrs)
+                            bt: _Utils_ap(options.bt, attrs)
                         });
                 case 0:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowVAlign, align, options);
                 default:
                     var align = modifier.a;
                     return A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$applyRowHAlign, align, options);
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$defaultRowOptions = {
-        bu: _List_Nil,
+        bt: _List_Nil,
+        bO: $elm$core$Maybe$Nothing,
         bP: $elm$core$Maybe$Nothing,
         bQ: $elm$core$Maybe$Nothing,
         bR: $elm$core$Maybe$Nothing,
         bS: $elm$core$Maybe$Nothing,
-        bT: $elm$core$Maybe$Nothing,
+        cK: $elm$core$Maybe$Nothing,
         cL: $elm$core$Maybe$Nothing,
         cM: $elm$core$Maybe$Nothing,
         cN: $elm$core$Maybe$Nothing,
-        cO: $elm$core$Maybe$Nothing,
-        cP: $elm$core$Maybe$Nothing
+        cO: $elm$core$Maybe$Nothing
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$horizontalAlignOption = function(align) {
         switch (align) {
             case 0:
                 return 'start';
             case 1:
                 return 'center';
@@ -7738,16 +7757,16 @@
             case 3:
                 return 'around';
             default:
                 return 'between';
         }
     };
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$hAlignClass = function(_v0) {
-        var align = _v0.dO;
-        var screenSize = _v0.eW;
+        var align = _v0.dL;
+        var screenSize = _v0.e_;
         return $elm$html$Html$Attributes$class(
             'justify-content-' + (A2(
                 $elm$core$Maybe$withDefault,
                 '',
                 A2(
                     $elm$core$Maybe$map,
                     function(v) {
@@ -7772,160 +7791,450 @@
                     $elm$html$Html$Attributes$class('row')
                 ]),
             _Utils_ap(
                 A2(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$vAlignsToAttributes,
                     'align-items-',
                     _List_fromArray(
-                        [options.cP, options.cN, options.cM, options.cL, options.cO])),
+                        [options.cO, options.cM, options.cL, options.cK, options.cN])),
                 _Utils_ap(
                     $rundis$elm_bootstrap$Bootstrap$Grid$Internal$hAlignsToAttributes(
                         _List_fromArray(
-                            [options.bT, options.bR, options.bQ, options.bP, options.bS])),
-                    options.bu)));
+                            [options.bS, options.bQ, options.bP, options.bO, options.bR])),
+                    options.bt)));
     };
     var $rundis$elm_bootstrap$Bootstrap$Grid$row = F2(
         function(options, cols) {
             return A2(
                 $elm$html$Html$div,
                 $rundis$elm_bootstrap$Bootstrap$Grid$Internal$rowAttributes(options),
                 A2($elm$core$List$map, $rundis$elm_bootstrap$Bootstrap$Grid$renderCol, cols));
         });
+    var $elm$virtual_dom$VirtualDom$style = _VirtualDom_style;
+    var $elm$html$Html$Attributes$style = $elm$virtual_dom$VirtualDom$style;
+    var $elm$virtual_dom$VirtualDom$text = _VirtualDom_text;
+    var $elm$html$Html$text = $elm$virtual_dom$VirtualDom$text;
+    var $author$project$CurrentReads$getCurrentReads = function(currentReads) {
+        return A2(
+            $rundis$elm_bootstrap$Bootstrap$Grid$container,
+            _List_fromArray(
+                [
+                    A2($elm$html$Html$Attributes$style, 'padding', '1em')
+                ]),
+            _List_fromArray(
+                [
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_fromArray(
+                            [
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$Attributes$class('align-items-center')
+                                        ]))
+                            ]),
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center'),
+                                                        A2($elm$html$Html$Attributes$style, 'padding', '2em')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $elm$html$Html$h1,
+                                                _List_fromArray(
+                                                    [
+                                                        A2(
+                                                            $elm$html$Html$Attributes$style,
+                                                            'color',
+                                                            A2(
+                                                                $elm$core$Maybe$withDefault,
+                                                                'black',
+                                                                A2($elm$core$Maybe$map, $author$project$EpaCommon$getColorForLevel, currentReads.d0)))
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $elm$html$Html$text(
+                                                            A2(
+                                                                $elm$core$Maybe$withDefault,
+                                                                'NA',
+                                                                A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.en)))
+                                                    ]))
+                                        ]))
+                            ])),
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_fromArray(
+                            [
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$Attributes$class('align-items-center')
+                                        ]))
+                            ]),
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center'),
+                                                        A2($elm$html$Html$Attributes$style, 'padding-bottom', '2em')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $elm$html$Html$a,
+                                                _List_fromArray(
+                                                    [
+                                                        $elm$html$Html$Attributes$href('https://www.airnow.gov/aqi/aqi-basics/')
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $elm$html$Html$text('EPA AQI Score')
+                                                    ]))
+                                        ]))
+                            ])),
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_fromArray(
+                            [
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$Attributes$class('align-items-center')
+                                        ]))
+                            ]),
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'right')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text('Last PM10:')
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center'),
+                                                        A2($elm$html$Html$Attributes$style, 'font-weight', 'bold')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(
+                                                A2(
+                                                    $elm$core$Maybe$withDefault,
+                                                    'NA',
+                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.ep)))
+                                        ]))
+                            ])),
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_fromArray(
+                            [
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$Attributes$class('align-items-center')
+                                        ]))
+                            ]),
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'right')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text('Last PM25:')
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center'),
+                                                        A2($elm$html$Html$Attributes$style, 'font-weight', 'bold')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(
+                                                A2(
+                                                    $elm$core$Maybe$withDefault,
+                                                    'NA',
+                                                    A2($elm$core$Maybe$map, $elm$core$String$fromFloat, currentReads.eq)))
+                                        ]))
+                            ]))
+                ]));
+    };
+    var $author$project$DeviceStatus$deviceStatusColor = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return 'green';
+            case 1:
+                return 'orange';
+            case 2:
+                return 'gray';
+            default:
+                return 'red';
+        }
+    };
+    var $author$project$DeviceStatus$deviceStatusImage = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return '/static/images/loading.gif';
+            case 1:
+                return '/static/images/warmingup.gif';
+            case 2:
+                return '/static/images/idle.png';
+            default:
+                return '/static/images/failing.png';
+        }
+    };
+    var $author$project$DeviceStatus$deviceStatusToString = function(deviceStatus) {
+        switch (deviceStatus) {
+            case 0:
+                return 'Reading';
+            case 1:
+                return 'Warming Up';
+            case 2:
+                return 'Idle';
+            default:
+                return 'Failing';
+        }
+    };
+    var $elm$core$Basics$modBy = _Basics_modBy;
+    var $elm$core$String$cons = _String_cons;
+    var $elm$core$String$fromChar = function(_char) {
+        return A2($elm$core$String$cons, _char, '');
+    };
+    var $elm$core$Bitwise$and = _Bitwise_and;
+    var $elm$core$Bitwise$shiftRightBy = _Bitwise_shiftRightBy;
+    var $elm$core$String$repeatHelp = F3(
+        function(n, chunk, result) {
+            return (n <= 0) ? result : A3(
+                $elm$core$String$repeatHelp,
+                n >> 1,
+                _Utils_ap(chunk, chunk),
+                (!(n & 1)) ? result : _Utils_ap(result, chunk));
+        });
+    var $elm$core$String$repeat = F2(
+        function(n, chunk) {
+            return A3($elm$core$String$repeatHelp, n, chunk, '');
+        });
+    var $elm$core$String$padLeft = F3(
+        function(n, _char, string) {
+            return _Utils_ap(
+                A2(
+                    $elm$core$String$repeat,
+                    n - $elm$core$String$length(string),
+                    $elm$core$String$fromChar(_char)),
+                string);
+        });
+    var $author$project$DeviceStatus$formatDuration = F2(
+        function(currentTime, scheduledTime) {
+            var durationMillis = $elm$time$Time$posixToMillis(scheduledTime) - $elm$time$Time$posixToMillis(currentTime);
+            var hour = (((((durationMillis / 1000) | 0) / 60) | 0) / 60) | 0;
+            var minute = A2($elm$core$Basics$modBy, 60, (((durationMillis / 1000) | 0) / 60) | 0);
+            var second = A2($elm$core$Basics$modBy, 60, (durationMillis / 1000) | 0);
+            return (durationMillis > 0) ? (A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(hour)) + (':' + (A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(minute)) + (':' + A3(
+                $elm$core$String$padLeft,
+                2,
+                '0',
+                $elm$core$String$fromInt(second)))))) : '00:00:00';
+        });
+    var $elm$html$Html$h5 = _VirtualDom_node('h5');
+    var $author$project$DeviceStatus$htmlIf = F2(
+        function(el, cond) {
+            return cond ? el : $elm$html$Html$text('');
+        });
+    var $elm$html$Html$img = _VirtualDom_node('img');
     var $author$project$DeviceStatus$shouldShowTimer = function(deviceState) {
         return (deviceState === 2) || (deviceState === 3);
     };
     var $elm$html$Html$Attributes$src = function(url) {
         return A2(
             $elm$html$Html$Attributes$stringProperty,
             'src',
             _VirtualDom_noJavaScriptOrHtmlUri(url));
     };
-    var $elm$virtual_dom$VirtualDom$style = _VirtualDom_style;
-    var $elm$html$Html$Attributes$style = $elm$virtual_dom$VirtualDom$style;
     var $author$project$DeviceStatus$getDeviceInfo = function(deviceInfo) {
         return A2(
             $rundis$elm_bootstrap$Bootstrap$Grid$container,
             _List_Nil,
             _List_fromArray(
                 [
                     A2(
                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                         _List_fromArray(
                             [
-                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
-                                    _List_fromArray(
-                                        [
-                                            $elm$html$Html$Attributes$class('align-items-center')
-                                        ]))
+                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(_List_Nil)
                             ]),
                         _List_fromArray(
                             [
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                     _List_fromArray(
                                         [
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
                                                 _List_fromArray(
                                                     [
-                                                        A2($elm$html$Html$Attributes$style, 'max-width', '64px'),
-                                                        A2($elm$html$Html$Attributes$style, 'margin-right', '1em')
+                                                        $elm$html$Html$Attributes$class('text-center'),
+                                                        A2($elm$html$Html$Attributes$style, 'padding', '2em')
                                                     ]))
                                         ]),
                                     _List_fromArray(
                                         [
                                             A2(
                                                 $elm$html$Html$img,
                                                 _List_fromArray(
                                                     [
                                                         $elm$html$Html$Attributes$src(
-                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.a2))
+                                                            $author$project$DeviceStatus$deviceStatusImage(deviceInfo.a1))
                                                     ]),
                                                 _List_Nil)
-                                        ])),
+                                        ]))
+                            ])),
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_Nil,
+                        _List_fromArray(
+                            [
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                    _List_Nil,
                                     _List_fromArray(
                                         [
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                                _List_Nil,
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
                                                 _List_fromArray(
                                                     [
-                                                        A2(
-                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    A2(
-                                                                        $elm$html$Html$h5,
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                A2(
-                                                                                    $elm$html$Html$Attributes$style,
-                                                                                    'color',
-                                                                                    $author$project$DeviceStatus$deviceStatusColor(deviceInfo.a2))
-                                                                            ]),
-                                                                        _List_fromArray(
-                                                                            [
-                                                                                $elm$html$Html$text(
-                                                                                    $author$project$DeviceStatus$deviceStatusToString(deviceInfo.a2))
-                                                                            ]))
-                                                                ]))
-                                                    ])),
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
                                             A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                                _List_Nil,
+                                                $elm$html$Html$h5,
                                                 _List_fromArray(
                                                     [
                                                         A2(
-                                                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    $elm$html$Html$text(
-                                                                        A2($elm$core$Maybe$withDefault, '', deviceInfo.eo))
-                                                                ]))
-                                                    ])),
-                                            A2(
-                                                $author$project$DeviceStatus$htmlIf,
-                                                A2(
-                                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                                    _List_Nil,
+                                                            $elm$html$Html$Attributes$style,
+                                                            'color',
+                                                            $author$project$DeviceStatus$deviceStatusColor(deviceInfo.a1))
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $elm$html$Html$text(
+                                                            $author$project$DeviceStatus$deviceStatusToString(deviceInfo.a1))
+                                                    ]))
+                                        ]))
+                            ])),
+                    A2(
+                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                        _List_Nil,
+                        _List_fromArray(
+                            [
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'text-align', 'center')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            $elm$html$Html$text(
+                                                A2($elm$core$Maybe$withDefault, '', deviceInfo.eo))
+                                        ]))
+                            ])),
+                    A2(
+                        $author$project$DeviceStatus$htmlIf,
+                        A2(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                            _List_Nil,
+                            _List_fromArray(
+                                [
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                        _List_fromArray(
+                                            [
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
                                                     _List_fromArray(
                                                         [
-                                                            A2(
-                                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                                _List_Nil,
-                                                                _List_fromArray(
-                                                                    [
-                                                                        $elm$html$Html$text(
-                                                                            'Next read in: ' + A2(
-                                                                                $elm$core$Maybe$withDefault,
-                                                                                '',
-                                                                                A3($elm$core$Maybe$map2, $author$project$DeviceStatus$formatDuration, deviceInfo.dW, deviceInfo.ey)))
-                                                                    ]))
-                                                        ])),
-                                                $author$project$DeviceStatus$shouldShowTimer(deviceInfo.a2))
-                                        ]))
-                            ]))
+                                                            A2($elm$html$Html$Attributes$style, 'text-align', 'center')
+                                                        ]))
+                                            ]),
+                                        _List_fromArray(
+                                            [
+                                                $elm$html$Html$text(
+                                                    'Next read in: ' + A2(
+                                                        $elm$core$Maybe$withDefault,
+                                                        '',
+                                                        A3($elm$core$Maybe$map2, $author$project$DeviceStatus$formatDuration, deviceInfo.dU, deviceInfo.eA)))
+                                            ]))
+                                ])),
+                        $author$project$DeviceStatus$shouldShowTimer(deviceInfo.a1))
                 ]));
     };
     var $terezka$elm_charts$Internal$Svg$Start = 1;
     var $terezka$elm_charts$Chart$Attributes$alignLeft = function(config) {
         return _Utils_update(
             config, {
                 i: $elm$core$Maybe$Just(1)
             });
     };
     var $terezka$elm_charts$Chart$Attributes$background = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    fn: v
+                    fq: v
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$blue = '#12A5ED';
     var $terezka$elm_charts$Chart$Attributes$blue = $terezka$elm_charts$Internal$Helpers$blue;
     var $terezka$elm_charts$Chart$Attributes$border = F2(
         function(v, config) {
             return _Utils_update(
@@ -7939,16 +8248,16 @@
                 config, {
                     x: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Event = F2(
         function(name, handler) {
             return {
-                d9: handler,
-                fW: name
+                d8: handler,
+                fZ: name
             };
         });
     var $elm$core$List$any = F2(
         function(isOkay, list) {
             any: while (true) {
                 if (!list.b) {
                     return false;
@@ -7975,15 +8284,14 @@
                 });
             return A3($elm$core$List$foldl, apply_, _default, funcs);
         });
     var $elm$svg$Svg$trustedNode = _VirtualDom_nodeNS('http://www.w3.org/2000/svg');
     var $elm$svg$Svg$clipPath = $elm$svg$Svg$trustedNode('clipPath');
     var $debois$elm_dom$DOM$offsetHeight = A2($elm$json$Json$Decode$field, 'offsetHeight', $elm$json$Json$Decode$float);
     var $debois$elm_dom$DOM$offsetWidth = A2($elm$json$Json$Decode$field, 'offsetWidth', $elm$json$Json$Decode$float);
-    var $elm$json$Json$Decode$map4 = _Json_map4;
     var $debois$elm_dom$DOM$offsetLeft = A2($elm$json$Json$Decode$field, 'offsetLeft', $elm$json$Json$Decode$float);
     var $elm$json$Json$Decode$null = _Json_decodeNull;
     var $debois$elm_dom$DOM$offsetParent = F2(
         function(x, decoder) {
             return $elm$json$Json$Decode$oneOf(
                 _List_fromArray(
                     [
@@ -8023,18 +8331,18 @@
     var $debois$elm_dom$DOM$boundingClientRect = A4(
         $elm$json$Json$Decode$map3,
         F3(
             function(_v0, width, height) {
                 var x = _v0.a;
                 var y = _v0.b;
                 return {
-                    eb: height,
-                    ep: x,
-                    e7: y,
-                    ff: width
+                    ea: height,
+                    er: x,
+                    fb: y,
+                    fi: width
                 };
             }),
         A2($debois$elm_dom$DOM$position, 0, 0),
         $debois$elm_dom$DOM$offsetWidth,
         $debois$elm_dom$DOM$offsetHeight);
     var $elm$json$Json$Decode$lazy = function(thunk) {
         return A2(
@@ -8059,93 +8367,92 @@
                 ]));
     }
     var $terezka$elm_charts$Internal$Svg$decodePosition = $terezka$elm_charts$Internal$Svg$cyclic$decodePosition();
     $terezka$elm_charts$Internal$Svg$cyclic$decodePosition = function() {
         return $terezka$elm_charts$Internal$Svg$decodePosition;
     };
     var $terezka$elm_charts$Internal$Coordinates$innerLength = function(axis) {
-        return A2($elm$core$Basics$max, 1, (axis.N - axis.fT) - axis.fS);
+        return A2($elm$core$Basics$max, 1, (axis.O - axis.fW) - axis.fV);
     };
     var $terezka$elm_charts$Internal$Coordinates$innerWidth = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fg);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fj);
     };
     var $terezka$elm_charts$Internal$Coordinates$range = function(axis) {
-        var diff = axis.er - axis.et;
+        var diff = axis.et - axis.ev;
         return (diff > 0) ? diff : 1;
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fg)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fj)) / $terezka$elm_charts$Internal$Coordinates$innerWidth(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.fg.fT) + plane.fg.et;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, value - plane.fj.fW) + plane.fj.ev;
         });
     var $terezka$elm_charts$Internal$Coordinates$innerHeight = function(plane) {
-        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fh);
+        return $terezka$elm_charts$Internal$Coordinates$innerLength(plane.fk);
     };
     var $terezka$elm_charts$Internal$Coordinates$scaleCartesianY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fh)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
+            return (value * $terezka$elm_charts$Internal$Coordinates$range(plane.fk)) / $terezka$elm_charts$Internal$Coordinates$innerHeight(plane);
         });
     var $terezka$elm_charts$Internal$Coordinates$toCartesianY = F2(
         function(plane, value) {
-            return ($terezka$elm_charts$Internal$Coordinates$range(plane.fh) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.fh.fT)) + plane.fh.et;
+            return ($terezka$elm_charts$Internal$Coordinates$range(plane.fk) - A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, value - plane.fk.fW)) + plane.fk.ev;
         });
     var $terezka$elm_charts$Internal$Svg$fromSvg = F2(
         function(plane, point) {
             return {
-                fg: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.fg),
-                fh: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.fh)
+                fj: A2($terezka$elm_charts$Internal$Coordinates$toCartesianX, plane, point.fj),
+                fk: A2($terezka$elm_charts$Internal$Coordinates$toCartesianY, plane, point.fk)
             };
         });
     var $debois$elm_dom$DOM$target = function(decoder) {
         return A2($elm$json$Json$Decode$field, 'target', decoder);
     };
     var $terezka$elm_charts$Internal$Svg$decoder = F2(
         function(plane, toMsg) {
             var handle = F3(
                 function(mouseX, mouseY, box) {
-                    var yPrev = plane.fh;
-                    var xPrev = plane.fg;
-                    var widthPercent = box.ff / plane.fg.N;
-                    var heightPercent = box.eb / plane.fh.N;
+                    var yPrev = plane.fk;
+                    var xPrev = plane.fj;
+                    var widthPercent = box.fi / plane.fj.O;
+                    var heightPercent = box.ea / plane.fk.O;
                     var newPlane = _Utils_update(
                         plane, {
-                            fg: _Utils_update(
+                            fj: _Utils_update(
                                 xPrev, {
-                                    N: box.ff,
-                                    fS: plane.fg.fS * widthPercent,
-                                    fT: plane.fg.fT * widthPercent
+                                    O: box.fi,
+                                    fV: plane.fj.fV * widthPercent,
+                                    fW: plane.fj.fW * widthPercent
                                 }),
-                            fh: _Utils_update(
+                            fk: _Utils_update(
                                 yPrev, {
-                                    N: box.eb,
-                                    fS: plane.fh.fS * heightPercent,
-                                    fT: plane.fh.fT * heightPercent
+                                    O: box.ea,
+                                    fV: plane.fk.fV * heightPercent,
+                                    fW: plane.fk.fW * heightPercent
                                 })
                         });
                     var searched = A2(
                         $terezka$elm_charts$Internal$Svg$fromSvg,
                         newPlane, {
-                            fg: mouseX - box.ep,
-                            fh: mouseY - box.e7
+                            fj: mouseX - box.er,
+                            fk: mouseY - box.fb
                         });
                     return A2(toMsg, newPlane, searched);
                 });
             return A4(
                 $elm$json$Json$Decode$map3,
                 handle,
                 A2($elm$json$Json$Decode$field, 'pageX', $elm$json$Json$Decode$float),
                 A2($elm$json$Json$Decode$field, 'pageY', $elm$json$Json$Decode$float),
                 $debois$elm_dom$DOM$target($terezka$elm_charts$Internal$Svg$decodePosition));
         });
     var $elm$svg$Svg$defs = $elm$svg$Svg$trustedNode('defs');
     var $elm$svg$Svg$Attributes$fill = _VirtualDom_attribute('fill');
-    var $elm$core$String$fromFloat = _String_fromNumber;
     var $elm$svg$Svg$Attributes$height = _VirtualDom_attribute('height');
     var $elm$svg$Svg$Attributes$id = _VirtualDom_attribute('id');
     var $elm$virtual_dom$VirtualDom$Normal = function(a) {
         return {
             $: 0,
             a: a
         };
@@ -8175,79 +8482,79 @@
             A2($elm$core$String$replace, '.', '-'));
         return A2(
             $elm$core$String$join,
             '_',
             _List_fromArray(
                 [
                     'elm-charts__id',
-                    numToStr(plane.fg.N),
-                    numToStr(plane.fg.et),
-                    numToStr(plane.fg.er),
-                    numToStr(plane.fg.fT),
-                    numToStr(plane.fg.fS),
-                    numToStr(plane.fh.N),
-                    numToStr(plane.fh.et),
-                    numToStr(plane.fh.er),
-                    numToStr(plane.fh.fT),
-                    numToStr(plane.fh.fS)
+                    numToStr(plane.fj.O),
+                    numToStr(plane.fj.ev),
+                    numToStr(plane.fj.et),
+                    numToStr(plane.fj.fW),
+                    numToStr(plane.fj.fV),
+                    numToStr(plane.fk.O),
+                    numToStr(plane.fk.ev),
+                    numToStr(plane.fk.et),
+                    numToStr(plane.fk.fW),
+                    numToStr(plane.fk.fV)
                 ]));
     };
     var $elm$svg$Svg$Attributes$viewBox = _VirtualDom_attribute('viewBox');
     var $elm$svg$Svg$Attributes$width = _VirtualDom_attribute('width');
     var $elm$svg$Svg$Attributes$x = _VirtualDom_attribute('x');
     var $elm$svg$Svg$Attributes$y = _VirtualDom_attribute('y');
     var $terezka$elm_charts$Internal$Svg$container = F5(
         function(plane, config, below, chartEls, above) {
             var toEvent = function(event) {
                 return A2(
                     $elm$svg$Svg$Events$on,
-                    event.fW,
-                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.d9));
+                    event.fZ,
+                    A2($terezka$elm_charts$Internal$Svg$decoder, plane, event.d8));
             };
-            var svgAttrsSize = config.cx ? _List_fromArray(
+            var svgAttrsSize = config.cw ? _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$viewBox(
-                        '0 0 ' + ($elm$core$String$fromFloat(plane.fg.N) + (' ' + $elm$core$String$fromFloat(plane.fh.N)))),
+                        '0 0 ' + ($elm$core$String$fromFloat(plane.fj.O) + (' ' + $elm$core$String$fromFloat(plane.fk.O)))),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]) : _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$width(
-                        $elm$core$String$fromFloat(plane.fg.N)),
+                        $elm$core$String$fromFloat(plane.fj.O)),
                     $elm$svg$Svg$Attributes$height(
-                        $elm$core$String$fromFloat(plane.fh.N)),
+                        $elm$core$String$fromFloat(plane.fk.O)),
                     A2($elm$html$Html$Attributes$style, 'display', 'block')
                 ]);
-            var htmlAttrsSize = config.cx ? _List_fromArray(
+            var htmlAttrsSize = config.cw ? _List_fromArray(
                 [
                     A2($elm$html$Html$Attributes$style, 'width', '100%'),
                     A2($elm$html$Html$Attributes$style, 'height', '100%')
                 ]) : _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'width',
-                        $elm$core$String$fromFloat(plane.fg.N) + 'px'),
+                        $elm$core$String$fromFloat(plane.fj.O) + 'px'),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'height',
-                        $elm$core$String$fromFloat(plane.fh.N) + 'px')
+                        $elm$core$String$fromFloat(plane.fk.O) + 'px')
                 ]);
             var htmlAttrsDef = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__container-inner')
                 ]);
             var htmlAttrs = _Utils_ap(
-                config.bY,
+                config.bX,
                 _Utils_ap(htmlAttrsDef, htmlAttrsSize));
             var chartPosition = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$x(
-                        $elm$core$String$fromFloat(plane.fg.fT)),
+                        $elm$core$String$fromFloat(plane.fj.fW)),
                     $elm$svg$Svg$Attributes$y(
-                        $elm$core$String$fromFloat(plane.fh.fT)),
+                        $elm$core$String$fromFloat(plane.fk.fW)),
                     $elm$svg$Svg$Attributes$width(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerWidth(plane))),
                     $elm$svg$Svg$Attributes$height(
                         $elm$core$String$fromFloat(
                             $terezka$elm_charts$Internal$Coordinates$innerHeight(plane))),
                     $elm$svg$Svg$Attributes$fill('transparent')
@@ -8269,19 +8576,19 @@
                                     A2($elm$svg$Svg$rect, chartPosition, _List_Nil)
                                 ]))
                     ]));
             var catcher = A2(
                 $elm$svg$Svg$rect,
                 _Utils_ap(
                     chartPosition,
-                    A2($elm$core$List$map, toEvent, config.bM)),
+                    A2($elm$core$List$map, toEvent, config.bL)),
                 _List_Nil);
             var chart = A2(
                 $elm$svg$Svg$svg,
-                _Utils_ap(svgAttrsSize, config.bv),
+                _Utils_ap(svgAttrsSize, config.bu),
                 _Utils_ap(
                     _List_fromArray(
                         [clipPathDefs]),
                     _Utils_ap(
                         chartEls,
                         _List_fromArray(
                             [catcher]))));
@@ -8305,17 +8612,17 @@
                                     above)))
                     ]));
         });
     var $terezka$elm_charts$Internal$Coordinates$Position = F4(
         function(x1, x2, y1, y2) {
             return {
                 aK: x1,
-                bf: x2,
-                gx: y1,
-                dL: y2
+                be: x2,
+                gA: y1,
+                dI: y2
             };
         });
     var $elm$core$Basics$min = F2(
         function(x, y) {
             return (_Utils_cmp(x, y) < 0) ? x : y;
         });
     var $terezka$elm_charts$Internal$Coordinates$foldPosition = F2(
@@ -8325,26 +8632,26 @@
                     if (!posM.$) {
                         var pos = posM.a;
                         return $elm$core$Maybe$Just({
                             aK: A2(
                                 $elm$core$Basics$min,
                                 func(datum).aK,
                                 pos.aK),
-                            bf: A2(
+                            be: A2(
                                 $elm$core$Basics$max,
-                                func(datum).bf,
-                                pos.bf),
-                            gx: A2(
+                                func(datum).be,
+                                pos.be),
+                            gA: A2(
                                 $elm$core$Basics$min,
-                                func(datum).gx,
-                                pos.gx),
-                            dL: A2(
+                                func(datum).gA,
+                                pos.gA),
+                            dI: A2(
                                 $elm$core$Basics$max,
-                                func(datum).dL,
-                                pos.dL)
+                                func(datum).dI,
+                                pos.dI)
                         });
                     } else {
                         return $elm$core$Maybe$Just(
                             func(datum));
                     }
                 });
             return A2(
@@ -8352,41 +8659,41 @@
                 A4($terezka$elm_charts$Internal$Coordinates$Position, 0, 0, 0, 0),
                 A3($elm$core$List$foldl, fold, $elm$core$Maybe$Nothing, data));
         });
     var $terezka$elm_charts$Chart$Attributes$lowest = F3(
         function(v, edit, b) {
             return _Utils_update(
                 b, {
-                    et: A3(edit, v, b.et, b.fw)
+                    ev: A3(edit, v, b.ev, b.fz)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$orLower = F3(
         function(least, real, _v0) {
             return (_Utils_cmp(real, least) > 0) ? least : real;
         });
     var $terezka$elm_charts$Chart$definePlane = F2(
         function(config, elements) {
-            var width = A2($elm$core$Basics$max, 1, (config.ff - config.R.ep) - config.R.a1);
+            var width = A2($elm$core$Basics$max, 1, (config.fi - config.S.er) - config.S.eW);
             var toLimit = F5(
                 function(length, marginMin, marginMax, min, max) {
                     return {
-                        fv: max,
-                        fw: min,
-                        N: length,
-                        fS: marginMax,
-                        fT: marginMin,
-                        er: max,
-                        et: min
+                        fy: max,
+                        fz: min,
+                        O: length,
+                        fV: marginMax,
+                        fW: marginMin,
+                        et: max,
+                        ev: min
                     };
                 });
-            var height = A2($elm$core$Basics$max, 1, (config.eb - config.R.aM) - config.R.e7);
+            var height = A2($elm$core$Basics$max, 1, (config.ea - config.S.dO) - config.S.fb);
             var fixSingles = function(bs) {
-                return _Utils_eq(bs.et, bs.er) ? _Utils_update(
+                return _Utils_eq(bs.ev, bs.et) ? _Utils_update(
                     bs, {
-                        er: bs.et + 10
+                        et: bs.ev + 10
                     }) : bs;
             };
             var collectLimits = F2(
                 function(el, acc) {
                     switch (el.$) {
                         case 0:
                             return acc;
@@ -8419,83 +8726,83 @@
                             return acc;
                         default:
                             return acc;
                     }
                 });
             var limits_ = function(pos) {
                 return function(_v3) {
-                    var x = _v3.fg;
-                    var y = _v3.fh;
+                    var x = _v3.fj;
+                    var y = _v3.fk;
                     return {
-                        fg: fixSingles(x),
-                        fh: fixSingles(y)
+                        fj: fixSingles(x),
+                        fk: fixSingles(y)
                     };
                 }({
-                    fg: A5(toLimit, width, config.ao.ep, config.ao.a1, pos.aK, pos.bf),
-                    fh: A5(toLimit, height, config.ao.e7, config.ao.aM, pos.gx, pos.dL)
+                    fj: A5(toLimit, width, config.ap.er, config.ap.eW, pos.aK, pos.be),
+                    fk: A5(toLimit, height, config.ap.fb, config.ap.dO, pos.gA, pos.dI)
                 });
             }(
                 A2(
                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                     $elm$core$Basics$identity,
                     A3($elm$core$List$foldl, collectLimits, _List_Nil, elements)));
             var calcRange = function() {
-                var _v2 = config.dp;
+                var _v2 = config.dn;
                 if (!_v2.b) {
-                    return limits_.fg;
+                    return limits_.fj;
                 } else {
                     var some = _v2;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.fg,
+                        limits_.fj,
                         some);
                 }
             }();
             var calcDomain = function() {
-                var _v1 = config.cZ;
+                var _v1 = config.cY;
                 if (!_v1.b) {
-                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.fh);
+                    return A3($terezka$elm_charts$Chart$Attributes$lowest, 0, $terezka$elm_charts$Chart$Attributes$orLower, limits_.fk);
                 } else {
                     var some = _v1;
                     return A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, b) {
                                 return f(b);
                             }),
-                        limits_.fh,
+                        limits_.fk,
                         some);
                 }
             }();
             var unpadded = {
-                fg: calcRange,
-                fh: calcDomain
+                fj: calcRange,
+                fk: calcDomain
             };
             var scalePadX = $terezka$elm_charts$Internal$Coordinates$scaleCartesianX(unpadded);
-            var xMax = calcRange.er + scalePadX(config.R.a1);
-            var xMin = calcRange.et - scalePadX(config.R.ep);
+            var xMax = calcRange.et + scalePadX(config.S.eW);
+            var xMin = calcRange.ev - scalePadX(config.S.er);
             var scalePadY = $terezka$elm_charts$Internal$Coordinates$scaleCartesianY(unpadded);
-            var yMax = calcDomain.er + scalePadY(config.R.e7);
-            var yMin = calcDomain.et - scalePadY(config.R.aM);
+            var yMax = calcDomain.et + scalePadY(config.S.fb);
+            var yMin = calcDomain.ev - scalePadY(config.S.dO);
             return {
-                fg: _Utils_update(
+                fj: _Utils_update(
                     calcRange, {
-                        N: config.ff,
-                        er: A2($elm$core$Basics$max, xMin, xMax),
-                        et: A2($elm$core$Basics$min, xMin, xMax)
+                        O: config.fi,
+                        et: A2($elm$core$Basics$max, xMin, xMax),
+                        ev: A2($elm$core$Basics$min, xMin, xMax)
                     }),
-                fh: _Utils_update(
+                fk: _Utils_update(
                     calcDomain, {
-                        N: config.eb,
-                        er: A2($elm$core$Basics$max, yMin, yMax),
-                        et: A2($elm$core$Basics$min, yMin, yMax)
+                        O: config.ea,
+                        et: A2($elm$core$Basics$max, yMin, yMax),
+                        ev: A2($elm$core$Basics$min, yMin, yMax)
                     })
             };
         });
     var $terezka$elm_charts$Chart$getItems = F2(
         function(plane, elements) {
             var toItems = F2(
                 function(el, acc) {
@@ -8578,18 +8885,18 @@
                 }
             });
         return A3($elm$core$List$foldl, toLegends, _List_Nil, elements);
     };
     var $terezka$elm_charts$Chart$TickValues = F4(
         function(xAxis, yAxis, xs, ys) {
             return {
-                bg: xAxis,
+                bf: xAxis,
                 A: xs,
-                bh: yAxis,
-                I: ys
+                bg: yAxis,
+                J: ys
             };
         });
     var $terezka$elm_charts$Chart$getTickValues = F3(
         function(plane, items, elements) {
             var toValues = F2(
                 function(el, acc) {
                     switch (el.$) {
@@ -8671,15 +8978,15 @@
             });
     };
     var $elm$svg$Svg$Attributes$class = _VirtualDom_attribute('class');
     var $terezka$elm_charts$Chart$Attributes$color = F2(
         function(v, config) {
             return (v === '') ? config : _Utils_update(
                 config, {
-                    bD: v
+                    bC: v
                 });
         });
     var $elm$core$List$append = F2(
         function(xs, ys) {
             if (!ys.b) {
                 return xs;
             } else {
@@ -8695,46 +9002,46 @@
                 A2($elm$core$List$map, f, list));
         });
     var $terezka$elm_charts$Internal$Helpers$darkGray = 'rgb(200 200 200)';
     var $terezka$elm_charts$Chart$Attributes$dashed = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    bG: value
+                    bF: value
                 });
         });
     var $terezka$elm_charts$Internal$Helpers$pink = '#ea60df';
     var $terezka$elm_charts$Internal$Svg$defaultDot = {
         v: '',
         x: 0,
-        bD: $terezka$elm_charts$Internal$Helpers$pink,
+        bC: $terezka$elm_charts$Internal$Helpers$pink,
         l: false,
-        fH: 0,
-        fI: '',
-        fJ: 5,
-        P: 1,
+        fK: 0,
+        fL: '',
+        fM: 5,
+        Q: 1,
         aG: $elm$core$Maybe$Nothing,
-        eZ: 6
+        e1: 6
     };
     var $elm$svg$Svg$circle = $elm$svg$Svg$trustedNode('circle');
     var $elm$svg$Svg$Attributes$cx = _VirtualDom_attribute('cx');
     var $elm$svg$Svg$Attributes$cy = _VirtualDom_attribute('cy');
     var $elm$svg$Svg$Attributes$d = _VirtualDom_attribute('d');
     var $elm$svg$Svg$Attributes$fillOpacity = _VirtualDom_attribute('fill-opacity');
     var $elm$svg$Svg$g = $elm$svg$Svg$trustedNode('g');
     var $elm$core$Basics$clamp = F3(
         function(low, high, number) {
             return (_Utils_cmp(number, low) < 0) ? low : ((_Utils_cmp(number, high) > 0) ? high : number);
         });
     var $terezka$elm_charts$Internal$Svg$isWithinPlane = F3(
         function(plane, x, y) {
             return _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.fg.et, plane.fg.er, x),
+                A3($elm$core$Basics$clamp, plane.fj.ev, plane.fj.et, x),
                 x) && _Utils_eq(
-                A3($elm$core$Basics$clamp, plane.fh.et, plane.fh.er, y),
+                A3($elm$core$Basics$clamp, plane.fk.ev, plane.fk.et, y),
                 y);
         });
     var $elm$core$Basics$not = _Basics_not;
     var $elm$svg$Svg$path = $elm$svg$Svg$trustedNode('path');
     var $elm$core$Basics$pi = _Basics_pi;
     var $elm$core$Basics$sqrt = _Basics_sqrt;
     var $terezka$elm_charts$Internal$Svg$plusPath = F4(
@@ -8766,27 +9073,27 @@
     var $elm$svg$Svg$Attributes$r = _VirtualDom_attribute('r');
     var $elm$svg$Svg$Attributes$stroke = _VirtualDom_attribute('stroke');
     var $elm$svg$Svg$Attributes$strokeOpacity = _VirtualDom_attribute('stroke-opacity');
     var $elm$svg$Svg$Attributes$strokeWidth = _VirtualDom_attribute('stroke-width');
     var $elm$svg$Svg$text = $elm$virtual_dom$VirtualDom$text;
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGX = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fg);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerWidth(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fj);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGX = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.fg.et) + plane.fg.fT;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, value - plane.fj.ev) + plane.fj.fW;
         });
     var $terezka$elm_charts$Internal$Coordinates$scaleSVGY = F2(
         function(plane, value) {
-            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fh);
+            return (value * $terezka$elm_charts$Internal$Coordinates$innerHeight(plane)) / $terezka$elm_charts$Internal$Coordinates$range(plane.fk);
         });
     var $terezka$elm_charts$Internal$Coordinates$toSVGY = F2(
         function(plane, value) {
-            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.fh.er - value) + plane.fh.fT;
+            return A2($terezka$elm_charts$Internal$Coordinates$scaleSVGY, plane, plane.fk.et - value) + plane.fk.fW;
         });
     var $elm$svg$Svg$Attributes$transform = _VirtualDom_attribute('transform');
     var $elm$core$Basics$degrees = function(angleInDegrees) {
         return (angleInDegrees * $elm$core$Basics$pi) / 180;
     };
     var $elm$core$Basics$tan = _Basics_tan;
     var $terezka$elm_charts$Internal$Svg$trianglePath = F4(
@@ -8817,38 +9124,38 @@
             var yOrg = toY(datum_);
             var y_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, yOrg);
             var xOrg = toX(datum_);
             var x_ = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, xOrg);
             var styleAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(
-                        (config.v === '') ? config.bD : config.v),
+                        (config.v === '') ? config.bC : config.v),
                     $elm$svg$Svg$Attributes$strokeWidth(
                         $elm$core$String$fromFloat(config.x)),
                     $elm$svg$Svg$Attributes$fillOpacity(
-                        $elm$core$String$fromFloat(config.P)),
-                    $elm$svg$Svg$Attributes$fill(config.bD),
+                        $elm$core$String$fromFloat(config.Q)),
+                    $elm$svg$Svg$Attributes$fill(config.bC),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot'),
                     config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                 ]);
             var showDot = A3($terezka$elm_charts$Internal$Svg$isWithinPlane, plane, xOrg, yOrg) || config.l;
-            var highlightColor = (config.fI === '') ? config.bD : config.fI;
+            var highlightColor = (config.fL === '') ? config.bC : config.fL;
             var highlightAttrs = _List_fromArray(
                 [
                     $elm$svg$Svg$Attributes$stroke(highlightColor),
                     $elm$svg$Svg$Attributes$strokeWidth(
-                        $elm$core$String$fromFloat(config.fJ)),
+                        $elm$core$String$fromFloat(config.fM)),
                     $elm$svg$Svg$Attributes$strokeOpacity(
-                        $elm$core$String$fromFloat(config.fH)),
+                        $elm$core$String$fromFloat(config.fK)),
                     $elm$svg$Svg$Attributes$fill('transparent'),
                     $elm$svg$Svg$Attributes$class('elm-charts__dot-highlight')
                 ]);
             var view = F3(
                 function(toEl, highlightOff, toAttrs) {
-                    return (config.fH > 0) ? A2(
+                    return (config.fK > 0) ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__dot-container')
                             ]),
                         _List_fromArray(
                             [
@@ -8867,29 +9174,29 @@
                             ])) : A2(
                         toEl,
                         _Utils_ap(
                             toAttrs(0),
                             styleAttrs),
                         _List_Nil);
                 });
-            var area_ = (2 * $elm$core$Basics$pi) * config.eZ;
+            var area_ = (2 * $elm$core$Basics$pi) * config.e1;
             if (!showDot) {
                 return $elm$svg$Svg$text('');
             } else {
                 var _v0 = config.aG;
                 if (_v0.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     switch (_v0.a) {
                         case 0:
                             var _v1 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$circle,
-                                config.fJ / 2,
+                                config.fM / 2,
                                 function(off) {
                                     var radius = $elm$core$Basics$sqrt(area_ / $elm$core$Basics$pi);
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$cx(
                                                 $elm$core$String$fromFloat(x_)),
                                             $elm$svg$Svg$Attributes$cy(
@@ -8899,28 +9206,28 @@
                                         ]);
                                 });
                         case 1:
                             var _v2 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fJ,
+                                config.fM,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$trianglePath, area_, off, x_, y_))
                                         ]);
                                 });
                         case 2:
                             var _v3 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fJ,
+                                config.fM,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -8933,15 +9240,15 @@
                                         ]);
                                 });
                         case 3:
                             var _v4 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$rect,
-                                config.fJ,
+                                config.fM,
                                 function(off) {
                                     var side = $elm$core$Basics$sqrt(area_);
                                     var sideOff = side + off;
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x(
                                                 $elm$core$String$fromFloat(x_ - (sideOff / 2))),
@@ -8956,30 +9263,30 @@
                                         ]);
                                 });
                         case 4:
                             var _v5 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fJ,
+                                config.fM,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_)),
                                             $elm$svg$Svg$Attributes$transform(
                                                 'rotate(45 ' + ($elm$core$String$fromFloat(x_) + (' ' + ($elm$core$String$fromFloat(y_) + ')'))))
                                         ]);
                                 });
                         default:
                             var _v6 = _v0.a;
                             return A3(
                                 view,
                                 $elm$svg$Svg$path,
-                                config.fJ,
+                                config.fM,
                                 function(off) {
                                     return _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$d(
                                                 A4($terezka$elm_charts$Internal$Svg$plusPath, area_, off, x_, y_))
                                         ]);
                                 });
@@ -8994,31 +9301,31 @@
                 plane,
                 toX,
                 toY,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Internal$Helpers$gray = '#EFF2FA';
     var $terezka$elm_charts$Internal$Svg$defaultLine = {
-        bv: _List_Nil,
-        fq: false,
-        bD: 'rgb(210, 210, 210)',
-        bG: _List_Nil,
+        bu: _List_Nil,
+        ft: false,
+        bC: 'rgb(210, 210, 210)',
+        bF: _List_Nil,
         e: false,
         l: false,
-        P: 1,
-        gb: -90,
-        gc: 0,
-        ff: 1,
+        Q: 1,
+        ge: -90,
+        gf: 0,
+        fi: 1,
         aK: $elm$core$Maybe$Nothing,
-        bf: $elm$core$Maybe$Nothing,
-        gw: $elm$core$Maybe$Nothing,
+        be: $elm$core$Maybe$Nothing,
+        gz: $elm$core$Maybe$Nothing,
         g: 0,
-        gx: $elm$core$Maybe$Nothing,
-        dL: $elm$core$Maybe$Nothing,
-        gy: $elm$core$Maybe$Nothing,
+        gA: $elm$core$Maybe$Nothing,
+        dI: $elm$core$Maybe$Nothing,
+        gB: $elm$core$Maybe$Nothing,
         h: 0
     };
     var $terezka$elm_charts$Internal$Commands$Line = F2(
         function(a, b) {
             return {
                 $: 1,
                 a: a,
@@ -9290,33 +9597,33 @@
                     A2(
                         $elm$core$List$map,
                         $elm$html$Html$Attributes$map($elm$core$Basics$never),
                         attrs)));
         });
     var $terezka$elm_charts$Internal$Svg$line = F2(
         function(plane, config) {
-            var angle = $elm$core$Basics$degrees(config.gb);
+            var angle = $elm$core$Basics$degrees(config.ge);
             var _v0 = function() {
                 var _v3 = _Utils_Tuple3(
-                    _Utils_Tuple2(config.aK, config.bf),
-                    _Utils_Tuple2(config.gx, config.dL),
-                    _Utils_Tuple2(config.gw, config.gy));
+                    _Utils_Tuple2(config.aK, config.be),
+                    _Utils_Tuple2(config.gA, config.dI),
+                    _Utils_Tuple2(config.gz, config.gB));
                 if (!_v3.a.a.$) {
                     if (!_v3.a.b.$) {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v4 = _v3.a;
                                 var a = _v4.a.a;
                                 var b = _v4.b.a;
                                 var _v5 = _v3.b;
                                 var _v6 = _v5.a;
                                 var _v7 = _v5.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
-                                    _Utils_Tuple2(plane.fh.et, plane.fh.et));
+                                    _Utils_Tuple2(plane.fk.ev, plane.fk.ev));
                             } else {
                                 var _v38 = _v3.a;
                                 var a = _v38.a.a;
                                 var b = _v38.b.a;
                                 var _v39 = _v3.b;
                                 var _v40 = _v39.a;
                                 var c = _v39.b.a;
@@ -9334,33 +9641,33 @@
                                 var _v43 = _v42.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, b),
                                     _Utils_Tuple2(c, c));
                             } else {
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.fg.et, config.aK),
-                                        A2($elm$core$Maybe$withDefault, plane.fg.er, config.bf)),
+                                        A2($elm$core$Maybe$withDefault, plane.fj.ev, config.aK),
+                                        A2($elm$core$Maybe$withDefault, plane.fj.et, config.be)),
                                     _Utils_Tuple2(
-                                        A2($elm$core$Maybe$withDefault, plane.fh.et, config.gx),
-                                        A2($elm$core$Maybe$withDefault, plane.fh.er, config.dL)));
+                                        A2($elm$core$Maybe$withDefault, plane.fk.ev, config.gA),
+                                        A2($elm$core$Maybe$withDefault, plane.fk.et, config.dI)));
                             }
                         }
                     } else {
                         if (_v3.b.a.$ === 1) {
                             if (_v3.b.b.$ === 1) {
                                 var _v8 = _v3.a;
                                 var a = _v8.a.a;
                                 var _v9 = _v8.b;
                                 var _v10 = _v3.b;
                                 var _v11 = _v10.a;
                                 var _v12 = _v10.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(a, a),
-                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
+                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v51 = _v3.a;
                                         var a = _v51.a.a;
                                         var _v52 = _v51.b;
                                         var _v53 = _v3.b;
@@ -9400,15 +9707,15 @@
                                         var _v46 = _v3.b;
                                         var _v47 = _v46.a;
                                         var b = _v46.b.a;
                                         var _v48 = _v3.c;
                                         var _v49 = _v48.a;
                                         var _v50 = _v48.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fg.er),
+                                            _Utils_Tuple2(a, plane.fj.et),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v62 = _v3.a;
                                         var a = _v62.a.a;
                                         var _v63 = _v62.b;
                                         var _v64 = _v3.b;
                                         var _v65 = _v64.a;
@@ -9478,15 +9785,15 @@
                                         var _v70 = _v3.b;
                                         var b = _v70.a.a;
                                         var _v71 = _v70.b;
                                         var _v72 = _v3.c;
                                         var _v73 = _v72.a;
                                         var _v74 = _v72.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fg.er),
+                                            _Utils_Tuple2(a, plane.fj.et),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v86 = _v3.a;
                                         var a = _v86.a.a;
                                         var _v87 = _v86.b;
                                         var _v88 = _v3.b;
                                         var b = _v88.a.a;
@@ -9512,15 +9819,15 @@
                                 var _v14 = _v13.a;
                                 var b = _v13.b.a;
                                 var _v15 = _v3.b;
                                 var _v16 = _v15.a;
                                 var _v17 = _v15.b;
                                 return _Utils_Tuple2(
                                     _Utils_Tuple2(b, b),
-                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
+                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
                             } else {
                                 if (!_v3.c.a.$) {
                                     if (!_v3.c.b.$) {
                                         var _v99 = _v3.a;
                                         var _v100 = _v99.a;
                                         var a = _v99.b.a;
                                         var _v101 = _v3.b;
@@ -9560,15 +9867,15 @@
                                         var _v94 = _v3.b;
                                         var _v95 = _v94.a;
                                         var b = _v94.b.a;
                                         var _v96 = _v3.c;
                                         var _v97 = _v96.a;
                                         var _v98 = _v96.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fg.er),
+                                            _Utils_Tuple2(a, plane.fj.et),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v110 = _v3.a;
                                         var _v111 = _v110.a;
                                         var a = _v110.b.a;
                                         var _v112 = _v3.b;
                                         var _v113 = _v112.a;
@@ -9638,15 +9945,15 @@
                                         var _v118 = _v3.b;
                                         var b = _v118.a.a;
                                         var _v119 = _v118.b;
                                         var _v120 = _v3.c;
                                         var _v121 = _v120.a;
                                         var _v122 = _v120.b;
                                         return _Utils_Tuple2(
-                                            _Utils_Tuple2(a, plane.fg.er),
+                                            _Utils_Tuple2(a, plane.fj.et),
                                             _Utils_Tuple2(b, b));
                                     } else {
                                         var _v134 = _v3.a;
                                         var _v135 = _v134.a;
                                         var a = _v134.b.a;
                                         var _v136 = _v3.b;
                                         var b = _v136.a.a;
@@ -9669,48 +9976,48 @@
                                 var _v18 = _v3.a;
                                 var _v19 = _v18.a;
                                 var _v20 = _v18.b;
                                 var _v21 = _v3.b;
                                 var a = _v21.a.a;
                                 var b = _v21.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fg.et, plane.fg.et),
+                                    _Utils_Tuple2(plane.fj.ev, plane.fj.ev),
                                     _Utils_Tuple2(a, b));
                             } else {
                                 var _v22 = _v3.a;
                                 var _v23 = _v22.a;
                                 var _v24 = _v22.b;
                                 var _v25 = _v3.b;
                                 var a = _v25.a.a;
                                 var _v26 = _v25.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
+                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
                                     _Utils_Tuple2(a, a));
                             }
                         } else {
                             if (!_v3.b.b.$) {
                                 var _v27 = _v3.a;
                                 var _v28 = _v27.a;
                                 var _v29 = _v27.b;
                                 var _v30 = _v3.b;
                                 var _v31 = _v30.a;
                                 var b = _v30.b.a;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
+                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
                                     _Utils_Tuple2(b, b));
                             } else {
                                 var _v140 = _v3.a;
                                 var _v141 = _v140.a;
                                 var _v142 = _v140.b;
                                 var _v143 = _v3.b;
                                 var _v144 = _v143.a;
                                 var _v145 = _v143.b;
                                 return _Utils_Tuple2(
-                                    _Utils_Tuple2(plane.fg.et, plane.fg.er),
-                                    _Utils_Tuple2(plane.fh.et, plane.fh.er));
+                                    _Utils_Tuple2(plane.fj.ev, plane.fj.et),
+                                    _Utils_Tuple2(plane.fk.ev, plane.fk.et));
                             }
                         }
                     }
                 }
             }();
             var _v1 = _v0.a;
             var x1 = _v1.a;
@@ -9718,86 +10025,86 @@
             var _v2 = _v0.b;
             var y1 = _v2.a;
             var y2 = _v2.b;
             var x1_ = x1 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var x2_ = x2 + A2($terezka$elm_charts$Internal$Svg$lengthInCartesianX, plane, config.g);
             var y1_ = y1 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
             var y2_ = y2 - A2($terezka$elm_charts$Internal$Svg$lengthInCartesianY, plane, config.h);
-            var _v146 = (config.gc > 0) ? _Utils_Tuple2(
+            var _v146 = (config.gf > 0) ? _Utils_Tuple2(
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianX,
                     plane,
-                    $elm$core$Basics$cos(angle) * config.gc),
+                    $elm$core$Basics$cos(angle) * config.gf),
                 A2(
                     $terezka$elm_charts$Internal$Svg$lengthInCartesianY,
                     plane,
-                    $elm$core$Basics$sin(angle) * config.gc)) : _Utils_Tuple2(0, 0);
+                    $elm$core$Basics$sin(angle) * config.gf)) : _Utils_Tuple2(0, 0);
             var tickOffsetX = _v146.a;
             var tickOffsetY = _v146.b;
             var cmds = config.e ? _Utils_ap(
-                (config.gc > 0) ? _List_fromArray(
+                (config.gf > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_ + tickOffsetX, y2_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x2_, y2_)
                     ]),
                 _Utils_ap(
-                    config.fq ? _List_fromArray(
+                    config.ft ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y1_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                         ]),
-                    (config.gc > 0) ? _List_fromArray(
+                    (config.gf > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_ + tickOffsetX, y1_ + tickOffsetY)
                         ]) : _List_Nil)) : _Utils_ap(
-                (config.gc > 0) ? _List_fromArray(
+                (config.gf > 0) ? _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_ + tickOffsetX, y1_ + tickOffsetY),
                         A2($terezka$elm_charts$Internal$Commands$Line, x1_, y1_)
                     ]) : _List_fromArray(
                     [
                         A2($terezka$elm_charts$Internal$Commands$Move, x1_, y1_)
                     ]),
                 _Utils_ap(
-                    config.fq ? _List_fromArray(
+                    config.ft ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x1_, y2_),
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]) : _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_, y2_)
                         ]),
-                    (config.gc > 0) ? _List_fromArray(
+                    (config.gf > 0) ? _List_fromArray(
                         [
                             A2($terezka$elm_charts$Internal$Commands$Line, x2_ + tickOffsetX, y2_ + tickOffsetY)
                         ]) : _List_Nil));
             return A4(
                 $terezka$elm_charts$Internal$Svg$withAttrs,
-                config.bv,
+                config.bu,
                 $elm$svg$Svg$path,
                 _List_fromArray(
                     [
                         $elm$svg$Svg$Attributes$class('elm-charts__line'),
                         $elm$svg$Svg$Attributes$fill('transparent'),
-                        $elm$svg$Svg$Attributes$stroke(config.bD),
+                        $elm$svg$Svg$Attributes$stroke(config.bC),
                         $elm$svg$Svg$Attributes$strokeWidth(
-                            $elm$core$String$fromFloat(config.ff)),
+                            $elm$core$String$fromFloat(config.fi)),
                         $elm$svg$Svg$Attributes$strokeOpacity(
-                            $elm$core$String$fromFloat(config.P)),
+                            $elm$core$String$fromFloat(config.Q)),
                         $elm$svg$Svg$Attributes$strokeDasharray(
                             A2(
                                 $elm$core$String$join,
                                 ' ',
-                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bG))),
+                                A2($elm$core$List$map, $elm$core$String$fromFloat, config.bF))),
                         $elm$svg$Svg$Attributes$d(
                             A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                         config.l ? $terezka$elm_charts$Internal$Svg$withinChartArea(plane) : $elm$svg$Svg$Attributes$class('')
                     ]),
                 _List_Nil);
         });
     var $terezka$elm_charts$Chart$Svg$line = F2(
@@ -9816,97 +10123,97 @@
                 },
                 xs);
         });
     var $terezka$elm_charts$Chart$Attributes$size = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    eZ: v
+                    e1: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$width = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    ff: v
+                    fi: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$x1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
                     aK: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$y1 = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    gx: $elm$core$Maybe$Just(v)
+                    gA: $elm$core$Maybe$Just(v)
                 });
         });
     var $terezka$elm_charts$Chart$grid = function(edits) {
         var config = A2(
             $terezka$elm_charts$Internal$Helpers$apply,
             edits, {
-                bD: '',
-                bG: _List_Nil,
+                bC: '',
+                bF: _List_Nil,
                 aP: false,
-                ff: 0
+                fi: 0
             });
-        var width = (!config.ff) ? (config.aP ? 0.5 : 1) : config.ff;
-        var color = $elm$core$String$isEmpty(config.bD) ? (config.aP ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.bD;
+        var width = (!config.fi) ? (config.aP ? 0.5 : 1) : config.fi;
+        var color = $elm$core$String$isEmpty(config.bC) ? (config.aP ? $terezka$elm_charts$Internal$Helpers$darkGray : $terezka$elm_charts$Internal$Helpers$gray) : config.bC;
         var toDot = F4(
             function(vs, p, x, y) {
-                return (A2($elm$core$List$member, x, vs.bg) || A2($elm$core$List$member, y, vs.bh)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return (A2($elm$core$List$member, x, vs.bf) || A2($elm$core$List$member, y, vs.bg)) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A5(
                         $terezka$elm_charts$Chart$Svg$dot,
                         p,
                         function($) {
-                            return $.fg;
+                            return $.fj;
                         },
                         function($) {
-                            return $.fh;
+                            return $.fk;
                         },
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$size(width),
                                 $terezka$elm_charts$Chart$Attributes$circle
                             ]), {
-                            fg: x,
-                            fh: y
+                            fj: x,
+                            fk: y
                         }));
             });
         var toXGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bg) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bf) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$x1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bG)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bF)
                             ])));
             });
         var toYGrid = F3(
             function(vs, p, v) {
-                return A2($elm$core$List$member, v, vs.bh) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
+                return A2($elm$core$List$member, v, vs.bg) ? $elm$core$Maybe$Nothing : $elm$core$Maybe$Just(
                     A2(
                         $terezka$elm_charts$Chart$Svg$line,
                         p,
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(color),
                                 $terezka$elm_charts$Chart$Attributes$width(width),
                                 $terezka$elm_charts$Chart$Attributes$y1(v),
-                                $terezka$elm_charts$Chart$Attributes$dashed(config.bG)
+                                $terezka$elm_charts$Chart$Attributes$dashed(config.bF)
                             ])));
             });
         return $terezka$elm_charts$Chart$GridElement(
             F2(
                 function(p, vs) {
                     return A2(
                         $elm$svg$Svg$g,
@@ -9916,15 +10223,15 @@
                             ]),
                         config.aP ? A2(
                             $elm$core$List$concatMap,
                             function(x) {
                                 return A2(
                                     $elm$core$List$filterMap,
                                     A3(toDot, vs, p, x),
-                                    vs.I);
+                                    vs.J);
                             },
                             vs.A) : _List_fromArray(
                             [
                                 A2(
                                     $elm$svg$Svg$g,
                                     _List_fromArray(
                                         [
@@ -9939,15 +10246,15 @@
                                     _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$class('elm-charts__y-grid')
                                         ]),
                                     A2(
                                         $elm$core$List$filterMap,
                                         A2(toYGrid, vs, p),
-                                        vs.I))
+                                        vs.J))
                             ]));
                 }));
     };
     var $elm$svg$Svg$Attributes$style = _VirtualDom_attribute('style');
     var $terezka$elm_charts$Chart$viewElements = F6(
         function(config, plane, tickValues, allItems, allLegends, elements) {
             var viewOne = F2(
@@ -10148,61 +10455,61 @@
                     $terezka$elm_charts$Chart$grid(_List_Nil),
                     indexedElements);
             }();
             var legends_ = $terezka$elm_charts$Chart$getLegends(elements);
             var config = A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
-                    bv: _List_fromArray(
+                    bu: _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$style('overflow: visible;')
                         ]),
-                    cZ: _List_Nil,
-                    bM: _List_Nil,
-                    eb: 300,
-                    bY: _List_Nil,
-                    ao: {
-                        aM: 0,
-                        ep: 0,
-                        a1: 0,
-                        e7: 0
+                    cY: _List_Nil,
+                    bL: _List_Nil,
+                    ea: 300,
+                    bX: _List_Nil,
+                    ap: {
+                        dO: 0,
+                        er: 0,
+                        eW: 0,
+                        fb: 0
                     },
-                    R: {
-                        aM: 0,
-                        ep: 0,
-                        a1: 0,
-                        e7: 0
+                    S: {
+                        dO: 0,
+                        er: 0,
+                        eW: 0,
+                        fb: 0
                     },
-                    dp: _List_Nil,
-                    cx: true,
-                    ff: 300
+                    dn: _List_Nil,
+                    cw: true,
+                    fi: 300
                 });
             var plane = A2($terezka$elm_charts$Chart$definePlane, config, elements);
             var items = A2($terezka$elm_charts$Chart$getItems, plane, elements);
             var toEvent = function(_v2) {
                 var event_ = _v2;
-                var _v1 = event_.fy;
+                var _v1 = event_.fB;
                 var decoder = _v1;
                 return A2(
                     $terezka$elm_charts$Internal$Svg$Event,
-                    event_.fW,
+                    event_.fZ,
                     decoder(items));
             };
             var tickValues = A3($terezka$elm_charts$Chart$getTickValues, plane, items, elements);
             var _v0 = A6($terezka$elm_charts$Chart$viewElements, config, plane, tickValues, items, legends_, elements);
             var beforeEls = _v0.a;
             var chartEls = _v0.b;
             var afterEls = _v0.c;
             return A5(
                 $terezka$elm_charts$Internal$Svg$container,
                 plane, {
-                    bv: config.bv,
-                    bM: A2($elm$core$List$map, toEvent, config.bM),
-                    bY: config.bY,
-                    cx: config.cx
+                    bu: config.bu,
+                    bL: A2($elm$core$List$map, toEvent, config.bL),
+                    bX: config.bX,
+                    cw: config.cw
                 },
                 beforeEls,
                 chartEls,
                 afterEls);
         });
     var $terezka$elm_charts$Internal$Many$Remodel = F2(
         function(a, b) {
@@ -10210,74 +10517,74 @@
                 $: 0,
                 a: a,
                 b: b
             };
         });
     var $terezka$elm_charts$Internal$Coordinates$center = function(pos) {
         return {
-            fg: pos.aK + ((pos.bf - pos.aK) / 2),
-            fh: pos.gx + ((pos.dL - pos.gx) / 2)
+            fj: pos.aK + ((pos.be - pos.aK) / 2),
+            fk: pos.gA + ((pos.dI - pos.gA) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Many$fromPoint = function(point) {
         return {
-            aK: point.fg,
-            bf: point.fg,
-            gx: point.fh,
-            dL: point.fh
+            aK: point.fj,
+            be: point.fj,
+            gA: point.fk,
+            dI: point.fk
         };
     };
     var $terezka$elm_charts$Internal$Item$getPosition = F2(
         function(plane, _v0) {
             var item = _v0;
-            return A2(item.gm, plane, item.fs);
+            return A2(item.gp, plane, item.fv);
         });
     var $terezka$elm_charts$Internal$Item$Dot = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Item$Rendered = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Item$isDot = function(_v0) {
         var item = _v0;
-        var _v1 = item.fs.f_;
+        var _v1 = item.fv.f1;
         if (!_v1.$) {
             var dot = _v1.a;
             return $elm$core$Maybe$Just({
-                fs: {
-                    f_: dot,
-                    gh: $terezka$elm_charts$Internal$Item$Dot,
-                    cI: item.fs.cI,
-                    gs: item.fs.gs
+                fv: {
+                    f1: dot,
+                    gk: $terezka$elm_charts$Internal$Item$Dot,
+                    cH: item.fv.cH,
+                    gv: item.fv.gv
                 },
-                gi: function(c) {
-                    return item.gi(item.fs);
+                gl: function(c) {
+                    return item.gl(item.fv);
                 },
-                gj: function(_v2) {
-                    return item.gj(item.fs);
+                gm: function(_v2) {
+                    return item.gm(item.fv);
                 },
-                gm: F2(
+                gp: F2(
                     function(plane, _v3) {
-                        return A2(item.gm, plane, item.fs);
+                        return A2(item.gp, plane, item.fv);
                     }),
-                gn: F3(
+                gq: F3(
                     function(plane, config, pos) {
-                        return config.gs.fQ ? A5(
+                        return config.gv.fT ? A5(
                             $terezka$elm_charts$Internal$Svg$dot,
                             plane,
                             function($) {
-                                return $.fg;
+                                return $.fj;
                             },
                             function($) {
-                                return $.fh;
+                                return $.fk;
                             },
-                            config.f_, {
-                                fg: config.gs.aK,
-                                fh: config.gs.fh
+                            config.f1, {
+                                fj: config.gv.aK,
+                                fk: config.gv.fk
                             }) : $elm$svg$Svg$text('');
                     })
             });
         } else {
             return $elm$core$Maybe$Nothing;
         }
     };
@@ -10361,15 +10668,15 @@
         function(defaultOffset, posixMinutes, eras) {
             toAdjustedMinutesHelp: while (true) {
                 if (!eras.b) {
                     return posixMinutes + defaultOffset;
                 } else {
                     var era = eras.a;
                     var olderEras = eras.b;
-                    if (_Utils_cmp(era.dD, posixMinutes) < 0) {
+                    if (_Utils_cmp(era.dz, posixMinutes) < 0) {
                         return posixMinutes + era.b;
                     } else {
                         var $temp$defaultOffset = defaultOffset,
                             $temp$posixMinutes = posixMinutes,
                             $temp$eras = olderEras;
                         defaultOffset = $temp$defaultOffset;
                         posixMinutes = $temp$posixMinutes;
@@ -10399,23 +10706,23 @@
         var dayOfEra = rawDay - (era * 146097);
         var yearOfEra = ((((dayOfEra - ((dayOfEra / 1460) | 0)) + ((dayOfEra / 36524) | 0)) - ((dayOfEra / 146096) | 0)) / 365) | 0;
         var dayOfYear = dayOfEra - (((365 * yearOfEra) + ((yearOfEra / 4) | 0)) - ((yearOfEra / 100) | 0));
         var mp = (((5 * dayOfYear) + 2) / 153) | 0;
         var month = mp + ((mp < 10) ? 3 : (-9));
         var year = yearOfEra + (era * 400);
         return {
-            dY: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
-            ev: month,
-            fi: year + ((month <= 2) ? 1 : 0)
+            dW: (dayOfYear - ((((153 * mp) + 2) / 5) | 0)) + 1,
+            ex: month,
+            fl: year + ((month <= 2) ? 1 : 0)
         };
     };
     var $elm$time$Time$toDay = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dY;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).dW;
         });
     var $elm$time$Time$toHour = F2(
         function(zone, time) {
             return A2(
                 $elm$core$Basics$modBy,
                 24,
                 A2(
@@ -10441,15 +10748,15 @@
     var $elm$time$Time$May = 4;
     var $elm$time$Time$Nov = 10;
     var $elm$time$Time$Oct = 9;
     var $elm$time$Time$Sep = 8;
     var $elm$time$Time$toMonth = F2(
         function(zone, time) {
             var _v0 = $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).ev;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).ex;
             switch (_v0) {
                 case 1:
                     return 0;
                 case 2:
                     return 1;
                 case 3:
                     return 2;
@@ -10482,15 +10789,15 @@
                     $elm$time$Time$flooredDiv,
                     $elm$time$Time$posixToMillis(time),
                     1000));
         });
     var $elm$time$Time$toYear = F2(
         function(zone, time) {
             return $elm$time$Time$toCivil(
-                A2($elm$time$Time$toAdjustedMinutes, zone, time)).fi;
+                A2($elm$time$Time$toAdjustedMinutes, zone, time)).fl;
         });
     var $elm$time$Time$utc = A2($elm$time$Time$Zone, 0, _List_Nil);
     var $author$project$Graph$formatTime = function(time) {
         var milliTime = $elm$time$Time$millisToPosix(
             $elm$core$Basics$floor(time) * 1000);
         var minute = $elm$core$String$fromInt(
             A2($elm$time$Time$toMinute, $elm$time$Time$utc, milliTime));
@@ -10511,46 +10818,55 @@
         function(_v0, items) {
             var func = _v0.b;
             return func(items);
         });
     var $terezka$elm_charts$Internal$Svg$closestPoint = F2(
         function(pos, searched) {
             return {
-                fg: A3($elm$core$Basics$clamp, pos.aK, pos.bf, searched.fg),
-                fh: A3($elm$core$Basics$clamp, pos.gx, pos.dL, searched.fh)
+                fj: A3($elm$core$Basics$clamp, pos.aK, pos.be, searched.fj),
+                fk: A3($elm$core$Basics$clamp, pos.gA, pos.dI, searched.fk)
             };
         });
     var $elm$core$Basics$abs = function(n) {
         return (n < 0) ? (-n) : n;
     };
     var $terezka$elm_charts$Internal$Svg$distanceX = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.fg) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.fg));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, point.fj) - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, searched.fj));
         });
     var $terezka$elm_charts$Internal$Svg$distanceY = F3(
         function(plane, searched, point) {
             return $elm$core$Basics$abs(
-                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.fh) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.fh));
+                A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, point.fk) - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, searched.fk));
         });
     var $elm$core$Basics$pow = _Basics_pow;
     var $terezka$elm_charts$Internal$Svg$distanceSquared = F3(
         function(plane, searched, point) {
             return A2(
                 $elm$core$Basics$pow,
                 A3($terezka$elm_charts$Internal$Svg$distanceX, plane, searched, point),
                 2) + A2(
                 $elm$core$Basics$pow,
                 A3($terezka$elm_charts$Internal$Svg$distanceY, plane, searched, point),
                 2);
         });
+    var $elm$core$List$head = function(list) {
+        if (list.b) {
+            var x = list.a;
+            var xs = list.b;
+            return $elm$core$Maybe$Just(x);
+        } else {
+            return $elm$core$Maybe$Nothing;
+        }
+    };
     var $terezka$elm_charts$Internal$Svg$keepOne = function(toPosition) {
         var toArea = function(a) {
             return function(pos) {
-                return (pos.aK - pos.bf) * (pos.gx - pos.dL);
+                return (pos.aK - pos.be) * (pos.gA - pos.dI);
             }(
                 toPosition(a));
         };
         var func = F2(
             function(one, acc) {
                 var _v0 = $elm$core$List$head(acc);
                 if (_v0.$ === 1) {
@@ -10617,56 +10933,56 @@
             });
     };
     var $terezka$elm_charts$Chart$Events$getNearest = $terezka$elm_charts$Internal$Events$getNearest;
     var $terezka$elm_charts$Chart$Attributes$height = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    eb: v
+                    ea: v
                 });
         });
     var $terezka$elm_charts$Chart$Attributes$htmlAttrs = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    bY: v
+                    bX: v
                 });
         });
     var $terezka$elm_charts$Internal$Svg$Linear = 0;
     var $terezka$elm_charts$Chart$Attributes$linear = function(config) {
         return _Utils_update(
             config, {
-                fU: $elm$core$Maybe$Just(0)
+                fX: $elm$core$Maybe$Just(0)
             });
     };
     var $terezka$elm_charts$Internal$Property$Property = function(a) {
         return {
             $: 0,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Property$property = F3(
         function(value, inter, attrs) {
             return $terezka$elm_charts$Internal$Property$Property({
-                bv: attrs,
-                d5: F5(
+                bu: attrs,
+                d4: F5(
                     function(_v0, _v1, _v2, _v3, _v4) {
                         return _List_Nil;
                     }),
                 F: A2(
                     $elm$core$Basics$composeR,
                     value,
                     A2(
                         $elm$core$Basics$composeR,
                         $elm$core$Maybe$map($elm$core$String$fromFloat),
                         $elm$core$Maybe$withDefault('N/A'))),
-                fO: inter,
-                es: $elm$core$Maybe$Nothing,
-                W: value,
-                a8: value
+                fR: inter,
+                eu: $elm$core$Maybe$Nothing,
+                Z: value,
+                a7: value
             });
         });
     var $terezka$elm_charts$Chart$interpolated = F2(
         function(y, inter) {
             return A2(
                 $terezka$elm_charts$Internal$Property$property,
                 A2($elm$core$Basics$composeR, y, $elm$core$Maybe$Just),
@@ -10680,21 +10996,21 @@
             $: 13,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$Axis = F7(
         function(length, marginMin, marginMax, dataMin, dataMax, min, max) {
             return {
-                fv: dataMax,
-                fw: dataMin,
-                N: length,
-                fS: marginMax,
-                fT: marginMin,
-                er: max,
-                et: min
+                fy: dataMax,
+                fz: dataMin,
+                O: length,
+                fV: marginMax,
+                fW: marginMin,
+                et: max,
+                ev: min
             };
         });
     var $terezka$elm_charts$Internal$Svg$apply = F2(
         function(funcs, _default) {
             var apply_ = F2(
                 function(f, a) {
                     return f(a);
@@ -10783,83 +11099,83 @@
             var _v0 = function() {
                 switch (design.$) {
                     case 0:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                bD: defaultColor,
+                                bC: defaultColor,
                                 o: 45,
-                                f6: 4,
-                                ff: 3
+                                f9: 4,
+                                fi: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.bD,
-                                    $elm$core$String$fromFloat(config.ff),
-                                    $elm$core$String$fromFloat(config.f6),
+                                    config.bC,
+                                    $elm$core$String$fromFloat(config.fi),
+                                    $elm$core$String$fromFloat(config.f9),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.f6,
+                                config.f9,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$line,
                                     _List_fromArray(
                                         [
                                             $elm$svg$Svg$Attributes$x1('0'),
                                             $elm$svg$Svg$Attributes$y('0'),
                                             $elm$svg$Svg$Attributes$x2('0'),
                                             $elm$svg$Svg$Attributes$y2(
-                                                $elm$core$String$fromFloat(config.f6)),
-                                            $elm$svg$Svg$Attributes$stroke(config.bD),
+                                                $elm$core$String$fromFloat(config.f9)),
+                                            $elm$svg$Svg$Attributes$stroke(config.bC),
                                             $elm$svg$Svg$Attributes$strokeWidth(
-                                                $elm$core$String$fromFloat(config.ff))
+                                                $elm$core$String$fromFloat(config.fi))
                                         ]),
                                     _List_Nil)),
                             theId);
                     case 1:
                         var edits = design.a;
                         var config = A2(
                             $terezka$elm_charts$Internal$Svg$apply,
                             edits, {
-                                bD: defaultColor,
+                                bC: defaultColor,
                                 o: 45,
-                                f6: 4,
-                                ff: 3
+                                f9: 4,
+                                fi: 3
                             });
                         var theId = toPatternId(
                             _List_fromArray(
                                 [
-                                    config.bD,
-                                    $elm$core$String$fromFloat(config.ff),
-                                    $elm$core$String$fromFloat(config.f6),
+                                    config.bC,
+                                    $elm$core$String$fromFloat(config.fi),
+                                    $elm$core$String$fromFloat(config.f9),
                                     $elm$core$String$fromFloat(config.o)
                                 ]));
                         return _Utils_Tuple2(
                             A4(
                                 toPatternDefs,
                                 theId,
-                                config.f6,
+                                config.f9,
                                 config.o,
                                 A2(
                                     $elm$svg$Svg$circle,
                                     _List_fromArray(
                                         [
-                                            $elm$svg$Svg$Attributes$fill(config.bD),
+                                            $elm$svg$Svg$Attributes$fill(config.bC),
                                             $elm$svg$Svg$Attributes$cx(
-                                                $elm$core$String$fromFloat(config.ff / 3)),
+                                                $elm$core$String$fromFloat(config.fi / 3)),
                                             $elm$svg$Svg$Attributes$cy(
-                                                $elm$core$String$fromFloat(config.ff / 3)),
+                                                $elm$core$String$fromFloat(config.fi / 3)),
                                             $elm$svg$Svg$Attributes$r(
-                                                $elm$core$String$fromFloat(config.ff / 3))
+                                                $elm$core$String$fromFloat(config.fi / 3))
                                         ]),
                                     _List_Nil)),
                             theId);
                     default:
                         var edits = design.a;
                         var colors = _Utils_eq(edits, _List_Nil) ? _List_fromArray(
                             [defaultColor, 'white']) : edits;
@@ -10908,15 +11224,15 @@
         });
     var $terezka$elm_charts$Internal$Svg$bar = F3(
         function(plane, config, point) {
             var viewBar = F6(
                 function(fill, fillOpacity, border, borderWidth, strokeOpacity, cmds) {
                     return A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bv,
+                        config.bu,
                         $elm$svg$Svg$path,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__bar'),
                                 $elm$svg$Svg$Attributes$fill(fill),
                                 $elm$svg$Svg$Attributes$fillOpacity(
                                     $elm$core$String$fromFloat(fillOpacity)),
@@ -10927,185 +11243,185 @@
                                     $elm$core$String$fromFloat(strokeOpacity)),
                                 $elm$svg$Svg$Attributes$d(
                                     A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                                 $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                             ]),
                         _List_Nil);
                 });
-            var highlightColor = (config.fI === '') ? config.bD : config.fI;
+            var highlightColor = (config.fL === '') ? config.bC : config.fL;
             var borderWidthCarY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.x / 2);
-            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fJ / 2);
+            var highlightWidthCarY = borderWidthCarY + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, config.fM / 2);
             var borderWidthCarX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.x / 2);
-            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fJ / 2);
+            var highlightWidthCarX = borderWidthCarX + A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, config.fM / 2);
             var pos = {
-                aK: A2($elm$core$Basics$min, point.aK, point.bf) + borderWidthCarX,
-                bf: A2($elm$core$Basics$max, point.aK, point.bf) - borderWidthCarX,
-                gx: A2($elm$core$Basics$min, point.gx, point.dL) + borderWidthCarY,
-                dL: A2($elm$core$Basics$max, point.gx, point.dL) - borderWidthCarY
+                aK: A2($elm$core$Basics$min, point.aK, point.be) + borderWidthCarX,
+                be: A2($elm$core$Basics$max, point.aK, point.be) - borderWidthCarX,
+                gA: A2($elm$core$Basics$min, point.gA, point.dI) + borderWidthCarY,
+                dI: A2($elm$core$Basics$max, point.gA, point.dI) - borderWidthCarY
             };
-            var height = $elm$core$Basics$abs(pos.dL - pos.gx);
+            var height = $elm$core$Basics$abs(pos.dI - pos.gA);
             var highlightPos = {
                 aK: pos.aK - highlightWidthCarX,
-                bf: pos.bf + highlightWidthCarX,
-                gx: pos.gx - highlightWidthCarY,
-                dL: pos.dL + highlightWidthCarY
+                be: pos.be + highlightWidthCarX,
+                gA: pos.gA - highlightWidthCarY,
+                dI: pos.dI + highlightWidthCarY
             };
-            var width = $elm$core$Basics$abs(pos.bf - pos.aK);
-            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f3);
+            var width = $elm$core$Basics$abs(pos.be - pos.aK);
+            var roundingBottom = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f6);
             var radiusBottomX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingBottom);
             var radiusBottomY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingBottom);
-            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f4);
+            var roundingTop = (A2($terezka$elm_charts$Internal$Coordinates$scaleSVGX, plane, width) * 0.5) * A3($elm$core$Basics$clamp, 0, 1, config.f7);
             var radiusTopX = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, roundingTop);
             var radiusTopY = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, roundingTop);
-            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.f4, config.f3);
+            var _v0 = ((((height - (radiusTopY * 0.8)) - (radiusBottomY * 0.8)) <= 0) || (((width - (radiusTopX * 0.8)) - (radiusBottomX * 0.8)) <= 0)) ? _Utils_Tuple2(0, 0) : _Utils_Tuple2(config.f7, config.f6);
             var roundTop = _v0.a;
             var roundBottom = _v0.b;
             var _v1 = function() {
-                if (_Utils_eq(pos.gx, pos.dL)) {
+                if (_Utils_eq(pos.gA, pos.dI)) {
                     return _Utils_Tuple2(_List_Nil, _List_Nil);
                 } else {
                     var _v2 = _Utils_Tuple2(roundTop > 0, roundBottom > 0);
                     if (!_v2.a) {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bf - radiusBottomX, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.be - radiusBottomX, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gA)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.gx + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bf - radiusBottomX, highlightPos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusBottomX, pos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bf, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.gA + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.be - radiusBottomX, highlightPos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusBottomX, pos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.be, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA)
                                     ]));
                         }
                     } else {
                         if (!_v2.b) {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusTopX, pos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bf, pos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusTopX, pos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.be, pos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf - radiusTopX, highlightPos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bf, highlightPos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bf - radiusTopX, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be - radiusTopX, highlightPos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.be, highlightPos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.be - radiusTopX, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA)
                                     ]));
                         } else {
                             return _Utils_Tuple2(
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusTopX, pos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.bf, pos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.bf - radiusBottomX, pos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, pos.aK + radiusBottomX, pos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.aK, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.aK + radiusTopX, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusTopX, pos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, pos.be, pos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, pos.be - radiusBottomX, pos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusBottomX, pos.gA)
                                     ]),
                                 _List_fromArray(
                                     [
-                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf - radiusTopX, highlightPos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.bf, highlightPos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.bf, highlightPos.gx + radiusBottomY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.bf - radiusBottomX, highlightPos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gx),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf - radiusBottomX, pos.gx),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.bf, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.dL - radiusTopY),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.bf - radiusTopX, pos.dL),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dL),
-                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dL - radiusTopY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gx + radiusBottomY),
-                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.bf, pos.gx)
+                                        A2($terezka$elm_charts$Internal$Commands$Move, highlightPos.aK + radiusBottomX, highlightPos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.aK, highlightPos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK, highlightPos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.aK + radiusTopX, highlightPos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be - radiusTopX, highlightPos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, true, highlightPos.be, highlightPos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.be, highlightPos.gA + radiusBottomY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, true, highlightPos.be - radiusBottomX, highlightPos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, highlightPos.aK + radiusBottomX, highlightPos.gA),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be - radiusBottomX, pos.gA),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingBottom, roundingBottom, -45, false, false, pos.be, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.dI - radiusTopY),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.be - radiusTopX, pos.dI),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK + radiusTopX, pos.dI),
+                                        A7($terezka$elm_charts$Internal$Commands$Arc, roundingTop, roundingTop, -45, false, false, pos.aK, pos.dI - radiusTopY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.aK, pos.gA + radiusBottomY),
+                                        A2($terezka$elm_charts$Internal$Commands$Line, pos.be, pos.gA)
                                     ]));
                         }
                     }
                 }
             }();
             var commands = _v1.a;
             var highlightCommands = _v1.b;
             var viewAuraBar = function(fill) {
-                return (!config.fH) ? A6(viewBar, fill, config.P, config.v, config.x, 1, commands) : A2(
+                return (!config.fK) ? A6(viewBar, fill, config.Q, config.v, config.x, 1, commands) : A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-highlight')
                         ]),
                     _List_fromArray(
                         [
-                            A6(viewBar, highlightColor, config.fH, 'transparent', 0, 0, highlightCommands),
-                            A6(viewBar, fill, config.P, config.v, config.x, 1, commands)
+                            A6(viewBar, highlightColor, config.fK, 'transparent', 0, 0, highlightCommands),
+                            A6(viewBar, fill, config.Q, config.v, config.x, 1, commands)
                         ]));
             };
-            var _v3 = config.cX;
+            var _v3 = config.cW;
             if (_v3.$ === 1) {
-                return viewAuraBar(config.bD);
+                return viewAuraBar(config.bC);
             } else {
                 var design = _v3.a;
-                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.bD, design);
+                var _v4 = A2($terezka$elm_charts$Internal$Svg$toPattern, config.bC, design);
                 var patternDefs = _v4.a;
                 var fill = _v4.b;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__bar-with-pattern')
@@ -11114,21 +11430,21 @@
                         [
                             patternDefs,
                             viewAuraBar(fill)
                         ]));
             }
         });
     var $terezka$elm_charts$Internal$Svg$defaultContainer = {
-        bv: _List_fromArray(
+        bu: _List_fromArray(
             [
                 $elm$svg$Svg$Attributes$style('overflow: visible;')
             ]),
-        bM: _List_Nil,
-        bY: _List_Nil,
-        cx: true
+        bL: _List_Nil,
+        bX: _List_Nil,
+        cw: true
     };
     var $terezka$elm_charts$Internal$Svg$barLegend = F2(
         function(config, barConfig) {
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
                     var size_ = _v0.a;
@@ -11137,118 +11453,118 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                fg: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ff, 0, 0, 0, 10, 0, 10),
-                fh: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
+                fj: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fi, 0, 0, 0, 10, 0, 10),
+                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ea, 0, 0, 0, 10, 0, 10)
             };
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bY),
+                    config.bX),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cx: false
+                                    cw: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Svg$bar,
                                         fakePlane,
                                         barConfig, {
                                             aK: 0,
-                                            bf: 10,
-                                            gx: 0,
-                                            dL: 10
+                                            be: 10,
+                                            gA: 0,
+                                            dI: 10
                                         })
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.f6) + 'px')
+                                        $elm$core$String$fromFloat(config.f9) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.gf)
+                                    $elm$html$Html$text(config.gi)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Internal$Svg$defaultBar = {
-        bv: _List_Nil,
+        bu: _List_Nil,
         v: 'white',
         x: 0,
-        bD: $terezka$elm_charts$Internal$Helpers$pink,
-        cX: $elm$core$Maybe$Nothing,
-        fH: 0,
-        fI: '',
-        fJ: 10,
-        P: 1,
-        f3: 0,
-        f4: 0
+        bC: $terezka$elm_charts$Internal$Helpers$pink,
+        cW: $elm$core$Maybe$Nothing,
+        fK: 0,
+        fL: '',
+        fM: 10,
+        Q: 1,
+        f6: 0,
+        f7: 0
     };
     var $terezka$elm_charts$Internal$Svg$defaultBarLegend = {
-        bD: '#808BAB',
+        bC: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        eb: 10,
-        bY: _List_Nil,
-        f6: 10,
-        gf: '',
-        ff: 10,
+        ea: 10,
+        bX: _List_Nil,
+        f9: 10,
+        gi: '',
+        fi: 10,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Chart$Svg$barLegend = F2(
         function(edits, barAttrs) {
             return A2(
                 $terezka$elm_charts$Internal$Svg$barLegend,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultBarLegend),
                 A2($terezka$elm_charts$Internal$Helpers$apply, barAttrs, $terezka$elm_charts$Internal$Svg$defaultBar));
         });
     var $terezka$elm_charts$Internal$Svg$Row = 0;
     var $terezka$elm_charts$Internal$Svg$defaultLegends = {
-        dP: 0,
+        dM: 0,
         i: $elm$core$Maybe$Nothing,
-        fn: '',
+        fq: '',
         v: '',
         x: 0,
-        bY: _List_Nil,
-        f6: 10,
+        bX: _List_Nil,
+        f9: 10,
         g: 0,
         h: 0
     };
     var $elm$virtual_dom$VirtualDom$node = function(tag) {
         return _VirtualDom_node(
             _VirtualDom_noScript(tag));
     };
     var $elm$html$Html$node = $elm$virtual_dom$VirtualDom$node;
     var $terezka$elm_charts$Internal$Svg$positionHtml = F7(
         function(plane, x, y, xOff, yOff, attrs, content) {
-            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.fh.N;
-            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.fg.N;
+            var yPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, y) - yOff) * 100) / plane.fk.O;
+            var xPercentage = ((A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, x) + xOff) * 100) / plane.fj.O;
             var posititonStyles = _List_fromArray(
                 [
                     A2(
                         $elm$html$Html$Attributes$style,
                         'left',
                         $elm$core$String$fromFloat(xPercentage) + '%'),
                     A2(
@@ -11264,15 +11580,15 @@
                 content);
         });
     var $terezka$elm_charts$Internal$Svg$legendsAt = F5(
         function(plane, x, y, config, children) {
             var otherAttrs = _List_fromArray(
                 [
                     $elm$html$Html$Attributes$class('elm-charts__legends'),
-                    A2($elm$html$Html$Attributes$style, 'background', config.fn),
+                    A2($elm$html$Html$Attributes$style, 'background', config.fq),
                     A2($elm$html$Html$Attributes$style, 'border-color', config.v),
                     A2(
                         $elm$html$Html$Attributes$style,
                         'border-width',
                         $elm$core$String$fromFloat(config.x) + 'px'),
                     A2($elm$html$Html$Attributes$style, 'border-style', 'solid')
                 ]);
@@ -11303,15 +11619,15 @@
                                 [
                                     A2($elm$html$Html$Attributes$style, 'transform', 'translate(-50%, 0%)')
                                 ]);
                     }
                 }
             }();
             var _v0 = function() {
-                var _v1 = config.dP;
+                var _v1 = config.dM;
                 if (!_v1) {
                     return _Utils_Tuple2(
                         _List_fromArray(
                             [
                                 A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                             ]),
@@ -11325,27 +11641,27 @@
                                 A2($elm$html$Html$Attributes$style, 'align-items', 'baseline')
                             ]),
                         'bottom');
                 }
             }();
             var alignmentAttrs = _v0.a;
             var direction = _v0.b;
-            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.f6) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
+            var paddingStyle = ' .elm-charts__legends .elm-charts__legend {\n              margin-' + (direction + (':' + ($elm$core$String$fromFloat(config.f9) + ('px;\n            }\n\n            .elm-charts__legends .elm-charts__legend:last-child {\n              margin-' + (direction + ': 0px;\n            }\n        ')))));
             return A7(
                 $terezka$elm_charts$Internal$Svg$positionHtml,
                 plane,
                 x,
                 y,
                 config.g,
                 -config.h,
                 _Utils_ap(
                     anchorAttrs,
                     _Utils_ap(
                         alignmentAttrs,
-                        _Utils_ap(otherAttrs, config.bY))),
+                        _Utils_ap(otherAttrs, config.bX))),
                 A2(
                     $elm$core$List$cons,
                     A3(
                         $elm$html$Html$node,
                         'style',
                         _List_Nil,
                         _List_fromArray(
@@ -11360,84 +11676,84 @@
                 $terezka$elm_charts$Internal$Svg$legendsAt,
                 plane,
                 x,
                 y,
                 A2($terezka$elm_charts$Internal$Helpers$apply, edits, $terezka$elm_charts$Internal$Svg$defaultLegends));
         });
     var $terezka$elm_charts$Internal$Svg$defaultInterpolation = {
-        bv: _List_Nil,
-        bD: $terezka$elm_charts$Internal$Helpers$pink,
-        bG: _List_Nil,
-        cX: $elm$core$Maybe$Nothing,
-        fU: $elm$core$Maybe$Nothing,
-        P: 0,
-        ff: 1
+        bu: _List_Nil,
+        bC: $terezka$elm_charts$Internal$Helpers$pink,
+        bF: _List_Nil,
+        cW: $elm$core$Maybe$Nothing,
+        fX: $elm$core$Maybe$Nothing,
+        Q: 0,
+        fi: 1
     };
     var $terezka$elm_charts$Internal$Svg$defaultLineLegend = {
-        bD: '#808BAB',
+        bC: '#808BAB',
         k: $elm$core$Maybe$Nothing,
-        eb: 16,
-        bY: _List_Nil,
-        f6: 10,
-        gf: '',
-        ff: 30,
+        ea: 16,
+        bX: _List_Nil,
+        f9: 10,
+        gi: '',
+        fi: 30,
         g: 0,
         h: 0
     };
     var $terezka$elm_charts$Internal$Svg$Point = F2(
         function(x, y) {
             return {
-                fg: x,
-                fh: y
+                fj: x,
+                fk: y
             };
         });
     var $elm$svg$Svg$Attributes$fillRule = _VirtualDom_attribute('fill-rule');
     var $terezka$elm_charts$Internal$Interpolation$linear = $elm$core$List$map(
         $elm$core$List$map(
             function(_v0) {
-                var x = _v0.fg;
-                var y = _v0.fh;
+                var x = _v0.fj;
+                var y = _v0.fk;
                 return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
             }));
     var $terezka$elm_charts$Internal$Interpolation$First = {
         $: 0
     };
     var $terezka$elm_charts$Internal$Interpolation$Previous = function(a) {
         return {
             $: 1,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Interpolation$monotoneCurve = F4(
         function(point0, point1, tangent0, tangent1) {
-            var dx = (point1.fg - point0.fg) / 3;
-            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.fg + dx, point0.fh + (dx * tangent0), point1.fg - dx, point1.fh - (dx * tangent1), point1.fg, point1.fh);
+            var dx = (point1.fj - point0.fj) / 3;
+            return A6($terezka$elm_charts$Internal$Commands$CubicBeziers, point0.fj + dx, point0.fk + (dx * tangent0), point1.fj - dx, point1.fk - (dx * tangent1), point1.fj, point1.fk);
         });
     var $elm$core$Basics$neq = _Utils_notEqual;
     var $terezka$elm_charts$Internal$Interpolation$slope2 = F3(
         function(point0, point1, t) {
-            var h = point1.fg - point0.fg;
-            return (!(!h)) ? ((((3 * (point1.fh - point0.fh)) / h) - t) / 2) : t;
+            var h = point1.fj - point0.fj;
+            return (!(!h)) ? ((((3 * (point1.fk - point0.fk)) / h) - t) / 2) : t;
         });
     var $elm$core$Basics$isNaN = _Basics_isNaN;
     var $terezka$elm_charts$Internal$Interpolation$sign = function(x) {
         return (x < 0) ? (-1) : 1;
     };
     var $terezka$elm_charts$Internal$Interpolation$toH = F2(
         function(h0, h1) {
             return (!h0) ? ((h1 < 0) ? (0 * (-1)) : h1) : h0;
         });
     var $terezka$elm_charts$Internal$Interpolation$slope3 = F3(
         function(point0, point1, point2) {
-            var h1 = point2.fg - point1.fg;
-            var h0 = point1.fg - point0.fg;
+            var h1 = point2.fj - point1.fj;
+            var h0 = point1.fj - point0.fj;
             var s0h = A2($terezka$elm_charts$Internal$Interpolation$toH, h0, h1);
-            var s0 = (point1.fh - point0.fh) / s0h;
+            var s0 = (point1.fk - point0.fk) / s0h;
             var s1h = A2($terezka$elm_charts$Internal$Interpolation$toH, h1, h0);
-            var s1 = (point2.fh - point1.fh) / s1h;
+            var s1 = (point2.fk - point1.fk) / s1h;
             var p = ((s0 * h1) + (s1 * h0)) / (h0 + h1);
             var slope = ($terezka$elm_charts$Internal$Interpolation$sign(s0) + $terezka$elm_charts$Internal$Interpolation$sign(s1)) * A2(
                 $elm$core$Basics$min,
                 A2(
                     $elm$core$Basics$min,
                     $elm$core$Basics$abs(s0),
                     $elm$core$Basics$abs(s1)),
@@ -11488,15 +11804,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t1, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fg, p1.fh)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fj, p1.fk)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     } else {
                         if (_v1.b.b && _v1.b.b.b) {
@@ -11534,15 +11850,15 @@
                                 return _Utils_Tuple2(
                                     $terezka$elm_charts$Internal$Interpolation$Previous(t1),
                                     _Utils_ap(
                                         commands,
                                         _List_fromArray(
                                             [
                                                 A4($terezka$elm_charts$Internal$Interpolation$monotoneCurve, p0, p1, t0, t1),
-                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fg, p1.fh)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, p1.fj, p1.fk)
                                             ])));
                             }
                         } else {
                             break _v1$4;
                         }
                     }
                 }
@@ -11559,15 +11875,15 @@
                     return A2(
                         $terezka$elm_charts$Internal$Interpolation$monotonePart,
                         A2($elm$core$List$cons, p0, rest),
                         _Utils_Tuple2(
                             tangent,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.fg, p0.fh)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, p0.fj, p0.fk)
                                 ])));
                 } else {
                     return _Utils_Tuple2(tangent, _List_Nil);
                 }
             }();
             var t0 = _v1.a;
             var commands = _v1.b;
@@ -11585,24 +11901,24 @@
             $terezka$elm_charts$Internal$Interpolation$monotoneSection,
             _Utils_Tuple2($terezka$elm_charts$Internal$Interpolation$First, _List_Nil),
             sections).b;
     };
     var $terezka$elm_charts$Internal$Interpolation$Point = F2(
         function(x, y) {
             return {
-                fg: x,
-                fh: y
+                fj: x,
+                fk: y
             };
         });
     var $terezka$elm_charts$Internal$Interpolation$after = F2(
         function(a, b) {
             return _List_fromArray(
                 [
                     a,
-                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.fg, a.fh),
+                    A2($terezka$elm_charts$Internal$Interpolation$Point, b.fj, a.fk),
                     b
                 ]);
         });
     var $terezka$elm_charts$Internal$Interpolation$stepped = function(sections) {
         var expand = F2(
             function(result, section) {
                 expand: while (true) {
@@ -11631,16 +11947,16 @@
         return A2(
             $elm$core$List$map,
             A2(
                 $elm$core$Basics$composeR,
                 expand(_List_Nil),
                 $elm$core$List$map(
                     function(_v2) {
-                        var x = _v2.fg;
-                        var y = _v2.fh;
+                        var x = _v2.fj;
+                        var y = _v2.fk;
                         return A2($terezka$elm_charts$Internal$Commands$Line, x, y);
                     })),
             sections);
     };
     var $elm$core$List$drop = F2(
         function(n, list) {
             drop: while (true) {
@@ -11707,25 +12023,25 @@
                             var rest = acc.b;
                             return A2(
                                 $elm$core$List$cons,
                                 _Utils_ap(
                                     latest,
                                     _List_fromArray(
                                         [{
-                                            fg: toX(datum_),
-                                            fh: y_
+                                            fj: toX(datum_),
+                                            fk: y_
                                         }])),
                                 rest);
                         } else {
                             return A2(
                                 $elm$core$List$cons,
                                 _List_fromArray(
                                     [{
-                                        fg: toX(datum_),
-                                        fh: y_
+                                        fj: toX(datum_),
+                                        fk: y_
                                     }]),
                                 acc);
                         }
                     } else {
                         return A2($elm$core$List$cons, _List_Nil, acc);
                     }
                 });
@@ -11745,37 +12061,37 @@
                 $elm$core$List$filterMap,
                 $elm$core$Basics$identity,
                 A3($elm$core$List$map2, toSets, points, commands));
         });
     var $terezka$elm_charts$Internal$Svg$area = F6(
         function(plane, toX, toY2M, toY, config, data) {
             var _v0 = function() {
-                var _v1 = config.cX;
+                var _v1 = config.cW;
                 if (_v1.$ === 1) {
                     return _Utils_Tuple2(
                         $elm$svg$Svg$text(''),
-                        config.bD);
+                        config.bC);
                 } else {
                     var design = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.bD, design);
+                    return A2($terezka$elm_charts$Internal$Svg$toPattern, config.bC, design);
                 }
             }();
             var patternDefs = _v0.a;
             var fill = _v0.b;
             var view = function(cmds) {
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bv,
+                    config.bu,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__area-section'),
                             $elm$svg$Svg$Attributes$fill(fill),
                             $elm$svg$Svg$Attributes$fillOpacity(
-                                $elm$core$String$fromFloat(config.P)),
+                                $elm$core$String$fromFloat(config.Q)),
                             $elm$svg$Svg$Attributes$strokeWidth('0'),
                             $elm$svg$Svg$Attributes$fillRule('evenodd'),
                             $elm$svg$Svg$Attributes$d(
                                 A2($terezka$elm_charts$Internal$Commands$description, plane, cmds)),
                             $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                         ]),
                     _List_Nil);
@@ -11788,53 +12104,53 @@
                     var firstTop = _v6.a;
                     var cmdsTop = _v6.b;
                     var endTop = _v6.c;
                     return view(
                         _Utils_ap(
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fg, firstBottom.fh),
-                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.fg, firstTop.fh)
+                                    A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fj, firstBottom.fk),
+                                    A2($terezka$elm_charts$Internal$Commands$Line, firstTop.fj, firstTop.fk)
                                 ]),
                             _Utils_ap(
                                 cmdsTop,
                                 _Utils_ap(
                                     _List_fromArray(
                                         [
-                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fg, firstBottom.fh)
+                                            A2($terezka$elm_charts$Internal$Commands$Move, firstBottom.fj, firstBottom.fk)
                                         ]),
                                     _Utils_ap(
                                         cmdsBottom,
                                         _List_fromArray(
                                             [
-                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.fg, endTop.fh)
+                                                A2($terezka$elm_charts$Internal$Commands$Line, endTop.fj, endTop.fk)
                                             ]))))));
                 });
             var withoutUnder = function(_v4) {
                 var first = _v4.a;
                 var cmds = _v4.b;
                 var end = _v4.c;
                 return view(
                     _Utils_ap(
                         _List_fromArray(
                             [
-                                A2($terezka$elm_charts$Internal$Commands$Move, first.fg, 0),
-                                A2($terezka$elm_charts$Internal$Commands$Line, first.fg, first.fh)
+                                A2($terezka$elm_charts$Internal$Commands$Move, first.fj, 0),
+                                A2($terezka$elm_charts$Internal$Commands$Line, first.fj, first.fk)
                             ]),
                         _Utils_ap(
                             cmds,
                             _List_fromArray(
                                 [
-                                    A2($terezka$elm_charts$Internal$Commands$Line, end.fg, 0)
+                                    A2($terezka$elm_charts$Internal$Commands$Line, end.fj, 0)
                                 ]))));
             };
-            if (config.P <= 0) {
+            if (config.Q <= 0) {
                 return $elm$svg$Svg$text('');
             } else {
-                var _v2 = config.fU;
+                var _v2 = config.fX;
                 if (_v2.$ === 1) {
                     return $elm$svg$Svg$text('');
                 } else {
                     var method = _v2.a;
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -11868,41 +12184,41 @@
     var $terezka$elm_charts$Internal$Svg$interpolation = F5(
         function(plane, toX, toY, config, data) {
             var view = function(_v1) {
                 var first = _v1.a;
                 var cmds = _v1.b;
                 return A4(
                     $terezka$elm_charts$Internal$Svg$withAttrs,
-                    config.bv,
+                    config.bu,
                     $elm$svg$Svg$path,
                     _List_fromArray(
                         [
                             $elm$svg$Svg$Attributes$class('elm-charts__interpolation-section'),
                             $elm$svg$Svg$Attributes$fill('transparent'),
-                            $elm$svg$Svg$Attributes$stroke(config.bD),
+                            $elm$svg$Svg$Attributes$stroke(config.bC),
                             $elm$svg$Svg$Attributes$strokeDasharray(
                                 A2(
                                     $elm$core$String$join,
                                     ' ',
-                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bG))),
+                                    A2($elm$core$List$map, $elm$core$String$fromFloat, config.bF))),
                             $elm$svg$Svg$Attributes$strokeWidth(
-                                $elm$core$String$fromFloat(config.ff)),
+                                $elm$core$String$fromFloat(config.fi)),
                             $elm$svg$Svg$Attributes$d(
                                 A2(
                                     $terezka$elm_charts$Internal$Commands$description,
                                     plane,
                                     A2(
                                         $elm$core$List$cons,
-                                        A2($terezka$elm_charts$Internal$Commands$Move, first.fg, first.fh),
+                                        A2($terezka$elm_charts$Internal$Commands$Move, first.fj, first.fk),
                                         cmds))),
                             $terezka$elm_charts$Internal$Svg$withinChartArea(plane)
                         ]),
                     _List_Nil);
             };
-            var _v0 = config.fU;
+            var _v0 = config.fX;
             if (_v0.$ === 1) {
                 return $elm$svg$Svg$text('');
             } else {
                 var method = _v0.a;
                 return A2(
                     $elm$svg$Svg$g,
                     _List_fromArray(
@@ -11937,15 +12253,15 @@
         });
     var $terezka$elm_charts$Internal$Svg$lineLegend = F3(
         function(config, interConfig, dotConfig) {
             var topMargin = function() {
                 var _v1 = dotConfig.aG;
                 if (!_v1.$) {
                     var shape = _v1.a;
-                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.eZ, shape);
+                    return A2($terezka$elm_charts$Internal$Svg$toRadius, dotConfig.e1, shape);
                 } else {
                     return 0;
                 }
             }();
             var fontStyle = function() {
                 var _v0 = config.k;
                 if (!_v0.$) {
@@ -11955,125 +12271,125 @@
                         'font-size',
                         $elm$core$String$fromInt(size_) + 'px');
                 } else {
                     return A2($elm$html$Html$Attributes$style, '', '');
                 }
             }();
             var fakePlane = {
-                fg: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ff, 0, 0, 0, 10, 0, 10),
-                fh: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.eb, 0, 0, 0, 10, 0, 10)
+                fj: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.fi, 0, 0, 0, 10, 0, 10),
+                fk: A7($terezka$elm_charts$Internal$Coordinates$Axis, config.ea, 0, 0, 0, 10, 0, 10)
             };
-            var bottomMargin = (!interConfig.P) ? topMargin : 0;
+            var bottomMargin = (!interConfig.Q) ? topMargin : 0;
             return A2(
                 $elm$html$Html$div,
                 _Utils_ap(
                     _List_fromArray(
                         [
                             $elm$html$Html$Attributes$class('elm-charts__legend'),
                             A2($elm$html$Html$Attributes$style, 'display', 'flex'),
                             A2($elm$html$Html$Attributes$style, 'align-items', 'center')
                         ]),
-                    config.bY),
+                    config.bX),
                 _List_fromArray(
                     [
                         A5(
                             $terezka$elm_charts$Internal$Svg$container,
                             fakePlane,
                             _Utils_update(
                                 $terezka$elm_charts$Internal$Svg$defaultContainer, {
-                                    cx: false
+                                    cw: false
                                 }),
                             _List_Nil,
                             _List_fromArray(
                                 [
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$interpolation,
                                         fakePlane,
                                         function($) {
-                                            return $.fg;
+                                            return $.fj;
                                         },
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.fh;
+                                                return $.fk;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A6(
                                         $terezka$elm_charts$Internal$Svg$area,
                                         fakePlane,
                                         function($) {
-                                            return $.fg;
+                                            return $.fj;
                                         },
                                         $elm$core$Maybe$Nothing,
                                         A2(
                                             $elm$core$Basics$composeR,
                                             function($) {
-                                                return $.fh;
+                                                return $.fk;
                                             },
                                             $elm$core$Maybe$Just),
                                         interConfig,
                                         _List_fromArray(
                                             [
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 0, 5),
                                                 A2($terezka$elm_charts$Internal$Svg$Point, 10, 5)
                                             ])),
                                     A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         fakePlane,
                                         function($) {
-                                            return $.fg;
+                                            return $.fj;
                                         },
                                         function($) {
-                                            return $.fh;
+                                            return $.fk;
                                         },
                                         dotConfig,
                                         A2($terezka$elm_charts$Internal$Svg$Point, 5, 5))
                                 ]),
                             _List_Nil),
                         A2(
                             $elm$html$Html$div,
                             _List_fromArray(
                                 [
                                     fontStyle,
                                     A2(
                                         $elm$html$Html$Attributes$style,
                                         'margin-left',
-                                        $elm$core$String$fromFloat(config.f6) + 'px')
+                                        $elm$core$String$fromFloat(config.f9) + 'px')
                                 ]),
                             _List_fromArray(
                                 [
-                                    $elm$html$Html$text(config.gf)
+                                    $elm$html$Html$text(config.gi)
                                 ]))
                     ]));
         });
     var $terezka$elm_charts$Chart$Attributes$opacity = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    P: v
+                    Q: v
                 });
         });
     var $terezka$elm_charts$Chart$Svg$lineLegend = F3(
         function(edits, interAttrsOrg, dotAttrsOrg) {
             var interpolationConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, interAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultInterpolation);
             var dotConfigOrg = A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrsOrg, $terezka$elm_charts$Internal$Svg$defaultDot);
             var adjustWidth = function(config) {
                 return _Utils_update(
                     config, {
-                        ff: 10
+                        fi: 10
                     });
             };
             var _v0 = function() {
-                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fU, dotConfigOrg.aG);
+                var _v1 = _Utils_Tuple2(interpolationConfigOrg.fX, dotConfigOrg.aG);
                 if (!_v1.a.$) {
                     if (_v1.b.$ === 1) {
                         var _v2 = _v1.b;
                         return _Utils_Tuple3(
                             dotAttrsOrg,
                             interAttrsOrg,
                             A2(
@@ -12121,15 +12437,15 @@
                 A2($terezka$elm_charts$Internal$Helpers$apply, interAttrs, $terezka$elm_charts$Internal$Svg$defaultInterpolation),
                 A2($terezka$elm_charts$Internal$Helpers$apply, dotAttrs, $terezka$elm_charts$Internal$Svg$defaultDot));
         });
     var $terezka$elm_charts$Chart$Attributes$title = F2(
         function(value, config) {
             return _Utils_update(
                 config, {
-                    gf: value
+                    gi: value
                 });
         });
     var $terezka$elm_charts$Chart$legendsAt = F4(
         function(toX, toY, attrs, children) {
             return $terezka$elm_charts$Chart$HtmlElement(
                 F2(
                     function(p, legends_) {
@@ -12157,58 +12473,58 @@
                                     interAttrs,
                                     dotAttrs);
                             }
                         };
                         return A5(
                             $terezka$elm_charts$Chart$Svg$legendsAt,
                             p,
-                            toX(p.fg),
-                            toY(p.fh),
+                            toX(p.fj),
+                            toY(p.fk),
                             attrs,
                             A2($elm$core$List$map, viewLegend, legends_));
                     }));
         });
+    var $terezka$elm_charts$Chart$Attributes$margin = F2(
+        function(v, config) {
+            return _Utils_update(
+                config, {
+                    ap: v
+                });
+        });
     var $terezka$elm_charts$Internal$Svg$Monotone = 1;
     var $terezka$elm_charts$Chart$Attributes$monotone = function(config) {
         return _Utils_update(
             config, {
-                fU: $elm$core$Maybe$Just(1)
+                fX: $elm$core$Maybe$Just(1)
             });
     };
-    var $terezka$elm_charts$Chart$Attributes$moveDown = F2(
-        function(v, config) {
-            return _Utils_update(
-                config, {
-                    h: config.h + v
-                });
-        });
     var $terezka$elm_charts$Internal$Property$Stacked = function(a) {
         return {
             $: 1,
             a: a
         };
     };
     var $terezka$elm_charts$Internal$Property$meta = F2(
         function(value, prop) {
             if (!prop.$) {
                 var con = prop.a;
                 return $terezka$elm_charts$Internal$Property$Property(
                     _Utils_update(
                         con, {
-                            es: $elm$core$Maybe$Just(value)
+                            eu: $elm$core$Maybe$Just(value)
                         }));
             } else {
                 var cons = prop.a;
                 return $terezka$elm_charts$Internal$Property$Stacked(
                     A2(
                         $elm$core$List$map,
                         function(con) {
                             return _Utils_update(
                                 con, {
-                                    es: $elm$core$Maybe$Just(value)
+                                    eu: $elm$core$Maybe$Just(value)
                                 });
                         },
                         cons));
             }
         });
     var $terezka$elm_charts$Chart$named = function(name) {
         return $terezka$elm_charts$Internal$Property$meta(name);
@@ -12233,20 +12549,20 @@
         });
     var $terezka$elm_charts$Chart$Events$map = $terezka$elm_charts$Internal$Events$map;
     var $terezka$elm_charts$Internal$Events$Event = $elm$core$Basics$identity;
     var $terezka$elm_charts$Internal$Events$on = F3(
         function(name, decoder, config) {
             return _Utils_update(
                 config, {
-                    bM: A2(
+                    bL: A2(
                         $elm$core$List$cons, {
-                            fy: decoder,
-                            fW: name
+                            fB: decoder,
+                            fZ: name
                         },
-                        config.bM)
+                        config.bL)
                 });
         });
     var $terezka$elm_charts$Chart$Events$on = $terezka$elm_charts$Internal$Events$on;
     var $terezka$elm_charts$Chart$Events$onMouseLeave = function(onMsg) {
         return A2(
             $terezka$elm_charts$Chart$Events$on,
             'mouseleave',
@@ -12258,25 +12574,18 @@
     var $terezka$elm_charts$Chart$Events$onMouseMove = F2(
         function(onMsg, decoder) {
             return A2(
                 $terezka$elm_charts$Chart$Events$on,
                 'mousemove',
                 A2($terezka$elm_charts$Chart$Events$map, onMsg, decoder));
         });
-    var $terezka$elm_charts$Chart$Attributes$rotate = F2(
-        function(v, config) {
-            return _Utils_update(
-                config, {
-                    o: config.o + v
-                });
-        });
     var $terezka$elm_charts$Chart$Attributes$row = function(config) {
         return _Utils_update(
             config, {
-                dP: 0
+                dM: 0
             });
     };
     var $terezka$elm_charts$Chart$Indexed = function(a) {
         return {
             $: 0,
             a: a
         };
@@ -12289,100 +12598,100 @@
                 b: b,
                 c: c,
                 d: d
             };
         });
     var $terezka$elm_charts$Internal$Item$toHtml = function(_v0) {
         var item = _v0;
-        return item.gi(item.fs);
+        return item.gl(item.fv);
     };
     var $terezka$elm_charts$Internal$Item$toSvg = F2(
         function(plane, _v0) {
             var item = _v0;
             return A3(
-                item.gn,
+                item.gq,
                 plane,
-                item.fs,
-                A2(item.gm, plane, item.fs));
+                item.fv,
+                A2(item.gp, plane, item.fv));
         });
     var $terezka$elm_charts$Internal$Item$generalize = F2(
         function(toAny, _v0) {
             var item = _v0;
             return {
-                fs: {
-                    f_: toAny(item.fs.f_),
-                    gh: $elm$core$Basics$identity,
-                    cI: item.fs.cI,
-                    gs: item.fs.gs
+                fv: {
+                    f1: toAny(item.fv.f1),
+                    gk: $elm$core$Basics$identity,
+                    cH: item.fv.cH,
+                    gv: item.fv.gv
                 },
-                gi: function(c) {
+                gl: function(c) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                gj: function(_v1) {
-                    return item.gj(item.fs);
+                gm: function(_v1) {
+                    return item.gm(item.fv);
                 },
-                gm: F2(
+                gp: F2(
                     function(plane, _v2) {
-                        return A2(item.gm, plane, item.fs);
+                        return A2(item.gp, plane, item.fv);
                     }),
-                gn: F3(
+                gq: F3(
                     function(plane, _v3, _v4) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $terezka$elm_charts$Internal$Many$getMembers = function(_v0) {
         var group_ = _v0;
         return function(_v1) {
             var x = _v1.a;
             var xs = _v1.b;
             return A2($elm$core$List$cons, x, xs);
-        }(group_.fs.el);
+        }(group_.fv.ek);
     };
     var $terezka$elm_charts$Internal$Many$getGenerals = function(group_) {
         var generalize = function(_v0) {
             var item = _v0;
-            return A2($terezka$elm_charts$Internal$Item$generalize, item.fs.gh, item);
+            return A2($terezka$elm_charts$Internal$Item$generalize, item.fv.gk, item);
         };
         return A2(
             $elm$core$List$map,
             generalize,
             $terezka$elm_charts$Internal$Many$getMembers(group_));
     };
     var $terezka$elm_charts$Internal$Item$getLimits = function(_v0) {
         var item = _v0;
-        return item.gj(item.fs);
+        return item.gm(item.fv);
     };
     var $terezka$elm_charts$Internal$Item$map = F2(
         function(func, _v0) {
             var item = _v0;
             return {
-                fs: {
-                    f_: item.fs.f_,
-                    gh: item.fs.gh,
-                    cI: item.fs.cI,
-                    gs: {
-                        fx: func(item.fs.gs.fx),
-                        fQ: item.fs.gs.fQ,
-                        aK: item.fs.gs.aK,
-                        bf: item.fs.gs.bf,
-                        fh: item.fs.gs.fh
+                fv: {
+                    f1: item.fv.f1,
+                    gk: item.fv.gk,
+                    cH: item.fv.cH,
+                    gv: {
+                        fA: func(item.fv.gv.fA),
+                        fT: item.fv.gv.fT,
+                        aK: item.fv.gv.aK,
+                        be: item.fv.gv.be,
+                        fk: item.fv.gv.fk
                     }
                 },
-                gi: function(_v1) {
+                gl: function(_v1) {
                     return $terezka$elm_charts$Internal$Item$toHtml(item);
                 },
-                gj: function(_v2) {
-                    return item.gj(item.fs);
+                gm: function(_v2) {
+                    return item.gm(item.fv);
                 },
-                gm: F2(
+                gp: F2(
                     function(plane, _v3) {
-                        return A2(item.gm, plane, item.fs);
+                        return A2(item.gp, plane, item.fv);
                     }),
-                gn: F3(
+                gq: F3(
                     function(plane, _v4, _v5) {
                         return A2($terezka$elm_charts$Internal$Item$toSvg, plane, item);
                     })
             };
         });
     var $elm$virtual_dom$VirtualDom$map = _VirtualDom_map;
     var $elm$svg$Svg$map = $elm$virtual_dom$VirtualDom$map;
@@ -12475,27 +12784,27 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fO);
+                        prop.fR);
                     var interConfig = toInterConfig(interAttr);
                     var defaultName = 'Property #' + $elm$core$String$fromInt(colorIndex + 1);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bD),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bD),
-                            _Utils_eq(interConfig.fU, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bC),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bC),
+                            _Utils_eq(interConfig.fX, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
-                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bv);
+                    var dotAttrs = _Utils_ap(defaultAttrs, prop.bu);
                     return A3(
                         $terezka$elm_charts$Internal$Legend$LineLegend,
-                        A2($elm$core$Maybe$withDefault, defaultName, prop.es),
+                        A2($elm$core$Maybe$withDefault, defaultName, prop.eu),
                         interAttr,
                         dotAttrs);
                 });
             return A2(
                 $elm$core$List$indexedMap,
                 F2(
                     function(propIndex, f) {
@@ -12562,120 +12871,120 @@
                 return A2($terezka$elm_charts$Internal$Helpers$apply, attrs, $terezka$elm_charts$Internal$Svg$defaultDot);
             };
             var toDotItem = F7(
                 function(lineIndex, stackIndex, colorIndex, prop, interConfig, dataIndex, datum_) {
                     var y_ = A2(
                         $elm$core$Maybe$withDefault,
                         0,
-                        prop.a8(datum_));
+                        prop.a7(datum_));
                     var x_ = toX(datum_);
                     var defaultAttrs = _List_fromArray(
                         [
-                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bD),
-                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bD),
-                            _Utils_eq(interConfig.fU, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
+                            $terezka$elm_charts$Chart$Attributes$color(interConfig.bC),
+                            $terezka$elm_charts$Chart$Attributes$border(interConfig.bC),
+                            _Utils_eq(interConfig.fX, $elm$core$Maybe$Nothing) ? $terezka$elm_charts$Chart$Attributes$circle : $elm$core$Basics$identity
                         ]);
                     var dotAttrs = _Utils_ap(
                         defaultAttrs,
                         _Utils_ap(
-                            prop.bv,
-                            A5(prop.d5, lineIndex, stackIndex, dataIndex, prop.es, datum_)));
+                            prop.bu,
+                            A5(prop.d4, lineIndex, stackIndex, dataIndex, prop.eu, datum_)));
                     var config = toDotConfig(dotAttrs);
                     return {
-                        fs: {
-                            f_: config,
-                            gh: $terezka$elm_charts$Internal$Item$Dot,
-                            cI: {
+                        fv: {
+                            f1: config,
+                            gk: $terezka$elm_charts$Internal$Item$Dot,
+                            cH: {
                                 v: config.v,
                                 x: config.x,
-                                bD: function() {
-                                    var _v6 = config.bD;
+                                bC: function() {
+                                    var _v6 = config.bC;
                                     if (_v6 === 'white') {
-                                        return interConfig.bD;
+                                        return interConfig.bC;
                                     } else {
-                                        return config.bD;
+                                        return config.bC;
                                     }
                                 }(),
-                                bH: dataIndex,
-                                fA: elIndex,
-                                d7: prop.F(datum_),
-                                fM: colorIndex,
-                                fW: prop.es,
-                                f$: lineIndex,
-                                f7: stackIndex
+                                bG: dataIndex,
+                                fD: elIndex,
+                                d6: prop.F(datum_),
+                                fP: colorIndex,
+                                fZ: prop.eu,
+                                f2: lineIndex,
+                                ga: stackIndex
                             },
-                            gs: {
-                                fx: datum_,
-                                fQ: function() {
-                                    var _v7 = prop.W(datum_);
+                            gv: {
+                                fA: datum_,
+                                fT: function() {
+                                    var _v7 = prop.Z(datum_);
                                     if (!_v7.$) {
                                         return true;
                                     } else {
                                         return false;
                                     }
                                 }(),
                                 aK: x_,
-                                bf: x_,
-                                fh: y_
+                                be: x_,
+                                fk: y_
                             }
                         },
-                        gi: function(c) {
+                        gl: function(c) {
                             return _List_fromArray(
                                 [
                                     A3(
                                         $terezka$elm_charts$Internal$Produce$tooltipRow,
-                                        c.cI.bD,
-                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cI.fW),
+                                        c.cH.bC,
+                                        A2($terezka$elm_charts$Internal$Produce$toDefaultName, colorIndex, c.cH.fZ),
                                         prop.F(datum_))
                                 ]);
                         },
-                        gj: function(_v8) {
+                        gm: function(_v8) {
                             return {
                                 aK: x_,
-                                bf: x_,
-                                gx: y_,
-                                dL: y_
+                                be: x_,
+                                gA: y_,
+                                dI: y_
                             };
                         },
-                        gm: F2(
+                        gp: F2(
                             function(plane, _v9) {
                                 var radius = A2(
                                     $elm$core$Maybe$withDefault,
                                     0,
                                     A2(
                                         $elm$core$Maybe$map,
-                                        $terezka$elm_charts$Internal$Svg$toRadius(config.eZ),
+                                        $terezka$elm_charts$Internal$Svg$toRadius(config.e1),
                                         config.aG));
                                 var radiusX_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianX, plane, radius);
                                 var radiusY_ = A2($terezka$elm_charts$Internal$Coordinates$scaleCartesianY, plane, radius);
                                 return {
                                     aK: x_ - radiusX_,
-                                    bf: x_ + radiusX_,
-                                    gx: y_ - radiusY_,
-                                    dL: y_ + radiusY_
+                                    be: x_ + radiusX_,
+                                    gA: y_ - radiusY_,
+                                    dI: y_ + radiusY_
                                 };
                             }),
-                        gn: F3(
+                        gq: F3(
                             function(plane, _v10, _v11) {
-                                var _v12 = prop.W(datum_);
+                                var _v12 = prop.Z(datum_);
                                 if (_v12.$ === 1) {
                                     return $elm$svg$Svg$text('');
                                 } else {
                                     return A5(
                                         $terezka$elm_charts$Internal$Svg$dot,
                                         plane,
                                         function($) {
-                                            return $.fg;
+                                            return $.fj;
                                         },
                                         function($) {
-                                            return $.fh;
+                                            return $.fk;
                                         },
                                         config, {
-                                            fg: x_,
-                                            fh: y_
+                                            fj: x_,
+                                            fk: y_
                                         });
                                 }
                             })
                     };
                 });
             var toSeriesItem = F5(
                 function(lineIndex, stacks, stackIndex, prop, colorIndex) {
@@ -12683,30 +12992,30 @@
                     var interAttr = _Utils_ap(
                         _List_fromArray(
                             [
                                 $terezka$elm_charts$Chart$Attributes$color(
                                     $terezka$elm_charts$Internal$Helpers$toDefaultColor(colorIndex)),
                                 $terezka$elm_charts$Chart$Attributes$opacity(defaultOpacity)
                             ]),
-                        prop.fO);
+                        prop.fR);
                     var interConfig = toInterConfig(interAttr);
                     var dotItems = A2(
                         $elm$core$List$indexedMap,
                         A5(toDotItem, lineIndex, stackIndex, colorIndex, prop, interConfig),
                         data);
                     if (!dotItems.b) {
                         return $elm$core$Maybe$Nothing;
                     } else {
                         var first = dotItems.a;
                         var rest = dotItems.b;
                         return $elm$core$Maybe$Just({
-                            fs: {
-                                el: _Utils_Tuple2(first, rest)
+                            fv: {
+                                ek: _Utils_Tuple2(first, rest)
                             },
-                            gi: function(c) {
+                            gl: function(c) {
                                 return _List_fromArray(
                                     [
                                         A2(
                                             $elm$html$Html$table,
                                             _List_fromArray(
                                                 [
                                                     A2($elm$html$Html$Attributes$style, 'margin', '0')
@@ -12714,67 +13023,67 @@
                                             A2(
                                                 $elm$core$List$concatMap,
                                                 $terezka$elm_charts$Internal$Item$toHtml,
                                                 function(_v1) {
                                                     var x = _v1.a;
                                                     var xs = _v1.b;
                                                     return A2($elm$core$List$cons, x, xs);
-                                                }(c.el)))
+                                                }(c.ek)))
                                     ]);
                             },
-                            gj: function(c) {
+                            gm: function(c) {
                                 return A2(
                                     $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                     $terezka$elm_charts$Internal$Item$getLimits,
                                     function(_v2) {
                                         var x = _v2.a;
                                         var xs = _v2.b;
                                         return A2($elm$core$List$cons, x, xs);
-                                    }(c.el));
+                                    }(c.ek));
                             },
-                            gm: F2(
+                            gp: F2(
                                 function(plane, c) {
                                     return A2(
                                         $terezka$elm_charts$Internal$Coordinates$foldPosition,
                                         $terezka$elm_charts$Internal$Item$getPosition(plane),
                                         function(_v3) {
                                             var x = _v3.a;
                                             var xs = _v3.b;
                                             return A2($elm$core$List$cons, x, xs);
-                                        }(c.el));
+                                        }(c.ek));
                                 }),
-                            gn: F3(
+                            gq: F3(
                                 function(plane, _v4, _v5) {
                                     var toBottom = function(datum_) {
                                         return A3(
                                             $elm$core$Maybe$map2,
                                             F2(
                                                 function(real, visual) {
                                                     return visual - real;
                                                 }),
-                                            prop.W(datum_),
-                                            prop.a8(datum_));
+                                            prop.Z(datum_),
+                                            prop.a7(datum_));
                                     };
                                     return A2(
                                         $elm$svg$Svg$g,
                                         _List_fromArray(
                                             [
                                                 $elm$svg$Svg$Attributes$class('elm-charts__series')
                                             ]),
                                         _List_fromArray(
                                             [
                                                 A6(
                                                     $terezka$elm_charts$Internal$Svg$area,
                                                     plane,
                                                     toX,
                                                     $elm$core$Maybe$Just(toBottom),
-                                                    prop.a8,
+                                                    prop.a7,
                                                     interConfig,
                                                     data),
-                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a8, interConfig, data),
+                                                A5($terezka$elm_charts$Internal$Svg$interpolation, plane, toX, prop.a7, interConfig, data),
                                                 A2(
                                                     $elm$svg$Svg$g,
                                                     _List_fromArray(
                                                         [
                                                             $elm$svg$Svg$Attributes$class('elm-charts__dots')
                                                         ]),
                                                     A2(
@@ -12847,118 +13156,118 @@
         function(toX, properties, data) {
             return A4($terezka$elm_charts$Chart$seriesMap, $elm$core$Basics$identity, toX, properties, data);
         });
     var $terezka$elm_charts$Chart$Attributes$spacing = F2(
         function(v, config) {
             return _Utils_update(
                 config, {
-                    f6: v
+                    f9: v
                 });
         });
     var $terezka$elm_charts$Chart$html = function(func) {
         return $terezka$elm_charts$Chart$HtmlElement(
             F2(
                 function(p, _v0) {
                     return func(p);
                 }));
     };
     var $terezka$elm_charts$Internal$Svg$defaultTooltip = {
-        aw: true,
-        fn: 'white',
+        ax: true,
+        fq: 'white',
         v: '#D8D8D8',
-        _: $elm$core$Maybe$Nothing,
-        fD: $elm$core$Maybe$Nothing,
-        eb: 0,
+        ac: $elm$core$Maybe$Nothing,
+        fG: $elm$core$Maybe$Nothing,
+        ea: 0,
         b: 8,
-        ff: 0
+        fi: 0
     };
     var $terezka$elm_charts$Internal$Svg$Bottom = 3;
     var $terezka$elm_charts$Internal$Svg$Left = 1;
     var $terezka$elm_charts$Internal$Svg$Right = 2;
     var $terezka$elm_charts$Internal$Svg$Top = 0;
     var $elm$core$List$all = F2(
         function(isOkay, list) {
             return !A2(
                 $elm$core$List$any,
                 A2($elm$core$Basics$composeL, $elm$core$Basics$not, isOkay),
                 list);
         });
     var $terezka$elm_charts$Internal$Coordinates$bottom = function(pos) {
         return {
-            fg: pos.aK + ((pos.bf - pos.aK) / 2),
-            fh: pos.gx
+            fj: pos.aK + ((pos.be - pos.aK) / 2),
+            fk: pos.gA
         };
     };
     var $terezka$elm_charts$Internal$Coordinates$left = function(pos) {
         return {
-            fg: pos.aK,
-            fh: pos.gx + ((pos.dL - pos.gx) / 2)
+            fj: pos.aK,
+            fk: pos.gA + ((pos.dI - pos.gA) / 2)
         };
     };
     var $elm$html$Html$map = $elm$virtual_dom$VirtualDom$map;
     var $terezka$elm_charts$Internal$Coordinates$right = function(pos) {
         return {
-            fg: pos.bf,
-            fh: pos.gx + ((pos.dL - pos.gx) / 2)
+            fj: pos.be,
+            fk: pos.gA + ((pos.dI - pos.gA) / 2)
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltipPointerStyle = F4(
         function(direction, className, background, borderColor) {
             var config = function() {
                 switch (direction) {
                     case 0:
                         return {
-                            af: 'right', K: 'top', S: 'left'
+                            aj: 'right', L: 'top', T: 'left'
                         };
                     case 3:
                         return {
-                            af: 'right', K: 'bottom', S: 'left'
+                            aj: 'right', L: 'bottom', T: 'left'
                         };
                     case 1:
                         return {
-                            af: 'bottom', K: 'left', S: 'top'
+                            aj: 'bottom', L: 'left', T: 'top'
                         };
                     case 2:
                         return {
-                            af: 'bottom', K: 'right', S: 'top'
+                            aj: 'bottom', L: 'right', T: 'top'
                         };
                     case 4:
                         return {
-                            af: 'bottom', K: 'left', S: 'top'
+                            aj: 'bottom', L: 'left', T: 'top'
                         };
                     default:
                         return {
-                            af: 'right', K: 'top', S: 'left'
+                            aj: 'right', L: 'top', T: 'left'
                         };
                 }
             }();
-            return '\n  .' + (className + (':before, .' + (className + (':after {\n    content: "";\n    position: absolute;\n    border-' + (config.S + (': 5px solid transparent;\n    border-' + (config.af + (': 5px solid transparent;\n    ' + (config.K + (': 100%;\n    ' + (config.S + (': 50%;\n    margin-' + (config.S + (': -5px;\n  }\n\n  .' + (className + (':after {\n    border-' + (config.K + (': 5px solid ' + (background + (';\n    margin-' + (config.K + (': -1px;\n    z-index: 1;\n    height: 0px;\n  }\n\n  .' + (className + (':before {\n    border-' + (config.K + (': 5px solid ' + (borderColor + ';\n    height: 0px;\n  }\n  ')))))))))))))))))))))))))));
+            return '\n  .' + (className + (':before, .' + (className + (':after {\n    content: "";\n    position: absolute;\n    border-' + (config.T + (': 5px solid transparent;\n    border-' + (config.aj + (': 5px solid transparent;\n    ' + (config.L + (': 100%;\n    ' + (config.T + (': 50%;\n    margin-' + (config.T + (': -5px;\n  }\n\n  .' + (className + (':after {\n    border-' + (config.L + (': 5px solid ' + (background + (';\n    margin-' + (config.L + (': -1px;\n    z-index: 1;\n    height: 0px;\n  }\n\n  .' + (className + (':before {\n    border-' + (config.L + (': 5px solid ' + (borderColor + ';\n    height: 0px;\n  }\n  ')))))))))))))))))))))))))));
         });
     var $terezka$elm_charts$Internal$Coordinates$top = function(pos) {
         return {
-            fg: pos.aK + ((pos.bf - pos.aK) / 2),
-            fh: pos.dL
+            fj: pos.aK + ((pos.be - pos.aK) / 2),
+            fk: pos.dI
         };
     };
     var $terezka$elm_charts$Internal$Svg$tooltip = F5(
         function(plane, pos, config, htmlAttrs, content) {
-            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dL);
-            var distanceRight = plane.fg.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aK);
-            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.bf);
-            var distanceBottom = plane.fh.N - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gx);
+            var distanceTop = A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.dI);
+            var distanceRight = plane.fj.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.aK);
+            var distanceLeft = A2($terezka$elm_charts$Internal$Coordinates$toSVGX, plane, pos.be);
+            var distanceBottom = plane.fk.O - A2($terezka$elm_charts$Internal$Coordinates$toSVGY, plane, pos.gA);
             var direction = function() {
-                var _v5 = config._;
+                var _v5 = config.ac;
                 if (!_v5.$) {
                     switch (_v5.a) {
                         case 4:
                             var _v6 = _v5.a;
-                            return (config.ff > 0) ? ((_Utils_cmp(distanceLeft, config.ff + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
+                            return (config.fi > 0) ? ((_Utils_cmp(distanceLeft, config.fi + config.b) > 0) ? 1 : 2) : ((_Utils_cmp(distanceLeft, distanceRight) > 0) ? 1 : 2);
                         case 5:
                             var _v7 = _v5.a;
-                            return (config.eb > 0) ? ((_Utils_cmp(distanceTop, config.eb + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
+                            return (config.ea > 0) ? ((_Utils_cmp(distanceTop, config.ea + config.b) > 0) ? 0 : 3) : ((_Utils_cmp(distanceTop, distanceBottom) > 0) ? 0 : 3);
                         default:
                             var dir = _v5.a;
                             return dir;
                     }
                 } else {
                     var isLargest = function(a) {
                         return $elm$core$List$all(
@@ -12978,15 +13287,15 @@
                         isLargest,
                         distanceLeft,
                         _List_fromArray(
                             [distanceTop, distanceBottom, distanceRight])) ? 1 : 2));
                 }
             }();
             var focalPoint = function() {
-                var _v2 = config.fD;
+                var _v2 = config.fG;
                 if (!_v2.$) {
                     var focal = _v2.a;
                     switch (direction) {
                         case 0:
                             return $terezka$elm_charts$Internal$Coordinates$top(
                                 focal(pos));
                         case 3:
@@ -13018,75 +13327,75 @@
                         case 4:
                             return $terezka$elm_charts$Internal$Coordinates$left(pos);
                         default:
                             return $terezka$elm_charts$Internal$Coordinates$right(pos);
                     }
                 }
             }();
-            var arrowWidth = config.aw ? 4 : 0;
+            var arrowWidth = config.ax ? 4 : 0;
             var _v0 = function() {
                 switch (direction) {
                     case 0:
                         return {
-                            ag: 'elm-charts__tooltip-top', ar: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
+                            ak: 'elm-charts__tooltip-top', as: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
                         };
                     case 3:
                         return {
-                            ag: 'elm-charts__tooltip-bottom', ar: 'translate(-50%, 0%)', g: 0, h: (-config.b) - arrowWidth
+                            ak: 'elm-charts__tooltip-bottom', as: 'translate(-50%, 0%)', g: 0, h: (-config.b) - arrowWidth
                         };
                     case 1:
                         return {
-                            ag: 'elm-charts__tooltip-left', ar: 'translate(-100%, -50%)', g: (-config.b) - arrowWidth, h: 0
+                            ak: 'elm-charts__tooltip-left', as: 'translate(-100%, -50%)', g: (-config.b) - arrowWidth, h: 0
                         };
                     case 2:
                         return {
-                            ag: 'elm-charts__tooltip-right', ar: 'translate(0, -50%)', g: config.b + arrowWidth, h: 0
+                            ak: 'elm-charts__tooltip-right', as: 'translate(0, -50%)', g: config.b + arrowWidth, h: 0
                         };
                     case 4:
                         return {
-                            ag: 'elm-charts__tooltip-leftOrRight', ar: 'translate(0, -50%)', g: (-config.b) - arrowWidth, h: 0
+                            ak: 'elm-charts__tooltip-leftOrRight', as: 'translate(0, -50%)', g: (-config.b) - arrowWidth, h: 0
                         };
                     default:
                         return {
-                            ag: 'elm-charts__tooltip-topOrBottom', ar: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
+                            ak: 'elm-charts__tooltip-topOrBottom', as: 'translate(-50%, -100%)', g: 0, h: config.b + arrowWidth
                         };
                 }
             }();
             var xOff = _v0.g;
             var yOff = _v0.h;
-            var transformation = _v0.ar;
-            var className = _v0.ag;
-            var children = config.aw ? A2(
+            var transformation = _v0.as;
+            var className = _v0.ak;
+            var children = config.ax ? A2(
                 $elm$core$List$cons,
                 A3(
                     $elm$html$Html$node,
                     'style',
                     _List_Nil,
                     _List_fromArray(
                         [
                             $elm$html$Html$text(
-                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.fn, config.v))
+                                A4($terezka$elm_charts$Internal$Svg$tooltipPointerStyle, direction, className, config.fq, config.v))
                         ])),
                 content) : content;
             var attributes = _Utils_ap(
                 _List_fromArray(
                     [
                         $elm$html$Html$Attributes$class(className),
                         A2($elm$html$Html$Attributes$style, 'transform', transformation),
                         A2($elm$html$Html$Attributes$style, 'padding', '5px 8px'),
-                        A2($elm$html$Html$Attributes$style, 'background', config.fn),
+                        A2($elm$html$Html$Attributes$style, 'background', config.fq),
                         A2($elm$html$Html$Attributes$style, 'border', '1px solid ' + config.v),
                         A2($elm$html$Html$Attributes$style, 'border-radius', '3px'),
                         A2($elm$html$Html$Attributes$style, 'pointer-events', 'none')
                     ]),
                 htmlAttrs);
             return A2(
                 $elm$html$Html$map,
                 $elm$core$Basics$never,
-                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.fg, focalPoint.fh, xOff, yOff, attributes, children));
+                A7($terezka$elm_charts$Internal$Svg$positionHtml, plane, focalPoint.fj, focalPoint.fk, xOff, yOff, attributes, children));
         });
     var $terezka$elm_charts$Chart$Svg$tooltip = F3(
         function(plane, pos, edits) {
             return A3(
                 $terezka$elm_charts$Internal$Svg$tooltip,
                 plane,
                 pos,
@@ -13094,15 +13403,15 @@
         });
     var $terezka$elm_charts$Chart$tooltip = F4(
         function(i, edits, attrs_, content) {
             return $terezka$elm_charts$Chart$html(
                 function(p) {
                     var pos = $terezka$elm_charts$Internal$Item$getLimits(i);
                     var content_ = _Utils_eq(content, _List_Nil) ? $terezka$elm_charts$Internal$Item$toHtml(i) : content;
-                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aK, pos.dL) ? A5(
+                    return A3($terezka$elm_charts$Internal$Svg$isWithinPlane, p, pos.aK, pos.dI) ? A5(
                         $terezka$elm_charts$Chart$Svg$tooltip,
                         p,
                         A2($terezka$elm_charts$Internal$Item$getPosition, p, i),
                         edits,
                         attrs_,
                         content_) : $elm$html$Html$text('');
                 });
@@ -13123,18 +13432,18 @@
                 a: a,
                 b: b,
                 c: c
             };
         });
     var $terezka$elm_charts$Internal$Svg$defaultLabel = {
         i: $elm$core$Maybe$Nothing,
-        bv: _List_Nil,
+        bu: _List_Nil,
         v: 'white',
         x: 0,
-        bD: '#808BAB',
+        bC: '#808BAB',
         j: $elm$core$Maybe$Nothing,
         k: $elm$core$Maybe$Nothing,
         l: false,
         o: 0,
         p: false,
         g: 0,
         h: 0
@@ -13493,15 +13802,15 @@
     var $terezka$intervals$Intervals$positions = F5(
         function(range, beginning, interval, m, acc) {
             positions: while (true) {
                 var nextPosition = A2(
                     $terezka$intervals$Intervals$correctFloat,
                     $terezka$intervals$Intervals$getPrecision(interval),
                     beginning + (m * interval));
-                if (_Utils_cmp(nextPosition, range.er) > 0) {
+                if (_Utils_cmp(nextPosition, range.et) > 0) {
                     return acc;
                 } else {
                     var $temp$range = range,
                         $temp$beginning = beginning,
                         $temp$interval = interval,
                         $temp$m = m + 1,
                         $temp$acc = _Utils_ap(
@@ -13515,18 +13824,18 @@
                     acc = $temp$acc;
                     continue positions;
                 }
             }
         });
     var $terezka$intervals$Intervals$values = F4(
         function(allowDecimals, exact, amountRough, range) {
-            var intervalRough = (range.er - range.et) / amountRough;
+            var intervalRough = (range.et - range.ev) / amountRough;
             var interval = A3($terezka$intervals$Intervals$getInterval, intervalRough, allowDecimals, exact);
             var intervalSafe = (!interval) ? 1 : interval;
-            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.et, intervalSafe);
+            var beginning = A2($terezka$intervals$Intervals$getBeginning, range.ev, intervalSafe);
             var amountRoughSafe = (!amountRough) ? 1 : amountRough;
             return A5($terezka$intervals$Intervals$positions, range, beginning, intervalSafe, 0, _List_Nil);
         });
     var $terezka$intervals$Intervals$floats = function(amount) {
         if (!amount.$) {
             var number = amount.a;
             return A3($terezka$intervals$Intervals$values, true, true, number);
@@ -13536,28 +13845,28 @@
         }
     };
     var $terezka$elm_charts$Internal$Svg$floats = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$floats,
                 $terezka$intervals$Intervals$around(i), {
-                    er: b.er,
-                    et: b.et
+                    et: b.et,
+                    ev: b.ev
                 });
         });
     var $terezka$elm_charts$Chart$Svg$floats = $terezka$elm_charts$Internal$Svg$floats;
     var $ryannhg$date_format$DateFormat$Language$Language = F6(
         function(toMonthName, toMonthAbbreviation, toWeekdayName, toWeekdayAbbreviation, toAmPm, toOrdinalSuffix) {
             return {
-                gg: toAmPm,
-                gk: toMonthAbbreviation,
-                gl: toMonthName,
+                gj: toAmPm,
+                gn: toMonthAbbreviation,
+                go: toMonthName,
                 aI: toOrdinalSuffix,
-                go: toWeekdayAbbreviation,
-                gp: toWeekdayName
+                gr: toWeekdayAbbreviation,
+                gs: toWeekdayName
             };
         });
     var $ryannhg$date_format$DateFormat$Language$toEnglishAmPm = function(hour) {
         return (hour > 11) ? 'pm' : 'am';
     };
     var $ryannhg$date_format$DateFormat$Language$toEnglishMonthName = function(month) {
         switch (month) {
@@ -13640,15 +13949,15 @@
             $elm$core$Basics$composeR,
             $ryannhg$date_format$DateFormat$Language$toEnglishWeekdayName,
             $elm$core$String$left(3)),
         $ryannhg$date_format$DateFormat$Language$toEnglishAmPm,
         $ryannhg$date_format$DateFormat$Language$toEnglishSuffix);
     var $ryannhg$date_format$DateFormat$amPm = F3(
         function(language, zone, posix) {
-            return language.gg(
+            return language.gj(
                 A2($elm$time$Time$toHour, zone, posix));
         });
     var $ryannhg$date_format$DateFormat$dayOfMonth = $elm$time$Time$toDay;
     var $elm$time$Time$Sun = 6;
     var $elm$time$Time$Fri = 4;
     var $elm$time$Time$Mon = 0;
     var $elm$time$Time$Sat = 5;
@@ -13988,18 +14297,18 @@
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 2:
                     return A2(
                         $ryannhg$date_format$DateFormat$toFixedLength,
                         2,
                         A2($ryannhg$date_format$DateFormat$monthNumber_, zone, posix));
                 case 3:
-                    return language.gk(
+                    return language.gn(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 4:
-                    return language.gl(
+                    return language.go(
                         A2($elm$time$Time$toMonth, zone, posix));
                 case 17:
                     return $elm$core$String$fromInt(
                         1 + A2($ryannhg$date_format$DateFormat$quarter, zone, posix));
                 case 18:
                     return function(num) {
                         return _Utils_ap(
@@ -14044,18 +14353,18 @@
                     return function(num) {
                         return _Utils_ap(
                             $elm$core$String$fromInt(num),
                             language.aI(num));
                     }(
                         A2($ryannhg$date_format$DateFormat$dayOfWeek, zone, posix));
                 case 13:
-                    return language.go(
+                    return language.gr(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 14:
-                    return language.gp(
+                    return language.gs(
                         A2($elm$time$Time$toWeekday, zone, posix));
                 case 19:
                     return $elm$core$String$fromInt(
                         A2($ryannhg$date_format$DateFormat$weekOfYear, zone, posix));
                 case 20:
                     return function(num) {
                         return _Utils_ap(
@@ -14231,30 +14540,30 @@
     };
     var $ryannhg$date_format$DateFormat$yearNumber = $ryannhg$date_format$DateFormat$YearNumber;
     var $terezka$elm_charts$Internal$Svg$formatYear = $ryannhg$date_format$DateFormat$format(
         _List_fromArray(
             [$ryannhg$date_format$DateFormat$yearNumber]));
     var $terezka$elm_charts$Internal$Svg$formatTime = F2(
         function(zone, time) {
-            var _v0 = A2($elm$core$Maybe$withDefault, time.gq, time.fr);
+            var _v0 = A2($elm$core$Maybe$withDefault, time.gt, time.fu);
             switch (_v0) {
                 case 0:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockMillis, zone, time.gh);
                 case 1:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClockSecond, zone, time.gh);
                 case 2:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gh);
                 case 3:
-                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatClock, zone, time.gh);
                 case 4:
-                    return (time.fV === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.ge) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.ge);
+                    return (time.fY === 7) ? A2($terezka$elm_charts$Internal$Svg$formatWeekday, zone, time.gh) : A2($terezka$elm_charts$Internal$Svg$formatDate, zone, time.gh);
                 case 5:
-                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatMonth, zone, time.gh);
                 default:
-                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.ge);
+                    return A2($terezka$elm_charts$Internal$Svg$formatYear, zone, time.gh);
             }
         });
     var $terezka$elm_charts$Chart$Svg$formatTime = $terezka$elm_charts$Internal$Svg$formatTime;
     var $terezka$elm_charts$Internal$Svg$generate = F3(
         function(amount, _v0, limits) {
             var func = _v0;
             return A2(func, amount, limits);
@@ -14276,16 +14585,16 @@
                 }());
         });
     var $terezka$elm_charts$Internal$Svg$ints = F2(
         function(i, b) {
             return A2(
                 $terezka$intervals$Intervals$ints,
                 $terezka$intervals$Intervals$around(i), {
-                    er: b.er,
-                    et: b.et
+                    et: b.et,
+                    ev: b.ev
                 });
         });
     var $terezka$elm_charts$Chart$Svg$ints = $terezka$elm_charts$Internal$Svg$ints;
     var $terezka$intervals$Intervals$Day = 4;
     var $terezka$intervals$Intervals$Hour = 3;
     var $terezka$intervals$Intervals$Millisecond = 0;
     var $terezka$intervals$Intervals$Minute = 2;
@@ -14437,17 +14746,17 @@
                         $temp$d = d - monthDays;
                     y = $temp$y;
                     m = $temp$m;
                     d = $temp$d;
                     continue toCalendarDateHelp;
                 } else {
                     return {
-                        dY: d,
-                        ev: m,
-                        fi: y
+                        dW: d,
+                        ex: m,
+                        fl: y
                     };
                 }
             }
         });
     var $justinmimbs$date$Date$divWithRemainder = F2(
         function(a, b) {
             return _Utils_Tuple2(
@@ -14471,38 +14780,38 @@
         var n = (!r1) ? 0 : 1;
         return ((((n400 * 400) + (n100 * 100)) + (n4 * 4)) + n1) + n;
     };
     var $justinmimbs$date$Date$toOrdinalDate = function(_v0) {
         var rd = _v0;
         var y = $justinmimbs$date$Date$year(rd);
         return {
-            dk: rd - $justinmimbs$date$Date$daysBeforeYear(y),
-            fi: y
+            di: rd - $justinmimbs$date$Date$daysBeforeYear(y),
+            fl: y
         };
     };
     var $justinmimbs$date$Date$toCalendarDate = function(_v0) {
         var rd = _v0;
         var date = $justinmimbs$date$Date$toOrdinalDate(rd);
-        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.fi, 0, date.dk);
+        return A3($justinmimbs$date$Date$toCalendarDateHelp, date.fl, 0, date.di);
     };
     var $justinmimbs$date$Date$add = F3(
         function(unit, n, _v0) {
             var rd = _v0;
             switch (unit) {
                 case 0:
                     return A3($justinmimbs$date$Date$add, 1, 12 * n, rd);
                 case 1:
                     var date = $justinmimbs$date$Date$toCalendarDate(rd);
-                    var wholeMonths = ((12 * (date.fi - 1)) + ($justinmimbs$date$Date$monthToNumber(date.ev) - 1)) + n;
+                    var wholeMonths = ((12 * (date.fl - 1)) + ($justinmimbs$date$Date$monthToNumber(date.ex) - 1)) + n;
                     var m = $justinmimbs$date$Date$numberToMonth(
                         A2($elm$core$Basics$modBy, 12, wholeMonths) + 1);
                     var y = A2($justinmimbs$date$Date$floorDiv, wholeMonths, 12) + 1;
                     return ($justinmimbs$date$Date$daysBeforeYear(y) + A2($justinmimbs$date$Date$daysBeforeMonth, y, m)) + A2(
                         $elm$core$Basics$min,
-                        date.dY,
+                        date.dW,
                         A2($justinmimbs$date$Date$daysInMonth, y, m));
                 case 2:
                     return rd + (7 * n);
                 default:
                     return rd + n;
             }
         });
@@ -14723,15 +15032,15 @@
     var $justinmimbs$date$Date$firstOfYear = function(y) {
         return $justinmimbs$date$Date$daysBeforeYear(y) + 1;
     };
     var $justinmimbs$date$Date$month = A2(
         $elm$core$Basics$composeR,
         $justinmimbs$date$Date$toCalendarDate,
         function($) {
-            return $.ev;
+            return $.ex;
         });
     var $justinmimbs$date$Date$monthToQuarter = function(m) {
         return (($justinmimbs$date$Date$monthToNumber(m) + 2) / 3) | 0;
     };
     var $justinmimbs$date$Date$quarter = A2($elm$core$Basics$composeR, $justinmimbs$date$Date$month, $justinmimbs$date$Date$monthToQuarter);
     var $justinmimbs$date$Date$quarterToMonth = function(q) {
         return $justinmimbs$date$Date$numberToMonth((q * 3) - 2);
@@ -14857,62 +15166,62 @@
     var $terezka$intervals$Intervals$Time$ceilingDay = F3(
         function(zone, mult, stamp) {
             return (mult === 7) ? A3($justinmimbs$time_extra$Time$Extra$ceiling, 3, zone, stamp) : A3($justinmimbs$time_extra$Time$Extra$ceiling, 11, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Hour = 12;
     var $justinmimbs$time_extra$Time$Extra$partsToPosix = F2(
         function(zone, _v0) {
-            var year = _v0.fi;
-            var month = _v0.ev;
-            var day = _v0.dY;
-            var hour = _v0.c2;
-            var minute = _v0.df;
-            var second = _v0.dv;
-            var millisecond = _v0.de;
+            var year = _v0.fl;
+            var month = _v0.ex;
+            var day = _v0.dW;
+            var hour = _v0.c0;
+            var minute = _v0.dd;
+            var second = _v0.dr;
+            var millisecond = _v0.dc;
             return A3(
                 $justinmimbs$time_extra$Time$Extra$posixFromDateTime,
                 zone,
                 A3($justinmimbs$date$Date$fromCalendarDate, year, month, day),
                 A4(
                     $justinmimbs$time_extra$Time$Extra$timeFromClock,
                     A3($elm$core$Basics$clamp, 0, 23, hour),
                     A3($elm$core$Basics$clamp, 0, 59, minute),
                     A3($elm$core$Basics$clamp, 0, 59, second),
                     A3($elm$core$Basics$clamp, 0, 999, millisecond)));
         });
     var $justinmimbs$time_extra$Time$Extra$posixToParts = F2(
         function(zone, posix) {
             return {
-                dY: A2($elm$time$Time$toDay, zone, posix),
-                c2: A2($elm$time$Time$toHour, zone, posix),
-                de: A2($elm$time$Time$toMillis, zone, posix),
-                df: A2($elm$time$Time$toMinute, zone, posix),
-                ev: A2($elm$time$Time$toMonth, zone, posix),
-                dv: A2($elm$time$Time$toSecond, zone, posix),
-                fi: A2($elm$time$Time$toYear, zone, posix)
+                dW: A2($elm$time$Time$toDay, zone, posix),
+                c0: A2($elm$time$Time$toHour, zone, posix),
+                dc: A2($elm$time$Time$toMillis, zone, posix),
+                dd: A2($elm$time$Time$toMinute, zone, posix),
+                ex: A2($elm$time$Time$toMonth, zone, posix),
+                dr: A2($elm$time$Time$toSecond, zone, posix),
+                fl: A2($elm$time$Time$toYear, zone, posix)
             };
         });
     var $terezka$intervals$Intervals$Time$ceilingHour = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 12, zone, stamp));
-            var rem = parts.c2 % mult;
+            var rem = parts.c0 % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 12, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Minute = 13;
     var $terezka$intervals$Intervals$Time$ceilingMinute = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 13, zone, stamp));
-            var rem = parts.df % mult;
+            var rem = parts.dd % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 13, mult - rem, zone, _new);
         });
     var $terezka$intervals$Intervals$Time$intAsMonth = function(_int) {
         switch (_int) {
             case 1:
                 return 0;
@@ -14972,61 +15281,61 @@
     };
     var $terezka$intervals$Intervals$Time$ceilingMonth = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 2, zone, stamp));
-            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.ev);
+            var monthInt = $terezka$intervals$Intervals$Time$monthAsInt(parts.ex);
             var rem = (monthInt - 1) % mult;
             var newMonth = (!rem) ? monthInt : ((monthInt - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 (newMonth > 12) ? _Utils_update(
                     parts, {
-                        ev: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
-                        fi: parts.fi + 1
+                        ex: $terezka$intervals$Intervals$Time$intAsMonth(newMonth - 12),
+                        fl: parts.fl + 1
                     }) : _Utils_update(
                     parts, {
-                        ev: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
+                        ex: $terezka$intervals$Intervals$Time$intAsMonth(newMonth)
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingMs = F3(
         function(zone, mult, stamp) {
             var parts = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, stamp);
-            var rem = parts.de % mult;
+            var rem = parts.dc % mult;
             return (!rem) ? A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts) : A4($justinmimbs$time_extra$Time$Extra$add, 15, mult - rem, zone, stamp);
         });
     var $justinmimbs$time_extra$Time$Extra$Second = 14;
     var $terezka$intervals$Intervals$Time$ceilingSecond = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 14, zone, stamp));
-            var rem = parts.dv % mult;
+            var rem = parts.dr % mult;
             var _new = A2($justinmimbs$time_extra$Time$Extra$partsToPosix, zone, parts);
             return (!rem) ? _new : A4($justinmimbs$time_extra$Time$Extra$add, 14, mult - rem, zone, _new);
         });
     var $justinmimbs$time_extra$Time$Extra$Year = 0;
     var $terezka$intervals$Intervals$Time$ceilingYear = F3(
         function(zone, mult, stamp) {
             var parts = A2(
                 $justinmimbs$time_extra$Time$Extra$posixToParts,
                 zone,
                 A3($justinmimbs$time_extra$Time$Extra$ceiling, 0, zone, stamp));
-            var rem = parts.fi % mult;
-            var newYear = (!rem) ? parts.fi : ((parts.fi - rem) + mult);
+            var rem = parts.fl % mult;
+            var newYear = (!rem) ? parts.fl : ((parts.fl - rem) + mult);
             return A2(
                 $justinmimbs$time_extra$Time$Extra$partsToPosix,
                 zone,
                 _Utils_update(
                     parts, {
-                        fi: newYear
+                        fl: newYear
                     }));
         });
     var $terezka$intervals$Intervals$Time$ceilingUnit = F3(
         function(zone, unit, mult) {
             switch (unit) {
                 case 0:
                     return A2($terezka$intervals$Intervals$Time$ceilingMs, zone, mult);
@@ -15051,15 +15360,15 @@
     var $terezka$intervals$Intervals$Time$Month = 5;
     var $terezka$intervals$Intervals$Time$Second = 1;
     var $terezka$intervals$Intervals$Time$Year = 6;
     var $terezka$intervals$Intervals$Time$getChange = F3(
         function(zone, a, b) {
             var bP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b);
             var aP = A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a);
-            return (!_Utils_eq(aP.fi, bP.fi)) ? 6 : ((!_Utils_eq(aP.ev, bP.ev)) ? 5 : ((!_Utils_eq(aP.dY, bP.dY)) ? 4 : ((!_Utils_eq(aP.c2, bP.c2)) ? 3 : ((!_Utils_eq(aP.df, bP.df)) ? 2 : ((!_Utils_eq(aP.dv, bP.dv)) ? 1 : 0)))));
+            return (!_Utils_eq(aP.fl, bP.fl)) ? 6 : ((!_Utils_eq(aP.ex, bP.ex)) ? 5 : ((!_Utils_eq(aP.dW, bP.dW)) ? 4 : ((!_Utils_eq(aP.c0, bP.c0)) ? 3 : ((!_Utils_eq(aP.dd, bP.dd)) ? 2 : ((!_Utils_eq(aP.dr, bP.dr)) ? 1 : 0)))));
         });
     var $danhandrea$elm_time_extra$Util$isLeapYear = function(year) {
         return (!A2($elm$core$Basics$modBy, 400, year)) || ((!(!A2($elm$core$Basics$modBy, 100, year))) && (!A2($elm$core$Basics$modBy, 4, year)));
     };
     var $danhandrea$elm_time_extra$Month$days = F2(
         function(year, month) {
             switch (month) {
@@ -15098,36 +15407,36 @@
                 $terezka$intervals$Intervals$Time$toMs(b)) < 0) ? _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b)) : _Utils_Tuple2(
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, b),
                 A2($justinmimbs$time_extra$Time$Extra$posixToParts, zone, a));
             var aP = _v0.a;
             var bP = _v0.b;
-            var dMsX = bP.de - aP.de;
+            var dMsX = bP.dc - aP.dc;
             var dMs = (dMsX < 0) ? (1000 + dMsX) : dMsX;
-            var dSecondX = (bP.dv - aP.dv) + ((dMsX < 0) ? (-1) : 0);
-            var dMinuteX = (bP.df - aP.df) + ((dSecondX < 0) ? (-1) : 0);
-            var dHourX = (bP.c2 - aP.c2) + ((dMinuteX < 0) ? (-1) : 0);
-            var dDayX = (bP.dY - aP.dY) + ((dHourX < 0) ? (-1) : 0);
-            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.fi, bP.ev) + dDayX) : dDayX;
-            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.ev) - $terezka$intervals$Intervals$Time$monthAsInt(aP.ev)) + ((dDayX < 0) ? (-1) : 0);
+            var dSecondX = (bP.dr - aP.dr) + ((dMsX < 0) ? (-1) : 0);
+            var dMinuteX = (bP.dd - aP.dd) + ((dSecondX < 0) ? (-1) : 0);
+            var dHourX = (bP.c0 - aP.c0) + ((dMinuteX < 0) ? (-1) : 0);
+            var dDayX = (bP.dW - aP.dW) + ((dHourX < 0) ? (-1) : 0);
+            var dDay = (dDayX < 0) ? (A2($danhandrea$elm_time_extra$TimeExtra$daysInMonth, bP.fl, bP.ex) + dDayX) : dDayX;
+            var dMonthX = ($terezka$intervals$Intervals$Time$monthAsInt(bP.ex) - $terezka$intervals$Intervals$Time$monthAsInt(aP.ex)) + ((dDayX < 0) ? (-1) : 0);
             var dMonth = (dMonthX < 0) ? (12 + dMonthX) : dMonthX;
             var dHour = (dHourX < 0) ? (24 + dHourX) : dHourX;
             var dMinute = (dMinuteX < 0) ? (60 + dMinuteX) : dMinuteX;
             var dSecond = (dSecondX < 0) ? (60 + dSecondX) : dSecondX;
-            var dYearX = (bP.fi - aP.fi) + ((dMonthX < 0) ? (-1) : 0);
-            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.ev) + dYearX) : dYearX;
+            var dYearX = (bP.fl - aP.fl) + ((dMonthX < 0) ? (-1) : 0);
+            var dYear = (dYearX < 0) ? ($terezka$intervals$Intervals$Time$monthAsInt(bP.ex) + dYearX) : dYearX;
             return {
-                dY: dDay,
-                c2: dHour,
-                de: dMs,
-                df: dMinute,
-                ev: dMonth,
-                dv: dSecond,
-                fi: dYear
+                dW: dDay,
+                c0: dHour,
+                dc: dMs,
+                dd: dMinute,
+                ex: dMonth,
+                dr: dSecond,
+                fl: dYear
             };
         });
     var $terezka$intervals$Intervals$Time$oneSecond = 1000;
     var $terezka$intervals$Intervals$Time$oneMinute = $terezka$intervals$Intervals$Time$oneSecond * 60;
     var $terezka$intervals$Intervals$Time$oneHour = $terezka$intervals$Intervals$Time$oneMinute * 60;
     var $terezka$intervals$Intervals$Time$oneDay = $terezka$intervals$Intervals$Time$oneHour * 24;
     var $terezka$intervals$Intervals$Time$oneMs = 1;
@@ -15169,20 +15478,20 @@
                 case 3:
                     return timeDiff($terezka$intervals$Intervals$Time$oneHour) + 1;
                 case 4:
                     return timeDiff($terezka$intervals$Intervals$Time$oneDay) + 1;
                 case 5:
                     return diff(
                         function(d) {
-                            return d.ev + (d.fi * 12);
+                            return d.ex + (d.fl * 12);
                         }) + 1;
                 default:
                     return diff(
                         function($) {
-                            return $.fi;
+                            return $.fl;
                         }) + 1;
             }
         });
     var $terezka$intervals$Intervals$Time$largerUnit = function(unit) {
         switch (unit) {
             case 0:
                 return $elm$core$Maybe$Just(1);
@@ -15304,22 +15613,22 @@
             var mult = _v0.b;
             var amount = A5($terezka$intervals$Intervals$Time$getNumOfTicks, zone, unit, mult, min, max);
             var initial = A4($terezka$intervals$Intervals$Time$ceilingUnit, zone, unit, mult, min);
             var tUnit = $terezka$intervals$Intervals$Time$toExtraUnit(unit);
             var toTick = F3(
                 function(x, timestamp, change) {
                     return {
-                        fr: (_Utils_cmp(
+                        fu: (_Utils_cmp(
                             $terezka$intervals$Intervals$Time$unitToInt(change),
                             $terezka$intervals$Intervals$Time$unitToInt(unit)) > 0) ? $elm$core$Maybe$Just(change) : $elm$core$Maybe$Nothing,
-                        dc: !x,
-                        fV: mult,
-                        ge: timestamp,
-                        gq: unit,
-                        dM: zone
+                        da: !x,
+                        fY: mult,
+                        gh: timestamp,
+                        gt: unit,
+                        dJ: zone
                     };
                 });
             var toTicks = F2(
                 function(xs, acc) {
                     toTicks: while (true) {
                         if (xs.b) {
                             var x = xs.a;
@@ -15364,66 +15673,66 @@
                         return 5;
                     default:
                         return 6;
                 }
             };
             var translateUnit = function(time) {
                 return {
-                    fr: A2($elm$core$Maybe$map, toUnit, time.fr),
-                    dc: time.dc,
-                    fV: time.fV,
-                    ge: time.ge,
-                    gq: toUnit(time.gq),
-                    dM: time.dM
+                    fu: A2($elm$core$Maybe$map, toUnit, time.fu),
+                    da: time.da,
+                    fY: time.fY,
+                    gh: time.gh,
+                    gt: toUnit(time.gt),
+                    dJ: time.dJ
                 };
             };
             var fromMs = function(ts) {
                 return $elm$time$Time$millisToPosix(
                     $elm$core$Basics$round(ts));
             };
             return A2(
                 $elm$core$List$map,
                 translateUnit,
                 A4(
                     $terezka$intervals$Intervals$Time$values,
                     zone,
                     amount,
-                    fromMs(range.et),
-                    fromMs(range.er)));
+                    fromMs(range.ev),
+                    fromMs(range.et)));
         });
     var $terezka$elm_charts$Internal$Svg$times = function(zone) {
         return F2(
             function(i, b) {
                 return A3(
                     $terezka$intervals$Intervals$times,
                     zone,
                     i, {
-                        er: b.er,
-                        et: b.et
+                        et: b.et,
+                        ev: b.ev
                     });
             });
     };
     var $terezka$elm_charts$Chart$Svg$times = $terezka$elm_charts$Internal$Svg$times;
     var $terezka$elm_charts$Chart$generateValues = F4(
         function(amount, tick, maybeFormat, axis) {
             var toTickValues = F2(
                 function(toValue, toString) {
                     return $elm$core$List$map(
                         function(i) {
                             return {
-                                en: function() {
+                                em: function() {
                                     if (!maybeFormat.$) {
                                         var formatter = maybeFormat.a;
                                         return formatter(
                                             toValue(i));
                                     } else {
                                         return toString(i);
                                     }
                                 }(),
-                                W: toValue(i)
+                                Z: toValue(i)
                             };
                         });
                 });
             switch (tick.$) {
                 case 0:
                     return A3(
                         toTickValues,
@@ -15440,15 +15749,15 @@
                     var zone = tick.a;
                     return A3(
                         toTickValues,
                         A2(
                             $elm$core$Basics$composeL,
                             A2($elm$core$Basics$composeL, $elm$core$Basics$toFloat, $elm$time$Time$posixToMillis),
                             function($) {
-                                return $.ge;
+                                return $.gh;
                             }),
                         $terezka$elm_charts$Chart$Svg$formatTime(zone),
                         A3(
                             $terezka$elm_charts$Chart$Svg$generate,
                             amount,
                             $terezka$elm_charts$Chart$Svg$times(zone),
                             axis));
@@ -15513,24 +15822,24 @@
                                 return 'text-anchor: middle;';
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bv,
+                        config.bu,
                         $elm$svg$Svg$text_,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$stroke(config.v),
                                 $elm$svg$Svg$Attributes$strokeWidth(
                                     $elm$core$String$fromFloat(config.x)),
-                                $elm$svg$Svg$Attributes$fill(config.bD),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fg, point.fh, config.g, config.h),
+                                $elm$svg$Svg$Attributes$fill(config.bC),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fj, point.fk, config.g, config.h),
                                 $elm$svg$Svg$Attributes$style(
                                     A2(
                                         $elm$core$String$join,
                                         ' ',
                                         _List_fromArray(
                                             ['pointer-events: none;', fontStyle, anchorStyle, uppercaseStyle])))
                             ]),
@@ -15539,26 +15848,26 @@
                                 A2($elm$svg$Svg$tspan, _List_Nil, inner)
                             ])));
             } else {
                 var ellipsis = _v0.a;
                 var xOffWithAnchor = function() {
                     var _v11 = config.i;
                     if (_v11.$ === 1) {
-                        return config.g - (ellipsis.ff / 2);
+                        return config.g - (ellipsis.fi / 2);
                     } else {
                         switch (_v11.a) {
                             case 0:
                                 var _v12 = _v11.a;
-                                return config.g - ellipsis.ff;
+                                return config.g - ellipsis.fi;
                             case 1:
                                 var _v13 = _v11.a;
                                 return config.g;
                             default:
                                 var _v14 = _v11.a;
-                                return config.g - (ellipsis.ff / 2);
+                                return config.g - (ellipsis.fi / 2);
                         }
                     }
                 }();
                 var withOverflowWrap = function(el) {
                     return config.l ? A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
@@ -15598,94 +15907,94 @@
                                 return A2($elm$html$Html$Attributes$style, 'text-align', 'center');
                         }
                     }
                 }();
                 return withOverflowWrap(
                     A4(
                         $terezka$elm_charts$Internal$Svg$withAttrs,
-                        config.bv,
+                        config.bu,
                         $elm$svg$Svg$foreignObject,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__label'),
                                 $elm$svg$Svg$Attributes$class('elm-charts__html-label'),
                                 $elm$svg$Svg$Attributes$width(
-                                    $elm$core$String$fromFloat(ellipsis.ff)),
+                                    $elm$core$String$fromFloat(ellipsis.fi)),
                                 $elm$svg$Svg$Attributes$height(
-                                    $elm$core$String$fromFloat(ellipsis.eb)),
-                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fg, point.fh, xOffWithAnchor, config.h - 10)
+                                    $elm$core$String$fromFloat(ellipsis.ea)),
+                                A6($terezka$elm_charts$Internal$Svg$position, plane, -config.o, point.fj, point.fk, xOffWithAnchor, config.h - 10)
                             ]),
                         _List_fromArray(
                             [
                                 A2(
                                     $elm$html$Html$div,
                                     _List_fromArray(
                                         [
                                             A2($elm$html$Html$Attributes$attribute, 'xmlns', 'http://www.w3.org/1999/xhtml'),
                                             A2($elm$html$Html$Attributes$style, 'white-space', 'nowrap'),
                                             A2($elm$html$Html$Attributes$style, 'overflow', 'hidden'),
                                             A2($elm$html$Html$Attributes$style, 'text-overflow', 'ellipsis'),
                                             A2($elm$html$Html$Attributes$style, 'height', '100%'),
                                             A2($elm$html$Html$Attributes$style, 'pointer-events', 'none'),
-                                            A2($elm$html$Html$Attributes$style, 'color', config.bD),
+                                            A2($elm$html$Html$Attributes$style, 'color', config.bC),
                                             fontStyle,
                                             uppercaseStyle,
                                             anchorStyle
                                         ]),
                                     inner)
                             ])));
             }
         });
     var $terezka$elm_charts$Chart$Attributes$zero = function(b) {
-        return A3($elm$core$Basics$clamp, b.et, b.er, 0);
+        return A3($elm$core$Basics$clamp, b.ev, b.et, 0);
     };
     var $terezka$elm_charts$Chart$xLabels = function(edits) {
         var toTicks = F2(
             function(p, config) {
                 return A4(
                     $terezka$elm_charts$Chart$generateValues,
-                    config.J,
-                    config.M,
+                    config.K,
+                    config.N,
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, x) {
                                 return f(x);
                             }),
-                        p.fg,
+                        p.fj,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
                         A: _Utils_ap(
                             ts.A,
                             A2(
                                 $elm$core$List$map,
                                 function($) {
-                                    return $.W;
+                                    return $.Z;
                                 },
                                 A2(toTicks, p, config)))
                     });
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
-                    J: 5,
+                    K: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bv: _List_Nil,
-                    bD: '#808BAB',
+                    bu: _List_Nil,
+                    bC: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
-                    M: $terezka$elm_charts$Internal$Svg$Floats,
+                    N: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
                     t: _List_Nil,
                     n: $terezka$elm_charts$Chart$Attributes$zero,
                     o: 0,
                     p: false,
                     g: 0,
@@ -15702,30 +16011,30 @@
                     var toLabel = function(item) {
                         return A4(
                             $terezka$elm_charts$Internal$Svg$label,
                             p,
                             _Utils_update(
                                 _default, {
                                     i: config.i,
-                                    bv: config.bv,
-                                    bD: config.bD,
+                                    bu: config.bu,
+                                    bC: config.bC,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.g,
                                     h: config.e ? ((-config.h) + 10) : config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.en)
+                                    $elm$svg$Svg$text(item.em)
                                 ]), {
-                                fg: item.W,
-                                fh: config.n(p.fh)
+                                fj: item.Z,
+                                fk: config.n(p.fk)
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__x-labels')
@@ -15738,53 +16047,53 @@
     };
     var $terezka$elm_charts$Internal$Svg$End = 0;
     var $terezka$elm_charts$Chart$yLabels = function(edits) {
         var toTicks = F2(
             function(p, config) {
                 return A4(
                     $terezka$elm_charts$Chart$generateValues,
-                    config.J,
-                    config.M,
+                    config.K,
+                    config.N,
                     config.F,
                     A3(
                         $elm$core$List$foldl,
                         F2(
                             function(f, y) {
                                 return f(y);
                             }),
-                        p.fh,
+                        p.fk,
                         config.t));
             });
         var toTickValues = F3(
             function(p, config, ts) {
                 return (!config.f) ? ts : _Utils_update(
                     ts, {
-                        I: _Utils_ap(
-                            ts.I,
+                        J: _Utils_ap(
+                            ts.J,
                             A2(
                                 $elm$core$List$map,
                                 function($) {
-                                    return $.W;
+                                    return $.Z;
                                 },
                                 A2(toTicks, p, config)))
                     });
             });
         var toConfig = function(p) {
             return A2(
                 $terezka$elm_charts$Internal$Helpers$apply,
                 edits, {
-                    J: 5,
+                    K: 5,
                     i: $elm$core$Maybe$Nothing,
-                    bv: _List_Nil,
-                    bD: '#808BAB',
+                    bu: _List_Nil,
+                    bC: '#808BAB',
                     j: $elm$core$Maybe$Nothing,
                     e: false,
                     k: $elm$core$Maybe$Nothing,
                     F: $elm$core$Maybe$Nothing,
-                    M: $terezka$elm_charts$Internal$Svg$Floats,
+                    N: $terezka$elm_charts$Internal$Svg$Floats,
                     f: false,
                     l: false,
                     t: _List_Nil,
                     n: $terezka$elm_charts$Chart$Attributes$zero,
                     o: 0,
                     p: false,
                     g: -10,
@@ -15810,30 +16119,30 @@
                                             return $elm$core$Maybe$Just(
                                                 config.e ? 1 : 0);
                                         } else {
                                             var anchor = _v0.a;
                                             return $elm$core$Maybe$Just(anchor);
                                         }
                                     }(),
-                                    bv: config.bv,
-                                    bD: config.bD,
+                                    bu: config.bu,
+                                    bC: config.bC,
                                     j: config.j,
                                     k: config.k,
                                     l: config.l,
                                     o: config.o,
                                     p: config.p,
                                     g: config.e ? (-config.g) : config.g,
                                     h: config.h
                                 }),
                             _List_fromArray(
                                 [
-                                    $elm$svg$Svg$text(item.en)
+                                    $elm$svg$Svg$text(item.em)
                                 ]), {
-                                fg: config.n(p.fg),
-                                fh: item.W
+                                fj: config.n(p.fj),
+                                fk: item.Z
                             });
                     };
                     return A2(
                         $elm$svg$Svg$g,
                         _List_fromArray(
                             [
                                 $elm$svg$Svg$Attributes$class('elm-charts__y-labels')
@@ -15846,80 +16155,88 @@
     };
     var $author$project$Graph$getEpaChart = F2(
         function(graphModel, onHover) {
             return A2(
                 $terezka$elm_charts$Chart$chart,
                 _List_fromArray(
                     [
-                        $terezka$elm_charts$Chart$Attributes$height(300),
-                        $terezka$elm_charts$Chart$Attributes$width(1000),
+                        $terezka$elm_charts$Chart$Attributes$height(200),
+                        $terezka$elm_charts$Chart$Attributes$width(800),
+                        $terezka$elm_charts$Chart$Attributes$margin({
+                            dO: 0,
+                            er: 40,
+                            eW: 20,
+                            fb: 0
+                        }),
                         A2(
                             $terezka$elm_charts$Chart$Events$onMouseMove,
                             onHover,
                             $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
                         $terezka$elm_charts$Chart$Events$onMouseLeave(
                             onHover(_List_Nil))
                     ]),
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$xLabels(
                             _List_fromArray(
                                 [
-                                    $terezka$elm_charts$Chart$Attributes$moveDown(25),
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid,
-                                    $terezka$elm_charts$Chart$Attributes$rotate(60),
                                     $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
                                 ])),
                         $terezka$elm_charts$Chart$yLabels(
                             _List_fromArray(
-                                [$terezka$elm_charts$Chart$Attributes$withGrid])),
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(10),
+                                    $terezka$elm_charts$Chart$Attributes$withGrid
+                                ])),
                         A3(
                             $terezka$elm_charts$Chart$series,
                             function($) {
-                                return $.cG;
+                                return $.cF;
                             },
                             _List_fromArray(
                                 [
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'EPA',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.d1;
+                                                return $.d$;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$blue)
                                                 ]),
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$circle,
                                                     $terezka$elm_charts$Chart$Attributes$size(3)
                                                 ])))
                                 ]),
-                            graphModel.bN),
+                            graphModel.bM),
                         A2(
                             $terezka$elm_charts$Chart$each,
-                            graphModel.bE,
+                            graphModel.bD,
                             F2(
                                 function(p, item) {
                                     return _List_fromArray(
                                         [
                                             A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
                                         ]);
                                 })),
                         A4(
                             $terezka$elm_charts$Chart$legendsAt,
                             function($) {
-                                return $.et;
+                                return $.ev;
                             },
                             function($) {
-                                return $.er;
+                                return $.et;
                             },
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$row,
                                     $terezka$elm_charts$Chart$Attributes$alignLeft,
                                     $terezka$elm_charts$Chart$Attributes$spacing(5),
                                     $terezka$elm_charts$Chart$Attributes$background('Azure'),
@@ -15933,58 +16250,178 @@
                                 ]),
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(12)
                                 ]))
                     ]));
         });
+    var $author$project$EpaCommon$getLabelForLevel = function(level) {
+        switch (level) {
+            case 0:
+                return 'Hazardous';
+            case 1:
+                return 'Very Unhealthy';
+            case 2:
+                return 'Unhealthy';
+            case 3:
+                return 'Unhealthy For Sensitive';
+            case 4:
+                return 'Moderate';
+            default:
+                return 'Good';
+        }
+    };
+    var $author$project$EpaLevel$selectedStyles = function(isSelected) {
+        return isSelected ? _List_fromArray(
+            [
+                A2($elm$html$Html$Attributes$style, 'border-radius', '1em')
+            ]) : _List_fromArray(
+            [
+                A2($elm$html$Html$Attributes$style, 'margin', '0 0.25em 0 0.25em')
+            ]);
+    };
+    var $author$project$EpaLevel$getRow = F2(
+        function(level, isSelected) {
+            return A2(
+                $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                _List_fromArray(
+                    [
+                        $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                            A2(
+                                $elm$core$List$append,
+                                _List_fromArray(
+                                    [
+                                        A2(
+                                            $elm$html$Html$Attributes$style,
+                                            'background-color',
+                                            $author$project$EpaCommon$getColorForLevel(level))
+                                    ]),
+                                $author$project$EpaLevel$selectedStyles(isSelected)))
+                    ]),
+                _List_fromArray(
+                    [
+                        A2(
+                            $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                            _List_fromArray(
+                                [
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                        _List_fromArray(
+                                            [
+                                                A2($elm$html$Html$Attributes$style, 'text-align', 'center'),
+                                                A2($elm$html$Html$Attributes$style, 'padding', '.25em'),
+                                                A2($elm$html$Html$Attributes$style, 'color', 'white')
+                                            ]))
+                                ]),
+                            _List_fromArray(
+                                [
+                                    $elm$html$Html$text(
+                                        $author$project$EpaCommon$getLabelForLevel(level))
+                                ]))
+                    ]));
+        });
+    var $author$project$EpaLevel$getEpaLevel = function(currentLevel) {
+        return A2(
+            $rundis$elm_bootstrap$Bootstrap$Grid$container,
+            _List_fromArray(
+                [
+                    $elm$html$Html$Attributes$class('align-middle'),
+                    A2($elm$html$Html$Attributes$style, 'padding', '1em')
+                ]),
+            _List_fromArray(
+                [
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        0,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(0))),
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        1,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(1))),
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        2,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(2))),
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        3,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(3))),
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        4,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(4))),
+                    A2(
+                        $author$project$EpaLevel$getRow,
+                        5,
+                        _Utils_eq(
+                            currentLevel,
+                            $elm$core$Maybe$Just(5)))
+                ]));
+    };
     var $terezka$elm_charts$Chart$Attributes$red = $terezka$elm_charts$Internal$Helpers$red;
     var $terezka$elm_charts$Chart$Attributes$yellow = $terezka$elm_charts$Internal$Helpers$yellow;
     var $author$project$Graph$getReadChart = F2(
         function(graphModel, onHover) {
             return A2(
                 $terezka$elm_charts$Chart$chart,
                 _List_fromArray(
                     [
-                        $terezka$elm_charts$Chart$Attributes$height(300),
-                        $terezka$elm_charts$Chart$Attributes$width(1000),
+                        $terezka$elm_charts$Chart$Attributes$height(200),
+                        $terezka$elm_charts$Chart$Attributes$width(800),
+                        $terezka$elm_charts$Chart$Attributes$margin({
+                            dO: 0,
+                            er: 40,
+                            eW: 20,
+                            fb: 0
+                        }),
                         A2(
                             $terezka$elm_charts$Chart$Events$onMouseMove,
                             onHover,
                             $terezka$elm_charts$Chart$Events$getNearest($terezka$elm_charts$Chart$Item$dots)),
                         $terezka$elm_charts$Chart$Events$onMouseLeave(
                             onHover(_List_Nil))
                     ]),
                 _List_fromArray(
                     [
                         $terezka$elm_charts$Chart$xLabels(
                             _List_fromArray(
                                 [
-                                    $terezka$elm_charts$Chart$Attributes$moveDown(25),
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(10),
                                     $terezka$elm_charts$Chart$Attributes$withGrid,
-                                    $terezka$elm_charts$Chart$Attributes$rotate(60),
                                     $terezka$elm_charts$Chart$Attributes$format($author$project$Graph$formatTime)
                                 ])),
                         $terezka$elm_charts$Chart$yLabels(
                             _List_fromArray(
-                                [$terezka$elm_charts$Chart$Attributes$withGrid])),
+                                [
+                                    $terezka$elm_charts$Chart$Attributes$fontSize(10),
+                                    $terezka$elm_charts$Chart$Attributes$withGrid
+                                ])),
                         A3(
                             $terezka$elm_charts$Chart$series,
                             function($) {
-                                return $.cG;
+                                return $.cF;
                             },
                             _List_fromArray(
                                 [
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'PM2.5',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.eE;
+                                                return $.eG;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$yellow)
                                                 ]),
                                             _List_fromArray(
@@ -15994,45 +16431,45 @@
                                                 ]))),
                                     A2(
                                         $terezka$elm_charts$Chart$named,
                                         'PM10',
                                         A3(
                                             $terezka$elm_charts$Chart$interpolated,
                                             function($) {
-                                                return $.eD;
+                                                return $.eF;
                                             },
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$monotone,
                                                     $terezka$elm_charts$Chart$Attributes$color($terezka$elm_charts$Chart$Attributes$red)
                                                 ]),
                                             _List_fromArray(
                                                 [
                                                     $terezka$elm_charts$Chart$Attributes$circle,
                                                     $terezka$elm_charts$Chart$Attributes$size(3)
                                                 ])))
                                 ]),
-                            graphModel.bN),
+                            graphModel.bM),
                         A2(
                             $terezka$elm_charts$Chart$each,
-                            graphModel.bE,
+                            graphModel.bD,
                             F2(
                                 function(p, item) {
                                     return _List_fromArray(
                                         [
                                             A4($terezka$elm_charts$Chart$tooltip, item, _List_Nil, _List_Nil, _List_Nil)
                                         ]);
                                 })),
                         A4(
                             $terezka$elm_charts$Chart$legendsAt,
                             function($) {
-                                return $.et;
+                                return $.ev;
                             },
                             function($) {
-                                return $.er;
+                                return $.et;
                             },
                             _List_fromArray(
                                 [
                                     $terezka$elm_charts$Chart$Attributes$row,
                                     $terezka$elm_charts$Chart$Attributes$alignLeft,
                                     $terezka$elm_charts$Chart$Attributes$spacing(5),
                                     $terezka$elm_charts$Chart$Attributes$background('Azure'),
@@ -16048,15 +16485,15 @@
                                 [
                                     $terezka$elm_charts$Chart$Attributes$fontSize(12)
                                 ]))
                     ]));
         });
     var $author$project$Main$ChangeWindow = function(a) {
         return {
-            $: 4,
+            $: 6,
             a: a
         };
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Attrs = function(a) {
         return {
             $: 4,
             a: a
@@ -16091,23 +16528,23 @@
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring = function(a) {
         return {
             $: 1,
             a: a
         };
     };
+    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Dark = 6;
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined = function(a) {
         return {
             $: 1,
             a: a
         };
     };
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Button$Primary = 0;
-    var $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary = $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring(
-        $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined(0));
+    var $rundis$elm_bootstrap$Bootstrap$Button$outlineDark = $rundis$elm_bootstrap$Bootstrap$Internal$Button$Coloring(
+        $rundis$elm_bootstrap$Bootstrap$Internal$Button$Outlined(6));
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$RadioButtonItem = $elm$core$Basics$identity;
     var $elm$html$Html$Attributes$autocomplete = function(bool) {
         return A2(
             $elm$html$Html$Attributes$stringProperty,
             'autocomplete',
             bool ? 'on' : 'off');
     };
@@ -16123,57 +16560,57 @@
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$applyModifier = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 0:
                     var size = modifier.a;
                     return _Utils_update(
                         options, {
-                            eZ: $elm$core$Maybe$Just(size)
+                            e1: $elm$core$Maybe$Just(size)
                         });
                 case 1:
                     var coloring = modifier.a;
                     return _Utils_update(
                         options, {
-                            Z: $elm$core$Maybe$Just(coloring)
+                            ab: $elm$core$Maybe$Just(coloring)
                         });
                 case 2:
                     return _Utils_update(
                         options, {
-                            bx: true
+                            bw: true
                         });
                 case 3:
                     var val = modifier.a;
                     return _Utils_update(
                         options, {
-                            bJ: val
+                            bI: val
                         });
                 default:
                     var attrs = modifier.a;
                     return _Utils_update(
                         options, {
-                            bu: _Utils_ap(options.bu, attrs)
+                            bt: _Utils_ap(options.bt, attrs)
                         });
             }
         });
     var $elm$html$Html$Attributes$classList = function(classes) {
         return $elm$html$Html$Attributes$class(
             A2(
                 $elm$core$String$join,
                 ' ',
                 A2(
                     $elm$core$List$map,
                     $elm$core$Tuple$first,
                     A2($elm$core$List$filter, $elm$core$Tuple$second, classes))));
     };
     var $rundis$elm_bootstrap$Bootstrap$Internal$Button$defaultOptions = {
-        bu: _List_Nil,
-        bx: false,
-        Z: $elm$core$Maybe$Nothing,
-        bJ: false,
-        eZ: $elm$core$Maybe$Nothing
+        bt: _List_Nil,
+        bw: false,
+        ab: $elm$core$Maybe$Nothing,
+        bI: false,
+        e1: $elm$core$Maybe$Nothing
     };
     var $elm$json$Json$Encode$bool = _Json_wrap;
     var $elm$html$Html$Attributes$boolProperty = F2(
         function(key, bool) {
             return A2(
                 _VirtualDom_property,
                 key,
@@ -16207,35 +16644,35 @@
         return _Utils_ap(
             _List_fromArray(
                 [
                     $elm$html$Html$Attributes$classList(
                         _List_fromArray(
                             [
                                 _Utils_Tuple2('btn', true),
-                                _Utils_Tuple2('btn-block', options.bx),
-                                _Utils_Tuple2('disabled', options.bJ)
+                                _Utils_Tuple2('btn-block', options.bw),
+                                _Utils_Tuple2('disabled', options.bI)
                             ])),
-                    $elm$html$Html$Attributes$disabled(options.bJ)
+                    $elm$html$Html$Attributes$disabled(options.bI)
                 ]),
             _Utils_ap(
                 function() {
-                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eZ);
+                    var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e1);
                     if (!_v0.$) {
                         var s = _v0.a;
                         return _List_fromArray(
                             [
                                 $elm$html$Html$Attributes$class('btn-' + s)
                             ]);
                     } else {
                         return _List_Nil;
                     }
                 }(),
                 _Utils_ap(
                     function() {
-                        var _v1 = options.Z;
+                        var _v1 = options.ab;
                         if (!_v1.$) {
                             if (!_v1.a.$) {
                                 var role = _v1.a.a;
                                 return _List_fromArray(
                                     [
                                         $elm$html$Html$Attributes$class(
                                             'btn-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
@@ -16248,15 +16685,15 @@
                                             'btn-outline-' + $rundis$elm_bootstrap$Bootstrap$Internal$Button$roleClass(role))
                                     ]);
                             }
                         } else {
                             return _List_Nil;
                         }
                     }(),
-                    options.bu)));
+                    options.bt)));
     };
     var $elm$html$Html$Attributes$checked = $elm$html$Html$Attributes$boolProperty('checked');
     var $elm$html$Html$input = _VirtualDom_node('input');
     var $elm$html$Html$label = _VirtualDom_node('label');
     var $elm$html$Html$Attributes$type_ = $elm$html$Html$Attributes$stringProperty('type');
     var $rundis$elm_bootstrap$Bootstrap$Button$radioButton = F3(
         function(checked, options, children) {
@@ -16294,29 +16731,34 @@
     var $author$project$Main$getSelector = F3(
         function(windowDuration, textDuration, currentDuration) {
             return A3(
                 $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButton,
                 _Utils_eq(windowDuration, currentDuration),
                 _List_fromArray(
                     [
-                        $rundis$elm_bootstrap$Bootstrap$Button$outlinePrimary,
+                        $rundis$elm_bootstrap$Bootstrap$Button$outlineDark,
                         $rundis$elm_bootstrap$Bootstrap$Button$onClick(
                             $author$project$Main$ChangeWindow(windowDuration))
                     ]),
                 _List_fromArray(
                     [
                         $elm$html$Html$text(textDuration)
                     ]));
         });
-    var $elm$html$Html$h1 = _VirtualDom_node('h1');
     var $elm$html$Html$h2 = _VirtualDom_node('h2');
     var $author$project$Main$htmlIf = F2(
         function(el, cond) {
             return cond ? el : $elm$html$Html$text('');
         });
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$Item = $elm$core$Basics$identity;
+    var $elm$html$Html$option = _VirtualDom_node('option');
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$item = F2(
+        function(attributes, children) {
+            return A2($elm$html$Html$option, attributes, children);
+        });
     var $rundis$elm_bootstrap$Bootstrap$General$Internal$LG = 3;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth = function(a) {
         return {
             $: 0,
             a: a
         };
     };
@@ -16324,72 +16766,81 @@
         function(size, count) {
             return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$ColWidth(
                 A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$Width, size, count));
         });
     var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 0);
     var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$Col3 = 3;
     var $rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3 = A2($rundis$elm_bootstrap$Bootstrap$Grid$Internal$width, 3, 3);
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$OnChange = function(a) {
+        return {
+            $: 4,
+            a: a
+        };
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$onChange = function(toMsg) {
+        return $rundis$elm_bootstrap$Bootstrap$Form$Select$OnChange(toMsg);
+    };
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$GroupItem = $elm$core$Basics$identity;
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier = F2(
         function(modifier, options) {
             switch (modifier.$) {
                 case 0:
                     var size = modifier.a;
                     return _Utils_update(
                         options, {
-                            eZ: $elm$core$Maybe$Just(size)
+                            e1: $elm$core$Maybe$Just(size)
                         });
                 case 1:
                     return _Utils_update(
                         options, {
-                            cR: true
+                            cQ: true
                         });
                 default:
                     var attrs_ = modifier.a;
                     return _Utils_update(
                         options, {
-                            bu: _Utils_ap(options.bu, attrs_)
+                            bt: _Utils_ap(options.bt, attrs_)
                         });
             }
         });
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions = {
-        bu: _List_Nil,
-        eZ: $elm$core$Maybe$Nothing,
-        cR: false
+        bt: _List_Nil,
+        e1: $elm$core$Maybe$Nothing,
+        cQ: false
     };
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes = F2(
         function(toggle, modifiers) {
             var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$applyModifier, $rundis$elm_bootstrap$Bootstrap$ButtonGroup$defaultOptions, modifiers);
             return _Utils_ap(
                 _List_fromArray(
                     [
                         A2($elm$html$Html$Attributes$attribute, 'role', 'group'),
                         $elm$html$Html$Attributes$classList(
                             _List_fromArray(
                                 [
                                     _Utils_Tuple2('btn-group', true),
                                     _Utils_Tuple2('btn-group-toggle', toggle),
-                                    _Utils_Tuple2('btn-group-vertical', options.cR)
+                                    _Utils_Tuple2('btn-group-vertical', options.cQ)
                                 ])),
                         A2($elm$html$Html$Attributes$attribute, 'data-toggle', 'buttons')
                     ]),
                 _Utils_ap(
                     function() {
-                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.eZ);
+                        var _v0 = A2($elm$core$Maybe$andThen, $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption, options.e1);
                         if (!_v0.$) {
                             var s = _v0.a;
                             return _List_fromArray(
                                 [
                                     $elm$html$Html$Attributes$class('btn-group-' + s)
                                 ]);
                         } else {
                             return _List_Nil;
                         }
                     }(),
-                    options.bu));
+                    options.bt));
         });
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem = F2(
         function(options, items) {
             return A2(
                 $elm$html$Html$div,
                 A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$groupAttributes, true, options),
                 A2(
@@ -16405,103 +16856,165 @@
         return elem;
     };
     var $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup = F2(
         function(options, items) {
             return $rundis$elm_bootstrap$Bootstrap$ButtonGroup$renderGroup(
                 A2($rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroupItem, options, items));
         });
-    var $rundis$elm_bootstrap$Bootstrap$Internal$Text$Center = 1;
-    var $rundis$elm_bootstrap$Bootstrap$Text$alignMd = function(dir) {
-        return {
-            d_: dir,
-            eZ: 2
-        };
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$Select = $elm$core$Basics$identity;
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$create = F2(
+        function(options, items) {
+            return {
+                ek: items,
+                dh: options
+            };
+        });
+    var $elm$html$Html$select = _VirtualDom_node('select');
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$applyModifier = F2(
+        function(modifier, options) {
+            switch (modifier.$) {
+                case 0:
+                    var size_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            e1: $elm$core$Maybe$Just(size_)
+                        });
+                case 1:
+                    var id_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            aT: $elm$core$Maybe$Just(id_)
+                        });
+                case 2:
+                    return _Utils_update(
+                        options, {
+                            C: true
+                        });
+                case 3:
+                    var val = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bI: val
+                        });
+                case 4:
+                    var onChange_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            ca: $elm$core$Maybe$Just(onChange_)
+                        });
+                case 5:
+                    var validation_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            cP: $elm$core$Maybe$Just(validation_)
+                        });
+                default:
+                    var attrs_ = modifier.a;
+                    return _Utils_update(
+                        options, {
+                            bt: _Utils_ap(options.bt, attrs_)
+                        });
+            }
+        });
+    var $elm$json$Json$Decode$at = F2(
+        function(fields, decoder) {
+            return A3($elm$core$List$foldr, $elm$json$Json$Decode$field, decoder, fields);
+        });
+    var $elm$html$Html$Events$targetValue = A2(
+        $elm$json$Json$Decode$at,
+        _List_fromArray(
+            ['target', 'value']),
+        $elm$json$Json$Decode$string);
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$customEventOnChange = function(tagger) {
+        return A2(
+            $elm$html$Html$Events$on,
+            'change',
+            A2($elm$json$Json$Decode$map, tagger, $elm$html$Html$Events$targetValue));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$defaultOptions = {
+        bt: _List_Nil,
+        C: false,
+        bI: false,
+        aT: $elm$core$Maybe$Nothing,
+        ca: $elm$core$Maybe$Nothing,
+        e1: $elm$core$Maybe$Nothing,
+        cP: $elm$core$Maybe$Nothing
     };
-    var $rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter = $rundis$elm_bootstrap$Bootstrap$Text$alignMd(1);
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign = function(a) {
-        return {
-            $: 7,
-            a: a
-        };
+    var $elm$html$Html$Attributes$id = $elm$html$Html$Attributes$stringProperty('id');
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$sizeAttribute = F2(
+        function(isCustom, size_) {
+            var prefix = isCustom ? 'custom-select-' : 'form-control-';
+            return A2(
+                $elm$core$Maybe$map,
+                function(s) {
+                    return $elm$html$Html$Attributes$class(
+                        _Utils_ap(prefix, s));
+                },
+                $rundis$elm_bootstrap$Bootstrap$General$Internal$screenSizeOption(size_));
+        });
+    var $rundis$elm_bootstrap$Bootstrap$Form$FormInternal$validationToString = function(validation) {
+        if (!validation) {
+            return 'is-valid';
+        } else {
+            return 'is-invalid';
+        }
     };
-    var $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign = function(align) {
-        return $rundis$elm_bootstrap$Bootstrap$Grid$Internal$TextAlign(align);
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$validationAttribute = function(validation_) {
+        return $elm$html$Html$Attributes$class(
+            $rundis$elm_bootstrap$Bootstrap$Form$FormInternal$validationToString(validation_));
     };
-    var $author$project$Main$viewBigNumber = F2(
-        function(value, numberType) {
-            return A2(
-                $rundis$elm_bootstrap$Bootstrap$Grid$container,
-                _List_fromArray(
-                    [
-                        A2($elm$html$Html$Attributes$style, 'background-clip', 'border-box'),
-                        A2($elm$html$Html$Attributes$style, 'border', '1px solid darkgray'),
-                        A2($elm$html$Html$Attributes$style, 'padding', '0'),
-                        A2($elm$html$Html$Attributes$style, 'border-radius', '.25rem')
-                    ]),
-                _List_fromArray(
-                    [
-                        A2(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                            _List_Nil,
-                            _List_fromArray(
-                                [
-                                    A2(
-                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                        _List_fromArray(
-                                            [
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
-                                            ]),
-                                        _List_fromArray(
-                                            [
-                                                A2(
-                                                    $elm$html$Html$h1,
-                                                    _List_fromArray(
-                                                        [
-                                                            A2($elm$html$Html$Attributes$style, 'padding', '.5em'),
-                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
-                                                            A2($elm$html$Html$Attributes$style, 'color', 'white'),
-                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightblue')
-                                                        ]),
-                                                    _List_fromArray(
-                                                        [
-                                                            $elm$html$Html$text(
-                                                                $elm$core$String$fromFloat(value))
-                                                        ]))
-                                            ]))
-                                ])),
-                        A2(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                            _List_Nil,
-                            _List_fromArray(
-                                [
-                                    A2(
-                                        $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                        _List_fromArray(
-                                            [
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$Col$textAlign($rundis$elm_bootstrap$Bootstrap$Text$alignMdCenter)
-                                            ]),
-                                        _List_fromArray(
-                                            [
-                                                A2(
-                                                    $elm$html$Html$h5,
-                                                    _List_fromArray(
-                                                        [
-                                                            A2($elm$html$Html$Attributes$style, 'padding', '.25em'),
-                                                            A2($elm$html$Html$Attributes$style, 'margin', '0'),
-                                                            A2($elm$html$Html$Attributes$style, 'color', 'darkblue'),
-                                                            A2($elm$html$Html$Attributes$style, 'background-color', 'lightgray')
-                                                        ]),
-                                                    _List_fromArray(
-                                                        [
-                                                            $elm$html$Html$text(numberType)
-                                                        ]))
-                                            ]))
-                                ]))
-                    ]));
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$toAttributes = function(modifiers) {
+        var options = A3($elm$core$List$foldl, $rundis$elm_bootstrap$Bootstrap$Form$Select$applyModifier, $rundis$elm_bootstrap$Bootstrap$Form$Select$defaultOptions, modifiers);
+        return _Utils_ap(
+            _List_fromArray(
+                [
+                    $elm$html$Html$Attributes$classList(
+                        _List_fromArray(
+                            [
+                                _Utils_Tuple2('form-control', !options.C),
+                                _Utils_Tuple2('custom-select', options.C)
+                            ])),
+                    $elm$html$Html$Attributes$disabled(options.bI)
+                ]),
+            _Utils_ap(
+                A2(
+                    $elm$core$List$filterMap,
+                    $elm$core$Basics$identity,
+                    _List_fromArray(
+                        [
+                            A2($elm$core$Maybe$map, $elm$html$Html$Attributes$id, options.aT),
+                            A2(
+                                $elm$core$Maybe$andThen,
+                                $rundis$elm_bootstrap$Bootstrap$Form$Select$sizeAttribute(options.C),
+                                options.e1),
+                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$customEventOnChange, options.ca),
+                            A2($elm$core$Maybe$map, $rundis$elm_bootstrap$Bootstrap$Form$Select$validationAttribute, options.cP)
+                        ])),
+                options.bt));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$view = function(_v0) {
+        var options = _v0.dh;
+        var items = _v0.ek;
+        return A2(
+            $elm$html$Html$select,
+            $rundis$elm_bootstrap$Bootstrap$Form$Select$toAttributes(options),
+            A2(
+                $elm$core$List$map,
+                function(_v1) {
+                    var e = _v1;
+                    return e;
+                },
+                items));
+    };
+    var $rundis$elm_bootstrap$Bootstrap$Form$Select$select = F2(
+        function(options, items) {
+            return $rundis$elm_bootstrap$Bootstrap$Form$Select$view(
+                A2($rundis$elm_bootstrap$Bootstrap$Form$Select$create, options, items));
         });
+    var $elm$html$Html$Attributes$value = $elm$html$Html$Attributes$stringProperty('value');
     var $author$project$Main$view = function(model) {
         return A2(
             $elm$html$Html$div,
             _List_Nil,
             _List_fromArray(
                 [
                     A2(
@@ -16515,52 +17028,100 @@
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
                                         [
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
                                                 _List_fromArray(
                                                     [
-                                                        $elm$html$Html$Attributes$class('bg-info'),
                                                         A2($elm$html$Html$Attributes$style, 'padding', '1em')
                                                     ]))
                                         ]),
                                     _List_fromArray(
                                         [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_Nil,
                                                 _List_fromArray(
                                                     [
                                                         A2(
                                                             $elm$html$Html$h1,
+                                                            _List_Nil,
                                                             _List_fromArray(
                                                                 [
-                                                                    $elm$html$Html$Attributes$class('text-center')
-                                                                ]),
+                                                                    $elm$html$Html$text('AQI Monitor')
+                                                                ]))
+                                                    ]))
+                                        ])),
+                                A2(
+                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                    _List_fromArray(
+                                        [
+                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                                _List_fromArray(
+                                                    [
+                                                        A2($elm$html$Html$Attributes$style, 'padding', '1em')
+                                                    ]))
+                                        ]),
+                                    _List_fromArray(
+                                        [
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                _List_fromArray(
+                                                    [
+                                                        $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
                                                             _List_fromArray(
                                                                 [
-                                                                    $elm$html$Html$text('AQI Monitor')
+                                                                    A2($elm$html$Html$Attributes$style, 'background-color', '#D9D9D9'),
+                                                                    A2($elm$html$Html$Attributes$style, 'margin', '1em')
                                                                 ]))
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $author$project$CurrentReads$getCurrentReads({
+                                                            d0: model.ad.d0,
+                                                            en: model.ad.d$,
+                                                            ep: model.ad.eF,
+                                                            eq: model.ad.eG
+                                                        })
                                                     ])),
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_Nil,
                                                 _List_fromArray(
                                                     [
-                                                        $author$project$DeviceStatus$getDeviceInfo(model.V)
+                                                        $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                            _List_fromArray(
+                                                                [
+                                                                    $elm$html$Html$Attributes$class('align-items-center'),
+                                                                    $elm$html$Html$Attributes$class('d-flex'),
+                                                                    A2($elm$html$Html$Attributes$style, 'background-color', '#D9D9D9'),
+                                                                    A2($elm$html$Html$Attributes$style, 'margin', '1em')
+                                                                ]))
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $author$project$EpaLevel$getEpaLevel(model.ad.d0)
+                                                    ])),
+                                            A2(
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                _List_fromArray(
+                                                    [
+                                                        $rundis$elm_bootstrap$Bootstrap$Grid$Col$attrs(
+                                                            _List_fromArray(
+                                                                [
+                                                                    A2($elm$html$Html$Attributes$style, 'background-color', '#D9D9D9'),
+                                                                    A2($elm$html$Html$Attributes$style, 'margin', '1em')
+                                                                ]))
+                                                    ]),
+                                                _List_fromArray(
+                                                    [
+                                                        $author$project$DeviceStatus$getDeviceInfo(model.Y)
                                                     ]))
-                                        ]))
-                            ])),
-                    A2(
-                        $author$project$Main$htmlIf,
-                        A2(
-                            $rundis$elm_bootstrap$Bootstrap$Grid$container,
-                            _List_Nil,
-                            _List_fromArray(
-                                [
+                                        ])),
+                                A2(
+                                    $author$project$Main$htmlIf,
                                     A2(
                                         $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                         _List_Nil,
                                         _List_fromArray(
                                             [
                                                 A2(
                                                     $rundis$elm_bootstrap$Bootstrap$Grid$col,
@@ -16576,208 +17137,189 @@
                                                     _List_fromArray(
                                                         [
                                                             A2(
                                                                 $elm$html$Html$h5,
                                                                 _List_Nil,
                                                                 _List_fromArray(
                                                                     [
-                                                                        $elm$html$Html$text(model.T.al)
+                                                                        $elm$html$Html$text(model.G.V)
                                                                     ])),
-                                                            $elm$html$Html$text(model.T.ak)
+                                                            $elm$html$Html$text(model.G.U)
                                                         ]))
-                                            ]))
-                                ])),
-                        model.T.an),
-                    A2(
-                        $rundis$elm_bootstrap$Bootstrap$Grid$container,
-                        _List_Nil,
-                        _List_fromArray(
-                            [
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                    _List_fromArray(
-                                        [$rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd]),
-                                    _List_fromArray(
-                                        [
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
-                                                _List_fromArray(
-                                                    [
-                                                        A2($author$project$Main$viewBigNumber, model.aE.d1, 'EPA')
-                                                    ])),
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
-                                                _List_fromArray(
-                                                    [
-                                                        A2($author$project$Main$viewBigNumber, model.aE.eE, 'PM2.5')
-                                                    ])),
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
-                                                _List_fromArray(
-                                                    [
-                                                        A2($author$project$Main$viewBigNumber, model.aE.eD, 'PM10')
-                                                    ]))
-                                        ])),
+                                            ])),
+                                    model.G.W),
                                 A2(
                                     $rundis$elm_bootstrap$Bootstrap$Grid$row,
                                     _List_fromArray(
                                         [
                                             $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
                                                 _List_fromArray(
                                                     [
-                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
-                                                        $elm$html$Html$Attributes$class('justify-content-end')
+                                                        A2($elm$html$Html$Attributes$style, 'padding', '1em')
                                                     ]))
                                         ]),
                                     _List_fromArray(
                                         [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
-                                                _List_fromArray(
-                                                    [
-                                                        A2(
-                                                            $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    A3($author$project$Main$getSelector, 0, 'All', model.ae),
-                                                                    A3($author$project$Main$getSelector, 1, 'Hour', model.ae),
-                                                                    A3($author$project$Main$getSelector, 2, 'Day', model.ae),
-                                                                    A3($author$project$Main$getSelector, 3, 'Week', model.ae)
-                                                                ]))
-                                                    ]))
-                                        ])),
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                    _List_Nil,
-                                    _List_fromArray(
-                                        [
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_Nil,
                                                 _List_fromArray(
                                                     [
                                                         A2(
                                                             $elm$html$Html$h2,
                                                             _List_Nil,
                                                             _List_fromArray(
                                                                 [
-                                                                    $elm$html$Html$text('EPA AQI')
+                                                                    $elm$html$Html$text('History')
                                                                 ]))
-                                                    ]))
-                                        ])),
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                    _List_fromArray(
-                                        [
-                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
-                                                _List_fromArray(
-                                                    [
-                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
-                                                        A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
                                                     ])),
-                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
-                                        ]),
-                                    _List_fromArray(
-                                        [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg]),
+                                                _List_Nil,
                                                 _List_fromArray(
                                                     [
                                                         A2(
-                                                            $elm$html$Html$div,
+                                                            $rundis$elm_bootstrap$Bootstrap$Form$Select$select,
                                                             _List_fromArray(
                                                                 [
-                                                                    A2($elm$html$Html$Attributes$style, 'height', '400px')
+                                                                    $rundis$elm_bootstrap$Bootstrap$Form$Select$onChange($author$project$Main$ChangeGraphView)
                                                                 ]),
                                                             _List_fromArray(
                                                                 [
                                                                     A2(
-                                                                        $author$project$Graph$getEpaChart, {
-                                                                            bE: model.bW,
-                                                                            bN: model.bq
-                                                                        },
-                                                                        $author$project$Main$OnEpaHover)
-                                                                ]))
-                                                    ]))
-                                        ])),
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                    _List_Nil,
-                                    _List_fromArray(
-                                        [
-                                            A2(
-                                                $rundis$elm_bootstrap$Bootstrap$Grid$col,
-                                                _List_Nil,
-                                                _List_fromArray(
-                                                    [
-                                                        A2(
-                                                            $elm$html$Html$h2,
-                                                            _List_Nil,
-                                                            _List_fromArray(
-                                                                [
-                                                                    $elm$html$Html$text('PM2.5/PM10 Reads')
+                                                                        $rundis$elm_bootstrap$Bootstrap$Form$Select$item,
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$Attributes$value('epa')
+                                                                            ]),
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$text('EPA AQI')
+                                                                            ])),
+                                                                    A2(
+                                                                        $rundis$elm_bootstrap$Bootstrap$Form$Select$item,
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$Attributes$value('pm')
+                                                                            ]),
+                                                                        _List_fromArray(
+                                                                            [
+                                                                                $elm$html$Html$text('Particulate Matter')
+                                                                            ]))
                                                                 ]))
-                                                    ]))
-                                        ])),
-                                A2(
-                                    $rundis$elm_bootstrap$Bootstrap$Grid$row,
-                                    _List_fromArray(
-                                        [
-                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
-                                                _List_fromArray(
-                                                    [
-                                                        A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
-                                                        A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
                                                     ])),
-                                            $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
-                                        ]),
-                                    _List_fromArray(
-                                        [
                                             A2(
                                                 $rundis$elm_bootstrap$Bootstrap$Grid$col,
                                                 _List_fromArray(
-                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg]),
+                                                    [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg3]),
                                                 _List_fromArray(
                                                     [
                                                         A2(
-                                                            $elm$html$Html$div,
+                                                            $rundis$elm_bootstrap$Bootstrap$ButtonGroup$radioButtonGroup,
                                                             _List_fromArray(
                                                                 [
-                                                                    A2($elm$html$Html$Attributes$style, 'height', '400px')
+                                                                    $rundis$elm_bootstrap$Bootstrap$ButtonGroup$attrs(_List_Nil)
                                                                 ]),
                                                             _List_fromArray(
                                                                 [
-                                                                    A2(
-                                                                        $author$project$Graph$getReadChart, {
-                                                                            bE: model.bX,
-                                                                            bN: model.br
-                                                                        },
-                                                                        $author$project$Main$OnReadHover)
+                                                                    A3($author$project$Main$getSelector, 0, 'All', model.ai),
+                                                                    A3($author$project$Main$getSelector, 1, 'Hour', model.ai),
+                                                                    A3($author$project$Main$getSelector, 2, 'Day', model.ai),
+                                                                    A3($author$project$Main$getSelector, 3, 'Week', model.ai)
                                                                 ]))
                                                     ]))
-                                        ]))
+                                        ])),
+                                A2(
+                                    $author$project$Main$htmlIf,
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                        _List_fromArray(
+                                            [
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                                    _List_fromArray(
+                                                        [
+                                                            A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
+                                                            A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
+                                                        ])),
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
+                                            ]),
+                                        _List_fromArray(
+                                            [
+                                                A2(
+                                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                    _List_fromArray(
+                                                        [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg]),
+                                                    _List_fromArray(
+                                                        [
+                                                            A2(
+                                                                $elm$html$Html$div,
+                                                                _List_fromArray(
+                                                                    [
+                                                                        A2($elm$html$Html$Attributes$style, 'height', '400px')
+                                                                    ]),
+                                                                _List_fromArray(
+                                                                    [
+                                                                        A2(
+                                                                            $author$project$Graph$getEpaChart, {
+                                                                                bD: model.bV,
+                                                                                bM: model.bp
+                                                                            },
+                                                                            $author$project$Main$OnEpaHover)
+                                                                    ]))
+                                                        ]))
+                                            ])),
+                                    !model.aO),
+                                A2(
+                                    $author$project$Main$htmlIf,
+                                    A2(
+                                        $rundis$elm_bootstrap$Bootstrap$Grid$row,
+                                        _List_fromArray(
+                                            [
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$attrs(
+                                                    _List_fromArray(
+                                                        [
+                                                            A2($elm$html$Html$Attributes$style, 'padding-top', '1em'),
+                                                            A2($elm$html$Html$Attributes$style, 'padding-bottom', '3em')
+                                                        ])),
+                                                $rundis$elm_bootstrap$Bootstrap$Grid$Row$centerMd
+                                            ]),
+                                        _List_fromArray(
+                                            [
+                                                A2(
+                                                    $rundis$elm_bootstrap$Bootstrap$Grid$col,
+                                                    _List_fromArray(
+                                                        [$rundis$elm_bootstrap$Bootstrap$Grid$Col$lg]),
+                                                    _List_fromArray(
+                                                        [
+                                                            A2(
+                                                                $elm$html$Html$div,
+                                                                _List_fromArray(
+                                                                    [
+                                                                        A2($elm$html$Html$Attributes$style, 'height', '400px')
+                                                                    ]),
+                                                                _List_fromArray(
+                                                                    [
+                                                                        A2(
+                                                                            $author$project$Graph$getReadChart, {
+                                                                                bD: model.bW,
+                                                                                bM: model.bq
+                                                                            },
+                                                                            $author$project$Main$OnReadHover)
+                                                                    ]))
+                                                        ]))
+                                            ])),
+                                    model.aO === 1)
                             ]))
                 ]));
     };
     var $author$project$Main$main = $elm$browser$Browser$element({
-        fN: $author$project$Main$init,
-        ga: $author$project$Main$subscriptions,
-        gr: $author$project$Main$update,
-        gt: $author$project$Main$view
+        fQ: $author$project$Main$init,
+        gd: $author$project$Main$subscriptions,
+        gu: $author$project$Main$update,
+        gw: $author$project$Main$view
     });
     _Platform_export({
         'Main': {
             'init': $author$project$Main$main(
                 $elm$json$Json$Decode$succeed(0))(0)
         }
     });
```

### Comparing `aqimon-0.3.0/aqimon/static/favicon-32x32.png` & `aqimon-0.4.0/aqimon/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/favicon.ico` & `aqimon-0.4.0/aqimon/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/images/failing.png` & `aqimon-0.4.0/aqimon/static/images/failing.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/images/idle.png` & `aqimon-0.4.0/aqimon/static/images/idle.png`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/static/index.html` & `aqimon-0.4.0/aqimon/static/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/aqimon/templates/index.html` & `aqimon-0.4.0/aqimon/templates/index.html`

 * *Files identical despite different names*

### Comparing `aqimon-0.3.0/pyproject.toml` & `aqimon-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aqimon"
-version = "0.3.0"
+version = "0.4.0"
 description = "Air Quality Index Monitor"
 authors = ["Tim Orme"]
 readme = "README.md"
 include = ["aqimon/static/elm.js"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `aqimon-0.3.0/PKG-INFO` & `aqimon-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqimon
-Version: 0.3.0
+Version: 0.4.0
 Summary: Air Quality Index Monitor
 Author: Tim Orme
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

