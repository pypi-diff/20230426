# Comparing `tmp/cronsim-2.3.tar.gz` & `tmp/cronsim-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cronsim-2.3.tar", last modified: Wed Sep 28 14:37:53 2022, max compression
+gzip compressed data, was "cronsim-2.4.tar", last modified: Wed Apr 26 15:06:37 2023, max compression
```

## Comparing `cronsim-2.3.tar` & `cronsim-2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2022-09-28 14:37:53.518799 cronsim-2.3/
--rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.3/LICENSE
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.3/MANIFEST.in
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     4916 2022-09-28 14:37:53.518799 cronsim-2.3/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     4123 2022-09-28 14:32:24.000000 cronsim-2.3/README.md
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2022-09-28 14:37:53.518799 cronsim-2.3/cronsim/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.3/cronsim/__init__.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    10435 2022-09-28 12:34:27.000000 cronsim-2.3/cronsim/cronsim.py
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.3/cronsim/py.typed
--rw-rw-r--   0 cepe      (1000) cepe      (1000)    21899 2022-09-28 11:47:02.000000 cronsim-2.3/cronsim/test_cronsim.py
-drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2022-09-28 14:37:53.518799 cronsim-2.3/cronsim.egg-info/
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     4916 2022-09-28 14:37:53.000000 cronsim-2.3/cronsim.egg-info/PKG-INFO
--rw-rw-r--   0 cepe      (1000) cepe      (1000)      272 2022-09-28 14:37:53.000000 cronsim-2.3/cronsim.egg-info/SOURCES.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.3/cronsim.egg-info/dependency_links.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.3/cronsim.egg-info/not-zip-safe
--rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2022-09-28 14:37:53.000000 cronsim-2.3/cronsim.egg-info/top_level.txt
--rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2022-09-28 14:37:53.518799 cronsim-2.3/setup.cfg
--rw-rw-r--   0 cepe      (1000) cepe      (1000)     1411 2022-09-28 14:37:33.000000 cronsim-2.3/setup.py
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/
+-rw-r--r--   0 cepe      (1000) cepe      (1000)     1484 2021-05-16 16:31:36.000000 cronsim-2.4/LICENSE
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       24 2022-09-28 14:26:08.000000 cronsim-2.4/MANIFEST.in
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     5497 2023-04-26 15:06:37.631533 cronsim-2.4/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     4704 2023-04-26 13:47:00.000000 cronsim-2.4/README.md
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/cronsim/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       70 2022-09-28 11:52:58.000000 cronsim-2.4/cronsim/__init__.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    10693 2023-04-24 10:56:48.000000 cronsim-2.4/cronsim/cronsim.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)    19156 2023-04-26 13:19:47.000000 cronsim-2.4/cronsim/explain.py
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        0 2022-09-28 07:26:47.000000 cronsim-2.4/cronsim/py.typed
+drwxrwxr-x   0 cepe      (1000) cepe      (1000)        0 2023-04-26 15:06:37.631533 cronsim-2.4/cronsim.egg-info/
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     5497 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/PKG-INFO
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)      267 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/SOURCES.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/dependency_links.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        1 2022-09-28 14:37:53.000000 cronsim-2.4/cronsim.egg-info/not-zip-safe
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)        8 2023-04-26 15:06:37.000000 cronsim-2.4/cronsim.egg-info/top_level.txt
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)       38 2023-04-26 15:06:37.631533 cronsim-2.4/setup.cfg
+-rw-rw-r--   0 cepe      (1000) cepe      (1000)     1447 2023-04-26 14:46:27.000000 cronsim-2.4/setup.py
```

### Comparing `cronsim-2.3/LICENSE` & `cronsim-2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cronsim-2.3/PKG-INFO` & `cronsim-2.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronsim
-Version: 2.3
+Version: 2.4
 Summary: Cron expression parser and evaluator
 Home-page: https://github.com/cuu508/cronsim
 Author: Pēteris Caune
 Author-email: cuu508@gmail.com
 License: BSD
 Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
 Keywords: cron,cronjob,crontab,schedule
@@ -12,23 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CronSim
 
 [![Tests](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml/badge.svg)](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml)
 
-Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.7+.
+Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.8+.
 CronSim is written for and being used in
 [Healthchecks](https://github.com/healthchecks/healthchecks/)
 (a cron job monitoring service).
 
 Development priorities:
 
 * Correctness. CronSim tries to match Debian's cron as closely as possible,
@@ -138,7 +138,31 @@
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
 of the month".
 
 Example: `0 0 * * MON#1` (at midnight of the first monday of every month).
 
+## The `explain()` Method
+
+Starting from version 2.4, the CronSim objects have an `explain()` method
+which generates a text description of the supplied cron expression.
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+expr = CronSim("*/5 9-17 * * *", datetime.now())
+print(expr.explain())
+```
+
+Outputs:
+
+```
+Every 5th minute from 9:00 through 17:59
+```
+
+The text descriptions are available in English only. The text descriptions
+use the 24-hour time format ("23:00" instead of "11:00 PM").
+
+For examples of generated descriptions see `tests/test_explain.py`.
+
```

### Comparing `cronsim-2.3/README.md` & `cronsim-2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # CronSim
 
 [![Tests](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml/badge.svg)](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml)
 
-Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.7+.
+Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.8+.
 CronSim is written for and being used in
 [Healthchecks](https://github.com/healthchecks/healthchecks/)
 (a cron job monitoring service).
 
 Development priorities:
 
 * Correctness. CronSim tries to match Debian's cron as closely as possible,
@@ -114,8 +114,32 @@
 
 Example: `0 0 * * 6L` (at the midnight of the last Saturday of every month).
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
 of the month".
 
-Example: `0 0 * * MON#1` (at midnight of the first monday of every month).
+Example: `0 0 * * MON#1` (at midnight of the first monday of every month).
+
+## The `explain()` Method
+
+Starting from version 2.4, the CronSim objects have an `explain()` method
+which generates a text description of the supplied cron expression.
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+expr = CronSim("*/5 9-17 * * *", datetime.now())
+print(expr.explain())
+```
+
+Outputs:
+
+```
+Every 5th minute from 9:00 through 17:59
+```
+
+The text descriptions are available in English only. The text descriptions
+use the 24-hour time format ("23:00" instead of "11:00 PM").
+
+For examples of generated descriptions see `tests/test_explain.py`.
```

### Comparing `cronsim-2.3/cronsim/cronsim.py` & `cronsim-2.4/cronsim/cronsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+from __future__ import annotations
+
 import calendar
-from datetime import date, datetime, timedelta as td, time, timezone
+from datetime import date, datetime, time
+from datetime import timedelta as td
+from datetime import timezone
 from enum import IntEnum
-from typing import cast, Set, Tuple, Union
+from typing import Set, Tuple, Union, cast
 
 UTC = timezone.utc
 
 SpecItem = Union[int, Tuple[int, int]]
 
 RANGES = [
     range(0, 60),
@@ -126,40 +130,40 @@
 
 class CronSim(object):
     LAST = -1000
 
     def __init__(self, expr: str, dt: datetime):
         self.dt = dt.replace(second=0, microsecond=0)
 
-        parts = expr.upper().split()
-        if len(parts) != 5:
+        self.parts = expr.upper().split()
+        if len(self.parts) != 5:
             raise CronSimError("Wrong number of fields")
 
         # In Debian cron, if either the day-of-month or the day-of-week field
         # starts with a star, then there is an "AND" relationship between them.
         # Otherwise it's "OR".
-        self.day_and = parts[2].startswith("*") or parts[4].startswith("*")
+        self.day_and = self.parts[2].startswith("*") or self.parts[4].startswith("*")
 
-        self.minutes = cast(Set[int], Field.MINUTE.parse(parts[0]))
-        self.hours = cast(Set[int], Field.HOUR.parse(parts[1]))
-        self.days = cast(Set[int], Field.DAY.parse(parts[2]))
-        self.months = cast(Set[int], Field.MONTH.parse(parts[3]))
-        self.weekdays = Field.DOW.parse(parts[4])
+        self.minutes = cast(Set[int], Field.MINUTE.parse(self.parts[0]))
+        self.hours = cast(Set[int], Field.HOUR.parse(self.parts[1]))
+        self.days = cast(Set[int], Field.DAY.parse(self.parts[2]))
+        self.months = cast(Set[int], Field.MONTH.parse(self.parts[3]))
+        self.weekdays = Field.DOW.parse(self.parts[4])
 
         if len(self.days) and min(self.days) > 29:
             # Check if we have any month with enough days
             if min(self.days) > max(DAYS_IN_MONTH[month] for month in self.months):
                 raise CronSimError(Field.DAY.msg())
 
         self.fixup_tz = None
         if self.dt.tzinfo in (None, UTC):
             # No special DST handling for UTC
             pass
         else:
-            if not parts[0].startswith("*") and not parts[1].startswith("*"):
+            if not self.parts[0].startswith("*") and not self.parts[1].startswith("*"):
                 # Will use special handling for jobs that run at specific time, or
                 # with a granularity greater than one hour (to mimic Debian cron).
                 self.fixup_tz = self.dt.tzinfo
                 self.dt = self.dt.replace(tzinfo=None)
 
     def tick(self, minutes: int = 1) -> None:
         """Roll self.dt forward by 1 or more minutes and fix timezone."""
@@ -323,7 +327,12 @@
                 while is_imaginary(result):
                     self.dt += td(minutes=1)
                     result = self.dt.replace(tzinfo=self.fixup_tz)
 
                 return result
 
             return self.dt
+
+    def explain(self) -> str:
+        from cronsim.explain import Expression
+
+        return Expression(self.parts).explain()
```

### Comparing `cronsim-2.3/cronsim.egg-info/PKG-INFO` & `cronsim-2.4/cronsim.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cronsim
-Version: 2.3
+Version: 2.4
 Summary: Cron expression parser and evaluator
 Home-page: https://github.com/cuu508/cronsim
 Author: Pēteris Caune
 Author-email: cuu508@gmail.com
 License: BSD
 Project-URL: Changelog, https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md
 Keywords: cron,cronjob,crontab,schedule
@@ -12,23 +12,23 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >= 3.7
+Requires-Python: >= 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CronSim
 
 [![Tests](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml/badge.svg)](https://github.com/cuu508/cronsim/actions/workflows/pytest.yml)
 
-Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.7+.
+Cron Sim(ulator), a cron expression parser and evaluator. Works with Python 3.8+.
 CronSim is written for and being used in
 [Healthchecks](https://github.com/healthchecks/healthchecks/)
 (a cron job monitoring service).
 
 Development priorities:
 
 * Correctness. CronSim tries to match Debian's cron as closely as possible,
@@ -138,7 +138,31 @@
 
 **Nth weekday of month**: support for "{weekday}#{nth}" syntax.
 For example, "MON#1" means "first Monday of the month", "MON#2" means "second Monday
 of the month".
 
 Example: `0 0 * * MON#1` (at midnight of the first monday of every month).
 
+## The `explain()` Method
+
+Starting from version 2.4, the CronSim objects have an `explain()` method
+which generates a text description of the supplied cron expression.
+
+```python
+from datetime import datetime
+from cronsim import CronSim
+
+expr = CronSim("*/5 9-17 * * *", datetime.now())
+print(expr.explain())
+```
+
+Outputs:
+
+```
+Every 5th minute from 9:00 through 17:59
+```
+
+The text descriptions are available in English only. The text descriptions
+use the 24-hour time format ("23:00" instead of "11:00 PM").
+
+For examples of generated descriptions see `tests/test_explain.py`.
+
```

### Comparing `cronsim-2.3/setup.py` & `cronsim-2.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # coding: utf-8
 
+from __future__ import annotations
+
 from setuptools import find_packages, setup
 
 setup(
     name="cronsim",
-    version="2.3",
+    version="2.4",
     url="https://github.com/cuu508/cronsim",
     license="BSD",
     author="Pēteris Caune",
     author_email="cuu508@gmail.com",
     description="Cron expression parser and evaluator",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords="cron,cronjob,crontab,schedule",
     packages=find_packages(),
     include_package_data=True,
     platforms="any",
-    python_requires=">= 3.7",
+    python_requires=">= 3.8",
     zip_safe=False,
     project_urls={
         "Changelog": "https://github.com/cuu508/cronsim/blob/main/CHANGELOG.md"
     },
     classifiers=[
         # As from http://pypi.python.org/pypi?%3Aaction=list_classifiers
         # 'Development Status :: 1 - Planning',
```

