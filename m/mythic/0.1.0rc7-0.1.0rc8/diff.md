# Comparing `tmp/mythic-0.1.0rc7.tar.gz` & `tmp/mythic-0.1.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mythic-0.1.0rc7.tar", last modified: Fri Apr 21 17:51:56 2023, max compression
+gzip compressed data, was "mythic-0.1.0rc8.tar", last modified: Tue Apr 25 16:39:04 2023, max compression
```

## Comparing `mythic-0.1.0rc7.tar` & `mythic-0.1.0rc8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.575304 mythic-0.1.0rc7/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-21 17:51:56.574032 mythic-0.1.0rc7/PKG-INFO
--rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc7/README.md
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.571264 mythic-0.1.0rc7/mythic/
--rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc7/mythic/__init__.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc7/mythic/graphql_queries.py
--rw-r--r--   0 itsafeature   (501) staff       (20)    95272 2023-04-21 17:51:11.000000 mythic-0.1.0rc7/mythic/mythic.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-21 17:51:52.000000 mythic-0.1.0rc7/mythic/mythic_classes.py
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc7/mythic/mythic_exceptions.py
--rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc7/mythic/mythic_utilities.py
-drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-21 17:51:56.573314 mythic-0.1.0rc7/mythic.egg-info/
--rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/PKG-INFO
--rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/SOURCES.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/dependency_links.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/requires.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-21 17:51:56.000000 mythic-0.1.0rc7/mythic.egg-info/top_level.txt
--rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-21 17:51:56.575740 mythic-0.1.0rc7/setup.cfg
--rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-21 17:51:43.000000 mythic-0.1.0rc7/setup.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.413421 mythic-0.1.0rc8/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-25 16:39:04.413068 mythic-0.1.0rc8/PKG-INFO
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)     1711 2023-04-06 15:01:27.000000 mythic-0.1.0rc8/README.md
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.410702 mythic-0.1.0rc8/mythic/
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)       29 2022-01-31 22:46:05.000000 mythic-0.1.0rc8/mythic/__init__.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7198 2023-04-06 01:01:59.000000 mythic-0.1.0rc8/mythic/graphql_queries.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)    97649 2023-04-25 15:11:39.000000 mythic-0.1.0rc8/mythic/mythic.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     3376 2023-04-25 16:38:38.000000 mythic-0.1.0rc8/mythic/mythic_classes.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2022-03-21 21:08:15.000000 mythic-0.1.0rc8/mythic/mythic_exceptions.py
+-rw-r--r--   0 itsafeature   (501) staff       (20)     7582 2023-03-22 20:38:43.000000 mythic-0.1.0rc8/mythic/mythic_utilities.py
+drwxr-xr-x   0 itsafeature   (501) staff       (20)        0 2023-04-25 16:39:04.412605 mythic-0.1.0rc8/mythic.egg-info/
+-rw-r--r--   0 itsafeature   (501) staff       (20)     2059 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/PKG-INFO
+-rw-r--r--   0 itsafeature   (501) staff       (20)      309 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/SOURCES.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        1 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/dependency_links.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       40 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/requires.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)        7 2023-04-25 16:39:04.000000 mythic-0.1.0rc8/mythic.egg-info/top_level.txt
+-rw-r--r--   0 itsafeature   (501) staff       (20)       38 2023-04-25 16:39:04.413520 mythic-0.1.0rc8/setup.cfg
+-rwxr-xr-x   0 itsafeature   (501) staff       (20)      821 2023-04-25 16:38:15.000000 mythic-0.1.0rc8/setup.py
```

### Comparing `mythic-0.1.0rc7/PKG-INFO` & `mythic-0.1.0rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc7
+Version: 0.1.0rc8
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc7/README.md` & `mythic-0.1.0rc8/README.md`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc7/mythic/graphql_queries.py` & `mythic-0.1.0rc8/mythic/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc7/mythic/mythic.py` & `mythic-0.1.0rc8/mythic/mythic.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 INFO = 20
 DEBUG = 10
 NOTSET = 0
 """
 
 
 async def login(
-    server_ip: str,
-    server_port: int = 7443,
-    username: str = None,
-    password: str = None,
-    apitoken: str = None,
-    ssl: bool = True,
-    timeout: int = -1,
-    logging_level: int = logging.WARNING,
+        server_ip: str,
+        server_port: int = 7443,
+        username: str = None,
+        password: str = None,
+        apitoken: str = None,
+        ssl: bool = True,
+        timeout: int = -1,
+        logging_level: int = logging.WARNING,
 ) -> mythic_classes.Mythic:
     """
     Create a new Mythic instance based on the connection information and attempt to validate the credentials.
     If a username and password is provided, this will log into Mythic and fetch/generate an API token to use for subsequent functions.
     If an api token is provided, this will validate that the api token is valid.
     """
     mythic = mythic_classes.Mythic(
@@ -75,16 +75,16 @@
                 mythic.apitoken = current_tokens["apitokens"][0]["token_value"]
             else:
                 # we need to generate an api token and use that so that future calls don't get timed out from an expired JWT
                 new_token = await mythic_utilities.graphql_post(
                     mythic=mythic, gql_query=graphql_queries.create_apitoken
                 )
                 if (
-                    new_token["createAPIToken"]["status"] == "success"
-                    and "token_value" in new_token["createAPIToken"]
+                        new_token["createAPIToken"]["status"] == "success"
+                        and "token_value" in new_token["createAPIToken"]
                 ):
                     mythic.apitoken = new_token["createAPIToken"]["token_value"]
                 else:
                     raise Exception(
                         f"Failed to get or generate an API token to use from Mythic\n{new_token['createAPIToken']['error']}"
                     )
             return mythic
@@ -96,49 +96,49 @@
             return mythic
         except Exception as e:
             logging.exception(f"[-] Failed to authenticate to Mythic: \n{str(e)}")
             raise e
 
 
 async def execute_custom_query(
-    mythic: mythic_classes.Mythic, query: str, variables: dict = None
+        mythic: mythic_classes.Mythic, query: str, variables: dict = None
 ) -> dict:
     try:
         return await mythic_utilities.graphql_post(
             mythic=mythic, query=query, variables=variables
         )
     except Exception as e:
         logging.info(f"Hit an exception within execute_custom_query: {e}")
         raise e
 
 
 async def subscribe_custom_query(
-    mythic: mythic_classes.Mythic, query: str, variables: dict = None, timeout: int = None
+        mythic: mythic_classes.Mythic, query: str, variables: dict = None, timeout: int = None
 ) -> AsyncGenerator:
     """
     Execute a custom graphql subscription.
     This returns an async iterator, which can be used as:
         async for item in execute_custom_subscription(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     """
     try:
         async for result in mythic_utilities.graphql_subscription(
-            mythic=mythic, query=query, variables=variables, timeout=timeout
+                mythic=mythic, query=query, variables=variables, timeout=timeout
         ):
             yield result
     except Exception as e:
         logging.info(f"Hit an exception within execute_custom_subscription: {e}")
         raise e
 
 
 # ########### Callback Functions #############
 
 
 async def get_all_callbacks(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None
 ) -> List[dict]:
     """
     Executes a graphql query to get information about all callbacks (including ones that are no longer active).
     The default set of attributes returned in the dictionary can be found at graphql_queries.callback_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
     """
     query = f"""
@@ -152,16 +152,16 @@
     initial_tasks = await mythic_utilities.graphql_post(
         mythic=mythic, query=query, variables=None
     )
     return initial_tasks["callback"]
 
 
 async def get_all_active_callbacks(
-    mythic: mythic_classes.Mythic,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        custom_return_attributes: str = None,
 ) -> List[dict]:
     """
     Executes a graphql query to get information about all currently active callbacks.
     The default set of attributes returned in the dictionary can be found at graphql_queries.callback_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
     """
     query = f"""
@@ -175,18 +175,18 @@
     initial_tasks = await mythic_utilities.graphql_post(
         mythic=mythic, query=query, variables=None
     )
     return initial_tasks["callback"]
 
 
 async def subscribe_new_callbacks(
-    mythic: mythic_classes.Mythic,
-    batch_size: int = 50,
-    timeout: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        batch_size: int = 50,
+        timeout: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Execute a graphql subscription for callbacks that have an initial checkin time greater than when this function is called.
     This returns an async iterator, which can be used as:
         async for item in subscribe_new_callbacks(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.callback_fragment.
@@ -199,65 +199,65 @@
                 {custom_return_attributes if custom_return_attributes is not None else '...callback_fragment'}
             }}
         }}
         {graphql_queries.callback_fragment if custom_return_attributes is None else ''}
         """
         variables = {"now": str(datetime.utcnow()), "batch_size": batch_size}
         async for result in mythic_utilities.graphql_subscription(
-            mythic=mythic, query=subscription, variables=variables, timeout=timeout
+                mythic=mythic, query=subscription, variables=variables, timeout=timeout
         ):
             yield result["callback_stream"]
     except StopAsyncIteration:
         logging.info("stopasynciteration exception in subscribe_new_callbacks")
         pass
     except Exception as e:
         logging.info("some other exception in subscribe_new_callbacks")
         raise e
 
 
 async def subscribe_all_active_callbacks(
-    mythic: mythic_classes.Mythic,
-    timeout: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        timeout: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Executes a graphql query to get information about all currently active callbacks so far, then opens up a subscription for new callbacks.
     This returns an async iterator, which can be used as:
         async for item in subscribe_all_active_callbacks(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.callback_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
     """
     for t in await get_all_active_callbacks(
-        mythic=mythic, custom_return_attributes=custom_return_attributes
+            mythic=mythic, custom_return_attributes=custom_return_attributes
     ):
         yield t
     async for t in subscribe_new_callbacks(
-        mythic=mythic, timeout=timeout, custom_return_attributes=custom_return_attributes, batch_size=1
+            mythic=mythic, timeout=timeout, custom_return_attributes=custom_return_attributes, batch_size=1
     ):
         yield t
 
 
 async def update_callback(
-    mythic: mythic_classes.Mythic,
-    callback_display_id: int,
-    active: bool = None,
-    sleep_info: str = None,
-    locked: bool = None,
-    description: str = None,
-    ips: list[str] = None,
-    user: str = None,
-    host: str = None,
-    os: str = None,
-    architecture: str = None,
-    extra_info: str = None,
-    pid: int = None,
-    process_name: str = None,
-    integrity_level: int = None,
-    domain: str = None
+        mythic: mythic_classes.Mythic,
+        callback_display_id: int,
+        active: bool = None,
+        sleep_info: str = None,
+        locked: bool = None,
+        description: str = None,
+        ips: list[str] = None,
+        user: str = None,
+        host: str = None,
+        os: str = None,
+        architecture: str = None,
+        extra_info: str = None,
+        pid: int = None,
+        process_name: str = None,
+        integrity_level: int = None,
+        domain: str = None
 ):
     update_status = await mythic_utilities.graphql_post(
         mythic=mythic,
         gql_query=graphql_queries.update_callback,
         variables={
             "callback_display_id": callback_display_id,
             "active": active,
@@ -279,17 +279,17 @@
     return update_status["updateCallback"]
 
 
 # ########## Task Functions #################
 
 
 async def get_all_tasks(
-    mythic: mythic_classes.Mythic,
-    custom_return_attributes: str = None,
-    callback_display_id: int = None,
+        mythic: mythic_classes.Mythic,
+        custom_return_attributes: str = None,
+        callback_display_id: int = None,
 ) -> List[dict]:
     """
     Executes a graphql query to get all tasks submitted so far (potentially limited to a single callback).
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
     """
     if callback_display_id is not None:
@@ -315,19 +315,19 @@
     initial_tasks = await mythic_utilities.graphql_post(
         mythic=mythic, query=query, variables=variables
     )
     return initial_tasks["task"]
 
 
 async def subscribe_new_tasks(
-    mythic: mythic_classes.Mythic,
-    batch_size: int = 50,
-    timeout: int = None,
-    callback_display_id: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        batch_size: int = 50,
+        timeout: int = None,
+        callback_display_id: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Execute a graphql subscription for tasks that have a timestamp greater than when this function is called.
     This will only fire once per task, this will not reflect updates to tasks as they go through the tasking process, get processed by agents, and become completed.
     For that, use the subscribe_new_tasks_and_updates function.
     This returns an async iterator, which can be used as:
         async for item in subscribe_new_tasks(...data):
@@ -360,27 +360,27 @@
             {graphql_queries.task_fragment if custom_return_attributes is None else ''}
             """
             variables = {
                 "now": str(datetime.utcnow()),
                 "batch_size": batch_size,
             }
         async for result in mythic_utilities.graphql_subscription(
-            mythic=mythic, query=subscription, variables=variables, timeout=timeout
+                mythic=mythic, query=subscription, variables=variables, timeout=timeout
         ):
             yield result["task_stream"]
     except Exception as e:
         raise e
 
 
 async def subscribe_new_tasks_and_updates(
-    mythic: mythic_classes.Mythic,
-    batch_size: int = 50,
-    timeout: int = None,
-    callback_display_id: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        batch_size: int = 50,
+        timeout: int = None,
+        callback_display_id: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Execute a graphql subscription for tasks that have a timestamp greater than when this function is called.
     This will include when the timestamp on a task updates (every time it gets a response, the status updates, marked as completed, etc).
     If you only want to be notified once about a task, use `subscribe_new_tasks` instead.
     This returns an async iterator, which can be used as:
         async for item in subscribe_new_tasks_and_updates(...data):
@@ -421,74 +421,74 @@
         ):
             yield result["task_stream"]
     except Exception as e:
         raise e
 
 
 async def subscribe_all_tasks(
-    mythic: mythic_classes.Mythic,
-    timeout: int = None,
-    callback_display_id: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        timeout: int = None,
+        callback_display_id: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Executes a graphql query to get information about every task submitted so far, then opens up a subscription for new tasks.
     This returns an async iterator, which can be used as:
         async for item in subscribe_all_tasks(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     for t in await get_all_tasks(
-        mythic=mythic,
-        custom_return_attributes=custom_return_attributes,
+            mythic=mythic,
+            custom_return_attributes=custom_return_attributes,
             callback_display_id=callback_display_id,
     ):
         yield t
     async for t in subscribe_new_tasks(
-        mythic=mythic,
-        timeout=timeout,
-        custom_return_attributes=custom_return_attributes,
+            mythic=mythic,
+            timeout=timeout,
+            custom_return_attributes=custom_return_attributes,
             callback_display_id=callback_display_id,
     ):
         yield t
 
 
 async def subscribe_all_tasks_and_updates(
-    mythic: mythic_classes.Mythic,
-    timeout: int = None,
-    callback_display_id: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        timeout: int = None,
+        callback_display_id: int = None,
+        custom_return_attributes: str = None,
 ) -> AsyncGenerator:
     """
     Executes a graphql query to get information about every task submitted so far, then opens up a subscription for new tasks and updates to all tasks.
     This returns an async iterator, which can be used as:
         async for item in subscribe_all_tasks_and_updates(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     for t in await get_all_tasks(
-        mythic=mythic,
-        custom_return_attributes=custom_return_attributes,
-        callback_display_id=callback_display_id,
+            mythic=mythic,
+            custom_return_attributes=custom_return_attributes,
+            callback_display_id=callback_display_id,
     ):
         yield t
     async for t in subscribe_new_tasks_and_updates(
-        mythic=mythic,
-        timeout=timeout,
-        custom_return_attributes=custom_return_attributes,
-        callback_display_id=callback_display_id,
-        batch_size=1
+            mythic=mythic,
+            timeout=timeout,
+            custom_return_attributes=custom_return_attributes,
+            callback_display_id=callback_display_id,
+            batch_size=1
     ):
         yield t[0]
 
 
 async def add_mitre_attack_to_task(
-    mythic: mythic_classes.Mythic, task_display_id: int, mitre_attack_numbers: List[str]
+        mythic: mythic_classes.Mythic, task_display_id: int, mitre_attack_numbers: List[str]
 ) -> bool:
     """
     Adds the supplied MITRE ATT&CK techniques to the specified task.
     :return: success or failure in adding the techniques
     """
     try:
         query = """
@@ -514,22 +514,22 @@
         return True
 
     except Exception as e:
         raise e
 
 
 async def issue_task(
-    mythic: mythic_classes.Mythic,
-    command_name: str,
-    parameters: Union[str, dict],
-    callback_display_id: int,
-    token_id: int = None,
-    wait_for_complete: bool = False,
-    custom_return_attributes: str = None,
-    timeout: int = None,
+        mythic: mythic_classes.Mythic,
+        command_name: str,
+        parameters: Union[str, dict],
+        callback_display_id: int,
+        token_id: int = None,
+        wait_for_complete: bool = False,
+        custom_return_attributes: str = None,
+        timeout: int = None,
 ) -> dict:
     """
     Create a new task within Mythic for a specific callback.
     `return_on_status` indicates if this command should return immediately, mythic_classes.MythicStatus.Preprocessing, or wait for a certain status before returning.
         This can be helpful if you want ot make sure a task is completed before continuing
     If you have files that you need to upload and leverage as part of your tasking, use the `register_file` function to get back a file_id.
     If you return immediately from this task, you'll get a dictionary with a status, error, and id field for your new task.
@@ -565,18 +565,18 @@
     else:
         raise Exception(
             f"Failed to create task: {submission_status['createTask']['error']}"
         )
 
 
 async def waitfor_task_complete(
-    mythic: mythic_classes.Mythic,
-    task_display_id: int,
-    custom_return_attributes: str = None,
-    timeout: int = None,
+        mythic: mythic_classes.Mythic,
+        task_display_id: int,
+        custom_return_attributes: str = None,
+        timeout: int = None,
 ) -> dict:
     """
     Execute a subscription to wait for a task to reach a certain status or timeout.
     This will return the graphql_queries.task_fragment attributes by default, but this can be overridden with the custom_return_attributes
     """
     subscription = f"""
     subscription TaskWaitForStatus($task_display_id: Int!){{
@@ -584,26 +584,26 @@
             {custom_return_attributes if custom_return_attributes is not None else '...task_fragment'}
         }}
     }}
     {graphql_queries.task_fragment if custom_return_attributes is None else ''}
     """
     variables = {"task_display_id": task_display_id}
     async for result in mythic_utilities.graphql_subscription(
-        mythic=mythic, query=subscription, variables=variables, timeout=timeout
+            mythic=mythic, query=subscription, variables=variables, timeout=timeout
     ):
         if len(result["task_stream"]) != 1:
             raise Exception("task not found")
         if "error" in result["task_stream"][0]["status"] or result["task_stream"][0]["completed"]:
             return result["task_stream"][0]
 
 
 async def issue_task_all_active_callbacks(
-    mythic: mythic_classes.Mythic,
-    command_name: str,
-    parameters: Union[str, dict],
+        mythic: mythic_classes.Mythic,
+        command_name: str,
+        parameters: Union[str, dict],
 ) -> List[dict]:
     """
     Create a new task within Mythic for all currently active callbacks.
     If you have files that you need to upload and leverage as part of your tasking, use the `register_file` function to get back a file_id.
     For each task created, you'll get a dictionary with:
     {
         "status": either "success" or "error",
@@ -643,20 +643,20 @@
         )
         submission_status["createTask"]["callback_display_id"] = callback["display_id"]
         created_tasks.append(submission_status["createTask"])
     return created_tasks
 
 
 async def issue_task_and_waitfor_task_output(
-    mythic: mythic_classes.Mythic,
-    command_name: str,
-    parameters: Union[str, dict],
-    callback_display_id: int,
-    token_id: int = None,
-    timeout: int = None,
+        mythic: mythic_classes.Mythic,
+        command_name: str,
+        parameters: Union[str, dict],
+        callback_display_id: int,
+        token_id: int = None,
+        timeout: int = None,
 ) -> bytes:
     task = await issue_task(
         mythic=mythic,
         command_name=command_name,
         parameters=parameters,
         callback_display_id=callback_display_id,
         token_id=token_id,
@@ -670,17 +670,17 @@
     )
 
 
 # ######### File Browser Functions ###########
 
 
 async def get_all_filebrowser(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None,
-    host: str = None,
-    batch_size: int = 100,
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None,
+        host: str = None,
+        batch_size: int = 100,
 ) -> AsyncGenerator:
     """
     Executes a graphql query to get information about all current filebrowser data.
     This returns an async iterator, which can be used as:
         async for item in get_all_filebrowser(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.filebrowser_fragment.
@@ -708,19 +708,19 @@
             yield output["mythictree"]
             offset += len(output["mythictree"])
         else:
             break
 
 
 async def subscribe_new_filebrowser(
-    mythic: mythic_classes.Mythic,
-    host: str = None,
-    batch_size: int = 50,
-    timeout: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        host: str = None,
+        batch_size: int = 50,
+        timeout: int = None,
+        custom_return_attributes: str = None,
 ):
     """
     Executes a graphql query to get information about new filebrowser data since the function was called.
     This returns an async iterator, which can be used as:
         async for item in subscribe_new_filebrowser(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.filebrowser_fragment.
@@ -744,47 +744,47 @@
             variables={"host": host_search, "batch_size": batch_size, "now": str(datetime.utcnow())},
             timeout=timeout
     ):
         yield output["mythictree_stream"]
 
 
 async def subscribe_all_filebrowser(
-    mythic: mythic_classes.Mythic,
-    host: str = None,
-    timeout: int = None,
-    batch_size: int = 100,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        host: str = None,
+        timeout: int = None,
+        batch_size: int = 100,
+        custom_return_attributes: str = None,
 ):
     """
     Executes a graphql query to get information about all filebrowser data so far, then opens up a subscription for new filebrowser data.
     This returns an async iterator, which can be used as:
         async for item in subscribe_all_filebrowser(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.filebrowser_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     async for t in get_all_filebrowser(
-        mythic=mythic, custom_return_attributes=custom_return_attributes,
-        host=host, batch_size=batch_size
+            mythic=mythic, custom_return_attributes=custom_return_attributes,
+            host=host, batch_size=batch_size
     ):
         yield t
     async for t in subscribe_new_filebrowser(
-        mythic=mythic, timeout=timeout, custom_return_attributes=custom_return_attributes,
-        host=host, batch_size=batch_size
+            mythic=mythic, timeout=timeout, custom_return_attributes=custom_return_attributes,
+            host=host, batch_size=batch_size
     ):
         yield t
 
 
 # ######### Command Functions ##############
 
 
 async def get_all_commands_for_payloadtype(
-    mythic: mythic_classes.Mythic,
-    payload_type_name: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        payload_type_name: str,
+        custom_return_attributes: str = None,
 ) -> List:
     """
     Executes a graphql query to get information about all current commands for a payload type.
     The default set of attributes returned in the dictionary can be found at graphql_queries.commands_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `attributes` and `cmd` fields, everything else is optional.
     """
     query = f"""
@@ -801,26 +801,26 @@
     return initial_commands["command"]
 
 
 # ######### Payload Functions ##############
 
 
 async def create_payload(
-    mythic: mythic_classes.Mythic,
-    payload_type_name: str,
-    filename: str,
-    operating_system: str,
-    c2_profiles: List[dict],
-    commands: List[str] = None,
-    build_parameters: List[dict] = None,
-    description: str = "",
-    return_on_complete: bool = True,
-    timeout: int = None,
-    custom_return_attributes: str = None,
-    include_all_commands: bool = False,
+        mythic: mythic_classes.Mythic,
+        payload_type_name: str,
+        filename: str,
+        operating_system: str,
+        c2_profiles: List[dict],
+        commands: List[str] = None,
+        build_parameters: List[dict] = None,
+        description: str = "",
+        return_on_complete: bool = True,
+        timeout: int = None,
+        custom_return_attributes: str = None,
+        include_all_commands: bool = False,
 ) -> dict:
     """
     This tasks Mythic to create a new payload based on the supplied parameters. If `return_on_complete` is false, then this will return immediately after issuing the task to Mythic.
     If `return_on_complete` is true, then this will do a subsequent subscription to wait for the payload container to finish building.
     c2_profiles is a list of dictionaries where each dictionary holds the following information:
         {
             "c2_profile": "name of the profile, like http",
@@ -847,15 +847,15 @@
     create_payload_dict["commands"] = commands if commands is not None else []
     for c in c2_profiles:
         if "c2_profile" not in c:
             raise Exception(
                 "C2 Profile instance must have 'c2_profile` key with name of c2 profile"
             )
         if "c2_profile_parameters" not in c or not isinstance(
-            c["c2_profile_parameters"], dict
+                c["c2_profile_parameters"], dict
         ):
             raise Exception(
                 "C2 Profile instance must have a 'c2_profile_parameters' dictionary where the keys are the c2 profile parameter names and the values are what you want to specify"
             )
     create_payload_dict["c2_profiles"] = c2_profiles
     if build_parameters is not None:
         for p in build_parameters:
@@ -876,29 +876,29 @@
             try:
                 attributes = c["attributes"]
                 passes_all_restrictions = True
                 if "filter_by_build_parameter" in attributes:
                     # check if the command is allowed by build parameter restrictions
                     for build_param in create_payload_dict["build_parameters"]:
                         if (
-                            build_param["name"] in attributes["filter_by_build_parameter"]
-                            and attributes["filter_by_build_parameter"]
-                            != build_param["value"]
+                                build_param["name"] in attributes["filter_by_build_parameter"]
+                                and attributes["filter_by_build_parameter"]
+                                != build_param["value"]
                         ):
                             passes_all_restrictions = False
                 if "load_only" in attributes and attributes["load_only"]:
                     passes_all_restrictions = False
                 # check if the command is allowed by supported_os
                 if (
-                    len(attributes["supported_os"]) != 0
-                    and operating_system not in attributes["supported_os"]
+                        len(attributes["supported_os"]) != 0
+                        and operating_system not in attributes["supported_os"]
                 ):
                     passes_all_restrictions = False
                 if passes_all_restrictions or (
-                    "builtin" in attributes and attributes["builtin"]
+                        "builtin" in attributes and attributes["builtin"]
                 ):
                     create_payload_dict["commands"].append(c["cmd"])
             except Exception as e:
                 print(f"[-] Error trying to parse command information: {e}")
                 pass
     payload = await mythic_utilities.graphql_post(
         mythic=mythic,
@@ -914,24 +914,24 @@
             custom_return_attributes=custom_return_attributes,
         )
     else:
         return payload["createPayload"]
 
 
 async def create_wrapper_payload(
-    mythic: mythic_classes.Mythic,
-    payload_type_name: str,
-    filename: str,
-    operating_system: str,
-    wrapped_payload_uuid: str,
-    build_parameters: List[dict] = None,
-    description: str = "",
-    return_on_complete: bool = True,
-    timeout: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        payload_type_name: str,
+        filename: str,
+        operating_system: str,
+        wrapped_payload_uuid: str,
+        build_parameters: List[dict] = None,
+        description: str = "",
+        return_on_complete: bool = True,
+        timeout: int = None,
+        custom_return_attributes: str = None,
 ):
     """
     This tasks Mythic to create a new payload based on the supplied parameters. If `return_on_complete` is false, then this will return immediately after issuing the task to Mythic.
     If `return_on_complete` is true, then this will do a subsequent subscription to wait for the payload container to finish building.
     build_parameters is a list of dictionaries where each dictionary holds the following information:
     {
         "name": "build parameter name", "value": "build parameter value"
@@ -968,18 +968,18 @@
             custom_return_attributes=custom_return_attributes,
         )
     else:
         return payload["createPayload"]
 
 
 async def waitfor_payload_complete(
-    mythic: mythic_classes.Mythic,
-    payload_uuid: str,
-    timeout: int = None,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        payload_uuid: str,
+        timeout: int = None,
+        custom_return_attributes: str = None,
 ) -> dict:
     """
     Execute a subscription to wait for the `build_phase` of the specified payload to be something other than 'building'.
     This will return when the payload is finished, either successfully or with an error, or when the timeout is reached.
     The default set of attributes returned in the dictionary can be found at graphql_queries.payload_build_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `build_phase` fields, everything else is optional.
     """
@@ -989,24 +989,24 @@
                 {custom_return_attributes if custom_return_attributes is not None else '...payload_build_fragment'}
             }}
         }}
         {graphql_queries.payload_build_fragment if custom_return_attributes is None else ''}
         """
     variables = {"uuid": payload_uuid}
     async for result in mythic_utilities.graphql_subscription(
-        mythic=mythic, query=subscription, variables=variables, timeout=timeout
+            mythic=mythic, query=subscription, variables=variables, timeout=timeout
     ):
         if len(result["payload"]) > 0:
             if result["payload"][0]["build_phase"] != "building":
                 return result["payload"][0]
     return None
 
 
 async def get_all_payloads(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None
 ) -> List[dict]:
     """
     Get information about all payloads currently registered with Mythic (this includes deleted payloads and autogenerated ones for tasking).
     The default attributes returned for each payload can be found at graphql_queries.payload_data_fragment, but can be modified with thte custom_return_attributes variable.
     """
     payload_query = f"""
     query PayloadInfoQuery{{
@@ -1017,17 +1017,17 @@
     {graphql_queries.payload_data_fragment if custom_return_attributes is None else ''}
     """
     payloads = await mythic_utilities.graphql_post(mythic=mythic, query=payload_query)
     return payloads["payload"]
 
 
 async def get_payload_by_uuid(
-    mythic: mythic_classes.Mythic,
-    payload_uuid: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        payload_uuid: str,
+        custom_return_attributes: str = None,
 ) -> dict:
     """
     Get information about the specified payload.
     The default parameters returned can be found at graphql_queries.payload_data_fragment, but can be modified with the custom_return_attributes
     """
     payload_query = f"""
     query PayloadInfoQuery($payload_uuid: String!){{
@@ -1042,16 +1042,16 @@
     )
     if len(payloads["payload"]) != 1:
         raise Exception("Failed to find payload")
     return payloads["payload"][0]
 
 
 async def download_payload(
-    mythic: mythic_classes.Mythic,
-    payload_uuid: str,
+        mythic: mythic_classes.Mythic,
+        payload_uuid: str,
 ) -> bytes:
     """
     Download the raw bytes for the payload specified by payload_uuid
     """
     payload_query = f"""
     query PayloadInfoQuery($uuid: String!){{
         payload(where: {{uuid: {{_eq: $uuid}}}}){{
@@ -1067,21 +1067,69 @@
         raise Exception("Failed to find payload")
     try:
         return await download_file(mythic=mythic, file_uuid=payload['payload'][0]['filemetum']['agent_file_id'])
     except Exception as e:
         raise e
 
 
+async def payload_check_config(mythic: mythic_classes.Mythic,
+                               payload_uuid: str,
+                               ) -> dict:
+    """
+    Check the payload's configuration against C2 profile configurations
+    :param mythic:
+    :param payload_uuid:
+    :return: dict with status, error, and output keys
+    """
+    config_query = f"""
+    query checkPayloadConfig($uuid: String!){{
+        config_check(uuid: $uuid){{
+            status
+            error
+            output
+        }}
+    }}
+    """
+    configStatus = await mythic_utilities.graphql_post(
+        mythic=mythic, query=config_query, variables={"uuid": payload_uuid}
+    )
+    return configStatus["config_check"]
+
+
+async def payload_redirect_rules(mythic: mythic_classes.Mythic,
+                                 payload_uuid: str,
+                                 ) -> dict:
+    """
+    Get redirect rules for a payload
+    :param mythic:
+    :param payload_uuid:
+    :return: dict with status, error, and output keys
+    """
+    config_query = f"""
+    query checkPayloadRedirectRules($uuid: String!){{
+        redirect_rules(uuid: $uuid){{
+            status
+            error
+            output
+        }}
+    }}
+    """
+    redirectRules = await mythic_utilities.graphql_post(
+        mythic=mythic, query=config_query, variables={"uuid": payload_uuid}
+    )
+    return redirectRules["redirect_rules"]
+
+
 # ######### Task Output Functions ###########
 
 
 async def waitfor_for_task_output(
-    mythic: mythic_classes.Mythic,
-    task_display_id: int,
-    timeout: int = None,
+        mythic: mythic_classes.Mythic,
+        task_display_id: int,
+        timeout: int = None,
 ) -> bytes:
     """
     Execute a subscription for the specified task and aggregate all of the output for it.
     This subscription returns when the task is done (completed or errored) or when the timeout is hit.
     The function returns an aggregated binary blob of all of the responses.
     """
     subscription = f"""
@@ -1095,27 +1143,27 @@
             }}
         }}
         {graphql_queries.user_output_fragment}
     """
     variables = {"task_display_id": task_display_id}
     aggregated_output = []
     async for result in mythic_utilities.graphql_subscription(
-        mythic=mythic, query=subscription, variables=variables, timeout=timeout
+            mythic=mythic, query=subscription, variables=variables, timeout=timeout
     ):
         aggregated_output = result["task_stream"][0]["responses"]
         if "error" in result["task_stream"][0]["status"] or result["task_stream"][0]["completed"]:
             break
     final_output = b""
     for output in aggregated_output:
         final_output += base64.b64decode(output["response_text"])
     return final_output
 
 
 async def get_all_task_output(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10
 ) -> AsyncGenerator:
     """
     Execute a query to get all current responses.
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_output_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     query = f"""
@@ -1135,15 +1183,15 @@
             yield initial["response"]
             offset += len(initial["response"])
         else:
             break
 
 
 async def get_all_task_output_by_id(
-    mythic: mythic_classes.Mythic, task_display_id: int, custom_return_attributes: str = None
+        mythic: mythic_classes.Mythic, task_display_id: int, custom_return_attributes: str = None
 ) -> List[dict]:
     """
     Execute a query to get all responses for a given task.
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_output_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     query = f"""
@@ -1157,18 +1205,18 @@
     initial = await mythic_utilities.graphql_post(
         mythic=mythic, query=query, variables={"task_display_id": task_display_id}
     )
     return initial["response"]
 
 
 async def subscribe_new_task_output(
-    mythic: mythic_classes.Mythic,
-    timeout: int = None,
-    custom_return_attributes: str = None,
-    batch_size: int = 50,
+        mythic: mythic_classes.Mythic,
+        timeout: int = None,
+        custom_return_attributes: str = None,
+        batch_size: int = 50,
 ) -> AsyncGenerator:
     """
     Execute a subscription to get all new responses.
     This returns an async iterator, which can be used as:
         async for item in subscribe_new_task_output(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_output_fragment.
@@ -1183,53 +1231,53 @@
     {graphql_queries.task_output_fragment if custom_return_attributes is None else ''}
     """
     try:
         latest_time = str(datetime.utcnow())
         while True:
             variables = {"now": latest_time, "batch_size": batch_size}
             async for result in mythic_utilities.graphql_subscription(
-                mythic=mythic, query=subscription, variables=variables, timeout=timeout
+                    mythic=mythic, query=subscription, variables=variables, timeout=timeout
             ):
                 yield result["response_stream"]
 
     except Exception as e:
         raise e
 
 
 async def subscribe_all_task_output(
-    mythic: mythic_classes.Mythic,
-    timeout: int = None,
-    custom_return_attributes: str = None,
-    batch_size: int = 10
+        mythic: mythic_classes.Mythic,
+        timeout: int = None,
+        custom_return_attributes: str = None,
+        batch_size: int = 10
 ) -> AsyncGenerator:
     """
     Execute a query to get all current responses, then execute a subscription to get all new responses.
     This returns an async iterator, which can be used as:
         async for item in subscribe_all_task_output(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.task_output_fragment.
     If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` and `timestamp` fields, everything else is optional.
     """
     async for t in get_all_task_output(
-        mythic=mythic, custom_return_attributes=custom_return_attributes, batch_size=batch_size
+            mythic=mythic, custom_return_attributes=custom_return_attributes, batch_size=batch_size
     ):
         yield t
     async for t in subscribe_new_task_output(
-        mythic=mythic, custom_return_attributes=custom_return_attributes, timeout=timeout, batch_size=batch_size
+            mythic=mythic, custom_return_attributes=custom_return_attributes, timeout=timeout, batch_size=batch_size
     ):
         yield t
 
 
 # ########## Operator Functions ##############
 
 
 async def create_operator(
-    mythic: mythic_classes.Mythic,
-    username: str,
-    password: str,
+        mythic: mythic_classes.Mythic,
+        username: str,
+        password: str,
 ) -> dict:
     """
     Create a new operator within Mythic with the specified username and password.
     If you want to then add that operator to an operation, use the add_operator_to_operation function.
     This returns a dictionary with the information from the graphql_queries.create_operator_fragment.
     """
     return await mythic_utilities.graphql_post(
@@ -1297,15 +1345,16 @@
         }
         """,
         variables={"username": username, "admin": active},
     )
     return resp
 
 
-async def set_password(mythic: mythic_classes.Mythic, username: str, new_password: str, old_password: str = None) -> dict:
+async def set_password(mythic: mythic_classes.Mythic, username: str, new_password: str,
+                       old_password: str = None) -> dict:
     resp = await execute_custom_query(
         mythic=mythic,
         query="""
         query getUserID($username: String!) {
             operator(where: {username: {_eq: $username}}){
                 id
             }
@@ -1359,19 +1408,20 @@
                 current_operation
             }}
         }}
         """,
     )
     return resp
 
+
 # ########## File Functions ##############
 
 
 async def register_file(
-    mythic: mythic_classes.Mythic, filename: str, contents: bytes
+        mythic: mythic_classes.Mythic, filename: str, contents: bytes
 ) -> str:
     """
     Upload a file to Mythic via a form and get back a file_id that can be used in tasking.
     Returns the new file_id that can be used in subsequent tasking.
     """
     form = aiohttp.FormData()
     form.add_field("file", value=contents, filename=filename)
@@ -1390,28 +1440,28 @@
         response = await mythic_utilities.http_get(mythic=mythic, url=url)
         return response
     except Exception as e:
         raise e
 
 
 async def download_file_chunked(
-    mythic: mythic_classes.Mythic, file_uuid: str, chunk_size: int = 512000
+        mythic: mythic_classes.Mythic, file_uuid: str, chunk_size: int = 512000
 ) -> AsyncGenerator:
     url = f"{mythic.http}{mythic.server_ip}:{mythic.server_port}/direct/download/{file_uuid}"
     try:
         async for t in mythic_utilities.http_get_chunked(
-            mythic=mythic, url=url, chunk_size=chunk_size
+                mythic=mythic, url=url, chunk_size=chunk_size
         ):
             yield t
     except Exception as e:
         raise e
 
 
 async def get_all_downloaded_files(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 100
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 100
 ) -> AsyncGenerator:
     """
     Execute a query to get metadata about all files Mythic knows about that are downloaded from agents.
     To download the contents of a file, use the `download_file` function with the agent_file_id.
     This returns an async iterator, which can be used as:
         async for item in get_all_downloaded_files(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
@@ -1453,15 +1503,16 @@
             filemeta_stream(where: {{is_download_from_agent: {{_eq: true}}, complete: {{_eq: true}}}}, cursor: {{initial_value: {{timestamp: $now}}}}, batch_size: $batch_size){{
                 {custom_return_attributes if custom_return_attributes is not None else '...file_data_fragment'}
             }}
         }}
         {graphql_queries.file_data_fragment if custom_return_attributes is None else ''}
         """
     async for result in mythic_utilities.graphql_subscription(
-        mythic=mythic, query=file_query, timeout=timeout, variables={"batch_size": batch_size, "now": str(datetime.utcnow())}
+            mythic=mythic, query=file_query, timeout=timeout,
+            variables={"batch_size": batch_size, "now": str(datetime.utcnow())}
     ):
         yield result["filemeta_stream"]
 
 
 async def subscribe_all_downloaded_files(mythic: mythic_classes.Mythic,
                                          custom_return_attributes: str = None,
                                          timeout: int = None,
@@ -1473,21 +1524,21 @@
         If you want to use your own `custom_return_attributes` string to identify what information you want back, you have to include the `id` field, everything else is optional.
         """
     async for result in get_all_downloaded_files(
             mythic=mythic, batch_size=batch_size, custom_return_attributes=custom_return_attributes
     ):
         yield result
     async for result in subscribe_new_downloaded_files(
-        mythic=mythic, batch_size=batch_size, timeout=timeout, custom_return_attributes=custom_return_attributes
+            mythic=mythic, batch_size=batch_size, timeout=timeout, custom_return_attributes=custom_return_attributes
     ):
         yield result
 
 
 async def get_all_screenshots(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10
 ) -> AsyncGenerator:
     """
     Execute a query to get metadata about all of the screenshots Mythic knows about that are downloaded from agents.
     To download the contents of a file, use the `download_file` function with the agent_file_id.
     This returns an async iterator, which can be used as:
         async for item in get_all_screenshots(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
@@ -1511,15 +1562,15 @@
             yield output["filemeta"]
             offset += len(output["filemeta"])
         else:
             break
 
 
 async def get_all_uploaded_files(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10,
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None, batch_size: int = 10,
 ) -> AsyncGenerator:
     """
     Execute a query to get metadata about all of the uploaded files Mythic knows about.
     To download the contents of a file, use the `download_file` function with the agent_file_id.
     This returns an async iterator, which can be used as:
         async for item in get_all_uploaded_files(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
@@ -1543,15 +1594,15 @@
             yield output["filemeta"]
             offset += len(output["filemeta"])
         else:
             break
 
 
 async def update_file_comment(
-    mythic: mythic_classes.Mythic, file_uuid: str, comment: str
+        mythic: mythic_classes.Mythic, file_uuid: str, comment: str
 ) -> dict:
     """
     Update a file's comment within Mythic
     """
     update_comment_mutation = """
     mutation updateCommentMutation($file_uuid: String!, $comment: String!){
         update_filemeta(where: {agent_file_id: {_eq: $file_uuid}}, _set: {comment: $comment}) {
@@ -1570,15 +1621,15 @@
     return updated["update_filemeta"]
 
 
 # ########## Operations Functions #############
 
 
 async def get_operations(
-    mythic: mythic_classes.Mythic, custom_return_attributes: str = None
+        mythic: mythic_classes.Mythic, custom_return_attributes: str = None
 ) -> List[dict]:
     """
     Get information about the current operations known to the authenticated user.
     Default return attributes for each operation can be found at graphql_queries.get_operations_fragment, but can be overridden with custom_return_attributes
     """
     get_operations_query = f"""
     query getOperations{{
@@ -1592,17 +1643,17 @@
         mythic=mythic,
         query=get_operations_query,
     )
     return operations["operation"]
 
 
 async def create_operation(
-    mythic: mythic_classes.Mythic,
-    operation_name: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        operation_name: str,
+        custom_return_attributes: str = None,
 ):
     """
     Create a new operation within Mythic (the account creating the operation will automatically be the operation lead).
     The default attributes returned are outlined in graphql_queries.create_operation_fragment. These can be overridden with the custom_retun_attributes.
     """
     create_operation_query = f"""
     mutation newOperationMutation($name: String){{
@@ -1617,18 +1668,18 @@
         query=create_operation_query,
         variables={"name": operation_name},
     )
     return created_operation["createOperation"]
 
 
 async def add_operator_to_operation(
-    mythic: mythic_classes.Mythic,
-    operation_name: str,
-    operator_username: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        operation_name: str,
+        operator_username: str,
+        custom_return_attributes: str = None,
 ) -> dict:
     """
     Add the specified operator to the specified operation. This will raise Exceptions if the operator/operation cannot be found or if the user is already added.
     If you want to adjust the lead of an operation, use the `update_operation` function.
     view_mode can either be "operator", "spectator", "lead" depending on the level of access you want to provide to the new operator in the operation.
     You must be authenticating as the lead of the operation or as a global admin to perform this sort of update.
     The default return values can be found at graphql_queries.add_operator_to_operation_fragment, but can be overridden with the custom_return_attributes.
@@ -1639,16 +1690,16 @@
         gql_query=graphql_queries.get_operation_and_operator_by_name,
         variables={
             "operation_name": operation_name,
             "operator_username": operator_username,
         },
     )
     if (
-        len(operator_and_operation["operation"]) != 1
-        or len(operator_and_operation["operator"]) != 1
+            len(operator_and_operation["operation"]) != 1
+            or len(operator_and_operation["operator"]) != 1
     ):
         raise Exception("Didn't find an exact match for the operation name and username")
     if len(operator_and_operation["operation"][0]["operatoroperations"]) != 0:
         raise Exception("Operator already added to operation")
     add_operator_to_operation_query = f"""
     mutation addNewOperators($operation_id: Int!, $add_users: [Int]) {{
         updateOperatorOperation(operation_id: $operation_id, add_users: $add_users) {{
@@ -1664,18 +1715,18 @@
     add_operator = await mythic_utilities.graphql_post(
         mythic=mythic, query=add_operator_to_operation_query, variables=variables
     )
     return add_operator["updateOperatorOperation"]
 
 
 async def remove_operator_from_operation(
-    mythic: mythic_classes.Mythic,
-    operation_name: str,
-    operator_username: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        operation_name: str,
+        operator_username: str,
+        custom_return_attributes: str = None,
 ) -> dict:
     """
     Removes the specified operator from the specified operation. This will raise Exceptions if the operator/operation cannot be found or if the user isn't part of the operation already.
     If you want to adjust the lead of an operation, use the `update_operation` function.
     You must be authenticating as the lead of the operation or as a global admin to perform this sort of update.
     The default return values can be found at graphql_queries.remove_operator_from_operation_fragment, but can be overridden with the custom_return_attributes.
     """
@@ -1684,16 +1735,16 @@
         gql_query=graphql_queries.get_operation_and_operator_by_name,
         variables={
             "operation_name": operation_name,
             "operator_username": operator_username,
         },
     )
     if (
-        len(operator_and_operation["operation"]) != 1
-        or len(operator_and_operation["operator"]) != 1
+            len(operator_and_operation["operation"]) != 1
+            or len(operator_and_operation["operator"]) != 1
     ):
         raise Exception("Didn't find an exact match for the operation name and username")
     if len(operator_and_operation["operation"][0]["operatoroperations"]) != 1:
         raise Exception("Operator not part of operation")
     remove_operator_mutation = f"""
     mutation removeOperators($operation_id: Int!, $remove_users: [Int]) {{
         updateOperatorOperation(operation_id: $operation_id, remove_users: $remove_users) {{
@@ -1709,19 +1760,19 @@
     remove_operator = await mythic_utilities.graphql_post(
         mythic=mythic, query=remove_operator_mutation, variables=variables
     )
     return remove_operator["updateOperatorOperation"]
 
 
 async def update_operator_in_operation(
-    mythic: mythic_classes.Mythic,
-    view_mode: str,
-    operation_name: str,
-    operator_username: str,
-    custom_return_attributes: str = None,
+        mythic: mythic_classes.Mythic,
+        view_mode: str,
+        operation_name: str,
+        operator_username: str,
+        custom_return_attributes: str = None,
 ) -> dict:
     """
     Updates the specified operator in the specified operation. This will raise Exceptions if the operator/operation cannot be found or if the user isn't part of the operation already.
     If you want to adjust the lead of an operation, use the `update_operation` function.
     You must be authenticating as the lead of the operation or as a global admin to perform this sort of update.
     The default return values can be found at graphql_queries.update_operator_in_operation_fragment, but can be overridden with the custom_return_attributes.
     """
@@ -1730,16 +1781,16 @@
         gql_query=graphql_queries.get_operation_and_operator_by_name,
         variables={
             "operation_name": operation_name,
             "operator_username": operator_username,
         },
     )
     if (
-        len(operator_and_operation["operation"]) != 1
-        or len(operator_and_operation["operator"]) != 1
+            len(operator_and_operation["operation"]) != 1
+            or len(operator_and_operation["operator"]) != 1
     ):
         raise Exception("Didn't find an exact match for the operation name and username")
     if len(operator_and_operation["operation"][0]["operatoroperations"]) != 1:
         raise Exception("Operator not part of operation")
     query = f"""
     mutation updateOperatorViewMode($operation_id: Int!, $view_mode_operators: [Int], $view_mode_spectators: [Int]) {{
         updateOperatorOperation(operation_id: $operation_id, view_mode_operators: $view_mode_operators, view_mode_spectators: $view_mode_spectators) {{
@@ -1756,22 +1807,22 @@
     update_operator = await mythic_utilities.graphql_post(
         mythic=mythic, query=query, variables=variables
     )
     return update_operator["updateOperatorOperation"]
 
 
 async def update_operation(
-    mythic: mythic_classes.Mythic,
-    operation_name: str,
-    lead_operator_username: str = None,
-    new_operation_name: str = None,
-    channel: str = None,
-    webhook: str = None,
-    complete: bool = None,
-    deleted: bool = None,
+        mythic: mythic_classes.Mythic,
+        operation_name: str,
+        lead_operator_username: str = None,
+        new_operation_name: str = None,
+        channel: str = None,
+        webhook: str = None,
+        complete: bool = None,
+        deleted: bool = None,
 ) -> None:
     """
     This function updates various aspects about the named operation. You must be either the lead of the operation or a global admin to edit this information.
     """
     get_operation_by_name = """
     query getOperationByName($operation_name: String!){
         operation(where: {name: {_eq: $operation_name}}){
@@ -1839,15 +1890,15 @@
         query=update_operation_mutation,
         variables=variables,
     )
     return result["updateOperation"]
 
 
 async def update_current_operation_for_user(
-    mythic: mythic_classes.Mythic, operator_id: int, operation_id: int
+        mythic: mythic_classes.Mythic, operator_id: int, operation_id: int
 ):
     """
     Sets the specified operation as current for the specified user.
     """
     query = """
     mutation updateCurrentOperationMutation($operator_id: Int!, $operation_id: Int!) {
         updateCurrentOperation(user_id: $operator_id, operation_id: $operation_id) {
@@ -1865,19 +1916,19 @@
     return results["updateCurrentOperation"]
 
 
 # ############ Process Functions ##############
 
 
 async def subscribe_new_processes(
-    mythic: mythic_classes.Mythic,
-    host: str = None,
-    custom_return_attributes: str = None,
-    batch_size: int = 100,
-    timeout: int = None
+        mythic: mythic_classes.Mythic,
+        host: str = None,
+        custom_return_attributes: str = None,
+        batch_size: int = 100,
+        timeout: int = None
 ) -> AsyncGenerator:
     """
     Execute a query against Mythic to get all processes on this host that hooks into Mythic's process browser.
     This returns an async iterator, which can be used as:
         async for item in stream_processes(...data):
             print(item) <--- item will always be a dictionary based on the data you're getting back
     The default set of attributes returned in the dictionary can be found at graphql_queries.mythictree_fragment.
@@ -1892,17 +1943,17 @@
         mythictree_stream(batch_size: $batch_size, where: {{host: {{_ilike: $host}}, tree_type: {{_eq: "process"}}}}, cursor: {{initial_value: {{timestamp: $now}}}}){{
             {custom_return_attributes if custom_return_attributes is not None else '...mythictree_fragment'}
         }}
     }}
     {graphql_queries.mythictree_fragment if custom_return_attributes is None else ''}
     """
     async for output in mythic_utilities.graphql_subscription(
-        mythic=mythic, query=process_query,
-        variables={"host": host_search, "batch_size": batch_size, "now": str(datetime.utcnow())},
-        timeout=timeout
+            mythic=mythic, query=process_query,
+            variables={"host": host_search, "batch_size": batch_size, "now": str(datetime.utcnow())},
+            timeout=timeout
     ):
         yield output["mythictree_stream"]
 
 
 async def get_all_processes(
         mythic: mythic_classes.Mythic,
         host: str = None,
@@ -1929,15 +1980,16 @@
         }}
     }}
     {graphql_queries.mythictree_fragment if custom_return_attributes is None else ''}
     """
     offset = 0
     while True:
         output = await mythic_utilities.graphql_post(
-                mythic=mythic, query=process_query, variables={"host": host_search, "batch_size": batch_size, "offset": offset}
+            mythic=mythic, query=process_query,
+            variables={"host": host_search, "batch_size": batch_size, "offset": offset}
         )
         if len(output["mythictree"]) > 0:
             yield output["mythictree"]
             offset += len(output["mythictree"])
         else:
             break
 
@@ -1955,16 +2007,17 @@
         yield t
     async for t in subscribe_new_processes(mythic=mythic, host=host,
                                            custom_return_attributes=custom_return_attributes,
                                            batch_size=batch_size,
                                            timeout=timeout):
         yield t
 
+
 # ####### Credential Functions #############
-async def create_credential(mythic:mythic_classes.Mythic,
+async def create_credential(mythic: mythic_classes.Mythic,
                             credential: str,
                             account: str = "",
                             realm: str = "",
                             comment: str = "",
                             credential_type: str = "") -> dict:
     createCredentialMutation = """
     mutation createCredential($comment: String!, $account: String!, $realm: String!, $credential_type: String!, $credential: String!) {
@@ -1987,15 +2040,15 @@
     return output["createCredential"]
 
 
 # ####### Analytic-based Functions ############
 
 
 async def get_unique_compromised_hosts(
-    mythic: mythic_classes.Mythic,
+        mythic: mythic_classes.Mythic,
 ) -> List[str]:
     """
     Query all callbacks, filebrowser data, and process data in the current operation and get a unique list of hostnames.
     """
     query = """
     query uniqueHosts{
         callback(distinct_on: host) {
@@ -2023,15 +2076,15 @@
     for r in results["payloadonhost"]:
         unique_results.add(r["host"])
     unique_results.discard("")
     return list(unique_results)
 
 
 async def get_unique_compromised_accounts(
-    mythic: mythic_classes.Mythic,
+        mythic: mythic_classes.Mythic,
 ) -> List[str]:
     """
     Get all of the user accounts from callbacks and credentials, then return a unique list of those.
     """
     query = """
     query uniqueAccounts{
         callback {
@@ -2054,15 +2107,15 @@
             unique_results.add(c["host"] + "/" + c["user"])
     for c in results["credential"]:
         unique_results.add(c["realm"] + "/" + c["account"])
     return list(unique_results)
 
 
 async def get_unique_compromised_ips(
-    mythic: mythic_classes.Mythic,
+        mythic: mythic_classes.Mythic,
 ) -> List[str]:
     """
     Query all callbacks to get a unique list of ip addresses.
     """
     query = """
     query uniqueIPs{
         callback {
@@ -2114,14 +2167,15 @@
         }
     }
     """
 
     return await mythic_utilities.graphql_post(mythic=mythic, query=query, variables={"webhook_data": webhook_data,
                                                                                       "webhook_type": webhook_type})
 
+
 # ####### Tag Functions ############
 
 
 async def create_tag_type(
         mythic: mythic_classes.Mythic,
         color: str = "#71a0d0",
         description: str = "",
@@ -2224,14 +2278,15 @@
             mutation createTag($tagtype_id: Int!, $source: String!, $url: String!, $data: jsonb!, ${target_object}: Int!) {{
               insert_tag_one(object: {{data: $data, source: $source, tagtype_id: $tagtype_id, url: $url, {target_object}:${target_object}}}) {{
                 id
                 {target_object}
               }}
             }}
             """
+
     output = []
     if credential_ids is not None:
         for target_id in credential_ids:
             resp = await mythic_utilities.graphql_post(mythic=mythic, query=get_mutation("credential_id"), variables={
                 "tagtype_id": tag_type_id, "source": source, "url": url, "data": data, "credential_id": target_id
             })
             output.append(resp)
@@ -2268,8 +2323,7 @@
     if taskartifact_ids is not None:
         for target_id in taskartifact_ids:
             resp = await mythic_utilities.graphql_post(mythic=mythic, query=get_mutation("taskartifact_id"), variables={
                 "tagtype_id": tag_type_id, "source": source, "url": url, "data": data, "taskartifact_id": target_id
             })
             output.append(resp)
     return output
-
```

### Comparing `mythic-0.1.0rc7/mythic/mythic_classes.py` & `mythic-0.1.0rc8/mythic/mythic_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.refresh_token = refresh_token
         self.server_ip = server_ip
         self.server_port = server_port
         self.ssl = ssl
         self.http = "http://" if not ssl else "https://"
         self.ws = "ws://" if not ssl else "wss://"
         self.global_timeout = global_timeout if global_timeout is not None else -1
-        self.scripting_version = "0.1.0rc7"
+        self.scripting_version = "0.1.0rc8"
         self.current_operation_id = 0
         self.schema = schema
 
     def __str__(self):
         return json.dumps(
             {
                 "username": self.username,
```

### Comparing `mythic-0.1.0rc7/mythic/mythic_utilities.py` & `mythic-0.1.0rc8/mythic/mythic_utilities.py`

 * *Files identical despite different names*

### Comparing `mythic-0.1.0rc7/mythic.egg-info/PKG-INFO` & `mythic-0.1.0rc8/mythic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mythic
-Version: 0.1.0rc7
+Version: 0.1.0rc8
 Summary: Interact with Mythic C2 Framework Instances
 Home-page: https://docs.mythic-c2.net/scripting
 Author: @its_a_feature_
 Author-email: 
 License: BSD3
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mythic-0.1.0rc7/setup.py` & `mythic-0.1.0rc8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="mythic",
-    version="0.1.0rc7",
+    version="0.1.0rc8",
     description="Interact with Mythic C2 Framework Instances",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://docs.mythic-c2.net/scripting",
     author="@its_a_feature_",
     author_email="",
     license="BSD3",
```

