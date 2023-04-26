# Comparing `tmp/tap-typeform-2.0.1.tar.gz` & `tmp/tap-typeform-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-typeform-2.0.1.tar", last modified: Thu Nov  3 14:44:40 2022, max compression
+gzip compressed data, was "dist/tap-typeform-2.1.0.tar", last modified: Wed Apr 26 05:22:26 2023, max compression
```

## Comparing `tap-typeform-2.0.1.tar` & `tap-typeform-2.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-03 14:44:40.018233 tap-typeform-2.0.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2022-11-03 14:44:40.018233 tap-typeform-2.0.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-11-03 14:44:40.018233 tap-typeform-2.0.1/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      837 2022-11-03 14:41:29.000000 tap-typeform-2.0.1/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-03 14:44:40.014233 tap-typeform-2.0.1/tap_typeform/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1562 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6601 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1021 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/discover.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1889 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schema.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-03 14:44:40.018233 tap-typeform-2.0.1/tap_typeform/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schemas/answers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1068 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schemas/forms.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5375 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schemas/questions.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schemas/submitted_landings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/schemas/unsubmitted_landings.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14426 2022-11-03 14:03:05.000000 tap-typeform-2.0.1/tap_typeform/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3294 2022-09-29 08:14:42.000000 tap-typeform-2.0.1/tap_typeform/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-11-03 14:44:40.018233 tap-typeform-2.0.1/tap_typeform.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      310 2022-11-03 14:44:39.000000 tap-typeform-2.0.1/tap_typeform.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2022-11-03 14:44:40.000000 tap-typeform-2.0.1/tap_typeform.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-11-03 14:44:39.000000 tap-typeform-2.0.1/tap_typeform.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2022-11-03 14:44:39.000000 tap-typeform-2.0.1/tap_typeform.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2022-11-03 14:44:39.000000 tap-typeform-2.0.1/tap_typeform.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2022-11-03 14:44:39.000000 tap-typeform-2.0.1/tap_typeform.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       52 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6601 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5375 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/questions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/answers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      777 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/unsubmitted_landings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1068 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/forms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schemas/submitted_landings.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14553 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1889 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1601 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3087 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/tap_typeform/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1021 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/tap_typeform/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       96 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       62 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      601 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       13 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/tap_typeform.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      100 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2023-04-26 05:22:26.000000 tap-typeform-2.1.0/PKG-INFO
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      837 2023-04-26 05:15:57.000000 tap-typeform-2.1.0/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3117 2022-11-02 08:28:59.000000 tap-typeform-2.1.0/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-typeform-2.0.1/LICENSE` & `tap-typeform-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/README.md` & `tap-typeform-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/setup.py` & `tap-typeform-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name="tap-typeform",
-    version="2.0.1",
+    version="2.1.0",
     description="Singer.io tap for extracting data from the TypeForm Responses API",
     author="bytcode.io",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     install_requires=[
         "singer-python==5.10.0",
         "pendulum",
```

### Comparing `tap-typeform-2.0.1/tap_typeform/__init__.py` & `tap-typeform-2.1.0/tap_typeform/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 #!/usr/bin/env python3
 import singer
 from singer import utils
 from tap_typeform.discover import discover as _discover
-from tap_typeform.sync import _forms_to_list, sync as _sync
+from tap_typeform.sync import sync as _sync
 from tap_typeform.client import Client
 from tap_typeform.streams import Forms
 
-REQUIRED_CONFIG_KEYS = ["start_date", "token", "forms"]
+REQUIRED_CONFIG_KEYS = ["start_date", "token"]
 
 LOGGER = singer.get_logger()
 
 class FormMistmatchError(Exception):
     pass
 
-class NoFormsProvidedError(Exception):
-    pass
 
 def validate_form_ids(client, config):
     """Validate the form ids passed in the config"""
     form_stream = Forms()
 
+    api_forms = {form.get('id') for res in form_stream.get_forms(client) for form in res if form}
     if not config.get('forms'):
-        raise NoFormsProvidedError("No forms were provided in the config")
+        LOGGER.info("No form ids provided in config, fetching all forms")
+        return api_forms
 
-    config_forms = _forms_to_list(config)
-    api_forms = {form.get('id') for res in form_stream.get_forms(client) for form in res}
+    config_forms = set(map(str.strip, config.get("forms").split(',')))
 
     mismatched_forms = config_forms.difference(api_forms)
 
     if len(mismatched_forms) > 0:
         # Raise an error if any form-id from config is not matching
         # from ids from API response
         raise FormMistmatchError("FormMistmatchError: forms {} not returned by API".format(mismatched_forms))
+    return config_forms
 
 
 @utils.handle_top_exception(LOGGER)
 def main():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     config = args.config
     client = Client(config)
-    validate_form_ids(client, config)
+    valid_forms = validate_form_ids(client, config)
     if args.discover:
         catalog = _discover()
         catalog.dump()
     else:
         catalog = args.catalog \
             if args.catalog else _discover()
-        _sync(client, config, args.state, catalog.to_dict())
+        _sync(client, config, args.state, catalog.to_dict(), valid_forms)
 
 if __name__ == "__main__":
     main()
```

### Comparing `tap-typeform-2.0.1/tap_typeform/client.py` & `tap-typeform-2.1.0/tap_typeform/client.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/discover.py` & `tap-typeform-2.1.0/tap_typeform/discover.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schema.py` & `tap-typeform-2.1.0/tap_typeform/schema.py`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schemas/answers.json` & `tap-typeform-2.1.0/tap_typeform/schemas/answers.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schemas/forms.json` & `tap-typeform-2.1.0/tap_typeform/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schemas/questions.json` & `tap-typeform-2.1.0/tap_typeform/schemas/questions.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schemas/submitted_landings.json` & `tap-typeform-2.1.0/tap_typeform/schemas/submitted_landings.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/schemas/unsubmitted_landings.json` & `tap-typeform-2.1.0/tap_typeform/schemas/unsubmitted_landings.json`

 * *Files identical despite different names*

### Comparing `tap-typeform-2.0.1/tap_typeform/streams.py` & `tap-typeform-2.1.0/tap_typeform/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from copy import deepcopy
 import json
 import pendulum
 from datetime import datetime
 import singer
 from singer import bookmarks
 
 
@@ -169,16 +168,20 @@
         LOGGER.info('Syncing  stream {} - form: {}'.format(
                     self.tap_stream_id, form_id))
         self.records_count = records_count
         full_url = client.build_url(self.endpoint).format(form_id)
         stream_catalog = get_schema(catalogs, self.tap_stream_id)
         response = client.request(full_url, params=self.params)
 
+        if self.data_key not in response:
+            LOGGER.info('There are no questions associated with form {}'.format(form_id))
+            return
+
         for record in response[self.data_key]:
-            self.add_fields_at_1st_level(record,{"form_id": form_id})
+            self.add_fields_at_1st_level(record, {"form_id": form_id})
 
         write_records(stream_catalog, self.tap_stream_id, response[self.data_key])
         self.records_count[self.tap_stream_id] += len(response[self.data_key])
 
 class Forms(IncrementalStream):
     tap_stream_id = 'forms'
     key_properties = ['id']
```

### Comparing `tap-typeform-2.0.1/tap_typeform/sync.py` & `tap-typeform-2.1.0/tap_typeform/sync.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,12 @@
 import singer
-import pendulum
 from tap_typeform.streams import STREAMS
 
 LOGGER = singer.get_logger()
 
-def _forms_to_list(config, keyword='forms'):
-    """
-    Splits entries into a list and strips out surrounding blank spaces.
-    """
-    return set(map(str.strip, config.get(keyword).split(',')))
-
 
 def write_schemas(stream_id, catalog, selected_streams):
     """
     Write the schemas for each stream.
     """
     stream_obj = STREAMS[stream_id]()
 
@@ -46,15 +39,15 @@
     """
     streams_to_sync = []
     for stream_name, stream_obj in STREAMS.items():
         if (stream_name in selected_streams) or any(child in selected_streams for child in stream_obj.children):
             streams_to_sync.append(stream_name)
     return streams_to_sync
 
-def sync(client, config, state, catalog):
+def sync(client, config, state, catalog, forms_to_sync):
     """
     Sync selected streams.
     """
 
     # Get selected streams, make sure stream dependencies are met
     selected_streams = get_selected_streams(catalog)
     streams_to_sync = get_stream_to_sync(selected_streams)
@@ -74,14 +67,14 @@
             write_schemas(stream, catalog, selected_streams)
 
             stream_obj.sync_obj(client, state, catalog['streams'], config["start_date"],
                                 selected_streams, records_count)
         elif not stream_obj.parent:
             write_schemas(stream, catalog, selected_streams)
 
-            for form in _forms_to_list(config):
+            for form in forms_to_sync:
 
                 stream_obj.sync_obj(client, state, catalog['streams'], form, config["start_date"],
                                     selected_streams, records_count)
 
     for stream_name, stream_count in records_count.items():
         LOGGER.info('%s: %d', stream_name, stream_count)
```

### Comparing `tap-typeform-2.0.1/tap_typeform.egg-info/SOURCES.txt` & `tap-typeform-2.1.0/tap_typeform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

