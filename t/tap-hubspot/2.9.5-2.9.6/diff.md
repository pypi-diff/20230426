# Comparing `tmp/tap-hubspot-2.9.5.tar.gz` & `tmp/tap-hubspot-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-hubspot-2.9.5.tar", last modified: Tue Feb 23 16:05:29 2021, max compression
+gzip compressed data, was "tap-hubspot-2.9.6.tar", last modified: Wed Jun 15 17:09:19 2022, max compression
```

## Comparing `tap-hubspot-2.9.5.tar` & `tap-hubspot-2.9.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    45313 2021-02-23 15:26:43.000000 tap-hubspot-2.9.5/tap_hubspot/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      164 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/companies.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     8716 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/forms.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      573 2021-02-19 19:47:02.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/versions.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1231 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/subscription_changes.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      955 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/deal_pipelines.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2340 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/email_events.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1919 2019-08-30 16:59:49.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/owners.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      908 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/workflows.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      769 2021-02-19 19:47:02.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/deals.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     5390 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/contacts.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      220 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/contacts_by_company.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1908 2019-08-30 16:59:49.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/campaigns.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     3879 2021-02-19 19:47:02.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/engagements.json
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2813 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/tap_hubspot/schemas/contact_lists.json
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      294 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       12 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      796 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      121 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/tap_hubspot.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2784 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/README.md
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)    32393 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/LICENSE
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      294 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       51 2019-02-25 17:58:12.000000 tap-hubspot-2.9.5/MANIFEST.in
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       79 2021-02-23 16:05:29.000000 tap-hubspot-2.9.5/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1248 2021-02-23 16:05:06.000000 tap-hubspot-2.9.5/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-15 17:09:19.878638 tap-hubspot-2.9.6/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       51 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      305 2022-06-15 17:09:19.878638 tap-hubspot-2.9.6/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2872 2022-06-14 22:44:31.000000 tap-hubspot-2.9.6/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2022-06-15 17:09:19.878638 tap-hubspot-2.9.6/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1248 2022-06-15 17:06:33.000000 tap-hubspot-2.9.6/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-15 17:09:19.874638 tap-hubspot-2.9.6/tap_hubspot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    46791 2022-06-14 22:44:31.000000 tap-hubspot-2.9.6/tap_hubspot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-15 17:09:19.878638 tap-hubspot-2.9.6/tap_hubspot/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1908 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      164 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/companies.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2813 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/contact_lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5485 2022-06-14 22:44:31.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/contacts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      220 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/contacts_by_company.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      955 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/deal_pipelines.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      769 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/deals.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2340 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/email_events.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3879 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/engagements.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8716 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/forms.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1919 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/owners.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1231 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/subscription_changes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      573 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/versions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      908 2022-06-08 22:21:46.000000 tap-hubspot-2.9.6/tap_hubspot/schemas/workflows.json
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-06-15 17:09:19.874638 tap-hubspot-2.9.6/tap_hubspot.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      305 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      796 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      121 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2022-06-15 17:09:19.000000 tap-hubspot-2.9.6/tap_hubspot.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-hubspot-2.9.5/tap_hubspot/__init__.py` & `tap-hubspot-2.9.6/tap_hubspot/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from singer import (transform,
                     UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING,
                     Transformer, _transform_datetime)
 
 LOGGER = singer.get_logger()
 SESSION = requests.Session()
 
+REQUEST_TIMEOUT = 300
 class InvalidAuthException(Exception):
     pass
 
 class SourceUnavailableException(Exception):
     pass
 
 class DependencyException(Exception):
@@ -224,15 +225,15 @@
         "redirect_uri": CONFIG['redirect_uri'],
         "refresh_token": CONFIG['refresh_token'],
         "client_id": CONFIG['client_id'],
         "client_secret": CONFIG['client_secret'],
     }
 
 
-    resp = requests.post(BASE_URL + "/oauth/v1/token", data=payload)
+    resp = requests.post(BASE_URL + "/oauth/v1/token", data=payload, timeout=get_request_timeout())
     if resp.status_code == 403:
         raise InvalidAuthException(resp.content)
 
     resp.raise_for_status()
     auth = resp.json()
     CONFIG['access_token'] = auth['access_token']
     CONFIG['refresh_token'] = auth['refresh_token']
@@ -284,14 +285,16 @@
 
     if 'user_agent' in CONFIG:
         headers['User-Agent'] = CONFIG['user_agent']
 
     return params, headers
 
 
+# backoff for Timeout error is already included in "requests.exceptions.RequestException"
+# as it is a parent class of "Timeout" error
 @backoff.on_exception(backoff.constant,
                       (requests.exceptions.RequestException,
                        requests.exceptions.HTTPError),
                       max_tries=5,
                       jitter=None,
                       giveup=giveup,
                       on_giveup=on_giveup,
@@ -299,15 +302,15 @@
 def request(url, params=None):
 
     params, headers = get_params_and_headers(params)
 
     req = requests.Request('GET', url, params=params, headers=headers).prepare()
     LOGGER.info("GET %s", req.url)
     with metrics.http_request_timer(parse_source_from_url(url)) as timer:
-        resp = SESSION.send(req)
+        resp = SESSION.send(req, timeout=get_request_timeout())
         timer.tags[metrics.Tag.http_status_code] = resp.status_code
         if resp.status_code == 403:
             raise SourceUnavailableException(resp.content)
         else:
             resp.raise_for_status()
 
     return resp
@@ -327,14 +330,16 @@
 
         if versions:
             if not record.get('properties_versions'):
                 record['properties_versions'] = []
             record['properties_versions'] += versions
     return record
 
+# backoff for Timeout error is already included in "requests.exceptions.RequestException"
+# as it is a parent class of "Timeout" error
 @backoff.on_exception(backoff.constant,
                       (requests.exceptions.RequestException,
                        requests.exceptions.HTTPError),
                       max_tries=5,
                       jitter=None,
                       giveup=giveup,
                       on_giveup=on_giveup,
@@ -345,14 +350,15 @@
     headers['content-type'] = "application/json"
 
     with metrics.http_request_timer(url) as timer:
         resp = requests.post(
             url=url,
             json=data,
             params=params,
+            timeout=get_request_timeout(),
             headers=headers
         )
 
         resp.raise_for_status()
 
     return resp
 
@@ -429,23 +435,25 @@
 
             singer.write_state(STATE)
 
     STATE = singer.clear_offset(STATE, tap_stream_id)
     singer.write_state(STATE)
 
 
-def _sync_contact_vids(catalog, vids, schema, bumble_bee):
+def _sync_contact_vids(catalog, vids, schema, bumble_bee, bookmark_values, bookmark_key):
     if len(vids) == 0:
         return
 
     data = request(get_url("contacts_detail"), params={'vid': vids, 'showListMemberships' : True, "formSubmissionMode" : "all"}).json()
     time_extracted = utils.now()
     mdata = metadata.to_map(catalog.get('metadata'))
 
     for record in data.values():
+        # Explicitly add the bookmark field "versionTimestamp" and its value in the record.
+        record[bookmark_key] = bookmark_values.get(record.get("vid"))
         record = bumble_bee.transform(lift_properties_and_versions(record), schema, mdata)
         singer.write_record("contacts", record, catalog.get('stream_alias'), time_extracted=time_extracted)
 
 default_contact_params = {
     'showListMemberships': True,
     'includeVersion': True,
     'count': 100,
@@ -461,34 +469,39 @@
     schema = load_schema("contacts")
 
     singer.write_schema("contacts", schema, ["vid"], [bookmark_key], catalog.get('stream_alias'))
 
     url = get_url("contacts_all")
 
     vids = []
+    # Dict to store replication key value for each contact record
+    bookmark_values = {}
     with Transformer(UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING) as bumble_bee:
         for row in gen_request(STATE, 'contacts', url, default_contact_params, 'contacts', 'has-more', ['vid-offset'], ['vidOffset']):
             modified_time = None
             if bookmark_key in row:
                 modified_time = utils.strptime_with_tz(
                     _transform_datetime( # pylint: disable=protected-access
                         row[bookmark_key],
                         UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING))
 
             if not modified_time or modified_time >= start:
                 vids.append(row['vid'])
+                # Adding replication key value in `bookmark_values` dict
+                # Here, key is vid(primary key) and value is replication key value.
+                bookmark_values[row['vid']] = utils.strftime(modified_time)
 
             if modified_time and modified_time >= max_bk_value:
                 max_bk_value = modified_time
 
             if len(vids) == 100:
-                _sync_contact_vids(catalog, vids, schema, bumble_bee)
+                _sync_contact_vids(catalog, vids, schema, bumble_bee, bookmark_values, bookmark_key)
                 vids = []
 
-        _sync_contact_vids(catalog, vids, schema, bumble_bee)
+        _sync_contact_vids(catalog, vids, schema, bumble_bee, bookmark_values, bookmark_key)
 
     STATE = singer.write_bookmark(STATE, 'contacts', bookmark_key, utils.strftime(max_bk_value))
     singer.write_state(STATE)
     return STATE
 
 class ValidationPredFailed(Exception):
     pass
@@ -937,22 +950,22 @@
     replication_key = attr.ib()
     replication_method = attr.ib()
 
 STREAMS = [
     # Do these first as they are incremental
     Stream('subscription_changes', sync_subscription_changes, ['timestamp', 'portalId', 'recipient'], 'startTimestamp', 'INCREMENTAL'),
     Stream('email_events', sync_email_events, ['id'], 'startTimestamp', 'INCREMENTAL'),
+    Stream('contacts', sync_contacts, ["vid"], 'versionTimestamp', 'INCREMENTAL'),
 
     # Do these last as they are full table
     Stream('forms', sync_forms, ['guid'], 'updatedAt', 'FULL_TABLE'),
     Stream('workflows', sync_workflows, ['id'], 'updatedAt', 'FULL_TABLE'),
     Stream('owners', sync_owners, ["ownerId"], 'updatedAt', 'FULL_TABLE'),
     Stream('campaigns', sync_campaigns, ["id"], None, 'FULL_TABLE'),
     Stream('contact_lists', sync_contact_lists, ["listId"], 'updatedAt', 'FULL_TABLE'),
-    Stream('contacts', sync_contacts, ["vid"], 'versionTimestamp', 'FULL_TABLE'),
     Stream('companies', sync_companies, ["companyId"], 'hs_lastmodifieddate', 'FULL_TABLE'),
     Stream('deals', sync_deals, ["dealId"], 'hs_lastmodifieddate', 'FULL_TABLE'),
     Stream('deal_pipelines', sync_deal_pipelines, ['pipelineId'], None, 'FULL_TABLE'),
     Stream('engagements', sync_engagements, ["engagement_id"], 'lastUpdated', 'FULL_TABLE')
 ]
 
 def get_streams_to_sync(streams, state):
@@ -1077,14 +1090,25 @@
 
     return result
 
 def do_discover():
     LOGGER.info('Loading schemas')
     json.dump(discover_schemas(), sys.stdout, indent=4)
 
+def get_request_timeout():
+    # Get `request_timeout` value from config.
+    config_request_timeout = CONFIG.get('request_timeout')
+    # if config request_timeout is other than 0, "0" or "" then use request_timeout
+    if config_request_timeout and float(config_request_timeout):
+        request_timeout = float(config_request_timeout)
+    else:
+        # If value is 0, "0", "" or not passed then it set default to 300 seconds.
+        request_timeout = REQUEST_TIMEOUT
+    return request_timeout
+
 def main_impl():
     args = utils.parse_args(
         ["redirect_uri",
          "client_id",
          "client_secret",
          "refresh_token",
          "start_date"])
```

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/forms.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/forms.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/versions.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/versions.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/subscription_changes.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/subscription_changes.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/deal_pipelines.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/deal_pipelines.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/email_events.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/email_events.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/owners.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/owners.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/workflows.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/deals.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/contacts.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/contacts.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692308%*

 * *Differences: {"'properties'": "{'versionTimestamp': OrderedDict([('type', ['null', 'string']), ('format', "*

 * *                 "'date-time')])}"}*

```diff
@@ -353,14 +353,21 @@
         },
         "profile-url": {
             "type": [
                 "null",
                 "string"
             ]
         },
+        "versionTimestamp": {
+            "format": "date-time",
+            "type": [
+                "null",
+                "string"
+            ]
+        },
         "vid": {
             "type": [
                 "null",
                 "integer"
             ]
         }
     },
```

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/campaigns.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/engagements.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/engagements.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot/schemas/contact_lists.json` & `tap-hubspot-2.9.6/tap_hubspot/schemas/contact_lists.json`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/tap_hubspot.egg-info/SOURCES.txt` & `tap-hubspot-2.9.6/tap_hubspot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/README.md` & `tap-hubspot-2.9.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   - [Subscription Changes](http://developers.hubspot.com/docs/methods/email/get_subscriptions_timeline)
   - [Workflows](http://developers.hubspot.com/docs/methods/workflows/v3/get_workflows)
 - Outputs the schema for each resource
 - Incrementally pulls data based on the input state
 
 ## Configuration
 
-This tap requires a `config.json` which specifies details regarding [OAuth 2.0](https://developers.hubspot.com/docs/methods/oauth2/oauth2-overview) authentication, a cutoff date for syncing historical data, and an optional flag which controls collection of anonymous usage metrics. See [config.sample.json](config.sample.json) for an example. You may specify an API key instead of OAuth parameters for development purposes, as detailed below.
+This tap requires a `config.json` which specifies details regarding [OAuth 2.0](https://developers.hubspot.com/docs/methods/oauth2/oauth2-overview) authentication, a cutoff date for syncing historical data, an optional parameter request_timeout for which request should wait to get the response and an optional flag which controls collection of anonymous usage metrics. See [config.sample.json](config.sample.json) for an example. You may specify an API key instead of OAuth parameters for development purposes, as detailed below.
 
 To run `tap-hubspot` with the configuration file, use this command:
 
 ```bash
 › tap-hubspot -c my-config.json
 ```
```

### Comparing `tap-hubspot-2.9.5/LICENSE` & `tap-hubspot-2.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-hubspot-2.9.5/setup.py` & `tap-hubspot-2.9.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-hubspot',
-      version='2.9.5',
+      version='2.9.6',
       description='Singer.io tap for extracting data from the HubSpot API',
       author='Stitch',
       url='http://singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_hubspot'],
       install_requires=[
           'attrs==16.3.0',
```

