# Comparing `tmp/doris_stream_load-2.3.tar.gz` & `tmp/doris_stream_load-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\doris_stream_load-2.3.tar", last modified: Thu Apr 28 06:37:06 2022, max compression
+gzip compressed data, was "dist\doris_stream_load-2.4.tar", last modified: Wed Apr 26 11:22:24 2023, max compression
```

## Comparing `doris_stream_load-2.3.tar` & `doris_stream_load-2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
-drwxrwxrwx   0        0        0        0 2022-04-28 06:37:06.000000 doris_stream_load-2.3/
--rw-rw-rw-   0        0        0     3917 2022-04-28 06:36:50.000000 doris_stream_load-2.3/doris_stream_load.py
--rw-rw-rw-   0        0        0      243 2022-04-28 06:37:06.000000 doris_stream_load-2.3/PKG-INFO
--rw-rw-rw-   0        0        0     1594 2022-04-28 06:27:46.000000 doris_stream_load-2.3/README
--rw-rw-rw-   0        0        0      260 2022-04-28 06:37:02.000000 doris_stream_load-2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 11:22:24.000000 doris_stream_load-2.4/
+-rw-rw-rw-   0        0        0     3918 2023-04-26 11:08:54.000000 doris_stream_load-2.4/doris_stream_load.py
+-rw-rw-rw-   0        0        0      243 2023-04-26 11:22:24.000000 doris_stream_load-2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2022-04-28 06:27:46.000000 doris_stream_load-2.4/README
+-rw-rw-rw-   0        0        0      260 2023-04-26 11:10:30.000000 doris_stream_load-2.4/setup.py
```

### Comparing `doris_stream_load-2.3/doris_stream_load.py` & `doris_stream_load-2.4/doris_stream_load.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.column_separator = column_separator
         self.requests_session = requests.session()
 
     def sendData(self,row_list):
         loadUrl = "http://%s:%s/api/%s/%s/_stream_load/" % (self.doris_host,self.doris_http_port, self.database, self.table_name)
         headers = {'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8',
                    'column_separator': self.column_separator,
-                   'two_phase_commit': 'true',
+                   'two_phase_commit': 'false',
                    'Accept': 'application/json;charset=UTF-8',
                    'Expect': '100-continue',
                    "Authorization": "Basic " + base64.b64encode(
                        bytes(self.doris_user + ":" + self.doris_password, 'utf-8')).decode(
                        'utf-8')}
         # print(loadUrl)
         # print(json_content)
```

### Comparing `doris_stream_load-2.3/README` & `doris_stream_load-2.4/README`

 * *Files identical despite different names*

