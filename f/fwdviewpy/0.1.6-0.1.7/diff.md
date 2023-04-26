# Comparing `tmp/fwdviewpy-0.1.6.tar.gz` & `tmp/fwdviewpy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.6.tar", last modified: Mon Apr 24 08:41:56 2023, max compression
+gzip compressed data, was "fwdviewpy-0.1.7.tar", last modified: Wed Apr 26 09:24:37 2023, max compression
```

## Comparing `fwdviewpy-0.1.6.tar` & `fwdviewpy-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.203409 fwdviewpy-0.1.6/
--rw-rw-rw-   0        0        0      620 2023-04-24 08:41:56.189909 fwdviewpy-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.156209 fwdviewpy-0.1.6/fwdviewpy/
--rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.6/fwdviewpy/__init__.py
--rw-rw-rw-   0        0        0    10707 2023-04-20 14:54:14.000000 fwdviewpy-0.1.6/fwdviewpy/main.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:41:56.189909 fwdviewpy-0.1.6/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      620 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 08:41:55.000000 fwdviewpy-0.1.6/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 08:41:56.203409 fwdviewpy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-04-24 08:41:27.000000 fwdviewpy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:24:37.543261 fwdviewpy-0.1.7/
+-rw-rw-rw-   0        0        0      620 2023-04-26 09:24:37.539249 fwdviewpy-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-26 09:24:37.489366 fwdviewpy-0.1.7/fwdviewpy/
+-rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.7/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    12777 2023-04-26 09:22:02.000000 fwdviewpy-0.1.7/fwdviewpy/main.py
+drwxrwxrwx   0        0        0        0 2023-04-26 09:24:37.533204 fwdviewpy-0.1.7/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-04-26 09:24:34.000000 fwdviewpy-0.1.7/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-04-26 09:24:34.000000 fwdviewpy-0.1.7/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-26 09:24:34.000000 fwdviewpy-0.1.7/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-04-26 09:24:34.000000 fwdviewpy-0.1.7/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-26 09:24:34.000000 fwdviewpy-0.1.7/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-26 09:24:37.543261 fwdviewpy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      827 2023-04-26 09:22:29.000000 fwdviewpy-0.1.7/setup.py
```

### Comparing `fwdviewpy-0.1.6/PKG-INFO` & `fwdviewpy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.6/fwdviewpy/main.py` & `fwdviewpy-0.1.7/fwdviewpy/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         This method creates a bookmark on the container of the Delphix Engine. 
 
         Args: 
             containerName: This is the name of the container to be bookmarked on the Delphix Engine. 
             bookmarkName: This argument is the name of the bookmark to be made on the containerName.
         
         Returns: 
-            This method does not return any value. 
+            This method returns True is the bookmark was made successfully & returns False if it failed to create a bookmark. 
         """
         containerReference, containerBranch = self._getTemplateBranch(containerName)
         # Send a POST request to the bookmark endpoint with cookies set from the session
         bookmark_url = f"http://{self.address}/resources/json/delphix/selfservice/bookmark"
         data = {
             "type": "JSBookmarkCreateParameters",
             "bookmark": {
@@ -80,25 +80,30 @@
                 "type": "JSTimelinePointLatestTimeInput",
                 "sourceDataLayout": containerReference
             }
         }
         session = self._login()
         response = session.post(bookmark_url, json=data)
         action = response.json()['action']
-        self._checkActionLoop(action)
-        session.close()
-        logging.debug(f"Bookmark has been created. \n Bookmark: {bookmarkName} \n Container: {containerName} \n Engine: {self.address}")
+        if self._checkActionLoop(action):
+            session.close()
+            logging.debug(f"Bookmark has been created. \n Bookmark: {bookmarkName} \n Container: {containerName} \n Engine: {self.address}")
+            return True
+        else:
+            session.close()
+            return False 
+
 
     def _checkActionLoop(self, action): 
         while True:
             if self._checkAction(action):
-                break
+                return True
             elif self._checkAction(action) == "FAILED":
                 logging.error("Failed to create Bookmark. Please see Engine logs.")
-                sys.exit()
+                return False
             else:
                 print("Not yet Completed, check again in 10 seconds")
                 time.sleep(10)
 
     def _checkAction(self, action):
         session = self.login()
         action_url = f"http://{self.address}/resources/json/delphix/action"
@@ -164,30 +169,31 @@
 
         Args: 
             environment: This is the environent on the Delphix masking engine on which to run the masking job. 
             maskingRule: This is the ruleset that we want to run on the delphix engine. 
             connectorName: This is the name of the connector for which connects the masking job to the data. 
         
         Returns: 
-            This method does not return any value. 
+            This returns True if it has run successfully and False if there is an Error. 
         """
         authKey = self.login()
         envID = self._getEnvironment(authKey, environment)
         ruleID = self._getJobId(authKey, maskingRule, envID)
         targetConnectorID = self._getTargetConnectorID(authKey, connectorName, envID)
         self._execute_job(authKey, ruleID, targetConnectorID)
         logging.info(f"Masking job triggered. Job: {maskingRule}")
         executionID = self._getExecutionID(authKey, ruleID)
         jobStatus = self._checkStatus(executionID) 
 
         if jobStatus == "SUCCEEDED":
             logging.info(f"Masking Successful. Job: {maskingRule}")
+            return True
         else:
             logging.error(f"Please check error logs for masking job: {maskingRule}")
-            sys.exit()
+            return False
     
     def _getEnvironment(self, authKey, envName):
         response = self._getRequest(authKey, "environments")
         response = json.loads(response)
         for env in response["responseList"]:
             if env["environmentName"] == envName:
                 envID = env["environmentId"]
@@ -246,8 +252,47 @@
         while True:
             status = self._getStatus(authKey, executionID)
             if status == "RUNNING":
                 time.sleep(300)
                 print("Job is still running, check again in 5 minutes.")
             else:
                 print(f"Job has finished running. Job Status is: {status}")
-                return status
+                return status
+            
+    def refreshRuleSets(self,EnvironmentName):
+        """
+        This function refreshes all rulesets in an environment. 
+
+        Args: 
+            EnvironmentName: This is the name of the environment on the Delphix masking engine. 
+        
+        Returns: True is successful and False if there is an Error. 
+        """
+        authKey = self.login()
+        environmentID = self._getEnvironment(authKey,EnvironmentName)
+        response = self._getRequest(authKey, f"database-rulesets?environment_id={environmentID}")
+        response = json.loads(response)
+        ruleSetIDList = [ruleSet["databaseRulesetId"] for ruleSet in response["responseList"]]
+        
+        for ruleSetID in ruleSetIDList: 
+            url = f"http://{self.address}/masking/api/v5.1.14/database-rulesets/{ruleSetID}/refresh"
+            headers = {
+            'Content-Type': 'application/json',
+            'Accept': 'application/json',
+            'Authorization': authKey
+            }
+            response = requests.put(url, headers=headers)
+            json_response = response.json()
+            try: 
+                async_task_id = json_response['asyncTaskId']
+            except KeyError:
+                print(f"There's a problem with refreshing id: {ruleSetID} \n Message: {json_response}") 
+                return False
+            while True: 
+                response = self._getRequest(authKey, f"async-tasks/{async_task_id}")
+                response = json.loads(response)
+                if response["status"] == "SUCCEEDED": 
+                    print(f"Successful for id: {ruleSetID}")
+                    return True 
+                else:
+                    print("Not yet Completed, check again in 10 seconds")
+                    time.sleep(10)
```

### Comparing `fwdviewpy-0.1.6/fwdviewpy.egg-info/PKG-INFO` & `fwdviewpy-0.1.7/fwdviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.6/setup.py` & `fwdviewpy-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fwdviewpy',
-    version='0.1.6',
+    version='0.1.7',
     description='Python package developed by FWD View - The Data Transformation Specialists.',
     long_description='Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.',
     packages=find_packages(),
     author='Cameron Bose & Ryan Springett',
     author_email="cameron.bose@fwdview.com",
 
     install_requires=[
```

