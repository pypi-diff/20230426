# Comparing `tmp/aiotaika-0.1.1.tar.gz` & `tmp/aiotaika-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotaika-0.1.1.tar", last modified: Wed Apr 26 07:35:00 2023, max compression
+gzip compressed data, was "aiotaika-0.1.2.tar", last modified: Wed Apr 26 09:47:25 2023, max compression
```

## Comparing `aiotaika-0.1.1.tar` & `aiotaika-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.959960 aiotaika-0.1.1/
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1687 2023-04-19 12:11:00.000000 aiotaika-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 jussi     (1000) jussi     (1000)      195 2023-04-25 12:33:57.000000 aiotaika-0.1.1/.readthedocs.yaml
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.956627 aiotaika-0.1.1/.vscode/
--rw-r--r--   0 jussi     (1000) jussi     (1000)      160 2023-04-19 07:49:27.000000 aiotaika-0.1.1/.vscode/extensions.json
--rw-r--r--   0 jussi     (1000) jussi     (1000)      262 2023-04-19 07:49:28.000000 aiotaika-0.1.1/.vscode/settings.json
--rw-r--r--   0 jussi     (1000) jussi     (1000)      172 2023-04-17 20:48:16.000000 aiotaika-0.1.1/AUTHORS.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)      343 2023-04-25 12:52:49.000000 aiotaika-0.1.1/CHANGELOG.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)    26526 2023-04-25 11:26:45.000000 aiotaika-0.1.1/LICENSE
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1659 2023-04-26 07:35:00.959960 aiotaika-0.1.1/PKG-INFO
--rw-r--r--   0 jussi     (1000) jussi     (1000)      470 2023-04-25 12:52:34.000000 aiotaika-0.1.1/README.md
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.956627 aiotaika-0.1.1/aiotaika/
--rw-r--r--   0 jussi     (1000) jussi     (1000)       14 2023-04-19 07:49:28.000000 aiotaika-0.1.1/aiotaika/.gitignore
--rw-r--r--   0 jussi     (1000) jussi     (1000)      186 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/__init__.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)      160 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika/_version.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)    15239 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/aiotaika.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1421 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/const.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)      659 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/discovery.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1154 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/entity.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)       39 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/errors.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     4809 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/events.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     3425 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/locator.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)      727 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/mqtthandler.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)    10876 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/ring.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     3556 2023-04-26 07:32:52.000000 aiotaika-0.1.1/aiotaika/utils.py
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.956627 aiotaika-0.1.1/aiotaika.egg-info/
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1659 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika.egg-info/PKG-INFO
--rw-r--r--   0 jussi     (1000) jussi     (1000)      953 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika.egg-info/SOURCES.txt
--rw-r--r--   0 jussi     (1000) jussi     (1000)        1 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika.egg-info/dependency_links.txt
--rw-r--r--   0 jussi     (1000) jussi     (1000)      204 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika.egg-info/requires.txt
--rw-r--r--   0 jussi     (1000) jussi     (1000)        9 2023-04-26 07:35:00.000000 aiotaika-0.1.1/aiotaika.egg-info/top_level.txt
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.959960 aiotaika-0.1.1/docs/
--rw-r--r--   0 jussi     (1000) jussi     (1000)        9 2023-04-25 12:40:53.000000 aiotaika-0.1.1/docs/.gitignore
--rw-r--r--   0 jussi     (1000) jussi     (1000)      634 2023-04-14 11:00:07.000000 aiotaika-0.1.1/docs/Makefile
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.959960 aiotaika-0.1.1/docs/_static/
--rw-r--r--   0 jussi     (1000) jussi     (1000)        0 2023-04-25 12:36:57.000000 aiotaika-0.1.1/docs/_static/.gitkeep
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.959960 aiotaika-0.1.1/docs/_templates/
--rw-r--r--   0 jussi     (1000) jussi     (1000)        0 2023-04-25 12:36:57.000000 aiotaika-0.1.1/docs/_templates/.gitkeep
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1451 2023-04-17 16:08:46.000000 aiotaika-0.1.1/docs/aiotaika.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)       28 2023-04-19 07:49:28.000000 aiotaika-0.1.1/docs/authors.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)       30 2023-04-19 12:20:15.000000 aiotaika-0.1.1/docs/changelog.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)      870 2023-04-19 08:02:06.000000 aiotaika-0.1.1/docs/conf.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     2873 2023-04-25 12:29:21.000000 aiotaika-0.1.1/docs/examples.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)      485 2023-04-19 12:19:59.000000 aiotaika-0.1.1/docs/index.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1280 2023-04-19 07:49:28.000000 aiotaika-0.1.1/docs/installation.rst
--rw-r--r--   0 jussi     (1000) jussi     (1000)      765 2023-04-19 07:49:28.000000 aiotaika-0.1.1/docs/make.bat
--rw-r--r--   0 jussi     (1000) jussi     (1000)       64 2023-04-25 12:33:58.000000 aiotaika-0.1.1/docs/requirements.in
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1315 2023-04-25 12:32:31.000000 aiotaika-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 07:35:00.959960 aiotaika-0.1.1/examples/
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1199 2023-04-25 11:04:50.000000 aiotaika-0.1.1/examples/async_generator_example.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1016 2023-04-19 12:14:23.000000 aiotaika-0.1.1/examples/connection_example.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1105 2023-04-19 12:14:23.000000 aiotaika-0.1.1/examples/locator_example.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1363 2023-04-20 14:56:10.000000 aiotaika-0.1.1/examples/ring_subscription_example.py
--rw-r--r--   0 jussi     (1000) jussi     (1000)     1723 2023-04-26 07:34:40.000000 aiotaika-0.1.1/pyproject.toml
--rw-r--r--   0 jussi     (1000) jussi     (1000)       38 2023-04-26 07:35:00.959960 aiotaika-0.1.1/setup.cfg
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.542985 aiotaika-0.1.2/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       27 2023-04-26 08:01:52.000000 aiotaika-0.1.2/.gitignore
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1687 2023-04-19 12:11:00.000000 aiotaika-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      195 2023-04-25 12:33:57.000000 aiotaika-0.1.2/.readthedocs.yaml
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.536318 aiotaika-0.1.2/.vscode/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      160 2023-04-19 07:49:27.000000 aiotaika-0.1.2/.vscode/extensions.json
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      262 2023-04-19 07:49:28.000000 aiotaika-0.1.2/.vscode/settings.json
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      172 2023-04-17 20:48:16.000000 aiotaika-0.1.2/AUTHORS.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      573 2023-04-26 09:45:59.000000 aiotaika-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)    26526 2023-04-25 11:26:45.000000 aiotaika-0.1.2/LICENSE
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     4799 2023-04-26 09:47:25.542985 aiotaika-0.1.2/PKG-INFO
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     3543 2023-04-26 09:39:33.000000 aiotaika-0.1.2/README.md
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.539652 aiotaika-0.1.2/aiotaika/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       14 2023-04-19 07:49:28.000000 aiotaika-0.1.2/aiotaika/.gitignore
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      542 2023-04-26 09:46:07.000000 aiotaika-0.1.2/aiotaika/__init__.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)    15595 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/aiotaika.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1778 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/const.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1015 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/discovery.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1510 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/entity.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      395 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/errors.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     5165 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/events.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     3781 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/locator.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1083 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/mqtthandler.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)    11232 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/ring.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     3912 2023-04-26 07:40:14.000000 aiotaika-0.1.2/aiotaika/utils.py
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.539652 aiotaika-0.1.2/aiotaika.egg-info/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     4799 2023-04-26 09:47:25.000000 aiotaika-0.1.2/aiotaika.egg-info/PKG-INFO
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      943 2023-04-26 09:47:25.000000 aiotaika-0.1.2/aiotaika.egg-info/SOURCES.txt
+-rw-r--r--   0 jussi     (1000) jussi     (1000)        1 2023-04-26 09:47:25.000000 aiotaika-0.1.2/aiotaika.egg-info/dependency_links.txt
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      204 2023-04-26 09:47:25.000000 aiotaika-0.1.2/aiotaika.egg-info/requires.txt
+-rw-r--r--   0 jussi     (1000) jussi     (1000)        9 2023-04-26 09:47:25.000000 aiotaika-0.1.2/aiotaika.egg-info/top_level.txt
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.539652 aiotaika-0.1.2/docs/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)        9 2023-04-25 12:40:53.000000 aiotaika-0.1.2/docs/.gitignore
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      634 2023-04-14 11:00:07.000000 aiotaika-0.1.2/docs/Makefile
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.539652 aiotaika-0.1.2/docs/_static/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)        0 2023-04-25 12:36:57.000000 aiotaika-0.1.2/docs/_static/.gitkeep
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.539652 aiotaika-0.1.2/docs/_templates/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)        0 2023-04-25 12:36:57.000000 aiotaika-0.1.2/docs/_templates/.gitkeep
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1451 2023-04-17 16:08:46.000000 aiotaika-0.1.2/docs/aiotaika.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       28 2023-04-19 07:49:28.000000 aiotaika-0.1.2/docs/authors.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       30 2023-04-19 12:20:15.000000 aiotaika-0.1.2/docs/changelog.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      870 2023-04-26 07:50:29.000000 aiotaika-0.1.2/docs/conf.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     2873 2023-04-25 12:29:21.000000 aiotaika-0.1.2/docs/examples.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      485 2023-04-19 12:19:59.000000 aiotaika-0.1.2/docs/index.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1280 2023-04-19 07:49:28.000000 aiotaika-0.1.2/docs/installation.rst
+-rw-r--r--   0 jussi     (1000) jussi     (1000)      765 2023-04-19 07:49:28.000000 aiotaika-0.1.2/docs/make.bat
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       64 2023-04-25 12:33:58.000000 aiotaika-0.1.2/docs/requirements.in
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1315 2023-04-25 12:32:31.000000 aiotaika-0.1.2/docs/requirements.txt
+drwxr-xr-x   0 jussi     (1000) jussi     (1000)        0 2023-04-26 09:47:25.542985 aiotaika-0.1.2/examples/
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1284 2023-04-26 09:39:49.000000 aiotaika-0.1.2/examples/async_generator_example.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1016 2023-04-19 12:14:23.000000 aiotaika-0.1.2/examples/connection_example.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1105 2023-04-19 12:14:23.000000 aiotaika-0.1.2/examples/locator_example.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1375 2023-04-26 09:39:49.000000 aiotaika-0.1.2/examples/ring_subscription_example.py
+-rw-r--r--   0 jussi     (1000) jussi     (1000)     1752 2023-04-26 08:02:01.000000 aiotaika-0.1.2/pyproject.toml
+-rw-r--r--   0 jussi     (1000) jussi     (1000)       38 2023-04-26 09:47:25.542985 aiotaika-0.1.2/setup.cfg
```

### Comparing `aiotaika-0.1.1/.pre-commit-config.yaml` & `aiotaika-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/LICENSE` & `aiotaika-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/aiotaika/aiotaika.py` & `aiotaika-0.1.2/aiotaika/aiotaika.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 import asyncio
 import logging
 from asyncio import AbstractEventLoop
 from collections.abc import Callable
 from contextlib import asynccontextmanager
 from types import TracebackType
 from typing import AsyncGenerator, Dict, Optional, Type
```

### Comparing `aiotaika-0.1.1/aiotaika/const.py` & `aiotaika-0.1.2/aiotaika/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,17 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 """Constants."""
+
 from typing import Final
 
 DEFAULT_DB_PORT: Final = 3306
 DEFAULT_MQTT_PORT: Final = 1883
 
 
 RING_DATA_HISTORY_LEN: Final = 100
```

### Comparing `aiotaika-0.1.1/aiotaika/entity.py` & `aiotaika-0.1.2/aiotaika/entity.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 from abc import ABC
 from enum import Enum
 
 
 class EntityType(Enum):
     """Enumerations for Taika Entity types."""
```

### Comparing `aiotaika-0.1.1/aiotaika/events.py` & `aiotaika-0.1.2/aiotaika/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 from collections.abc import Awaitable, Callable
 from dataclasses import dataclass
 from enum import Flag, auto
 from typing import Generic, TypeVar
 
 
 class EventType(Flag):
```

### Comparing `aiotaika-0.1.1/aiotaika/locator.py` & `aiotaika-0.1.2/aiotaika/locator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 from collections.abc import Awaitable, Callable
 from dataclasses import dataclass
 from typing import Any
 
 from .const import MQTT_LOCATOR_ANGLE_TOPIC, MQTT_LOCATOR_ORIENTATION_TOPIC
 from .entity import EntityType, TaikaEntity
 from .events import Event, EventBaseType, EventGenerator, EventType, Metadata
```

### Comparing `aiotaika-0.1.1/aiotaika/ring.py` & `aiotaika-0.1.2/aiotaika/ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 from collections.abc import Awaitable, Callable
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Type
 
 from .const import (
     MQTT_GESTURE_KEY,
```

### Comparing `aiotaika-0.1.1/aiotaika/utils.py` & `aiotaika-0.1.2/aiotaika/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+# Taika asynchronous client library for Python
+#    Copyright (C) 2023 Taika Tech Oy
+#    Author Jussi Hietanen
+#
+# This library is free software; you can redistribute it and/or modify it under the
+# terms of the GNU Lesser General Public License as published by the Free Software
+# Foundation. See the GNU Lesser General Public License for more details.
+
 """Utility functionality for Taika use."""
 import math
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 
 @dataclass
```

### Comparing `aiotaika-0.1.1/aiotaika.egg-info/SOURCES.txt` & `aiotaika-0.1.2/aiotaika.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+.gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 AUTHORS.rst
 CHANGELOG.rst
 LICENSE
 README.md
 pyproject.toml
 .vscode/extensions.json
 .vscode/settings.json
 aiotaika/.gitignore
 aiotaika/__init__.py
-aiotaika/_version.py
 aiotaika/aiotaika.py
 aiotaika/const.py
 aiotaika/discovery.py
 aiotaika/entity.py
 aiotaika/errors.py
 aiotaika/events.py
 aiotaika/locator.py
```

### Comparing `aiotaika-0.1.1/docs/Makefile` & `aiotaika-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/aiotaika.rst` & `aiotaika-0.1.2/docs/aiotaika.rst`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/conf.py` & `aiotaika-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/examples.rst` & `aiotaika-0.1.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/installation.rst` & `aiotaika-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/make.bat` & `aiotaika-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/docs/requirements.txt` & `aiotaika-0.1.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/examples/async_generator_example.py` & `aiotaika-0.1.2/examples/async_generator_example.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from os.path import abspath, dirname
 from sys import path
 
 path.insert(1, dirname(dirname(abspath(__file__))))
 
 from aiotaika import TaikaClient  # NOQA
-from aiotaika.ring import RingGestureEvent  # NOQA
+from aiotaika.ring import RingMoveEvent  # NOQA
 
 parser = argparse.ArgumentParser(description="Taika AIO library example")
 parser.add_argument("host", help="hostname of Taika centralunit")
 parser.add_argument("username", help="Username for centralunit login")
 parser.add_argument("password", help="Password for centralunit login")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
@@ -24,15 +24,16 @@
             format="%(asctime)-15s %(levelname)-5s %(name)s -- %(message)s",
         )
     async with TaikaClient(
         host=args.host, username=args.username, password=args.password
     ) as taika:
         async with taika.events() as events:
             async for event in events:
-                if isinstance(event, RingGestureEvent):
-                    print(event.gesture)
+                if isinstance(event, RingMoveEvent):
+                    print(f"x: {event.position.x}, z: {event.position.z}")
+                    print(f"height: {event.position.y}")
 
 
 try:
     asyncio.run(main())
 except KeyboardInterrupt:
     pass
```

### Comparing `aiotaika-0.1.1/examples/connection_example.py` & `aiotaika-0.1.2/examples/connection_example.py`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/examples/locator_example.py` & `aiotaika-0.1.2/examples/locator_example.py`

 * *Files identical despite different names*

### Comparing `aiotaika-0.1.1/examples/ring_subscription_example.py` & `aiotaika-0.1.2/examples/ring_subscription_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 parser.add_argument("host", help="hostname of Taika centralunit")
 parser.add_argument("username", help="Username for centralunit login")
 parser.add_argument("password", help="Password for centralunit login")
 parser.add_argument("--debug", help="enable debug logging", action="store_true")
 args = parser.parse_args()
 
 
-async def my_cb(event: RingMoveEvent) -> None:
+async def my_callback(event: RingMoveEvent) -> None:
     print(event.position)
 
 
 async def main() -> None:
     if args.debug:
         logging.basicConfig(
             level=logging.DEBUG,
@@ -30,15 +30,15 @@
         )
     async with TaikaClient(
         host=args.host, username=args.username, password=args.password
     ) as taika:
         rings = taika.rings
         for key, ring in rings.items():
             print("{}: {}".format(key, ring.metadata))
-        await rings[3].register_event_cb(EventType.RING_MOVE_EVT, my_cb)
+        await rings[3].register_event_cb(EventType.RING_MOVE_EVT, my_callback)
         await asyncio.sleep(5)
 
 
 try:
     asyncio.run(main())
 except KeyboardInterrupt:
     pass
```

### Comparing `aiotaika-0.1.1/pyproject.toml` & `aiotaika-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -32,18 +32,19 @@
     "asyncio_mqtt>=0.16.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source code" = "https://github.com/Taika-Tech/aiotaika-python"
 "Issue tracker" = "https://github.com/Taika-Tech/aiotaika-python/issues"
+"Documentation" = "https://aiotaika-python.readthedocs.io"
 
 [project.optional-dependencies]
 lint = ["mypy>=1.2.0", "ruff==0.0.261", "markdownlint>=0.12.0"]
 format = ["black>=23.3.0", "flake8>=6.0.0", "bandit>=1.7.4", "isort>=5.12.0"]
 docs = ["sphinx>=5.3.0", "sphinx-rtd-theme>=1.2.0"]
 
 [tool.setuptools] # https://setuptools.pypa.io/en/latest/userguide/package_discovery.html
 packages = ["aiotaika"]
 
-[tool.setuptools_scm] # https://github.com/pypa/setuptools_scm/
-write_to = "aiotaika/_version.py"
+[tool.setuptools.dynamic]
+version = {attr = "aiotaika.__version__"}
```

