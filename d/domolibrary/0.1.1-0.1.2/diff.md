# Comparing `tmp/domolibrary-0.1.1.tar.gz` & `tmp/domolibrary-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.1.tar", last modified: Wed Apr 26 12:51:22 2023, max compression
+gzip compressed data, was "domolibrary-0.1.2.tar", last modified: Wed Apr 26 13:37:55 2023, max compression
```

## Comparing `domolibrary-0.1.1.tar` & `domolibrary-0.1.2.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.523016 domolibrary-0.1.1/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.363017 domolibrary-0.1.1/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.1/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.371017 domolibrary-0.1.1/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.423017 domolibrary-0.1.1/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.1/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.1/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.1/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.1/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.1/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.1/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.1/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.435017 domolibrary-0.1.1/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.1/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.1/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.1/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.1/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.1/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.439017 domolibrary-0.1.1/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.1/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.1/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.1/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 12:51:22.523016 domolibrary-0.1.1/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.1/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.439017 domolibrary-0.1.1/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   147817 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.475017 domolibrary-0.1.1/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17100 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 12:43:29.000000 domolibrary-0.1.1/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 12:43:29.000000 domolibrary-0.1.1/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13808 2023-04-26 12:43:29.000000 domolibrary-0.1.1/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.475017 domolibrary-0.1.1/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.479017 domolibrary-0.1.1/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3181 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.495016 domolibrary-0.1.1/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8160 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9050 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.499016 domolibrary-0.1.1/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      865 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 12:43:30.000000 domolibrary-0.1.1/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.455017 domolibrary-0.1.1/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.1/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 12:51:22.000000 domolibrary-0.1.1/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 12:51:16.000000 domolibrary-0.1.1/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 12:51:22.527016 domolibrary-0.1.1/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.1/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 12:51:22.519016 domolibrary-0.1.1/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.1/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.1/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.1/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.1/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.063516 domolibrary-0.1.2/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.895516 domolibrary-0.1.2/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.2/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.907516 domolibrary-0.1.2/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.951516 domolibrary-0.1.2/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.2/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.2/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.2/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.999516 domolibrary-0.1.2/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.2/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.2/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.2/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.003516 domolibrary-0.1.2/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.2/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.2/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.2/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 13:37:55.063516 domolibrary-0.1.2/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.2/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.007516 domolibrary-0.1.2/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   147817 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17100 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.035516 domolibrary-0.1.2/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8202 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.039516 domolibrary-0.1.2/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      865 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.019516 domolibrary-0.1.2/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.2/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 13:37:50.000000 domolibrary-0.1.2/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 13:37:55.063516 domolibrary-0.1.2/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.2/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.059516 domolibrary-0.1.2/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.2/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.2/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.2/utils/upload_data.py
```

### Comparing `domolibrary-0.1.1/Automation/automation.py` & `domolibrary-0.1.2/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DataOcean/Transport.py` & `domolibrary-0.1.2/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.2/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.2/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DataOcean/cnfg_s3.py` & `domolibrary-0.1.2/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.2/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoAccount.py` & `domolibrary-0.1.2/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.2/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.2/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoApplication.py` & `domolibrary-0.1.2/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoAuth.py` & `domolibrary-0.1.2/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.2/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoCard.py` & `domolibrary-0.1.2/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoCertification.py` & `domolibrary-0.1.2/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.2/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.2/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoDataset.py` & `domolibrary-0.1.2/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoGrant.py` & `domolibrary-0.1.2/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoGroup.py` & `domolibrary-0.1.2/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.2/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoJob.py` & `domolibrary-0.1.2/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoLineage.py` & `domolibrary-0.1.2/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoPDP.py` & `domolibrary-0.1.2/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoPage.py` & `domolibrary-0.1.2/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoPublish.py` & `domolibrary-0.1.2/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoRole.py` & `domolibrary-0.1.2/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.2/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoStream.py` & `domolibrary-0.1.2/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoTag.py` & `domolibrary-0.1.2/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/DomoUser.py` & `domolibrary-0.1.2/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/get_data.py` & `domolibrary-0.1.2/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.2/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/LICENSE` & `domolibrary-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/PKG-INFO` & `domolibrary-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.1/README.md` & `domolibrary-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/_modidx.py` & `domolibrary-0.1.2/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.2/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.2/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.2/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.2/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.2/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.2/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.2/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.2/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.2/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.2/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.2/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.2/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.2/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.2/domolibrary/classes/DomoUser.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,26 +97,30 @@
         dd = user_obj
         if isinstance(user_obj, dict):
             dd = util_dd.DictDot(user_obj)
 
         return cls(id=dd.id, display_name=dd.displayName, auth=auth)
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 8
-@patch_to(DomoUser, cls_method= True)
-async def get_by_id(cls: DomoUser, user_id, auth :dmda.DomoAuth, debug_api: bool = False, session : httpx.AsyncClient = None):
-
+@patch_to(DomoUser, cls_method=True)
+async def get_by_id(cls: DomoUser, user_id, auth: dmda.DomoAuth,
+                    return_raw: bool = False,
+                    debug_api: bool = False, session: httpx.AsyncClient = None):
 
     res = await user_routes.get_by_id(
-        auth=auth, user_id=user_id, debug_api=debug_api, session = session
+        auth=auth, user_id=user_id, debug_api=debug_api, session=session
     )
 
+    if return_raw:
+        return res
+
     if not res.is_success:
         raise Exception(res.response)
-
-    return cls._from_search_json(user_obj = res.response, auth = auth)
+    
+    return cls._from_search_json(user_obj=res.response, auth=auth)
 
 
 # %% ../../nbs/classes/50_DomoUser.ipynb 10
 @patch_to(DomoUser)
 async def reset_password(self: DomoUser, new_password: str, debug_api: bool = False):
     """reset your password, will respect password restrictions set up in the Domo UI"""
```

### Comparing `domolibrary-0.1.1/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.2/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/client/DomoError.py` & `domolibrary-0.1.2/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/client/Logger.py` & `domolibrary-0.1.2/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.2/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/client/get_data.py` & `domolibrary-0.1.2/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.2/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.2/domolibrary/integrations/RoleHierarchy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/integrations/RoleHierarchy.ipynb.
 
 # %% auto 0
-__all__ = ['get_roles_w_hierarchy', 'calc_role']
+__all__ = ['extract_role_hierarchy', 'get_roles_w_hierarchy', 'calc_role']
 
 # %% ../../nbs/integrations/RoleHierarchy.ipynb 2
 import pandas as pd
 from fastcore.basics import patch_to
 
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.classes.DomoRole as dmr
```

### Comparing `domolibrary-0.1.1/domolibrary/routes/account.py` & `domolibrary-0.1.2/domolibrary/routes/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,18 @@
     return res
 
 
 
 
 # %% ../../nbs/routes/account.ipynb 11
 class AccountConfig_InvalidDataProvider(de.DomoError):
-    def __init__(self, account_id:str, data_provider_type:str, domo_instance: str, function_name = 'route.get_account_config'):
-        message = f"account data_provider_type '{data_provider_type}' did not return a config"
+    def __init__(self, account_id:str, data_provider_type:str, status, domo_instance: str, function_name = 'route.get_account_config'):
+        message = f"account {account_id} with data_provider_type '{data_provider_type}' does not return a config"
 
-        super().__init__(entity_id = account_id, message = message, function_name = function_name, domo_instance = domo_instance)
+        super().__init__( message = message, status = status, function_name = function_name, domo_instance = domo_instance)
 
 async def get_account_config(auth: dmda.DomoAuth,
                              account_id: int,
                              data_provider_type: str ,
                              debug_api: bool = False, 
                              session: Union[httpx.AsyncClient, httpx.AsyncClient, None] = None) -> rgd.ResponseGetData:
 
@@ -90,15 +90,15 @@
         url=url,
         method='GET',
         debug_api=debug_api,
         session=session
     )
 
     if res.response == {} and res.is_success:
-        raise AccountConfig_InvalidDataProvider(account_id= account_id, data_provider_type= data_provider_type, domo_instance=auth.domo_instance)
+        raise AccountConfig_InvalidDataProvider(account_id= account_id, data_provider_type= data_provider_type, domo_instance=auth.domo_instance, status = res.status)
     
     return res
 
 # %% ../../nbs/routes/account.ipynb 14
 async def update_account_config(auth: dmda.DomoAuth,
                                 account_id: int,
                                 config_body: dict,
```

### Comparing `domolibrary-0.1.1/domolibrary/routes/activity_log.py` & `domolibrary-0.1.2/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.2/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/card.py` & `domolibrary-0.1.2/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/datacenter.py` & `domolibrary-0.1.2/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/dataflow.py` & `domolibrary-0.1.2/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/dataset.py` & `domolibrary-0.1.2/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/grant.py` & `domolibrary-0.1.2/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/group.py` & `domolibrary-0.1.2/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/instance_config.py` & `domolibrary-0.1.2/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/page.py` & `domolibrary-0.1.2/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/pdp.py` & `domolibrary-0.1.2/domolibrary/routes/pdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                 body=body,
                 debug_api=debug_api,
                 session=session,
             )
 
     return res
 
-# %% ../../nbs/routes/pdp.ipynb 23
+# %% ../../nbs/routes/pdp.ipynb 20
 async def update_policy(
     auth: dmda.DomoAuth,
     dataset_id: str,
     policy_id: str,
     body: dict,  # generated using generate_policy_parameter_simple & generate_policy_body
     session: httpx.AsyncClient = None,
     debug_api: bool = False,
@@ -200,15 +200,15 @@
         body=body,
         debug_api=debug_api,
         session=session,
     )
 
     return res
 
-# %% ../../nbs/routes/pdp.ipynb 27
+# %% ../../nbs/routes/pdp.ipynb 24
 async def delete_policy(
     auth: dmda.DomoAuth,
     dataset_id: str = None,
     policy_id: str = None,
     session: httpx.AsyncClient = None,
     debug_api: bool = False,
 ) -> rgd.ResponseGetData:
@@ -224,15 +224,15 @@
         method="DELETE",
         debug_api=debug_api,
         session=session,
     )
 
     return res
 
-# %% ../../nbs/routes/pdp.ipynb 31
+# %% ../../nbs/routes/pdp.ipynb 28
 async def toggle_pdp(
         auth: dmda.DomoAuth,
         dataset_id: str,
         is_enable: bool = True,
         debug_api: bool = False,
         session: httpx.AsyncClient = None
     )-> rgd.ResponseGetData:
```

### Comparing `domolibrary-0.1.1/domolibrary/routes/publish.py` & `domolibrary-0.1.2/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/role.py` & `domolibrary-0.1.2/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/routes/user.py` & `domolibrary-0.1.2/domolibrary/routes/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
            'search_virtual_user_by_subscriber_instance', 'create_user', 'set_user_landing_page', 'reset_password',
            'request_password_reset', 'UserProperty_Type', 'UserProperty', 'generate_patch_user_property_body',
            'update_user']
 
 # %% ../../nbs/routes/user.ipynb 3
 from enum import Enum
 import httpx
+import asyncio
 
 import utils.DictDot as dd
 import domolibrary.client.get_data as gd
 import domolibrary.client.ResponseGetData as rgd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.DomoError as de
 
@@ -26,17 +27,28 @@
     url = f"https://{ auth.domo_instance}.domo.com/api/content/v2/users"
 
     return await gd.get_data(url=url, method="GET", auth=auth, debug_api=debug_api)
 
 
 # %% ../../nbs/routes/user.ipynb 9
 async def get_by_id(user_id, auth: dmda.DomoAuth, debug_api: bool = False, session: httpx.AsyncClient = None):
-    url = f'https://{auth.domo_instance}.domo.com/api/content/v2/users/{user_id}'
+    v2_url = f'https://{auth.domo_instance}.domo.com/api/content/v2/users/{user_id}' # does not include role_id
+
+    v3_url = f'https://{auth.domo_instance}.domo.com/api/content/v3/users/{user_id}'
+    
+    params = {'includeDetails' :True}
+
+    
+    res_v2, res_v3 = await asyncio.gather(gd.get_data(url=v2_url, method="GET", auth=auth, debug_api=debug_api, session=session, params=params) , 
+    gd.get_data(url=v3_url, method="GET", auth=auth, debug_api=debug_api, session=session, params=params))
+
+    res_v2.response.update({'roleId': res_v3.response.get('roleId')})
+
+    return res_v2
 
-    return await gd.get_data(url=url, method="GET", auth=auth, debug_api=debug_api, session=session)
 
 
 # %% ../../nbs/routes/user.ipynb 11
 def generate_search_users_body_by_id(
     user_ids: list[str],  # list of user ids to search
 ) -> dict:  # dict to pass to search v1_users_search_api
     """search v1_users_search_api"""
```

### Comparing `domolibrary-0.1.1/domolibrary/utils/DictDot.py` & `domolibrary-0.1.2/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.2/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/utils/convert.py` & `domolibrary-0.1.2/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.2/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary/utils/upload_data.py` & `domolibrary-0.1.2/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.2/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.1
+Version: 0.1.2
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.1/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.2/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/settings.ini` & `domolibrary-0.1.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.01
+version = 0.1.02
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.1/setup.py` & `domolibrary-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/Base.py` & `domolibrary-0.1.2/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/DictDot.py` & `domolibrary-0.1.2/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/Exceptions.py` & `domolibrary-0.1.2/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/LoggerClass.py` & `domolibrary-0.1.2/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/chunk_execution.py` & `domolibrary-0.1.2/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/consol_get_creds.py` & `domolibrary-0.1.2/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/convert.py` & `domolibrary-0.1.2/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.2/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.1/utils/upload_data.py` & `domolibrary-0.1.2/utils/upload_data.py`

 * *Files identical despite different names*

