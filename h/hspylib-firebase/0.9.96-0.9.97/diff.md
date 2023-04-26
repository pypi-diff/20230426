# Comparing `tmp/hspylib-firebase-0.9.96.tar.gz` & `tmp/hspylib-firebase-0.9.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-firebase-0.9.96.tar", last modified: Wed Apr 19 19:04:54 2023, max compression
+gzip compressed data, was "hspylib-firebase-0.9.97.tar", last modified: Tue Apr 25 19:08:15 2023, max compression
```

## Comparing `hspylib-firebase-0.9.96.tar` & `hspylib-firebase-0.9.97.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.250276 hspylib-firebase-0.9.96/
--rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.96/MANIFEST.in
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-19 19:04:54.249626 hspylib-firebase-0.9.96/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/README.md
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.222685 hspylib-firebase-0.9.96/firebase/
--rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/.version
--rw-r--r--   0 hjunior    (504) staff       (20)      722 2022-12-23 00:36:53.000000 hspylib-firebase-0.9.96/firebase/__classpath__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      221 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/__main__.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.232660 hspylib-firebase-0.9.96/firebase/core/
--rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/core/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     6536 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/agent_config.py
--rw-r--r--   0 hjunior    (504) staff       (20)     5008 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/file_processor.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2946 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/firebase.py
--rw-r--r--   0 hjunior    (504) staff       (20)     2608 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/core/firebase_auth.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.236900 hspylib-firebase-0.9.96/firebase/domain/
--rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/domain/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)     3338 2023-04-18 23:04:54.000000 hspylib-firebase-0.9.96/firebase/domain/firebase_dto.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.241230 hspylib-firebase-0.9.96/firebase/exception/
--rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-04-19 19:04:53.000000 hspylib-firebase-0.9.96/firebase/exception/__init__.py
--rw-r--r--   0 hjunior    (504) staff       (20)      765 2022-12-22 23:12:20.000000 hspylib-firebase-0.9.96/firebase/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.242463 hspylib-firebase-0.9.96/firebase/resources/
--rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.96/firebase/resources/application.properties
--rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.96/firebase/welcome.txt
-drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-19 19:04:54.248703 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/
--rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/requires.txt
--rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-04-19 19:04:54.000000 hspylib-firebase-0.9.96/hspylib_firebase.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-19 19:04:54.250390 hspylib-firebase-0.9.96/setup.cfg
--rw-r--r--   0 hjunior    (504) staff       (20)     1865 2023-04-05 21:45:47.000000 hspylib-firebase-0.9.96/setup.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.760093 hspylib-firebase-0.9.97/
+-rw-r--r--   0 hjunior    (504) staff       (20)       95 2022-06-17 15:16:57.000000 hspylib-firebase-0.9.97/MANIFEST.in
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-25 19:08:15.759235 hspylib-firebase-0.9.97/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      708 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/README.md
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.718462 hspylib-firebase-0.9.97/firebase/
+-rw-r--r--   0 hjunior    (504) staff       (20)        6 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/.version
+-rw-r--r--   0 hjunior    (504) staff       (20)      722 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.97/firebase/__classpath__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      186 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4427 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.97/firebase/__main__.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.730540 hspylib-firebase-0.9.97/firebase/core/
+-rw-r--r--   0 hjunior    (504) staff       (20)      226 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/core/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     6370 2023-04-25 19:05:44.000000 hspylib-firebase-0.9.97/firebase/core/agent_config.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     4926 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/core/file_processor.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2923 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/core/firebase.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     2644 2023-04-25 19:05:08.000000 hspylib-firebase-0.9.97/firebase/core/firebase_auth.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.736912 hspylib-firebase-0.9.97/firebase/domain/
+-rw-r--r--   0 hjunior    (504) staff       (20)      172 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/domain/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)     3171 2023-04-19 22:17:54.000000 hspylib-firebase-0.9.97/firebase/domain/firebase_dto.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.742195 hspylib-firebase-0.9.97/firebase/exception/
+-rw-r--r--   0 hjunior    (504) staff       (20)      173 2023-04-25 19:08:14.000000 hspylib-firebase-0.9.97/firebase/exception/__init__.py
+-rw-r--r--   0 hjunior    (504) staff       (20)      765 2023-04-19 22:01:55.000000 hspylib-firebase-0.9.97/firebase/exception/exceptions.py
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.744469 hspylib-firebase-0.9.97/firebase/resources/
+-rw-r--r--   0 hjunior    (504) staff       (20)      130 2022-11-12 19:14:41.000000 hspylib-firebase-0.9.97/firebase/resources/application.properties
+-rw-r--r--   0 hjunior    (504) staff       (20)      237 2022-02-18 20:00:37.000000 hspylib-firebase-0.9.97/firebase/welcome.txt
+drwxr-xr-x   0 hjunior    (504) staff       (20)        0 2023-04-25 19:08:15.757868 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/
+-rw-r--r--   0 hjunior    (504) staff       (20)     1580 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/PKG-INFO
+-rw-r--r--   0 hjunior    (504) staff       (20)      647 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/SOURCES.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        1 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/dependency_links.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       73 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/requires.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)        9 2023-04-25 19:08:15.000000 hspylib-firebase-0.9.97/hspylib_firebase.egg-info/top_level.txt
+-rw-r--r--   0 hjunior    (504) staff       (20)       38 2023-04-25 19:08:15.760277 hspylib-firebase-0.9.97/setup.cfg
+-rw-r--r--   0 hjunior    (504) staff       (20)     1864 2023-04-19 22:13:48.000000 hspylib-firebase-0.9.97/setup.py
```

### Comparing `hspylib-firebase-0.9.96/PKG-INFO` & `hspylib-firebase-0.9.97/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.96
-Summary: HSPyLib - Firebase integration
+Version: 0.9.97
+Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
 Keywords: firebase,google,integration,application
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.96/README.md` & `hspylib-firebase-0.9.97/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.96/firebase/__classpath__.py` & `hspylib-firebase-0.9.97/firebase/__classpath__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase
       @file: __classpath__.py
    @created: Wed, 8 Jun 2022
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 from hspylib.core.metaclass.classpath import Classpath
 from hspylib.core.tools.commons import get_path, run_dir
 
 
 class _Classpath(Classpath):
```

### Comparing `hspylib-firebase-0.9.96/firebase/__main__.py` & `hspylib-firebase-0.9.97/firebase/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase
       @file: __main__.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-import logging as log
-import os
-import sys
-import urllib3
 from clitt.core.tui.tui_application import TUIApplication
+from firebase.__classpath__ import _Classpath
+from firebase.core.firebase import Firebase
 from hspylib.core.enums.charset import Charset
 from hspylib.core.tools.commons import syserr
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
 from textwrap import dedent
 
-from firebase.__classpath__ import _Classpath
-from firebase.core.firebase import Firebase
+import logging as log
+import os
+import sys
+import urllib3
 
 # Disable this warning because we are hitting our own database
 urllib3.disable_warnings()
 
 
 class Main(TUIApplication):
     """Firebase Agent - Manage your firebase integration"""
```

### Comparing `hspylib-firebase-0.9.96/firebase/core/agent_config.py` & `hspylib-firebase-0.9.97/firebase/core/agent_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.core
       @file: agent_config.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 import logging as log
 import os
+from collections import defaultdict
+from os.path import basename
+from typing import Any, Optional
+
 from clitt.core.tui.minput.input_validator import InputValidator
 from clitt.core.tui.minput.minput import MenuInput, minput
 from datasource.firebase.firebase_configuration import FirebaseConfiguration
 from hspylib.core.config.app_config import AppConfigs
 from hspylib.core.config.properties import Properties
 from hspylib.core.enums.charset import Charset
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import dirname, file_is_not_empty, sysout, touch_file
 from hspylib.core.tools.dict_tools import get_or_default_by_key
-from os.path import basename
-from requests.structures import CaseInsensitiveDict
-from typing import Any, Optional
 
 from firebase.core.firebase_auth import FirebaseAuth
 from firebase.exception.exceptions import FirebaseAuthenticationError
 
 
 class AgentConfig(metaclass=Singleton):
-    """Holds the firebase agent configurations.
-    """
+    """Holds the firebase agent configurations."""
 
     def __init__(self, filename: str) -> None:
         self.app_configs = AppConfigs(dirname(filename))
         self.firebase_configs = None
         if file_is_not_empty(self.filename):
             self._load()
             log.debug("Found and loaded a Firebase configuration: %s", self)
@@ -47,46 +47,44 @@
 
     def __repr__(self):
         return str(self)
 
     def __getitem__(self, item) -> Any:
         return self.app_configs[item]
 
-    def setup(self, load_dir: str, filename: str, config_dict: CaseInsensitiveDict) -> None:
+    def setup(self, load_dir: str, filename: str, config_dict: dict) -> None:
         """Setup firebase from a dict configuration
         :param load_dir: the directory where to load the configurations from.
         :param filename: the configuration file name.
         :param config_dict: firebase configuration dictionary.
         """
 
         user = FirebaseAuth.authenticate(config_dict["PROJECT_ID"], config_dict["UID"])
         if user:
             if user.uid != config_dict["UID"]:
                 raise FirebaseAuthenticationError(
                     f"Provided UID: {config_dict['UID']} is different from retrieved UID: {user.uid}"
                 )
             config_dict["UID"] = user.uid
-            self.firebase_configs = (
-                FirebaseConfiguration.INSTANCE or FirebaseConfiguration.of(load_dir, filename, config_dict)
+            self.firebase_configs = FirebaseConfiguration.INSTANCE or FirebaseConfiguration.of(
+                load_dir, filename, config_dict
             )
             self.firebase_configs.update(dict(config_dict))
             self._save()
         else:
             raise FirebaseAuthenticationError("Unable to authenticate to Firebase (user is None)")
 
     def prompt(self) -> None:
-        """Create a new firebase configuration by prompting the user for information.
-        """
+        """Create a new firebase configuration by prompting the user for information."""
         config = None
         if os.path.exists(self.filename):
-            with open(self.filename, "r") as fh_configs:
-                config = Properties.read_properties(fh_configs)
+            config = Properties.read_properties(self.filename)
         else:
             touch_file(self.filename)
-        config = config if config else CaseInsensitiveDict()
+        config = config.as_dict if config else defaultdict()
         sysout("%ORANGE%### Firebase setup")
         sysout("-=" * 15 + "%EOL%%%NC%")
         # fmt: off
         form_fields = MenuInput.builder() \
             .field() \
                 .label('UID') \
                 .validator(InputValidator.words()) \
@@ -123,53 +121,45 @@
             config["PROJECT_ID"] = result.project_id
             config["EMAIL"] = result.email
             config["DATABASE"] = result.database
             self.setup(dirname(self.filename), basename(self.filename), config)
 
     @property
     def filename(self) -> str:
-        """Return the configuration file.
-        """
+        """Return the configuration file."""
         file = self.app_configs["hhs.firebase.config.file"]
         return file if file else f"{os.getenv('HOME', os.getcwd())}/.firebase"
 
     @property
     def project_id(self) -> Optional[str]:
-        """Return the firebase Project ID.
-        """
+        """Return the firebase Project ID."""
         return self.firebase_configs.project_id
 
     @property
     def uid(self) -> Optional[str]:
-        """Return the firebase User ID.
-        """
+        """Return the firebase User ID."""
         return self.firebase_configs.uid
 
     @property
     def email(self) -> Optional[str]:
-        """Return the firebase user's email.
-        """
+        """Return the firebase user's email."""
         return self.firebase_configs.email
 
     @property
     def database(self) -> Optional[str]:
-        """Return the firebase project database name.
-        """
+        """Return the firebase project database name."""
         return self.firebase_configs.database
 
     def url(self, db_alias: str) -> str:
-        """Return the firebase project URL.
-        """
+        """Return the firebase project URL."""
         final_alias = db_alias.replace(".", "/")
         return self.firebase_configs.url(final_alias)
 
     def _load(self) -> None:
-        """Load configurations from file.
-        """
+        """Load configurations from file."""
         self.firebase_configs = FirebaseConfiguration.of_file(self.filename)
 
     def _save(self) -> None:
-        """Save current firebase configurations to file.
-        """
+        """Save current firebase configurations to file."""
         with open(self.filename, "w+", encoding=Charset.UTF_8.val) as f_config:
             f_config.write(str(self))
-            sysout(f"Firebase configuration saved => {self.filename} !")
+            sysout(f"%BLUE%Firebase configuration saved => {self.filename} !%NC%")
```

### Comparing `hspylib-firebase-0.9.96/firebase/core/file_processor.py` & `hspylib-firebase-0.9.97/firebase/core/file_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.core
       @file: file_processor.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import json
-import logging as log
-import os
 from abc import ABC
+from firebase.domain.firebase_dto import FirebaseDto
 from fnmatch import fnmatch
 from hspylib.core.enums.http_code import HttpCode
 from hspylib.core.preconditions import check_argument, check_not_none
 from hspylib.core.tools.commons import syserr, sysout
 from hspylib.modules.fetch.fetch import get, put
 from requests.exceptions import HTTPError
 from typing import List
 
-from firebase.domain.firebase_dto import FirebaseDto
+import json
+import logging as log
+import os
 
 
 class FileProcessor(ABC):
-    """Utility class to upload / download B64-encoded files.
-    """
+    """Utility class to upload / download B64-encoded files."""
 
     @staticmethod
     def upload_files(url: str, file_paths: List[str], glob_exp: str) -> int:
         """Upload files to URL.
         :param url: the URL to upload the files.
         :param file_paths: the file paths to be uploaded. File paths will be filtered by glob expressions.
         :param glob_exp: the GLOB expressions to filter the input files/folders.
@@ -74,19 +73,15 @@
 
     @staticmethod
     def download_files(url: str, dest_dir: str) -> int:
         """Download files from URL.
         :param url: the URL to download the files.
         :param dest_dir: the destination directory.
         """
-        check_argument(
-            dest_dir and os.path.exists(dest_dir),
-            "Unable find destination directory: {}",
-            dest_dir,
-        )
+        check_argument(dest_dir and os.path.exists(dest_dir), "Unable find destination directory: {}", dest_dir)
         sysout(f'%BLUE%Downloading files from Firebase into "{dest_dir}" ...')
         response = get(url)
         check_not_none(response)
         check_not_none(response.body)
         if response.status_code != HttpCode.OK:
             raise HTTPError(f"{response.status_code} - Unable to download from={url} with response={response}")
         dto_list = FirebaseDto.from_json(response.body)
@@ -108,17 +103,15 @@
     @staticmethod
     def _decode_and_write(dest_dir: str, *data: FirebaseDto) -> None:
         """B64-decode and write entries to a text file.
         :param dest_dir: the destination directory.
         :param data: the file content to be written.
         """
         for entry in data:
-            FirebaseDto.from_file(
-                f"{dest_dir}/{os.path.basename(entry.path)}", entry.data
-            ).decode().save()
+            FirebaseDto.from_file(f"{dest_dir}/{os.path.basename(entry.path)}", entry.data).decode().save()
         paths = ", \n  |- ".join([f.path for f in data])
         sysout(f'%EOL%%GREEN%File(s) [\n  |- {paths}\n] successfully downloaded into: "{dest_dir}"%NC%')
 
     @staticmethod
     def _create_request(entries: List[FirebaseDto]) -> str:
         """Create a Firebase request by converting a list of DTOs into JSON formatted string.
         :param entries: the file entries to be converted.
```

### Comparing `hspylib-firebase-0.9.96/firebase/core/firebase.py` & `hspylib-firebase-0.9.97/firebase/core/firebase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.core
       @file: firebase.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
-import logging as log
-import os
-from hspylib.core.preconditions import check_argument
-from typing import List
-
 from firebase.core.agent_config import AgentConfig
 from firebase.core.file_processor import FileProcessor
 from firebase.core.firebase_auth import FirebaseAuth
+from hspylib.core.preconditions import check_argument
+from typing import List
+
+import logging as log
+import os
 
 
 class Firebase:
-    """Provides the firebase application functionalities.
-    """
+    """Provides the firebase application functionalities."""
 
     def __init__(self) -> None:
         self.processor = FileProcessor()
         filename = os.environ.get(
-            "HHS_FIREBASE_CONFIG_FILE", f"{os.environ.get('HOME', os.curdir)}/firebase.properties")
+            "HHS_FIREBASE_CONFIG_FILE", f"{os.environ.get('HOME', os.curdir)}/firebase.properties"
+        )
         self.agent_config = AgentConfig(filename)
 
     def __str__(self):
         return str(self.agent_config)
 
     def setup(self) -> None:
-        """Setup a firebase configuration by creating or reading an existing configuration file.
-        """
+        """Setup a firebase configuration by creating or reading an existing configuration file."""
         self.agent_config.prompt()
         log.debug("New firebase setup: %s", self.agent_config)
 
     def upload(self, db_alias: str, file_paths: List[str], glob_exp: str) -> bool:
         """Upload files to firebase.
         :param db_alias: the firebase database alias.
         :param file_paths: the file paths to be uploaded. File paths will be filtered by glob expressions.
@@ -61,16 +60,14 @@
         """
         self._authenticate()
         url = f"{self.agent_config.url(db_alias)}.json"
         log.debug("Downloading files  alias=%s  dest_dir=%s", db_alias, dest_dir)
         return self.processor.download_files(url, dest_dir or os.environ.get("HOME")) > 0
 
     def is_configured(self) -> bool:
-        """Checks whether firebase is properly configured or not.
-        """
+        """Checks whether firebase is properly configured or not."""
         return self.agent_config is not None and self.agent_config.firebase_configs is not None
 
     def _authenticate(self) -> None:
-        """Authenticate to Firebase using the user UID.
-        """
+        """Authenticate to Firebase using the user UID."""
         configs = self.agent_config.firebase_configs
         FirebaseAuth.authenticate(configs.project_id, configs.uid)
```

### Comparing `hspylib-firebase-0.9.96/firebase/core/firebase_auth.py` & `hspylib-firebase-0.9.97/firebase/core/firebase_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.core
       @file: firebase_auth.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import firebase_admin
-import os
 from abc import ABC
+from firebase.exception.exceptions import FirebaseAuthenticationError, FirebaseException, InvalidFirebaseCredentials
 from firebase_admin import auth, credentials
 from firebase_admin.auth import UserNotFoundError, UserRecord
 from firebase_admin.exceptions import FirebaseError
 from hspylib.core.preconditions import check_not_none
 from hspylib.core.tools.commons import sysout
 from typing import Optional
 
-from firebase.exception.exceptions import FirebaseAuthenticationError, FirebaseException, InvalidFirebaseCredentials
+import firebase_admin
+import os
 
 
 class FirebaseAuth(ABC):
     """Firebase authentication utils
     Ref: https://www.youtube.com/watch?v=esqNgnayVE8
     """
 
     @staticmethod
     def _credentials(project_id: str) -> credentials.Certificate:
         """Create Firebase credentials based on the configured credentials file.
         :param project_id: the Firebase Realtime database project ID.
         """
 
-        creds_file = os.environ.get(
-            "HHS_FIREBASE_CREDS_FILE", f"{os.environ.get('HOME')}/firebase-credentials.json")
+        creds_file = os.environ.get("HHS_FIREBASE_CREDS_FILE", f"{os.environ.get('HOME')}/firebase-credentials.json")
         check_not_none(creds_file, project_id)
         try:
             creds = credentials.Certificate(creds_file.format(project_id=project_id))
         except (IOError, KeyError, ValueError) as err:
-            raise InvalidFirebaseCredentials(f"Invalid credentials or credential file \"{creds_file}\"") from err
+            raise InvalidFirebaseCredentials(f'Invalid credentials or credential file "{creds_file}"') from err
 
         return creds
 
     @staticmethod
     def authenticate(project_id: str, uid: str) -> Optional[UserRecord]:
         """Authenticate to Firebase using valid credentials.
         :param project_id: the Firebase Realtime database project ID.
         :param uid: the Firebase User ID.
         """
-
+        sysout("%BLUE%Authenticating to Firebase ...%NC%")
         firebase_admin.initialize_app(FirebaseAuth._credentials(project_id))
         try:
             if user := auth.get_user(uid):
-                sysout("%ORANGE%Firebase authentication succeeded%EOL%")
+                sysout("%GREEN%Firebase authentication succeeded!")
                 return user
-            raise FirebaseAuthenticationError(f"Failed to authenticate to Firebase. User ID \"{uid}\" not found.")
+            raise FirebaseAuthenticationError(f'Failed to authenticate to Firebase. User ID "{uid}" not found.')
         except UserNotFoundError as err:
             raise FirebaseAuthenticationError(f"Failed to authenticate to Firebase => {err}") from err
         except (ValueError, FirebaseError) as err:
             raise FirebaseException(f"An error occurred authenticating Firebase user => {err}") from err
```

### Comparing `hspylib-firebase-0.9.96/firebase/domain/firebase_dto.py` & `hspylib-firebase-0.9.97/firebase/domain/firebase_dto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,86 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.domain
       @file: firebase_dto.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
-import json
-import logging as log
-import os
 from hspylib.core.enums.charset import Charset
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.security.security import b64_decode, b64_encode
 from typing import List
 
+import json
+import logging as log
+import os
+
 
 class FirebaseDto:
-    """Represents a Firebase DTO.
-    """
+    """Represents a Firebase DTO."""
 
     @staticmethod
-    def from_file(filepath: str, contents: str | bytes, encoding: str = Charset.UTF_8.val) -> 'FirebaseDto':
+    def from_file(filepath: str, contents: str | bytes, encoding: str = Charset.UTF_8.val) -> "FirebaseDto":
         """Create a new file entry with the specified contents and expected size.
         :param filepath: the file path.
         :param contents: the file content.
         :param encoding: the file encoding type.
         """
         entry = FirebaseDto(
-            filepath,
-            len(contents),
-            str(contents, encoding=encoding) if isinstance(contents, bytes) else contents
+            filepath, len(contents), str(contents, encoding=encoding) if isinstance(contents, bytes) else contents
         )
 
         return entry
 
     @staticmethod
-    def from_json(json_string: str) -> List['FirebaseDto']:
+    def from_json(json_string: str) -> List["FirebaseDto"]:
         """Convert a JSON formatted string into a Firebase DTO.
         :param json_string: the JSON string to be converted.
         """
         json_obj = json.loads(json_string)
-        return list(map(lambda o: FirebaseDto(o['path'], o['size'], o['data'], o['modified']), json_obj))
+        return list(map(lambda o: FirebaseDto(o["path"], o["size"], o["data"], o["modified"]), json_obj))
 
     def __init__(self, file_path: str, size: int = 0, data: str = None, modified: str = None):
         self.path = file_path
         self.size = size
         self.data = data
         self.modified = modified or now()
 
     def __str__(self) -> str:
-        return str(
-            {
-                "path": self.path,
-                "data": str(self.data),
-                "size": self.size,
-                "modified": self.modified
-            }
-        )
+        return str({"path": self.path, "data": str(self.data), "size": self.size, "modified": self.modified})
 
     def load(self) -> "FirebaseDto":
-        """Loads the file contents.
-        """
+        """Loads the file contents."""
         if os.path.exists(self.path):
             with open(self.path, "r", encoding=Charset.UTF_8.val) as f_in:
                 self.data = f_in.read()
                 if (size := len(self.data)) == 0:
                     log.warning('Nothing to be loaded. File "%s" is empty', self.path)
                 self.size = size
                 return self
-        raise FileNotFoundError(f"The path \"{self.path}\" does represent an existing file!")
+        raise FileNotFoundError(f'The path "{self.path}" does represent an existing file!')
 
     def save(self) -> "FirebaseDto":
-        """Saves current DTO content (overwrites current file content).
-        """
+        """Saves current DTO content (overwrites current file content)."""
         if os.path.exists(self.path):
             with open(self.path, "w+", encoding=Charset.UTF_8.val) as f_out:
                 f_out.write(self.data)
                 f_out.flush()
                 return self
-        raise FileNotFoundError(f"File could not be save because it's path: \"{self.path}\" was not found!")
+        raise FileNotFoundError(f'File could not be save because it\'s path: "{self.path}" was not found!')
 
-    def encode(self) -> 'FirebaseDto':
-        """B64-Encode the entry contents.
-        """
+    def encode(self) -> "FirebaseDto":
+        """B64-Encode the entry contents."""
         self.data = b64_encode(self.data)
         return self
 
-    def decode(self) -> 'FirebaseDto':
-        """B64-Decode the entry contents.
-        """
+    def decode(self) -> "FirebaseDto":
+        """B64-Decode the entry contents."""
         self.data = b64_decode(self.data)
         return self
```

### Comparing `hspylib-firebase-0.9.96/firebase/exception/exceptions.py` & `hspylib-firebase-0.9.97/firebase/exception/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
    @package: firebase.exception
       @file: exceptions.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class FirebaseAuthenticationError(HSBaseException):
     """Raised when authenticate to Firebase"""
```

### Comparing `hspylib-firebase-0.9.96/hspylib_firebase.egg-info/PKG-INFO` & `hspylib-firebase-0.9.97/hspylib_firebase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: hspylib-firebase
-Version: 0.9.96
-Summary: HSPyLib - Firebase integration
+Version: 0.9.97
+Summary: HsPyLib - Firebase integration
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-firebase/
 Keywords: firebase,google,integration,application
@@ -24,12 +24,12 @@
 Description-Content-Type: text/markdown
 
 # HomeSetup - Firebase integration
 
 ## Upload and Download files to/from your firebase database
 
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v0.9.96/gray)](CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v0.9.97/gray)](CHANGELOG.md#unreleased)
 [![PyPi](https://badgen.net/badge/icon/python?icon=pypi&label)](https://pypi.org/project/hspylib-firebase)
 [![GitHub](https://badgen.net/badge/icon/github?icon=github&label)](https://github.com/yorevs/hspylib)
 [![Gitter](https://badgen.net/badge/icon/gitter?icon=gitter&label)](https://gitter.im/hspylib/community)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
```

### Comparing `hspylib-firebase-0.9.96/hspylib_firebase.egg-info/SOURCES.txt` & `hspylib-firebase-0.9.97/hspylib_firebase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hspylib-firebase-0.9.96/setup.py` & `hspylib-firebase-0.9.97/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
-   @project: HSPyLib-Firebase
+   @project: HsPyLib-Firebase
       @file: setup.py
    @created: Tue, 4 May 2021
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
       @site: https://github.com/yorevs/hspylib
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright 2022, HSPyLib team
+   Copyright 2023, HsPyLib team
 """
 
 import pathlib
-
 import setuptools
 
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
@@ -27,15 +26,15 @@
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name="hspylib-firebase",
     version=VERSION,
-    description="HSPyLib - Firebase integration",
+    description="HsPyLib - Firebase integration",
     author="Hugo Saporetti Junior",
     author_email="yorevs@hotmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
     project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-firebase/"},
     license="MIT",
```

