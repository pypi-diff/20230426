# Comparing `tmp/waldur-slurm-agent-0.1.3.tar.gz` & `tmp/waldur-slurm-agent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waldur-slurm-agent-0.1.3.tar", last modified: Tue Mar 14 14:58:06 2023, max compression
+gzip compressed data, was "waldur-slurm-agent-0.1.4.tar", last modified: Wed Apr 26 11:22:21 2023, max compression
```

## Comparing `waldur-slurm-agent-0.1.3.tar` & `waldur-slurm-agent-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/LICENCE
--rw-r--r--   0 root         (0) root         (0)     6387 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5947 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      860 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/waldur_slurm/
--rw-rw-rw-   0 root         (0) root         (0)     1810 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1431 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/common_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10433 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/backend.py
--rw-rw-rw-   0 root         (0) root         (0)     1317 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5356 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/client.py
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3386 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/structures.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-03-02 03:03:49.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6726 2023-03-14 14:55:19.000000 waldur-slurm-agent-0.1.3/waldur_slurm/slurm_waldur_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     7250 2023-03-14 14:55:19.000000 waldur-slurm-agent-0.1.3/waldur_slurm/waldur_slurm_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-14 14:58:06.661909 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6387 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      676 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-14 14:58:06.000000 waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:22:21.562389 waldur-slurm-agent-0.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2023-03-02 10:53:49.000000 waldur-slurm-agent-0.1.4/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     6257 2023-04-26 11:22:21.558389 waldur-slurm-agent-0.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5817 2023-03-16 13:36:43.000000 waldur-slurm-agent-0.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-26 11:22:21.562389 waldur-slurm-agent-0.1.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      860 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:22:21.558389 waldur-slurm-agent-0.1.4/waldur_slurm/
+-rw-rw-rw-   0 root         (0) root         (0)     1247 2023-03-16 13:36:43.000000 waldur-slurm-agent-0.1.4/waldur_slurm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6981 2023-03-27 13:11:15.000000 waldur-slurm-agent-0.1.4/waldur_slurm/common_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-03-27 13:11:15.000000 waldur-slurm-agent-0.1.4/waldur_slurm/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:22:21.558389 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-03-27 13:11:15.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10850 2023-03-27 09:59:12.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-03-02 10:53:49.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2023-03-27 09:59:12.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-03-02 10:53:49.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3386 2023-03-02 10:53:49.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2023-03-17 12:14:03.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/structures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-03-02 10:53:49.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5816 2023-03-27 13:11:15.000000 waldur-slurm-agent-0.1.4/waldur_slurm/slurm_waldur_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-03-27 13:11:15.000000 waldur-slurm-agent-0.1.4/waldur_slurm/waldur_slurm_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 11:22:21.558389 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6257 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      676 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 11:22:21.000000 waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/top_level.txt
```

### Comparing `waldur-slurm-agent-0.1.3/LICENCE` & `waldur-slurm-agent-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `waldur-slurm-agent-0.1.3/PKG-INFO` & `waldur-slurm-agent-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waldur-slurm-agent
-Version: 0.1.3
+Version: 0.1.4
 Summary: SLURM integration module for Waldur.
 Home-page: https://docs.waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,15 +44,14 @@
 - `SLURM_DEPLOYMENT_TYPE` - type of SLURM deployment. accepts two values: `docker` and `native`, default is `docker`.
 - `SLURM_CUSTOMER_PREFIX` - prefix used for customer's accounts, default is `hpc_`.
 - `SLURM_PROJECT_PREFIX` - prefix used for project's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_PREFIX` - prefix used for allocation's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_NAME_MAX_LEN` - maximum length of account name created by the application.
 - `SLURM_DEFAULT_ACCOUNT` - default account name existing in SLURM cluster for creation of new accounts. Default is `waldur`.
 - `SLURM_CONTAINER_NAME` - name of a headnode SLURM container; must be set if SLURM_DEPLOYMENT_TYPE is docker.
-- `WALDUR_SLURM_USERNAME_SOURCE` - source of SLURM username in Waldur. It can be either `freeipa` or `local`, default is `local`.
 - `SENTRY_DSN` - Data Source Name for Sentry (more info [here](https://docs.sentry.io/product/sentry-basics/dsn-explainer/))
 
 ## Deployment
 
 ### Test environment
 
 In order to test the service, a user should deploy 2 separate instances of the service.
```

### Comparing `waldur-slurm-agent-0.1.3/README.md` & `waldur-slurm-agent-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 - `SLURM_DEPLOYMENT_TYPE` - type of SLURM deployment. accepts two values: `docker` and `native`, default is `docker`.
 - `SLURM_CUSTOMER_PREFIX` - prefix used for customer's accounts, default is `hpc_`.
 - `SLURM_PROJECT_PREFIX` - prefix used for project's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_PREFIX` - prefix used for allocation's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_NAME_MAX_LEN` - maximum length of account name created by the application.
 - `SLURM_DEFAULT_ACCOUNT` - default account name existing in SLURM cluster for creation of new accounts. Default is `waldur`.
 - `SLURM_CONTAINER_NAME` - name of a headnode SLURM container; must be set if SLURM_DEPLOYMENT_TYPE is docker.
-- `WALDUR_SLURM_USERNAME_SOURCE` - source of SLURM username in Waldur. It can be either `freeipa` or `local`, default is `local`.
 - `SENTRY_DSN` - Data Source Name for Sentry (more info [here](https://docs.sentry.io/product/sentry-basics/dsn-explainer/))
 
 ## Deployment
 
 ### Test environment
 
 In order to test the service, a user should deploy 2 separate instances of the service.
```

### Comparing `waldur-slurm-agent-0.1.3/setup.py` & `waldur-slurm-agent-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 tests_requires = [
     "freezegun==0.3.4",
     "pytest==7.1.2",
 ]
 
 setup(
     name="waldur-slurm-agent",
-    version="0.1.3",
+    version="0.1.4",
     author="OpenNode Team",
     author_email="info@opennodecloud.com",
     url="https://docs.waldur.com",
     license="MIT",
     description="SLURM integration module for Waldur.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/__init__.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,21 +10,14 @@
 # "pull" stands for sync from Waldur to SLURM cluster
 # "push" stands for sync from SLURM cluster to Waldur
 class WaldurSyncDirection(Enum):
     PULL = "pull"
     PUSH = "push"
 
 
-# "local" stands for getting a username from local Waldur user account
-# "freeipa" stands for getting a username from FreeIPA user profile
-class WaldurSlurmUsernameSource:
-    LOCAL = "local"
-    FREEIPA = "freeipa"
-
-
 WALDUR_API_URL = os.environ["WALDUR_API_URL"]
 WALDUR_API_TOKEN = os.environ["WALDUR_API_TOKEN"]
 
 WALDUR_SYNC_DIRECTION = os.environ["WALDUR_SYNC_DIRECTION"]
 
 if WALDUR_SYNC_DIRECTION not in [
     WaldurSyncDirection.PULL.value,
@@ -40,26 +33,14 @@
 
 WALDUR_OFFERING_UUID = os.environ.get("WALDUR_OFFERING_UUID")
 
 if not WALDUR_OFFERING_UUID:
     logger.error("WALDUR_OFFERING_UUID is empty")
     exit(1)
 
-WALDUR_SLURM_USERNAME_SOURCE = os.environ.get("WALDUR_SLURM_USERNAME_SOURCE", "local")
-
-if WALDUR_SLURM_USERNAME_SOURCE not in [
-    WaldurSlurmUsernameSource.LOCAL,
-    WaldurSlurmUsernameSource.FREEIPA,
-]:
-    logger.error(
-        "WALDUR_SLURM_USERNAME_SOURCE has invalid value: %s",
-        WALDUR_SLURM_USERNAME_SOURCE,
-    )
-    exit(1)
-
 waldur_rest_client = WaldurClient(WALDUR_API_URL, WALDUR_API_TOKEN)
 
 slurm_backend = SlurmBackend()
 
 sentry_dsn = os.environ.get("SENTRY_DSN")
 
 if sentry_dsn:
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/backend.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,28 @@
 
 class SlurmBackend:
     def __init__(
         self,
     ):
         self.client = SlurmClient(SLURM_DEPLOYMENT_TYPE, SLURM_CONTAINER_NAME)
 
+    def ping(self, raise_exception=False):
+        try:
+            self.client.list_accounts()
+        except SlurmError as err:
+            if raise_exception:
+                raise err
+            logger.info("Error: %s", err)
+            return False
+        else:
+            return True
+
+    def list_tres(self):
+        return self.client.list_tres()
+
     def pull_allocations(self):
         report = {}
         for account in self.client.list_accounts():
             try:
                 logger.info("Pulling allocation %s", account.name)
                 users, usage, limits = self.pull_allocation(account.name)
                 report[account.name] = {
@@ -158,15 +172,15 @@
         return existing_users
 
     def create_allocation(
         self,
         allocation: Allocation,
         customer_name: str,
         project_name: str,
-        usernames: Set[str],
+        limits: dict,
     ):
         customer_account = self.get_customer_name(allocation.customer_uuid)
         project_account = self.get_project_name(allocation.project_uuid)
         allocation_account = self.get_allocation_name(allocation)
 
         if not self.client.get_account(customer_account):
             logger.info(
@@ -189,31 +203,38 @@
             self.client.create_account(
                 name=project_account,
                 description=project_name,
                 organization=project_account,
                 parent_name=customer_account,
             )
 
-        if not self.client.get_account(allocation_account):
+        if self.client.get_account(allocation_account) is not None:
             logger.info(
-                "Creating SLURM account for allocation %s (backend id = %s)",
-                allocation.name,
+                "The account %s already exists in the cluster, skipping creation",
                 allocation_account,
             )
-            self.client.create_account(
-                name=allocation_account,
-                description=allocation.name,
-                organization=project_account,
-            )
+            return
+
+        logger.info(
+            "Creating SLURM account for allocation %s (backend id = %s)",
+            allocation.name,
+            allocation_account,
+        )
+        self.client.create_account(
+            name=allocation_account,
+            description=allocation.name,
+            organization=project_account,
+        )
+
         allocation.backend_id = allocation_account
 
-        limits = utils.get_tres_limits()
+        logger.info("Setting limits: %s", limits)
         self.set_allocation_limits(allocation, limits)
-        added_users = self.add_users_to_account(allocation, usernames)
-        return added_users, limits, allocation_account
+
+        return allocation_account
 
     def sync_users(
         self,
         allocation: Allocation,
         usernames: Set[str],
         all_usernames: Set[str],
     ):
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/base.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/base.py`

 * *Files identical despite different names*

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/client.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 
     def list_accounts(self):
         output = self._execute_command(["list", "account"])
         return [
             self._parse_account(line) for line in output.splitlines() if "|" in line
         ]
 
+    def list_tres(self):
+        output = self._execute_command(["list", "tres"])
+        return [line.split("|")[0] for line in output.splitlines() if "|" in line]
+
     def get_account(self, name):
         output = self._execute_command(["show", "account", name])
         lines = [line for line in output.splitlines() if "|" in line]
         if len(lines) == 0:
             return None
         return self._parse_account(lines[0])
 
@@ -151,13 +155,17 @@
             value = int(match.group(1))
         return structures.Association(
             account=parts[1],
             user=parts[2],
             value=value,
         )
 
-    def _execute_command(self, command, command_name="sacctmgr", immediate=True):
-        account_command = [command_name, "--parsable2", "--noheader"]
+    def _execute_command(
+        self, command, command_name="sacctmgr", immediate=True, parsable=True
+    ):
+        account_command = [command_name]
+        if parsable:
+            account_command.extend(["--parsable2", "--noheader"])
         if immediate:
             account_command.append("--immediate")
         account_command.extend(command)
         return self.execute_command(account_command)
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/parser.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/parser.py`

 * *Files identical despite different names*

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_client/utils.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_client/utils.py`

 * *Files identical despite different names*

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/slurm_waldur_utils.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/slurm_waldur_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,33 @@
 from time import sleep
-from typing import Any, Dict, List
+from typing import Dict, List
 
-from waldur_client import ComponentUsage, OfferingComponent, WaldurClientException
+from waldur_client import ComponentUsage, WaldurClientException
 
-from waldur_slurm.slurm_client import SLURM_TRES, logger
+from waldur_slurm import common_utils
+from waldur_slurm.slurm_client import logger
 from waldur_slurm.slurm_client.exceptions import BackendError
+from waldur_slurm.slurm_client.structures import Allocation
 
 from . import WALDUR_OFFERING_UUID, slurm_backend, waldur_rest_client
 
 
-def drop_users_from_allocation(marketplace_resource: dict, usernames: set):
-    logger.info("Stale usernames: %s", " ,".join(usernames))
-    for username in usernames:
-        try:
-            waldur_rest_client.delete_slurm_association(
-                marketplace_resource["uuid"], username
-            )
-            logger.info(
-                "The user %s has been dropped from %s (backend_id: %s)",
-                username,
-                marketplace_resource["name"],
-                marketplace_resource["backend_id"],
-            )
-        except WaldurClientException as e:
-            logger.error("User %s can not be dropped due to: %s", username, e)
-
-
-def add_users_to_allocation(marketplace_resource: dict, usernames: set):
-    logger.info("New usernames: %s", " ,".join(usernames))
-    for username in usernames:
-        try:
-            waldur_rest_client.create_slurm_association(
-                marketplace_resource["uuid"], username
-            )
-            logger.info(
-                "The user %s has been added to %s (backend_id: %s)",
-                username,
-                marketplace_resource["name"],
-                marketplace_resource["backend_id"],
-            )
-        except WaldurClientException as e:
-            logger.error("User %s can not be added due to: %s", username, e)
-
-
 def submit_total_usage_for_allocation(
-    marketplace_resource: dict, total_usage: Dict[str, float], waldur_components
+    allocation: Allocation, total_usage: Dict[str, float], waldur_components
 ):
     logger.info("Setting usages: %s", total_usage)
-    resource_uuid = marketplace_resource["uuid"]
+    resource_uuid = allocation.marketplace_uuid
     plan_periods = waldur_rest_client.marketplace_resource_get_plan_periods(
         resource_uuid
     )
 
     if len(plan_periods) == 0:
         logger.warning(
             "A corresponding ResourcePlanPeriod for allocation %s was not found",
-            marketplace_resource["name"],
+            allocation.name,
         )
         return
 
     plan_period = plan_periods[0]
     component_types = [component["type"] for component in waldur_components]
     missing_components = set(total_usage) - set(component_types)
 
@@ -73,18 +41,51 @@
         ComponentUsage(type=component, amount=amount)
         for component, amount in total_usage.items()
         if component in component_types
     ]
     waldur_rest_client.create_component_usages(plan_period["uuid"], usage_objects)
 
 
-def sync_data_from_slurm_to_waldur(allocation_report, waldur_offering):
-    # Push SLURM data to mastermind using REST client
+def sync_allocation_users(allocation: Allocation, usernames: List[str]):
+    logger.info("Syncing associations")
+    associations = waldur_rest_client.list_slurm_associations(
+        {"allocation_uuid": allocation.uuid}
+    )
+    remote_usernames = {association["username"] for association in associations}
+    local_usernames = set(usernames)
+
+    stale_usernames = remote_usernames - local_usernames
+    common_utils.drop_users_from_allocation(allocation, stale_usernames)
+
+    new_usernames = local_usernames - remote_usernames
+    common_utils.add_users_to_allocation(allocation, new_usernames)
+
+    # Offering users sync
+    logger.info("Creating associations for offering users")
+    offering_users = waldur_rest_client.list_remote_offering_users(
+        {
+            "offering_uuid": WALDUR_OFFERING_UUID,
+        }
+    )
+
+    offering_user_usernames = [
+        offering_user["username"]
+        for offering_user in offering_users
+        if offering_user["username"] not in local_usernames
+    ]
+
+    common_utils.add_users_to_allocation(allocation, offering_user_usernames)
+    slurm_backend.add_users_to_account(allocation, offering_user_usernames)
+
+
+def sync_data_from_slurm_to_waldur(allocation_report):
+    waldur_offering = waldur_rest_client._get_offering(WALDUR_OFFERING_UUID)
+    # Push SLURM data to Mastermind using REST client
     for allocation_backend_id, allocation_data in allocation_report.items():
-        print("-" * 30)
+        logger.info("-" * 30)
         try:
             logger.info("Processing %s", allocation_backend_id)
             usernames: List[str] = allocation_data["users"]
             usages: Dict[str, Dict[str, float]] = allocation_data["usage"]
             limits: Dict[str, float] = allocation_data["limits"]
 
             waldur_resources = waldur_rest_client.filter_marketplace_resources(
@@ -99,42 +100,37 @@
                     "There are no resources in Waldur with backend_id '%s',"
                     "skipping sync",
                     allocation_backend_id,
                 )
                 continue
 
             marketplace_resource = waldur_resources[0]
-
-            allocation_waldur_uuid = marketplace_resource["resource_uuid"]
-
-            # Sync users
-            marketplace_resource_uuid = marketplace_resource["uuid"]
-            associations = waldur_rest_client.list_slurm_associations(
-                {"allocation_uuid": allocation_waldur_uuid}
+            allocation = Allocation(
+                name=marketplace_resource["name"],
+                uuid=marketplace_resource["resource_uuid"],
+                marketplace_uuid=marketplace_resource["uuid"],
+                backend_id=allocation_backend_id,
+                project_uuid=marketplace_resource["project_uuid"],
+                customer_uuid=marketplace_resource["customer_uuid"],
             )
-            remote_usernames = {association["username"] for association in associations}
-            local_usernames = set(usernames)
 
-            stale_usernames = remote_usernames - local_usernames
-            drop_users_from_allocation(marketplace_resource, stale_usernames)
-
-            new_usernames = local_usernames - remote_usernames
-            add_users_to_allocation(marketplace_resource, new_usernames)
+            # Sync users
+            sync_allocation_users(allocation, usernames)
 
             # Submit limits
             if limits is not None:
                 logger.info("Setting limits to %s", limits)
                 waldur_rest_client.set_slurm_allocation_limits(
-                    marketplace_resource_uuid, limits
+                    allocation.marketplace_uuid, limits
                 )
 
             # Submit usage
             total_usage = usages["TOTAL_ACCOUNT_USAGE"]
             submit_total_usage_for_allocation(
-                marketplace_resource, total_usage, waldur_offering["components"]
+                allocation, total_usage, waldur_offering["components"]
             )
         except WaldurClientException as e:
             logger.exception(
                 "Waldur REST client error while processing allocation %s: %s",
                 allocation_backend_id,
                 e,
             )
@@ -142,35 +138,19 @@
             logger.exception(
                 "Waldur SLURM client error while processing allocation %s: %s",
                 allocation_backend_id,
                 e,
             )
 
 
-def create_offering_components(waldur_offering, tres_data: Dict[str, Dict[str, Any]]):
-    components = [
-        OfferingComponent(
-            billing_type=tres_info["accounting_type"],
-            type=tres_type,
-            name=tres_info["label"],
-            measured_unit=tres_info["measured_unit"],
-        )
-        for tres_type, tres_info in tres_data.items()
-    ]
-    logger.info(
-        "Updating offering components data for the following tres: %s",
-        ", ".join(tres_data.keys()),
-    )
-    waldur_rest_client.update_offering_components(waldur_offering["uuid"], components)
-
-
 def slurm_waldur_sync():
-    waldur_offering = waldur_rest_client._get_offering(WALDUR_OFFERING_UUID)
-    create_offering_components(waldur_offering, SLURM_TRES)
+    logger.info("Synching data from SLURM cluster to Waldur")
+    common_utils.create_offering_components()
     while True:
         try:
             logger.info("Fetching data from SLURM cluster")
             allocation_report = slurm_backend.pull_allocations()
-            sync_data_from_slurm_to_waldur(allocation_report, waldur_offering)
-            sleep(60 * 60)  # Once per hour
+            sync_data_from_slurm_to_waldur(allocation_report)
         except Exception as e:
             logger.exception("The application crashed due to the error: %s", e)
+        logger.info("/" * 30)
+        sleep(60 * 60)  # Once per hour
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm/waldur_slurm_utils.py` & `waldur-slurm-agent-0.1.4/waldur_slurm/waldur_slurm_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,137 @@
 import traceback
 from time import sleep
 
 from waldur_client import SlurmAllocationState, WaldurClientException, is_uuid
 
 from waldur_slurm.slurm_client import logger
+from waldur_slurm.slurm_client import utils as slurm_utils
 from waldur_slurm.slurm_client.exceptions import BackendError
 from waldur_slurm.slurm_client.structures import Allocation
 
-from . import (
-    WALDUR_OFFERING_UUID,
-    WALDUR_SLURM_USERNAME_SOURCE,
-    WaldurSlurmUsernameSource,
-    common_utils,
-    slurm_backend,
-    waldur_rest_client,
-)
-
-
-def fetch_usernames_registered_in_freeipa(team):
-    usernames = set()
-    all_freeipa_profiles = waldur_rest_client.list_freeipa_profiles()
-    user_profile_mapping = {
-        profile["user_uuid"]: profile["username"] for profile in all_freeipa_profiles
-    }
-    for user in team:
-        freeipa_username = user_profile_mapping.get(user["uuid"])
-        if freeipa_username:
-            usernames.add(freeipa_username)
-        else:
-            logger.warning(
-                "The user %s (%s) doesn't have any FreeIPA profiles," "skipping.",
-                user["username"],
-                user["full_name"],
-            )
-    return usernames
+from . import WALDUR_OFFERING_UUID, common_utils, slurm_backend, waldur_rest_client
 
 
-def process_order_for_creation(order_item: dict):
-    if "marketplace_resource_uuid" not in order_item:
-        logger.error(
-            "The order item %s (%s) does not have a connected resource, skipping it.",
-            order_item["uuid"],
-            order_item["attributes"]["name"],
-        )
-        return
+def create_allocation(order_item):
     resource_uuid = order_item["marketplace_resource_uuid"]
     resource_name = order_item["resource_name"]
     waldur_allocation_uuid = order_item["resource_uuid"]
+    allocation_limits = slurm_utils.get_tres_limits()
+
+    logger.info("Creating allocation %s", resource_name)
     resource = waldur_rest_client.get_marketplace_resource(resource_uuid)
 
     if not is_uuid(resource_uuid):
         logger.error("Unexpected resource UUID format, skipping the order")
         return
 
     if not is_uuid(waldur_allocation_uuid):
         logger.error("Unexpected allocation UUID format, skipping the order")
         return
 
     allocation = Allocation(
         name=order_item["resource_name"],
         uuid=waldur_allocation_uuid,
+        marketplace_uuid=resource_uuid,
         project_uuid=order_item["project_uuid"],
         customer_uuid=order_item["customer_uuid"],
     )
 
     if resource["state"] != "Creating":
         logger.info(
             "Setting resource state (%s) to CREATING (current state is %s)",
             resource["uuid"],
             resource["state"],
         )
         waldur_rest_client.set_slurm_allocation_state(
-            resource_uuid, SlurmAllocationState.CREATING
+            allocation.marketplace_uuid, SlurmAllocationState.CREATING
         )
 
-    team = waldur_rest_client.marketplace_resource_get_team(resource_uuid)
-    username_fetching_function = {
-        WaldurSlurmUsernameSource.LOCAL: lambda team: [
-            user["username"] for user in team
-        ],
-        WaldurSlurmUsernameSource.FREEIPA: fetch_usernames_registered_in_freeipa,
-    }
-    usernames = username_fetching_function[WALDUR_SLURM_USERNAME_SOURCE](team)
-
-    added_users, limits, backend_id = slurm_backend.create_allocation(
+    logger.info("Creating account in SLURM cluster")
+    slurm_backend.create_allocation(
         allocation,
         project_name=order_item["project_name"],
         customer_name=order_item["customer_name"],
-        usernames=usernames,
+        limits=allocation_limits,
     )
 
-    waldur_rest_client.marketplace_resource_set_backend_id(resource_uuid, backend_id)
-    waldur_rest_client.set_slurm_allocation_backend_id(resource_uuid, backend_id)
+    logger.info("Updating allocation metadata in Waldur")
+    waldur_rest_client.marketplace_resource_set_backend_id(
+        allocation.marketplace_uuid, allocation.backend_id
+    )
+    waldur_rest_client.set_slurm_allocation_backend_id(
+        allocation.marketplace_uuid, allocation.backend_id
+    )
 
-    allocation_waldur = {
-        "marketplace_resource_uuid": resource_uuid,
-        "name": resource_name,
-        "backend_id": allocation.backend_id,
-    }
-    common_utils.add_users_to_allocation(allocation_waldur, added_users)
-    waldur_rest_client.set_slurm_allocation_limits(resource_uuid, limits)
+    logger.info("Updating allocation limits in Waldur")
+    waldur_rest_client.set_slurm_allocation_limits(
+        allocation.marketplace_uuid, allocation_limits
+    )
 
+    logger.info("Updating order item state")
     waldur_rest_client.marketplace_order_item_set_state_done(order_item["uuid"])
+
+    logger.info("Updating Waldur allocation state")
     waldur_rest_client.set_slurm_allocation_state(
-        resource_uuid, SlurmAllocationState.OK
+        allocation.marketplace_uuid, SlurmAllocationState.OK
     )
 
+    return allocation
+
+
+def add_users_to_allocation(resource_uuid, allocation: Allocation):
+    logger.info("Adding users to account in SLURM cluster")
+
+    logger.info("Fetching Waldur resource team")
+    team = waldur_rest_client.marketplace_resource_get_team(resource_uuid)
+    user_uuids = {user["uuid"] for user in team}
+
+    logger.info("Fetching Waldur offering users")
+    offering_users_all = waldur_rest_client.list_remote_offering_users(
+        {"offering_uuid": WALDUR_OFFERING_UUID}
+    )
+    offering_usernames = [
+        offering_user["username"]
+        for offering_user in offering_users_all
+        if offering_user["user_uuid"] in user_uuids
+    ]
+
+    logger.info("Adding usernames to account in SLURM cluster")
+    added_users = slurm_backend.add_users_to_account(allocation, offering_usernames)
+
+    common_utils.add_users_to_allocation(allocation, added_users)
+
+
+def process_order_for_creation(order_item: dict):
+    # Wait until resource is created
+    attempts = 0
+    while "marketplace_resource_uuid" not in order_item:
+        if attempts > 4:
+            logger.error("Order item processing timed out")
+            return
+
+        if order_item["state"] != "executing":
+            logger.error("Order item has unexpected state %s", order_item["state"])
+            return
+
+        logger.info("Waiting for resource creation...")
+        sleep(5)
+
+        order_item = waldur_rest_client.get_order_item(order_item["uuid"])
+        attempts += 1
+
+    resource_uuid = order_item["marketplace_resource_uuid"]
+
+    allocation: Allocation = create_allocation(order_item)
+
+    if allocation is None:
+        return
+
+    add_users_to_allocation(resource_uuid, allocation)
+
 
 def process_order_for_limits_update(order_item: dict):
     logger.info("Updating limits for %s", order_item["resource_name"])
     resource_uuid = order_item["marketplace_resource_uuid"]
     allocation_uuid = order_item["resource_uuid"]
 
     allocation_waldur = waldur_rest_client.get_slurm_allocation(allocation_uuid)
@@ -159,24 +181,39 @@
 
 
 def sync_data_from_waldur_to_slurm():
     # Pull data form Mastermind using REST client
     order_items = waldur_rest_client.list_order_items(
         {
             "offering_uuid": WALDUR_OFFERING_UUID,
-            "state": "executing",
+            "state": ["pending", "executing"],
         }
     )
 
     if len(order_items) == 0:
-        logger.info("There are no approved order items")
+        logger.info("There are no pending or executing order items")
         return
 
     for order_item in order_items:
         try:
+            logger.info(
+                "Processing order item %s (%s) with state %s",
+                order_item["attributes"].get("name", "N/A"),
+                order_item["uuid"],
+                order_item["state"],
+            )
+
+            if order_item["state"] == "executing":
+                logger.info("Order item is executing already, no need for approval")
+            else:
+                logger.info("Approving order item")
+                waldur_rest_client.marketplace_order_item_approve(order_item["uuid"])
+                logger.info("Refreshing the order item")
+                order_item = waldur_rest_client.get_order_item(order_item["uuid"])
+
             if order_item["type"] == "Create":
                 process_order_for_creation(order_item)
 
             if order_item["type"] == "Update":
                 process_order_for_limits_update(order_item)
 
             if order_item["type"] == "Terminate":
@@ -196,17 +233,21 @@
             )
             waldur_rest_client.marketplace_order_item_set_state_erred(
                 order_item["uuid"],
                 error_message=str(e),
                 error_traceback=traceback.format_exc(),
             )
 
+        logger.info("-" * 30)
+
 
 def waldur_slurm_sync():
+    logger.info("Synching data from Waldur to SLURM cluster")
+    common_utils.create_offering_components()
     while True:
         logger.info("Pulling data from Waldur to SLURM cluster")
         try:
             sync_data_from_waldur_to_slurm()
         except Exception as e:
             logger.exception("The application crashed due to the error: %s", e)
-        print("/" * 30)
+        logger.info("/" * 30)
         sleep(2 * 60)  # Once per 2 minutes
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/PKG-INFO` & `waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waldur-slurm-agent
-Version: 0.1.3
+Version: 0.1.4
 Summary: SLURM integration module for Waldur.
 Home-page: https://docs.waldur.com
 Author: OpenNode Team
 Author-email: info@opennodecloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -44,15 +44,14 @@
 - `SLURM_DEPLOYMENT_TYPE` - type of SLURM deployment. accepts two values: `docker` and `native`, default is `docker`.
 - `SLURM_CUSTOMER_PREFIX` - prefix used for customer's accounts, default is `hpc_`.
 - `SLURM_PROJECT_PREFIX` - prefix used for project's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_PREFIX` - prefix used for allocation's accounts, default is `hpc_`.
 - `SLURM_ALLOCATION_NAME_MAX_LEN` - maximum length of account name created by the application.
 - `SLURM_DEFAULT_ACCOUNT` - default account name existing in SLURM cluster for creation of new accounts. Default is `waldur`.
 - `SLURM_CONTAINER_NAME` - name of a headnode SLURM container; must be set if SLURM_DEPLOYMENT_TYPE is docker.
-- `WALDUR_SLURM_USERNAME_SOURCE` - source of SLURM username in Waldur. It can be either `freeipa` or `local`, default is `local`.
 - `SENTRY_DSN` - Data Source Name for Sentry (more info [here](https://docs.sentry.io/product/sentry-basics/dsn-explainer/))
 
 ## Deployment
 
 ### Test environment
 
 In order to test the service, a user should deploy 2 separate instances of the service.
```

### Comparing `waldur-slurm-agent-0.1.3/waldur_slurm_agent.egg-info/SOURCES.txt` & `waldur-slurm-agent-0.1.4/waldur_slurm_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

