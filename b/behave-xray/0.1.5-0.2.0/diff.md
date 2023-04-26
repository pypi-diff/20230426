# Comparing `tmp/behave_xray-0.1.5-py3-none-any.whl.zip` & `tmp/behave_xray-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,17 @@
-Zip file size: 13521 bytes, number of entries: 12
--rw-r--r--  2.0 unx       71 b- defN 22-Oct-22 15:16 behave_xray/__init__.py
--rw-r--r--  2.0 unx     1764 b- defN 22-Oct-22 16:24 behave_xray/authentication.py
+Zip file size: 15613 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      129 b- defN 23-Apr-25 14:09 behave_xray/__init__.py
+-rw-r--r--  2.0 unx     1765 b- defN 23-Apr-04 19:53 behave_xray/authentication.py
+-rw-r--r--  2.0 unx     1625 b- defN 23-Apr-25 16:01 behave_xray/evidence.py
 -rw-r--r--  2.0 unx      137 b- defN 22-Oct-09 13:17 behave_xray/exceptions.py
--rw-r--r--  2.0 unx     8507 b- defN 22-Nov-01 13:13 behave_xray/formatter.py
--rw-r--r--  2.0 unx     1674 b- defN 22-Nov-01 13:13 behave_xray/helper.py
--rw-r--r--  2.0 unx     4304 b- defN 22-Oct-22 18:31 behave_xray/model.py
--rw-r--r--  2.0 unx     2749 b- defN 22-Oct-22 16:24 behave_xray/xray_publisher.py
--rw-r--r--  2.0 unx    11357 b- defN 22-Nov-01 13:14 behave_xray-0.1.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     4159 b- defN 22-Nov-01 13:14 behave_xray-0.1.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Nov-01 13:14 behave_xray-0.1.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-Nov-01 13:14 behave_xray-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      974 b- defN 22-Nov-01 13:14 behave_xray-0.1.5.dist-info/RECORD
-12 files, 35800 bytes uncompressed, 11887 bytes compressed:  66.8%
+-rw-r--r--  2.0 unx    10199 b- defN 23-Apr-25 14:09 behave_xray/formatter.py
+-rw-r--r--  2.0 unx     1866 b- defN 23-Apr-25 14:09 behave_xray/helper.py
+-rw-r--r--  2.0 unx      239 b- defN 23-Mar-19 17:44 behave_xray/hookimpl.py
+-rw-r--r--  2.0 unx      239 b- defN 23-Apr-25 14:09 behave_xray/hookspecs.py
+-rw-r--r--  2.0 unx     4458 b- defN 23-Apr-25 14:09 behave_xray/model.py
+-rw-r--r--  2.0 unx     2798 b- defN 23-Apr-25 14:09 behave_xray/xray_publisher.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4698 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1215 b- defN 23-Apr-25 16:02 behave_xray-0.2.0.dist-info/RECORD
+15 files, 40829 bytes uncompressed, 13611 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -1,37 +1,46 @@
 Filename: behave_xray/__init__.py
 Comment: 
 
 Filename: behave_xray/authentication.py
 Comment: 
 
+Filename: behave_xray/evidence.py
+Comment: 
+
 Filename: behave_xray/exceptions.py
 Comment: 
 
 Filename: behave_xray/formatter.py
 Comment: 
 
 Filename: behave_xray/helper.py
 Comment: 
 
+Filename: behave_xray/hookimpl.py
+Comment: 
+
+Filename: behave_xray/hookspecs.py
+Comment: 
+
 Filename: behave_xray/model.py
 Comment: 
 
 Filename: behave_xray/xray_publisher.py
 Comment: 
 
-Filename: behave_xray-0.1.5.dist-info/LICENSE
+Filename: behave_xray-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: behave_xray-0.1.5.dist-info/METADATA
+Filename: behave_xray-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: behave_xray-0.1.5.dist-info/WHEEL
+Filename: behave_xray-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: behave_xray-0.1.5.dist-info/top_level.txt
+Filename: behave_xray-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: behave_xray-0.1.5.dist-info/RECORD
+Filename: behave_xray-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## behave_xray/__init__.py

```diff
@@ -1 +1,6 @@
-from .formatter import XrayFormatter, XrayCloudFormatter  # noqa: F401
+import pluggy
+
+from .formatter import XrayCloudFormatter, XrayFormatter  # noqa: F401
+
+
+hookimpl = pluggy.HookimplMarker('xray')
```

## behave_xray/authentication.py

```diff
@@ -2,14 +2,15 @@
 import logging
 
 import requests
 from requests.auth import AuthBase
 
 from behave_xray.exceptions import XrayError
 
+
 _logger = logging.getLogger(__name__)
 
 
 class PersonalAccessTokenAuth(AuthBase):
     """Personal access token authentication."""
 
     def __init__(self, token: str) -> None:
```

## behave_xray/formatter.py

```diff
@@ -1,39 +1,72 @@
 from collections import defaultdict
 from dataclasses import dataclass, field
+from enum import Enum, auto
+import importlib
 from os import environ, getenv
-from typing import Dict, List, Optional
+from typing import AnyStr, Dict, List, Optional, Tuple, Union
 
+import pluggy
 from behave.formatter.base import Formatter
+from behave.model import Feature as BehaveFeature
+from behave.model import Scenario as BehaveScenario
+from behave.model import ScenarioOutline as BehaveScenarioOutline
 from behave.model import Status
 
-from behave_xray.authentication import BearerAuth, PersonalAccessTokenAuth
+from behave_xray import hookspecs
+from behave_xray.authentication import AuthBase, BearerAuth, PersonalAccessTokenAuth
 from behave_xray.exceptions import XrayError
 from behave_xray.helper import (
+    get_overall_status,
     get_test_execution_key_from_tag,
     get_test_plan_key_from_tag,
     get_testcase_key_from_tag,
-    get_overall_status
 )
-from behave_xray.model import TestExecution, TestCase, TestCaseCloud
+from behave_xray.model import TestCase, TestCaseCloud, TestExecution
 from behave_xray.xray_publisher import (
-    XrayPublisher,
     TEST_EXECUTION_ENDPOINT,
-    TEST_EXECUTION_ENDPOINT_CLOUD
+    TEST_EXECUTION_ENDPOINT_CLOUD,
+    XrayPublisher,
 )
 
 
+class AuthType(Enum):
+    bearer = auto()  # client id & client secret
+    token = auto()
+    basic = auto()
+
+
 @dataclass
-class ScenarioOutline:
-    """Class store Scenario Outline information."""
+class JiraConfig:
+    jira_url: str
+    user_name: str = ''
+    user_password: str = ''
+    client_id: str = ''
+    client_secret: str = ''
+    token: str = ''
+
+    @property
+    def auth_method(self) -> AuthType:
+        if self.client_id and self.client_id:
+            return AuthType.bearer
+        if self.token:
+            return AuthType.token
+        else:
+            return AuthType.basic
+
+
+@dataclass
+class ScenarioResult:
+    """Class stores scenario result."""
 
     testcase_key: Optional[str] = None
     statuses: List[Status] = field(default_factory=list)
     comment: str = ''
     is_outline: bool = False
+    evidences: List[Dict[str, AnyStr]] = field(default_factory=list)
 
 
 @dataclass
 class Verdict:
     status: Status
     message: str
 
@@ -42,39 +75,56 @@
     name = 'xray'
     description = 'Jira XRAY formatter'
 
     STATUS_MAPS: Dict[str, str] = {}
 
     def __init__(self, stream, config, publisher: XrayPublisher):
         super().__init__(stream, config)
+        self.pm = self._get_plugin_manager()
+        self._register_user_hook()
         self.xray_publisher = publisher
-        self.current_feature = None
-        self.current_scenario = None
-        self.current_test_key = None
+        self.current_feature: Optional[BehaveFeature] = None
+        self.current_scenario: Optional[BehaveScenario] = None
+        self.current_test_key: Optional[str] = None
         self.test_execution: TestExecution = TestExecution(
             summary=self._get_summary(),
             user=self._get_user(),
             revision=self._get_revision(),
             version=self._get_version()
         )
-        self.testcases: dict = defaultdict(lambda: ScenarioOutline())
+        # store Jira Xray test ID with corresponding Behave's scenario
+        self.testcases: Dict[str, ScenarioResult] = defaultdict(lambda: ScenarioResult())
+
+    def _get_plugin_manager(self):
+        pm = pluggy.PluginManager('xray')
+        pm.add_hookspecs(hookspecs)
+        return pm
+
+    def _register_user_hook(self):
+        try:
+            module_name = str(self.config.environment_file).split('.')[0]
+        except KeyError:
+            return
+        try:
+            self.pm.register(importlib.import_module(module_name))
+        except ImportError:
+            pass
 
     @staticmethod
-    def _get_auth(jira_config):
-        if jira_config.auth_method == 'bearer':
-            auth = BearerAuth(
+    def _get_auth(jira_config: JiraConfig) -> Union[Tuple[str, str], AuthBase]:
+        if jira_config.auth_method == AuthType.bearer:
+            return BearerAuth(
                 base_url=jira_config.jira_url,
                 client_id=jira_config.client_id,
                 client_secret=jira_config.client_secret
             )
-        elif jira_config.auth_method == 'token':
-            auth = PersonalAccessTokenAuth(token=jira_config.token)
-        else:
-            auth = (jira_config.user_name, jira_config.user_password)
-        return auth
+        elif jira_config.auth_method == AuthType.token:
+            return PersonalAccessTokenAuth(token=jira_config.token)
+        else:  # basic
+            return (jira_config.user_name, jira_config.user_password)
 
     def _get_summary(self) -> str:
         return self.config.userdata.get('xray.summary', '')
 
     def _get_user(self) -> str:
         return self.config.userdata.get('xray.user', '')
 
@@ -85,15 +135,15 @@
         return self.config.userdata.get('xray.version', '')
 
     def reset(self):
         self.current_feature = None
         self.current_scenario = None
         self.current_test_key = None
         self.test_execution = TestExecution()
-        self.testcases = defaultdict(lambda: ScenarioOutline())
+        self.testcases = defaultdict(lambda: ScenarioResult())
 
     def feature(self, feature):
         self.current_feature = feature
 
         # description is a mandatory Xray field, use feature name if it doesn't have a description
         description_text = '\n'.join(feature.description) if feature.description else feature.name
         self.test_execution.description = description_text
@@ -102,18 +152,19 @@
             if test_exec_key:
                 self.test_execution.test_execution_key = test_exec_key
             test_plan_key = get_test_plan_key_from_tag(tag)
             if test_plan_key:
                 self.test_execution.test_plan_key = test_plan_key
 
     def is_scenario_outline(self):
-        return True if 'Scenario Outline' in self.current_scenario.keyword else False
+        return isinstance(self.current_scenario, BehaveScenarioOutline)
 
     def scenario(self, scenario):
         self.current_scenario = scenario
+        self.current_test_key = None
         if not scenario.tags:
             return
 
         for tag in scenario.tags:
             testcase_key = get_testcase_key_from_tag(tag)
             if testcase_key:
                 self.current_test_key = testcase_key
@@ -131,49 +182,63 @@
             verdict.message = step.error_message
         if step.status == Status.untested:
             verdict.message = 'Untested'
         if step.status == Status.skipped:
             verdict.message = self.current_scenario.skip_reason
         return verdict
 
+    @property
+    def current_test_case(self) -> ScenarioResult:
+        try:
+            return self.testcases[self.current_test_key]
+        except KeyError:
+            return None
+
     def result(self, step):
         if self.current_scenario.status == Status.untested:
             return
 
         if self.current_test_key is None:
             return
 
         verdict = self.get_verdict(step)
-        self.testcases[self.current_test_key].statuses.append(verdict.status)
+        self.current_test_case.statuses.append(verdict.status)
+        self.pm.hook.scenario_xray_result(
+            result=self.current_test_case,
+            scenario=self.current_scenario
+        )
         if not self.is_scenario_outline():
-            self.testcases[self.current_test_key].comment = verdict.message
+            self.current_test_case.comment = verdict.message
 
     @staticmethod
     def _get_test_case(test_key) -> TestCase:
         return TestCase(test_key=test_key)
 
     def eof(self) -> None:
+        # run when current feature is done
         if self.config.dry_run:
             return
 
         self.collect_tests()
         if self.test_execution.tests:
             self.xray_publisher.publish(self.test_execution.as_dict())
         self.test_execution.flush()
         self.reset()
 
     def collect_tests(self) -> None:
+        """Update test execution with test cases."""
         for tc_id, tc_status in self.testcases.items():
             testcase = self._get_test_case(test_key=tc_id)
             if tc_status.is_outline:
                 testcase.status = self._get_xray_status(get_overall_status(tc_status.statuses).name)
                 testcase.examples = [self._get_xray_status(s.name) for s in tc_status.statuses]
             else:
                 testcase.status = self._get_xray_status(tc_status.statuses[0].name)
                 testcase.comment = tc_status.comment
+            testcase.evidences = tc_status.evidences
             self.test_execution.append(testcase)
 
 
 class XrayFormatter(_XrayFormatterBase):
     """Formatter publish test results to Jira Xray."""
     endpoint: str = TEST_EXECUTION_ENDPOINT
 
@@ -213,34 +278,16 @@
         super().__init__(stream, config, publisher)
 
     @staticmethod
     def _get_test_case(test_key):
         return TestCaseCloud(test_key=test_key)
 
 
-@dataclass
-class JiraConfig:
-    jira_url: str
-    user_name: str = ''
-    user_password: str = ''
-    client_id: str = ''
-    client_secret: str = ''
-    token: str = ''
-
-    @property
-    def auth_method(self) -> str:
-        if self.client_id and self.client_id:
-            return 'bearer'  # client id & client secret
-        if self.token:
-            return 'token'
-        else:
-            return 'basic'
-
-
 def _get_jira_config() -> JiraConfig:
+    """Return jira configuration from env variables."""
     try:
         jira_url = environ['XRAY_API_BASE_URL']
     except KeyError:
         raise XrayError('Environment variable `XRAY_API_BASE_URL` must be set')
     user_name = getenv('XRAY_API_USER', '')
     user_password = getenv('XRAY_API_PASSWORD', '')
     client_id = getenv('XRAY_CLIENT_ID', '')
```

## behave_xray/helper.py

```diff
@@ -1,30 +1,33 @@
 import re
 from typing import List, Optional
 
 from behave.model import Status
 
 
 def get_test_execution_key_from_tag(tag: str) -> Optional[str]:
+    """Return Jira Xray test execution ID or None if not defined."""
     match = re.match(r"^jira\.test_execution\('(.+)'\)$", tag, flags=re.IGNORECASE)
     if match:
         return match.group(1)
     else:
         return None
 
 
 def get_test_plan_key_from_tag(tag: str) -> Optional[str]:
+    """Return Jira Xray test plan ID or None if not defined."""
     match = re.match(r"^jira\.test_plan\('(.+)'\)$", tag, flags=re.IGNORECASE)
     if match:
         return match.group(1)
     else:
         return None
 
 
 def get_testcase_key_from_tag(tag: str) -> Optional[str]:
+    """Return Jira Xray test ID or None if not defined."""
     match = re.match(r"^(allure|jira)\.testcase\(['\"](.+)['\"]\)$", tag, flags=re.IGNORECASE)
     if match:
         return match.group(2)
     # for outline scenario
     match = re.match(r'^(allure|jira)\.testcase(.+)$', tag, flags=re.IGNORECASE)
     if match:
         return match.group(2)
```

## behave_xray/model.py

```diff
@@ -1,53 +1,49 @@
 import datetime as dt
-from typing import (
-    Any,
-    Dict,
-    List,
-    Optional,
-    Union,
-)
+from typing import Any, AnyStr, Dict, List, Optional, Union
 
 
 DATETIME_FORMAT: str = '%Y-%m-%dT%H:%M:%S%z'
 DEFAULT_SUMMARY: str = 'Execution of automated tests'
 
 
 class TestCase:
     """Class represents Test Case."""
+
     VALID_STATUSES = (
         'TODO',
         'ABORTED',
         'PASS',
         'FAIL',
         'EXECUTING',
         'PENDING',
         'BLOCKED'
     )
 
     def __init__(
-            self,
-            test_key: str = '',
-            status: str = 'TODO',
-            comment: str = '',
-            examples: Optional[List[str]] = None,
-            duration: float = 0.0,
+        self,
+        test_key: str = '',
+        status: str = 'TODO',
+        comment: str = '',
+        examples: Optional[List[str]] = None,
+        duration: float = 0.0,
     ):
         """
         :param test_key: Test Case ID
         :param status: Status
         :param comment: Comment
         :param examples: Outline tests results
         :param duration: Duration
         """
         self.test_key = test_key
         self.status = status
         self.comment = comment
         self.examples = examples or []
         self.duration = duration
+        self.evidences: List[Dict[str, AnyStr]] = []
 
     def __repr__(self):
         return f"{self.__class__.__name__}(test_key='{self.test_key}', status='{self.status}')"
 
     @property
     def status(self):
         return self._status
@@ -57,22 +53,25 @@
         self._validate_status(value)
         self._status = value
 
     def _validate_status(self, status: str):
         if status not in self.VALID_STATUSES:
             raise ValueError(f'Status must be one of {", ".join(self.VALID_STATUSES)}, but was {status}')
 
-    def as_dict(self) -> Dict[str, str]:
+    def as_dict(self) -> Dict[str, Any]:
         """Serialize Test Case."""
-        return dict(
+        data: Dict[str, Any] = dict(
             testKey=self.test_key,
             status=self.status,
             comment=self.comment,
             examples=self.examples
         )
+        if self.evidences:
+            data['evidences'] = self.evidences
+        return data
 
 
 class TestCaseCloud(TestCase):
     """Class represents Test Case."""
 
     VALID_STATUSES = (
         'TODO',
@@ -82,25 +81,26 @@
         'EXECUTING',
         'PENDING',
         'BLOCKED'
     )
 
 
 class TestExecution:
+    """Class stores information about test execution and tests."""
 
     def __init__(
-            self,
-            test_execution_key: str = '',
-            test_plan_key: str = '',
-            user: str = '',
-            revision: str = '',
-            version: str = '',
-            summary: str = '',
-            description: str = '',
-            tests: Optional[List[TestCase]] = None
+        self,
+        test_execution_key: str = '',
+        test_plan_key: str = '',
+        user: str = '',
+        revision: str = '',
+        version: str = '',
+        summary: str = '',
+        description: str = '',
+        tests: Optional[List[TestCase]] = None
     ):
         """
         :param test_execution_key: Test execution Xray ID
         :param test_plan_key: Test plan Xray ID
         :param user: Xray user
         :param revision: Revision
         :param version: Version
```

## behave_xray/xray_publisher.py

```diff
@@ -1,22 +1,24 @@
 import logging
-from typing import Union, Tuple
+from typing import Tuple, Union
 
 import requests
 from requests.auth import AuthBase
 
 from behave_xray.exceptions import XrayError
 
+
 TEST_EXECUTION_ENDPOINT = '/rest/raven/2.0/import/execution'
 TEST_EXECUTION_ENDPOINT_CLOUD = '/api/v2/import/execution'
 
 _logger = logging.getLogger(__name__)
 
 
 class XrayPublisher:
+    """Sends Xray report to the Jira server."""
 
     def __init__(self, base_url: str, endpoint: str, auth: Union[AuthBase, Tuple[str, str]]) -> None:
         if base_url.endswith('/'):
             base_url = base_url[:-1]
         self.base_url = base_url
         self.endpoint = endpoint
         self.auth = auth
```

## Comparing `behave_xray-0.1.5.dist-info/LICENSE` & `behave_xray-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `behave_xray-0.1.5.dist-info/METADATA` & `behave_xray-0.2.0.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: behave-xray
-Version: 0.1.5
+Version: 0.2.0
 Summary: Behave JIRA XRAY results uploader
 Home-page: https://github.com/fundakol/behave-xray
 Author: Lukasz Fundakowski
 Author-email: fundakol@yahoo.com
 Keywords: behave JIRA XRAY
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: behave
+Requires-Dist: pluggy
 Requires-Dist: requests
 
 # behave-xray
 
 [![PyPi](https://img.shields.io/pypi/v/behave-xray.png)](https://pypi.python.org/pypi/behave-xray)
 [![Build Status](https://github.com/fundakol/behave-xray/actions/workflows/main.yml/badge.svg?branch=master)](https://github.com/fundakol/behave-xray/actions?query=workflow?master)
 [![codecov](https://codecov.io/gh/fundakol/behave-xray/branch/master/graph/badge.svg?token=VV1DMT3605)](https://codecov.io/gh/fundakol/behave-xray)
@@ -132,14 +134,30 @@
 ```
 
 and use with shorter name:
 ```shell
 $ behave --f xray
 ```
 
+### Attach an evidence to the scenario
+
+One can implement `scenario_xray_result` hook to update results for a scenario.
+
+```python
+# - FILE: environment.py
+from behave.model import Status
+from behave_xray import hookimpl
+from behave_xray.evidence import text
+
+@hookimpl
+def scenario_xray_result(result, scenario):
+    if scenario.status == Status.failed:
+        result.evidences.append(text(data='This is scenario evidence', filename=f'{scenario.name}.txt'))
+```
+
 ### Customize report
 
 Add summary to a report:
 
 ```shell
 $ behave -f behave_xray:XrayCloudFormatter -D xray.summary='Report generated by behave'
 ```
@@ -148,11 +166,12 @@
 ```ini
 # -- FILE: behave.ini
 [behave.userdata]
 xray.summary = Report generated by behave
 ```
 
 Available options:
+
 * `xray.summary`
 * `xray.user`
 * `xray.version`
 * `xray.revision`
```

## Comparing `behave_xray-0.1.5.dist-info/RECORD` & `behave_xray-0.2.0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-behave_xray/__init__.py,sha256=3lYTVQ-CvIIBzYCnuQMBfLJNR_9zkmyZ1dCYPZj1HeA,71
-behave_xray/authentication.py,sha256=i5UKgFGhkWGZULyq4w8SSjk7zmSOu-xJ4o0xOq8UBDo,1764
+behave_xray/__init__.py,sha256=fH09Qs25fPbpmzvbit-j6zx0RRgPf7rnaSNCyKpzv08,129
+behave_xray/authentication.py,sha256=gC8YDPe2kgKy7s3IpG6WH_ayKAQHf2uR0AyImIvuF4k,1765
+behave_xray/evidence.py,sha256=leBrNulch6jOo-KC7j2TAhUnM3LIQw-1mTemZIDDVOA,1625
 behave_xray/exceptions.py,sha256=IS-_20kUX3rUTdg_22x5itn2rq-JgpXXO1r5BMq42Xo,137
-behave_xray/formatter.py,sha256=QwEImNMd9OvL3PKUa41zrWEWlyFjR7H4pkg2gjHbWi8,8507
-behave_xray/helper.py,sha256=rvl54osnxapdz2AjE9dYloJZtHoH52pTCTFXHk8mHUM,1674
-behave_xray/model.py,sha256=O1TQtdU0fBYmIBHrt4hz78TqxisG9QDnOhJNfPX_w5A,4304
-behave_xray/xray_publisher.py,sha256=J_0Qq-t_ticcKnb8JnB8e6IMl18CXHFgmClY_itNQPo,2749
-behave_xray-0.1.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-behave_xray-0.1.5.dist-info/METADATA,sha256=0qdsHtuirqYrUbO2_D2_MJzOJezwnx7zlgesMh2BzX8,4159
-behave_xray-0.1.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-behave_xray-0.1.5.dist-info/top_level.txt,sha256=OYIfJ2lUkKf_kjicCEoXpvVm3yp17ORgb_M-rPkX5Jg,12
-behave_xray-0.1.5.dist-info/RECORD,,
+behave_xray/formatter.py,sha256=n3o42OivmeMhvwShsoeD6VE3FXNrgIhP4wxCAMgSEhc,10199
+behave_xray/helper.py,sha256=HP5pNQL-Ya444FCctX7AVw4JLrXMHTrHurTw6XsQHOU,1866
+behave_xray/hookimpl.py,sha256=2IkfiSVg6uetFS6YWw8Uia7texma5sIkK0h5nlla_ms,239
+behave_xray/hookspecs.py,sha256=LcznKPkPTvyvb2yG3Bte3nRtXAo_krrAVV36Gr61gL8,239
+behave_xray/model.py,sha256=IXcAhABj-UAdWawrLjkQ5weYG7BrKBfPZkT8TKClHWg,4458
+behave_xray/xray_publisher.py,sha256=0GI1mF5KBlQzxb2FzJd-Pzf3E__PV2t2uLgSRBglqio,2798
+behave_xray-0.2.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+behave_xray-0.2.0.dist-info/METADATA,sha256=FtF6dNgrZD2FDF9fvnbueL4K6KNL23a3x1RrTWEEqX0,4698
+behave_xray-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+behave_xray-0.2.0.dist-info/top_level.txt,sha256=OYIfJ2lUkKf_kjicCEoXpvVm3yp17ORgb_M-rPkX5Jg,12
+behave_xray-0.2.0.dist-info/RECORD,,
```

