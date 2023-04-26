# Comparing `tmp/opentf_tools-0.39.0-py3-none-any.whl.zip` & `tmp/opentf_tools-0.40.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 36459 bytes, number of entries: 13
--rw-r--r--  2.0 unx    27029 b- defN 23-Mar-28 12:55 opentf/tools/ctl.py
--rw-r--r--  2.0 unx     7256 b- defN 23-Mar-28 12:55 opentf/tools/ctlcommons.py
--rw-r--r--  2.0 unx    29452 b- defN 23-Mar-28 12:55 opentf/tools/ctlconfig.py
--rw-r--r--  2.0 unx     8070 b- defN 23-Mar-28 12:55 opentf/tools/ctlnetworking.py
--rw-r--r--  2.0 unx    31666 b- defN 23-Mar-28 12:55 opentf/tools/ctlworkflows.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Mar-28 12:55 opentf/tools/done.py
--rw-r--r--  2.0 unx     9391 b- defN 23-Mar-28 12:55 opentf/tools/ready.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1737 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1088 b- defN 23-Mar-28 12:55 opentf_tools-0.39.0.dist-info/RECORD
-13 files, 130472 bytes uncompressed, 34643 bytes compressed:  73.4%
+Zip file size: 36828 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    27203 b- defN 23-Apr-25 14:33 opentf/tools/ctl.py
+-rw-r--r--  2.0 unx     7773 b- defN 23-Apr-25 14:33 opentf/tools/ctlcommons.py
+-rw-r--r--  2.0 unx    29452 b- defN 23-Apr-25 14:33 opentf/tools/ctlconfig.py
+-rw-r--r--  2.0 unx     8138 b- defN 23-Apr-25 14:33 opentf/tools/ctlnetworking.py
+-rw-r--r--  2.0 unx    32205 b- defN 23-Apr-25 14:33 opentf/tools/ctlworkflows.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Apr-25 14:33 opentf/tools/done.py
+-rw-r--r--  2.0 unx     9391 b- defN 23-Apr-25 14:33 opentf/tools/ready.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1737 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1088 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/RECORD
+13 files, 131770 bytes uncompressed, 35012 bytes compressed:  73.4%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: opentf/tools/done.py
 Comment: 
 
 Filename: opentf/tools/ready.py
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/LICENSE
+Filename: opentf_tools-0.40.0.dist-info/LICENSE
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/METADATA
+Filename: opentf_tools-0.40.0.dist-info/METADATA
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/WHEEL
+Filename: opentf_tools-0.40.0.dist-info/WHEEL
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/entry_points.txt
+Filename: opentf_tools-0.40.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/top_level.txt
+Filename: opentf_tools-0.40.0.dist-info/top_level.txt
 Comment: 
 
-Filename: opentf_tools-0.39.0.dist-info/RECORD
+Filename: opentf_tools-0.40.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opentf/tools/ctl.py

```diff
@@ -18,14 +18,15 @@
 from typing import Any, Dict, Iterable, List
 
 import sys
 
 import jwt
 
 from opentf.tools.ctlcommons import (
+    _make_params_from_selectors,
     _ensure_options,
     _is_command,
     _error,
     _warning,
     _get_columns,
     _emit_csv,
     _get_arg,
@@ -406,15 +407,20 @@
     # Raised exceptions
 
     Abort with an error code 1 if the orchestrator replied with a non-ok
     code.
 
     Abort with an error code 2 if another error occurred.
     """
-    what = _get(_observer(), '/channels', 'Could not get channels list')
+    what = _get(
+        _observer(),
+        '/channels',
+        'Could not get channels list',
+        params=_make_params_from_selectors(),
+    )
 
     try:
         columns = _get_columns(WIDE_CHANNEL_COLUMNS, CHANNEL_COLUMNS)
     except ValueError as err:
         _error('Invalid parameters: %s.', err)
         sys.exit(2)
     _emit_csv(_generate_channels_rows(what['details']['items'], columns), columns)
@@ -845,15 +851,17 @@
         read_configuration()
         delete_subscription(sys.argv[3])
     elif _is_command('get agents', sys.argv):
         _ensure_options(sys.argv[3:], [('--output', '-o')])
         read_configuration()
         list_agents()
     elif _is_command('get channels', sys.argv):
-        _ensure_options(sys.argv[3:], [('--output', '-o')])
+        _ensure_options(
+            sys.argv[3:], [('--output', '-o'), ('--field-selector', '--selector', '-l')]
+        )
         read_configuration()
         list_channels()
     elif _is_command('delete agent _', sys.argv):
         _ensure_options(sys.argv[4:])
         read_configuration()
         delete_agent(sys.argv[3])
     elif (
```

## opentf/tools/ctlcommons.py

```diff
@@ -248,7 +248,22 @@
     ):
         _error(
             'Parameter %s is not a valid UUID.  UUIDs should only contains '
             'digits, dashes ("-"), and lower case letters ranging from "a" to "f".',
             parameter,
         )
         sys.exit(2)
+
+
+def _make_params_from_selectors() -> dict:
+    """
+    Get selectors from command line and return parameters dictionary
+    which could then be passed in a request.
+    Currently supports two types of parameters:
+    labelSelector and fieldSelector.
+    """
+    params = {}
+    if label_selector := _get_arg('--selector=') or _get_arg('-l='):
+        params['labelSelector'] = label_selector
+    if field_selector := _get_arg('--field-selector='):
+        params['fieldSelector'] = field_selector
+    return params
```

## opentf/tools/ctlnetworking.py

```diff
@@ -102,14 +102,16 @@
 ########################################################################
 
 
 def _get(
     base_url: str,
     path: str = '',
     msg: Optional[str] = None,
+    *,
+    params=None,
     statuses=(200,),
     handler=None,
     raw: bool = False,
 ):
     """Perform a GET request.
 
     # Required parameters
@@ -125,14 +127,15 @@
     - raw: a boolean (False by default)
     """
     if msg is None:
         msg = f'Could not query {base_url}{path}'
     try:
         what = requests.get(
             base_url + path,
+            params=params,
             headers=HEADERS,
             verify=not CONFIG['orchestrator']['insecure-skip-tls-verify'],
         )
         if what.status_code in statuses:
             if not raw:
                 what = what.json()
         elif handler is not None:
@@ -169,15 +172,15 @@
     - statuses: a tuple of integers (`(200,)` by default)
     - handler: a function or None (None by default)
 
     # Returned value
 
     A dictionary.
     """
-    result = _get(base_url, path, msg, statuses, handler, raw=False)
+    result = _get(base_url, path, msg, statuses=statuses, handler=handler, raw=False)
     if not isinstance(result, dict):
         _error(
             'Internal error, was expecting a dictionary, got a %s.', result.__class__
         )
         sys.exit(2)
     return result
```

## opentf/tools/ctlworkflows.py

```diff
@@ -22,14 +22,15 @@
 import sys
 
 from time import sleep
 
 import yaml
 
 from opentf.tools.ctlcommons import (
+    _make_params_from_selectors,
     _ensure_options,
     _is_command,
     _get_arg,
     _get_columns,
     _emit_csv,
     _ensure_uuid,
     _error,
@@ -421,17 +422,21 @@
         sys.exit(2)
 
     if '--wait' in sys.argv or '--watch' in sys.argv or '-w' in sys.argv:
         url = (
             _observer()
             + f'/workflows/{result["details"]["workflow_id"]}/status?per_page=1'
         )
+        params = _make_params_from_selectors()
         sleep(WAIT_WARMUP_DELAY)
         try:
-            while _get(url, handler=lambda _: False, raw=True).status_code != 200:
+            while (
+                _get(url, params=params, handler=lambda _: False, raw=True).status_code
+                != 200
+            ):
                 sleep(WAIT_DELAY)
             get_workflow(result['details']['workflow_id'], watch=True)
         except Exception as err:
             _error('Could not show workflow execution result: %s.', err)
             sys.exit(2)
 
 
@@ -616,14 +621,15 @@
             response.text,
         )
         sys.exit(1)
 
     return _get(
         _observer(),
         f'/workflows/{workflow_id}/status',
+        params=_make_params_from_selectors(),
         handler=_handler_unknown_workflowid,
         raw=True,
     )
 
 
 def _get_outputformat(allowed: Iterable[str]) -> Optional[str]:
     """Ensure the specified format, if any, is in the allowed set."""
@@ -641,14 +647,15 @@
     return output_format
 
 
 def _get_workflow_events(workflow_id: str, watch: bool) -> Iterable[Dict[str, Any]]:
     current_item = 0
     response = _get_first_page(workflow_id)
     current_page = _observer() + f'/workflows/{workflow_id}/status'
+    params = _make_params_from_selectors()
 
     while True:
         status = response.json()
         for event in status['details']['items'][current_item:]:
             yield event
 
         if 'next' in response.links:
@@ -673,20 +680,23 @@
             break
         if response.json()['details']['status'] != 'RUNNING':
             break
 
         current_item = len(status['details']['items'])
         while len(status['details']['items']) <= current_item:
             sleep(REFRESH_DELAY)
-            response = _get(current_page, raw=True)
+            response = _get(current_page, params=params, raw=True)
             status = response.json()
             if len(status['details']['items']) != current_item:
                 break
             if 'next' in response.links:
                 break
+            if current_item == 0 and len(status['details']['items']) == 0:
+                _warning(f'Could not find items matching selectors: {params}')
+                break
 
 
 def get_workflow(workflow_id: str, watch=False) -> None:
     """Get a workflow.
 
     # Required parameters
 
@@ -933,14 +943,15 @@
             [
                 ('-e',),
                 ('-f',),
                 ('--step-depth', '--step_depth', '-s'),
                 ('--job-depth', '--job_depth', '-j'),
                 ('--max-command-length', '--max_command_length', '-c'),
                 ('--namespace', '-n'),
+                ('--selector', '-l', '--field-selector'),
             ],
             [
                 ('--wait', '--watch', '-w'),
                 ('--show-notifications', '-a'),
                 ('--verbose', '-v'),
             ],
         )
@@ -950,14 +961,15 @@
         _ensure_options(
             sys.argv[4:],
             [
                 ('--step-depth', '--step_depth', '-s'),
                 ('--job-depth', '--job_depth', '-j'),
                 ('--max-command-length', '--max_command_length', '-c'),
                 ('--output', '-o'),
+                ('--selector', '-l', '--field-selector'),
             ],
             [('--watch', '-w'), ('--show-notifications', '-a'), ('--verbose', '-v')],
         )
         read_configuration()
         get_workflow(sys.argv[3], '--watch' in sys.argv or '-w' in sys.argv)
     elif _is_command('kill workflow _', sys.argv):
         _ensure_options(sys.argv[4:])
```

## Comparing `opentf_tools-0.39.0.dist-info/LICENSE` & `opentf_tools-0.40.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opentf_tools-0.39.0.dist-info/METADATA` & `opentf_tools-0.40.0.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentf-tools
-Version: 0.39.0
+Version: 0.40.0
 Summary: OpenTestFactory Orchestrator Tools
 Home-page: https://gitlab.com/opentestfactory/tools
 Author: Martin Lafaix
 Author-email: mlafaix@henix.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

