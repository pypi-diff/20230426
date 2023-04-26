# Comparing `tmp/jps_api_wrapper-1.4.1.tar.gz` & `tmp/jps_api_wrapper-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jps_api_wrapper-1.4.1.tar", last modified: Fri Apr  7 04:56:22 2023, max compression
+gzip compressed data, was "jps_api_wrapper-1.5.0.tar", last modified: Tue Apr 25 16:37:28 2023, max compression
```

## Comparing `jps_api_wrapper-1.4.1.tar` & `jps_api_wrapper-1.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 04:56:22.382578 jps_api_wrapper-1.4.1/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8112 2023-04-07 04:56:22.382578 jps_api_wrapper-1.4.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-07 04:56:22.383578 jps_api_wrapper-1.4.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 04:56:22.377578 jps_api_wrapper-1.4.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 04:56:22.380578 jps_api_wrapper-1.4.1/src/jps_api_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 04:55:54.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   262861 2023-04-07 04:48:50.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper/classic.py
--rw-rw-rw-   0 root         (0) root         (0)   309263 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper/pro.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper/request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     6752 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 04:56:22.381578 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8112 2023-04-07 04:56:22.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-04-07 04:56:22.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-07 04:56:22.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-07 04:56:22.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-07 04:56:22.000000 jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-07 04:56:22.381578 jps_api_wrapper-1.4.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)   290397 2023-04-07 04:48:50.000000 jps_api_wrapper-1.4.1/tests/test_classic.py
--rw-rw-rw-   0 root         (0) root         (0)   209408 2023-04-07 04:10:59.000000 jps_api_wrapper-1.4.1/tests/test_pro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.788352 jps_api_wrapper-1.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-04-25 16:37:28.788352 jps_api_wrapper-1.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-25 16:37:28.789352 jps_api_wrapper-1.5.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.784352 jps_api_wrapper-1.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.786352 jps_api_wrapper-1.5.0/src/jps_api_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 16:37:01.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   262861 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   309635 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/pro.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.787352 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.787352 jps_api_wrapper-1.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   290397 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/tests/test_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   209507 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/tests/test_pro.py
```

### Comparing `jps_api_wrapper-1.4.1/LICENSE` & `jps_api_wrapper-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/PKG-INFO` & `jps_api_wrapper-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps_api_wrapper
-Version: 1.4.1
+Version: 1.5.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.4.1/README.md` & `jps_api_wrapper-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/setup.cfg` & `jps_api_wrapper-1.5.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jps_api_wrapper
-version = 1.4.1
+version = 1.5.0
 description = Jamf Pro Server API Python wrapper
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 readme = README.md
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `jps_api_wrapper-1.4.1/src/jps_api_wrapper/classic.py` & `jps_api_wrapper-1.5.0/src/jps_api_wrapper/classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/src/jps_api_wrapper/pro.py` & `jps_api_wrapper-1.5.0/src/jps_api_wrapper/pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -5017,28 +5017,28 @@
         """
         Returns information about if Local Admin Password auto-deploy feature
         is enabled. When it is enabled, all computers will have the
         SetAutoAdminPassword command sent to them automatically.
 
         :returns: Local Admin Password auto-deploy information in JSON
         """
-        endpoint = "/api/v1/local-admin-password/settings"
+        endpoint = "/api/v2/local-admin-password/settings"
 
         return self._get(endpoint)
 
     def get_local_admin_password_accounts(self, clientManagementId: str) -> dict:
         """
         Returns a full list of admin accounts that are LAPS capable
 
         :param clientManagementId: Client management ID of target device
 
         :returns:
             All LAPS capable accounts for the device in JSON
         """
-        endpoint = f"/api/v1/local-admin-password/{clientManagementId}/accounts"
+        endpoint = f"/api/v2/local-admin-password/{clientManagementId}/accounts"
 
         return self._get(endpoint)
 
     def get_local_admin_password_user_history(
         self, clientManagementId: str, username: str
     ) -> dict:
         """
@@ -5051,15 +5051,15 @@
         :param username: Username to view audit information for
 
         :returns:
             Full history of all local admin passwords used for user on device
             in JSON
         """
         endpoint = (
-            f"/api/v1/local-admin-password/{clientManagementId}/account/"
+            f"/api/v2/local-admin-password/{clientManagementId}/account/"
             f"{username}/audit"
         )
 
         return self._get(endpoint)
 
     def get_local_admin_password_user_current(
         self, clientManagementId: str, username: str
@@ -5073,32 +5073,51 @@
         :param clientManagementId: Client management ID of target device
         :param username: Username to view audit information for
 
         :returns:
             Current local admin password used for user on device in JSON
         """
         endpoint = (
-            f"/api/v1/local-admin-password/{clientManagementId}/account/"
+            f"/api/v2/local-admin-password/{clientManagementId}/account/"
             f"{username}/password"
         )
 
         return self._get(endpoint)
 
     def update_local_admin_password_settings(self, data: dict) -> dict:
         """
         Updates Local Admin Password auto-deploy feature to be enabled or not.
         When it is enabled (true), all computers will have the
         SetAutoAdminPassword command sent to them automatically.
 
         :param data:
             JSON data to update local admin password settings with. For syntax
             information view `Jamf's documentation.
-            <TODO: Add URL on 10.44 release>`__
+            <TODO: Add URL on 10.46 release>`__
+
+        :returns: Updated local admin password settings in JSON
+        """
+        endpoint = "/api/v2/local-admin-password/settings"
+
+        return self._put(endpoint, data)
+
+    def update_local_admin_password(self, data: dict, clientManagementId: str) -> dict:
+        """
+        Updates the LAPS password for a device. This will set the password for
+        all LAPS capable accounts.
+
+        :param data:
+            JSON data to update local admin password with. For syntax
+            information view `Jamf's documentation.
+            <TODO: Add URL on 10.46 release>`__
+        :param clientManagementId: Client management ID of target device
+
+        :returns: Information on the updated account in JSON
         """
-        endpoint = "/api/v1/local-admin-password/settings"
+        endpoint = f"/api/v2/local-admin-password/{clientManagementId}/set-password"
 
         return self._put(endpoint, data)
 
     """
     locales-preview
     """
 
@@ -5548,15 +5567,15 @@
     def create_mobile_device_group_static(self, data: dict) -> dict:
         """
         Creates mobile device static group with JSON data
 
         :param data:
             JSON data to create the mobile device static group with. For syntax
             information view `Jamf's documentation.
-            <TODO: Add URL on release>`__
+            <https://developer.jamf.com/jamf-pro/reference/post_v1-mobile-device-groups-static-groups>`__
 
         :returns: New mobile device static group information in JSON
         """
         endpoint = "/api/v1/mobile-device-groups/static-groups"
 
         return self._post(endpoint, data)
 
@@ -5565,15 +5584,15 @@
     ) -> dict:
         """
         Updates mobile device static group with JSON by ID
 
         :param data:
             JSON data to update the mobile device static group with.For syntax
             information view `Jamf's documentation.
-            <TODO: Add URL on release>`__
+            <https://developer.jamf.com/jamf-pro/reference/patch_v1-mobile-device-groups-static-groups-id>`__
         :param id: Mobile device static group ID
 
         :returns: Updated mobile device static group information in JSON
         """
         endpoint = f"/api/v1/mobile-device-groups/static-groups/{id}"
 
         return self._patch(endpoint, data)
@@ -6389,15 +6408,15 @@
         """
         Sends retry attempts for a specific device in a patch policy with JSON
         by ID
 
         :param data:
             JSON data to create patch policy log retries with. For syntax
             information view `Jamf's documentation.
-            <TODO: ADD URL ON RELEASE>`__
+            <https://developer.jamf.com/jamf-pro/reference/post_v2-patch-policies-id-logs-retry>`__
         :param id: Patch policy ID
 
         :returns:
             Success message stating that the specified patch policy log for the
             specified devices were retried
         """
         endpoint = f"/api/v2/patch-policies/{id}/logs/retry"
@@ -6548,20 +6567,21 @@
             Sorting criteria in the format: property:asc/desc. Default sort is
             ["computerName:asc"]. Multiple sort criteria are supported and must
             be separated with a comma.
 
             Example: ["deviceId:asc", "computerName:desc"]
 
         :param filter:
-            Query in the RSQL format, allowing to filter history notes
-            collection. Default filter is empty query - returning all results
-            for the requested page. Fields allowed in the query: computerName,
-            deviceId, username, operatingSystemVersion, lastContactTime,
-            buildingName, departmentName, siteName, version. This param can be
-            combined with paging and sorting.
+            Query in the RSQL format, allowing to filter Patch Report
+            collection on version equality only. Default filter is empty query
+            - returning all results for the requested page. Fields allowed in
+            the query: version. Comparators allowed in the query: ==, != This
+            param can be combined with paging and sorting.
+
+            Example: "version==10.1"
 
         :returns:
             CSV formatted string of the requested patch software title
             configuration
         """
         if "all" in columns_to_export:
             columns_to_export = [
@@ -6734,15 +6754,15 @@
     def create_patch_software_title_configuration(self, data: dict) -> dict:
         """
         Creates patch software title configuration with JSON data
 
         :param data:
             JSON data to create the patch software title configuration with.
             For syntax information view `Jamf's documentation.
-            <TODO: ADD URL ON RELEASE OF 10.44>`__
+            <https://developer.jamf.com/jamf-pro/reference/post_v2-patch-software-title-configurations>`__
 
         :returns: New patch software title configuration information in JSON
         """
         endpoint = "/api/v2/patch-software-title-configurations"
 
         return self._post(endpoint, data)
 
@@ -6772,15 +6792,15 @@
     ) -> dict:
         """
         Creates patch software title configuration history note by ID with JSON
 
         :param data:
             JSON data to create the patch software title configuration history
             note with. For syntax information view `Jamf's documentation.
-            <TODO: ADD URL ON RELEASE OF 10.44>`__
+            <https://developer.jamf.com/jamf-pro/reference/post_v2-patch-software-title-configurations-id-history>`__
         :param id: Patch software title configuration ID
 
         :returns:
             New patch policy title configuration history note information in
             JSON
         """
         endpoint = f"/api/v2/patch-software-title-configurations/{id}/history"
@@ -6792,15 +6812,15 @@
     ) -> dict:
         """
         Updates patch software title configuration with JSON by ID
 
         :param data:
             JSON data to update the patch software title configuration history
             note with. For syntax information view `Jamf's documentation.
-            <TODO: ADD URL ON RELEASE OF 10.44>`__
+            <https://developer.jamf.com/jamf-pro/reference/patch_v2-patch-software-title-configurations-id>`__
         :param id: Patch software title configuration ID
 
         :returns:
             Updated patch policy title configuration history note information
             in JSON
         """
         endpoint = f"/api/v2/patch-software-title-configurations/{id}"
@@ -6910,37 +6930,14 @@
 
         endpoint = "/api/patch/disclaimerAgree"
 
         return self._post(
             endpoint, success_message="Patch reporting disclaimer accepted."
         )
 
-    def update_patch_report(self, data: dict, id: Union[int, str]) -> dict:
-        """
-        .. deprecated:: 1.3.0
-
-        Updates patch report by ID with JSON
-
-        :param data:
-            JSON data to update patch report with. For syntax information view
-            `Jamf's documentation.
-            <https://developer.jamf.com/jamf-pro/reference/put_patch-obj-id>`__
-        :param id: Patch ID
-
-        :returns: Updated patch report information in JSON
-        """
-        warnings.warn(
-            ("Pro.update_patch_report has been deprecated by Jamf Pro v10.44.0."),
-            category=DeprecationWarning,
-        )
-
-        endpoint = f"/api/patch/obj/{id}"
-
-        return self._put(endpoint, data)
-
     """
     policies-preview
     """
 
     def get_policy_properties(self) -> dict:
         """
         Returns policy properties
```

### Comparing `jps_api_wrapper-1.4.1/src/jps_api_wrapper/request_builder.py` & `jps_api_wrapper-1.5.0/src/jps_api_wrapper/request_builder.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/src/jps_api_wrapper/utils.py` & `jps_api_wrapper-1.5.0/src/jps_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/src/jps_api_wrapper.egg-info/PKG-INFO` & `jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps-api-wrapper
-Version: 1.4.1
+Version: 1.5.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.4.1/tests/test_classic.py` & `jps_api_wrapper-1.5.0/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.4.1/tests/test_pro.py` & `jps_api_wrapper-1.5.0/tests/test_pro.py`

 * *Files 0% similar despite different names*

```diff
@@ -3971,29 +3971,29 @@
 
 @responses.activate
 def test_get_local_admin_password_settings(pro):
     """
     Ensures that get_local_admin_password_settings returns JSON when used
     """
     responses.add(
-        response_builder("GET", jps_url("/api/v1/local-admin-password/settings"))
+        response_builder("GET", jps_url("/api/v2/local-admin-password/settings"))
     )
     assert pro.get_local_admin_password_settings() == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_local_admin_password_user_history(pro):
     """
     Ensures that get_local_admin_password_user_history returns JSON when used
     with required params
     """
     responses.add(
         response_builder(
             "GET",
-            jps_url("/api/v1/local-admin-password/1a2b-3c4d/account/testuser/audit"),
+            jps_url("/api/v2/local-admin-password/1a2b-3c4d/account/testuser/audit"),
         )
     )
     assert (
         pro.get_local_admin_password_user_history("1a2b-3c4d", "testuser")
         == EXPECTED_JSON
     )
 
@@ -4002,30 +4002,30 @@
 def test_get_local_admin_password_accounts(pro):
     """
     Ensures that get_local_admin_password_accounts returns JSON when used with
     required params
     """
     responses.add(
         response_builder(
-            "GET", jps_url("/api/v1/local-admin-password/1a2b-3c4d/accounts")
+            "GET", jps_url("/api/v2/local-admin-password/1a2b-3c4d/accounts")
         )
     )
     assert pro.get_local_admin_password_accounts("1a2b-3c4d") == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_local_admin_password_user_current(pro):
     """
     Ensures that get_local_admin_password_user_current returns JSON when used
     with required params
     """
     responses.add(
         response_builder(
             "GET",
-            jps_url("/api/v1/local-admin-password/1a2b-3c4d/account/testuser/password"),
+            jps_url("/api/v2/local-admin-password/1a2b-3c4d/account/testuser/password"),
         )
     )
     assert (
         pro.get_local_admin_password_user_current("1a2b-3c4d", "testuser")
         == EXPECTED_JSON
     )
 
@@ -4033,19 +4033,33 @@
 @responses.activate
 def test_update_local_admin_password_settings(pro):
     """
     Ensures that update_local_admin_password_settings returns JSON when used
     with required params
     """
     responses.add(
-        response_builder("PUT", jps_url("/api/v1/local-admin-password/settings"))
+        response_builder("PUT", jps_url("/api/v2/local-admin-password/settings"))
     )
     assert pro.update_local_admin_password_settings(EXPECTED_JSON) == EXPECTED_JSON
 
 
+@responses.activate
+def test_update_local_admin_password(pro):
+    """
+    Ensures that update_local_admin_password returns JSON when used with
+    required params
+    """
+    responses.add(
+        response_builder(
+            "PUT", jps_url("/api/v2/local-admin-password/1a2b-3c4d/set-password")
+        )
+    )
+    assert pro.update_local_admin_password(EXPECTED_JSON, "1a2b-3c4d") == EXPECTED_JSON
+
+
 """
 locales-preview
 """
 
 
 @responses.activate
 def test_get_locales(pro):
@@ -5466,24 +5480,14 @@
     """
     responses.add(response_builder("POST", jps_url("/api/patch/disclaimerAgree")))
     assert (
         pro.create_patch_disclaimer_accept() == "Patch reporting disclaimer accepted."
     )
 
 
-@responses.activate
-def test_update_patch_report(pro):
-    """
-    Ensures that update_patch_report returns JSON when used with required
-    params
-    """
-    responses.add(response_builder("PUT", jps_url("/api/patch/obj/1001")))
-    assert pro.update_patch_report(EXPECTED_JSON, 1001) == EXPECTED_JSON
-
-
 """
 policies-preview
 """
 
 
 @responses.activate
 def test_get_policy_properties(pro):
```

