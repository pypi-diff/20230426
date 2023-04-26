# Comparing `tmp/domolibrary-0.1.4.tar.gz` & `tmp/domolibrary-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.4.tar", last modified: Wed Apr 26 17:44:22 2023, max compression
+gzip compressed data, was "domolibrary-0.1.5.tar", last modified: Wed Apr 26 18:04:21 2023, max compression
```

## Comparing `domolibrary-0.1.4.tar` & `domolibrary-0.1.5.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.967860 domolibrary-0.1.4/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.947860 domolibrary-0.1.4/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.4/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.947860 domolibrary-0.1.4/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.951860 domolibrary-0.1.4/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.4/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.4/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.4/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.4/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.4/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.4/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.4/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.955860 domolibrary-0.1.4/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.4/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.4/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.4/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.4/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.4/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.955860 domolibrary-0.1.4/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.4/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.4/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.4/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 17:44:22.967860 domolibrary-0.1.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.955860 domolibrary-0.1.4/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148167 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.959860 domolibrary-0.1.4/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18287 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 17:43:33.000000 domolibrary-0.1.4/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 17:43:33.000000 domolibrary-0.1.4/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 17:43:33.000000 domolibrary-0.1.4/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 17:43:33.000000 domolibrary-0.1.4/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.959860 domolibrary-0.1.4/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.959860 domolibrary-0.1.4/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.963860 domolibrary-0.1.4/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8202 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.963860 domolibrary-0.1.4/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 17:43:34.000000 domolibrary-0.1.4/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.955860 domolibrary-0.1.4/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.4/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 17:44:22.000000 domolibrary-0.1.4/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 17:44:16.000000 domolibrary-0.1.4/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 17:44:22.967860 domolibrary-0.1.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.4/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 17:44:22.963860 domolibrary-0.1.4/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.4/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.4/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.4/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.4/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.380382 domolibrary-0.1.5/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.356382 domolibrary-0.1.5/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.5/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.356382 domolibrary-0.1.5/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.360382 domolibrary-0.1.5/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.5/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.5/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.5/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.5/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.5/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.5/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.5/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.368382 domolibrary-0.1.5/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.5/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.5/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.5/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.5/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.5/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.368382 domolibrary-0.1.5/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.5/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.5/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.5/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 18:04:21.380382 domolibrary-0.1.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.368382 domolibrary-0.1.5/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   148101 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.372382 domolibrary-0.1.5/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    18120 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.372382 domolibrary-0.1.5/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.372382 domolibrary-0.1.5/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.376382 domolibrary-0.1.5/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8277 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.376382 domolibrary-0.1.5/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      875 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 18:03:19.000000 domolibrary-0.1.5/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.368382 domolibrary-0.1.5/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.5/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 18:04:21.000000 domolibrary-0.1.5/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 18:04:02.000000 domolibrary-0.1.5/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 18:04:21.380382 domolibrary-0.1.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.5/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 18:04:21.380382 domolibrary-0.1.5/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.5/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.5/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.5/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.5/utils/upload_data.py
```

### Comparing `domolibrary-0.1.4/Automation/automation.py` & `domolibrary-0.1.5/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DataOcean/Transport.py` & `domolibrary-0.1.5/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.5/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.5/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DataOcean/cnfg_s3.py` & `domolibrary-0.1.5/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.5/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoAccount.py` & `domolibrary-0.1.5/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.5/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.5/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoApplication.py` & `domolibrary-0.1.5/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoAuth.py` & `domolibrary-0.1.5/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.5/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoCard.py` & `domolibrary-0.1.5/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoCertification.py` & `domolibrary-0.1.5/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.5/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.5/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoDataset.py` & `domolibrary-0.1.5/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoGrant.py` & `domolibrary-0.1.5/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoGroup.py` & `domolibrary-0.1.5/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.5/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoJob.py` & `domolibrary-0.1.5/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoLineage.py` & `domolibrary-0.1.5/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoPDP.py` & `domolibrary-0.1.5/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoPage.py` & `domolibrary-0.1.5/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoPublish.py` & `domolibrary-0.1.5/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoRole.py` & `domolibrary-0.1.5/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.5/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoStream.py` & `domolibrary-0.1.5/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoTag.py` & `domolibrary-0.1.5/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/DomoUser.py` & `domolibrary-0.1.5/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/get_data.py` & `domolibrary-0.1.5/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.5/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/LICENSE` & `domolibrary-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/PKG-INFO` & `domolibrary-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.4
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.4/README.md` & `domolibrary-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/_modidx.py` & `domolibrary-0.1.5/domolibrary/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,17 +86,15 @@
                                                  'domolibrary.classes.DomoAccount.DomoAccount_UpdateName_Error': ( 'classes/domoaccount.html#domoaccount_updatename_error',
                                                                                                                    'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccount_UpdateName_Error.__init__': ( 'classes/domoaccount.html#domoaccount_updatename_error.__init__',
                                                                                                                             'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccounts': ( 'classes/domoaccount.html#domoaccounts',
                                                                                                    'domolibrary/classes/DomoAccount.py'),
                                                  'domolibrary.classes.DomoAccount.DomoAccounts.get_accounts': ( 'classes/domoaccount.html#domoaccounts.get_accounts',
-                                                                                                                'domolibrary/classes/DomoAccount.py'),
-                                                 'domolibrary.classes.DomoAccount.ShareAccount_AccessLevel': ( 'classes/domoaccount.html#shareaccount_accesslevel',
-                                                                                                               'domolibrary/classes/DomoAccount.py')},
+                                                                                                                'domolibrary/classes/DomoAccount.py')},
             'domolibrary.classes.DomoActivityLog': { 'domolibrary.classes.DomoActivityLog.ActivityLog_ObjectType': ( 'classes/domoactivitylog.html#activitylog_objecttype',
                                                                                                                      'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog': ( 'classes/domoactivitylog.html#domoactivitylog',
                                                                                                               'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog._process_activity_log_row': ( 'classes/domoactivitylog.html#domoactivitylog._process_activity_log_row',
                                                                                                                                         'domolibrary/classes/DomoActivityLog.py'),
                                                      'domolibrary.classes.DomoActivityLog.DomoActivityLog.get_activity_log': ( 'classes/domoactivitylog.html#domoactivitylog.get_activity_log',
@@ -671,14 +669,16 @@
                                                                                                               'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.AccountConfig_InvalidDataProvider.__init__': ( 'routes/account.html#accountconfig_invaliddataprovider.__init__',
                                                                                                                        'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.GetAccount_NoMatch': ( 'routes/account.html#getaccount_nomatch',
                                                                                                'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.GetAccount_NoMatch.__init__': ( 'routes/account.html#getaccount_nomatch.__init__',
                                                                                                         'domolibrary/routes/account.py'),
+                                            'domolibrary.routes.account.ShareAccount': ( 'routes/account.html#shareaccount',
+                                                                                         'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.ShareAccount_V1_AccessLevel': ( 'routes/account.html#shareaccount_v1_accesslevel',
                                                                                                         'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.ShareAccount_V2_AccessLevel': ( 'routes/account.html#shareaccount_v2_accesslevel',
                                                                                                         'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.create_account': ( 'routes/account.html#create_account',
                                                                                            'domolibrary/routes/account.py'),
                                             'domolibrary.routes.account.delete_account': ( 'routes/account.html#delete_account',
```

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.5/domolibrary/classes/DomoAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoAccount.ipynb.
 
 # %% auto 0
 __all__ = ['DomoAccount_Config', 'DomoAccount_Config_AbstractCredential', 'DomoAccount_Config_DatasetCopy',
            'DomoAccount_Config_Governance', 'DomoAccount_Config_AmazonS3', 'DomoAccount_Config_AwsAthena',
            'DomoAccount_Config_HighBandwidthConnector', 'AccountConfig', 'DomoAccount',
            'DomoAccount_DataProviderType_ConfigNotDefined', 'DomoAccount_UpdateName_Error',
-           'DomoAccount_CreateAccount_Error', 'DomoAccount_DeleteAccount_Error', 'ShareAccount_AccessLevel',
-           'DomoAccounts']
+           'DomoAccount_CreateAccount_Error', 'DomoAccount_DeleteAccount_Error', 'DomoAccounts']
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 3
+from ..routes.account import ShareAccount_V1_AccessLevel, ShareAccount_V2_AccessLevel, ShareAccount
+
+
+# %% ../../nbs/classes/50_DomoAccount.ipynb 4
 from enum import Enum
 from dataclasses import dataclass, field
 from abc import ABC, abstractmethod
 
 from typing import Union
 
 import datetime as dt
@@ -25,15 +28,16 @@
 
 import domolibrary.utils.convert as cd
 import domolibrary.utils.DictDot as util_dd
 import domolibrary.client.DomoAuth as dmda
 import domolibrary.client.DomoError as de
 import domolibrary.routes.account as account_routes
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 5
+
+# %% ../../nbs/classes/50_DomoAccount.ipynb 6
 class DomoAccount_Config(ABC):
     """DomoAccount Config abstract base class"""
 
     data_provider_type: str
 
     @classmethod
     @abstractmethod
@@ -43,15 +47,15 @@
 
     @abstractmethod
     def to_json(self):
         """convert class object into a format the accounts API expects"""
         pass
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 7
+# %% ../../nbs/classes/50_DomoAccount.ipynb 8
 @dataclass
 class DomoAccount_Config_AbstractCredential(DomoAccount_Config):
     data_provider_type = "abstract-credential-store"
     credentials: dict
 
     @classmethod
     def _from_json(cls, obj):
@@ -62,15 +66,15 @@
             credentials=dd.credentials,
         )
 
     def to_json(self):
         return {"credentials": self.credentials}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 8
+# %% ../../nbs/classes/50_DomoAccount.ipynb 9
 @dataclass
 class DomoAccount_Config_DatasetCopy(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
     data_provider_type = "dataset-copy"
 
@@ -81,15 +85,15 @@
 
         return cls(access_token=dd.accessToken, domo_instance=dd.instance)
 
     def to_json(self):
         return {"accessToken": self.access_token, "instance": self.domo_instance}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 9
+# %% ../../nbs/classes/50_DomoAccount.ipynb 10
 @dataclass
 class DomoAccount_Config_Governance(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
     data_provider_type = "domo-governance-d14c2fef-49a8-4898-8ddd-f64998005600"
 
@@ -100,15 +104,15 @@
 
         return cls(access_token=dd.apikey, domo_instance=dd.customer)
 
     def to_json(self):
         return {"apikey": self.access_token, "customer": self.domo_instance}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 11
+# %% ../../nbs/classes/50_DomoAccount.ipynb 12
 @dataclass
 class DomoAccount_Config_AmazonS3(DomoAccount_Config):
     access_key: str
     secret_key: str = field(repr=False)
     bucket: str
     region: str = "us-west-2"
     data_provider_type = "amazon-s3"
@@ -133,15 +137,15 @@
         return {
             "accessKey": self.access_key,
             "secretKey": self.secret_key,
             "bucket": bucket,
             "region": self.region,
         }
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 12
+# %% ../../nbs/classes/50_DomoAccount.ipynb 13
 @dataclass
 class DomoAccount_Config_AwsAthena(DomoAccount_Config):
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
     workgroup: str
 
@@ -166,15 +170,15 @@
             "awsAccessKey": self.aws_access_key,
             "awsSecretKey": self.aws_secret_key,
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
             "workgroup": self.workgroup,
         }
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 13
+# %% ../../nbs/classes/50_DomoAccount.ipynb 14
 @dataclass
 class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
     """ this connector is not enabled by default contact your CSM / AE"""
     
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
@@ -199,15 +203,15 @@
             "awsAccessKey": self.aws_access_key,
             "awsSecretKey": self.aws_secret_key,
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
         }
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 16
+# %% ../../nbs/classes/50_DomoAccount.ipynb 17
 class AccountConfig(Enum):
     """
     Enum provides appropriate spelling for data_provider_type and config object.
     The name of the enum should correspond with the data_provider_type with hyphens replaced with underscores.
     """
 
     amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
@@ -219,15 +223,15 @@
     domo_governance_d14c2fef_49a8_4898_8ddd_f64998005600 = DomoAccount_Config_Governance
 
     aws_athena = DomoAccount_Config_AwsAthena
 
     amazon_s3 = DomoAccount_Config_AmazonS3
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 18
+# %% ../../nbs/classes/50_DomoAccount.ipynb 19
 @dataclass
 class DomoAccount:
     name: str
     data_provider_type: str
 
     id: int = None
     created_dt: dt.datetime = None
@@ -247,15 +251,15 @@
             name=dd.displayName,
             data_provider_type=dd.dataProviderType,
             created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt),
             modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt),
             auth=auth,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 19
+# %% ../../nbs/classes/50_DomoAccount.ipynb 20
 class DomoAccount_DataProviderType_ConfigNotDefined(de.DomoError):
     def __init__(
         self, account_id, data_provider_type, domo_instance, function_name="_get_config"
     ):
 
         message = f"🛑 data provider type {data_provider_type} for account_id {account_id} not defined yet.  Extend the AccountConfig class"
 
@@ -296,15 +300,15 @@
             function_name = '_get_config'
         )
 
     self.config = AccountConfig[enum_clean].value._from_json(res_config.response)
 
     return self.config
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 20
+# %% ../../nbs/classes/50_DomoAccount.ipynb 21
 @patch_to(DomoAccount, cls_method=True)
 async def get_from_id(
     cls,
     auth: dmda.DomoAuth,
     account_id: int,
     session: httpx.AsyncClient = None,
     return_raw: bool = False,
@@ -334,15 +338,15 @@
     
     except Exception as e:
         print(e)
 
     finally:
         return acc
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 24
+# %% ../../nbs/classes/50_DomoAccount.ipynb 25
 @patch_to(DomoAccount)
 async def update_config(
     self: DomoAccount,
     auth: dmda.DomoAuth = None,
     debug_api: bool = False,
     config: DomoAccount_Config = None,
     session: httpx.AsyncClient = None,
@@ -366,15 +370,15 @@
         return res
 
     await self._get_config(session=session, debug_api=debug_api)
 
     return self
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 27
+# %% ../../nbs/classes/50_DomoAccount.ipynb 28
 class DomoAccount_UpdateName_Error(de.DomoError):
     def __init__(
         self,
         domo_instance,
         status,
         message,
         entity_id,
@@ -423,15 +427,15 @@
             message=res.response,
         )
 
     self = await self.get_from_id(auth=auth, account_id=self.id)
 
     return self
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 31
+# %% ../../nbs/classes/50_DomoAccount.ipynb 32
 class DomoAccount_CreateAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -442,15 +446,15 @@
             function_name=function_name,
             entity_id=entity_id,
             domo_instance=domo_instance,
             status=status,
             message=message,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 32
+# %% ../../nbs/classes/50_DomoAccount.ipynb 33
 @patch_to(DomoAccount, cls_method=True)
 def generate_create_body(cls, account_name, config):
     return {
         "displayName": account_name,
         "dataProviderType": config.data_provider_type,
         "name": config.data_provider_type,
         "configurations": config.to_json(),
@@ -479,15 +483,15 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return await cls.get_from_id(auth=auth, account_id=res.response.get("id"))
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 33
+# %% ../../nbs/classes/50_DomoAccount.ipynb 34
 class DomoAccount_DeleteAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -524,22 +528,15 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return True
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 34
-class ShareAccount_AccessLevel(Enum):
-    "enumerates access levels for Domo Users and Domo Accounts"
-    CAN_VIEW = "CAN_VIEW"
-    CAN_EDIT = "CAN_EDIT" # only available with accounts_v2 feature switch (group ownership beta)
-    CAN_SHARE = "CAN_SHARE" # only available with accounts_v2 feature switch (group ownership beta)
-
-
+# %% ../../nbs/classes/50_DomoAccount.ipynb 35
 @patch_to(DomoAccount)
 async def _is_group_ownership_beta(self, auth : dmda.DomoAuth):
     import domolibrary.classes.DomoBootstrap as dmbs
 
     domo_bsr = dmbs.DomoBootstrap(auth=auth or self.auth)
     domo_feature_ls = await domo_bsr.get_features()
 
@@ -551,15 +548,15 @@
 
 @patch_to(DomoAccount)
 async def share_account(
     self,
     user_id: int,
     auth: dmda.DomoAuth = None,
     is_v2 :bool = None,
-    access_level: ShareAccount_AccessLevel = ShareAccount_AccessLevel.CAN_VIEW,
+    access_level: ShareAccount = None, # will default to Read
     debug_api: bool = False,
     debug_prn:bool = False,
     session: httpx.AsyncClient = None,
 ):
     auth = auth or self.auth
 
     if isinstance(auth, dmda.DomoFullAuth):
@@ -573,27 +570,27 @@
             """🛑 ERROR must pass `is_v2` bool to share_accounts function IF NOT pass `dmda.DomoFullAuth`.
 the group management v2 API has a different body.  
 Alternatively pass a full auth object to auto check the bootstrap.
 """)
 
     if is_v2:
         share_payload = account_routes.generate_share_account_payload_v2(
-            user_id=user_id, access_level=access_level.value
+            user_id=user_id, access_level=access_level or ShareAccount_V2_AccessLevel.CAN_VIEW
         )
 
         return await account_routes.share_account_v2(
             auth=auth,
             account_id=self.id,
             share_payload=share_payload,
             debug_api=debug_api,
             session=session,
         )
 
     share_payload = account_routes.generate_share_account_payload_v1(
-        user_id=user_id, access_level=access_level.value
+        user_id=user_id, access_level=access_level or ShareAccount_V1_AccessLevel.CAN_VIEW
     )
 
     res = await account_routes.share_account_v1(
         auth=auth,
         account_id=self.id,
         share_payload=share_payload,
         debug_api=debug_api,
@@ -601,20 +598,20 @@
     )
 
     if res.status == 500 and res.response == 'Internal Server Error':
         res.response = f'ℹ️ - {res.response + "| User may own account."}'
     return res
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 37
+# %% ../../nbs/classes/50_DomoAccount.ipynb 38
 @dataclass
 class DomoAccounts:
     auth: dmda.DomoAuth
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 38
+# %% ../../nbs/classes/50_DomoAccount.ipynb 39
 @patch_to(DomoAccounts, cls_method=True)
 async def get_accounts(
     cls: DomoAccounts,
     auth: dmda.DomoAuth,
     account_name: str = None, # account string to search for, must be an exact match in spelling.  case insensitive
     account_type: AccountConfig = None, #to retrieve a specific account type
     debug_api: bool = False,
```

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.5/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.5/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.5/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.5/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.5/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.5/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.5/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.5/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.5/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.5/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.5/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.5/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.5/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.5/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/client/DomoError.py` & `domolibrary-0.1.5/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/client/Logger.py` & `domolibrary-0.1.5/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.5/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/client/get_data.py` & `domolibrary-0.1.5/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.5/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.5/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/account.py` & `domolibrary-0.1.5/domolibrary/routes/account.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/routes/account.ipynb.
 
 # %% auto 0
 __all__ = ['get_accounts', 'GetAccount_NoMatch', 'get_account_from_id', 'AccountConfig_InvalidDataProvider', 'get_account_config',
-           'update_account_config', 'update_account_name', 'create_account', 'delete_account',
+           'update_account_config', 'update_account_name', 'create_account', 'delete_account', 'ShareAccount',
            'ShareAccount_V1_AccessLevel', 'ShareAccount_V2_AccessLevel', 'generate_share_account_payload_v1',
            'generate_share_account_payload_v2', 'share_account_v2', 'share_account_v1']
 
 # %% ../../nbs/routes/account.ipynb 3
 from typing import Union
 from enum import Enum
 import httpx
@@ -176,33 +176,38 @@
         url=url,
         method='DELETE',
         debug_api=debug_api,
         session=session
     )
 
 # %% ../../nbs/routes/account.ipynb 19
-class ShareAccount_V1_AccessLevel(Enum):
+class ShareAccount():
+    pass
+
+
+class ShareAccount_V1_AccessLevel(ShareAccount, Enum):
     CAN_VIEW = 'READ'
 
 
-class ShareAccount_V2_AccessLevel(Enum):
+class ShareAccount_V2_AccessLevel(ShareAccount, Enum):
     CAN_VIEW = 'CAN_VIEW'
     CAN_EDIT = 'CAN_EDIT'
     CAN_SHARE = 'CAN_SHARE'
 
 
-def generate_share_account_payload_v1(user_id: int, access_level: str):
-    return {"type": "USER", "id": user_id, "permissions": [ShareAccount_V1_AccessLevel[access_level].value]}
+def generate_share_account_payload_v1(user_id: int,
+                                      access_level: ShareAccount):
+    return {"type": "USER", "id": user_id, "permissions": [access_level.value]}
 
 
 def generate_share_account_payload_v2(user_id: int,
-                                      access_level: str
+                                      access_level: ShareAccount
                                       ):
 
-    return {"type": "USER", "id": user_id, "accessLevel": ShareAccount_V2_AccessLevel[access_level].value}
+    return {"type": "USER", "id": user_id, "accessLevel": access_level.value}
 
 
 # %% ../../nbs/routes/account.ipynb 21
 async def share_account_v2(auth: dmda.DomoAuth,
                            account_id: str,
                            share_payload: dict,
                            debug_api: bool = False,
```

### Comparing `domolibrary-0.1.4/domolibrary/routes/activity_log.py` & `domolibrary-0.1.5/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.5/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/card.py` & `domolibrary-0.1.5/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/datacenter.py` & `domolibrary-0.1.5/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/dataflow.py` & `domolibrary-0.1.5/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/dataset.py` & `domolibrary-0.1.5/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/grant.py` & `domolibrary-0.1.5/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/group.py` & `domolibrary-0.1.5/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/instance_config.py` & `domolibrary-0.1.5/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/page.py` & `domolibrary-0.1.5/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/pdp.py` & `domolibrary-0.1.5/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/publish.py` & `domolibrary-0.1.5/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/role.py` & `domolibrary-0.1.5/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/routes/user.py` & `domolibrary-0.1.5/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/utils/DictDot.py` & `domolibrary-0.1.5/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.5/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/utils/convert.py` & `domolibrary-0.1.5/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.5/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary/utils/upload_data.py` & `domolibrary-0.1.5/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.5/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.4
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.4/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.5/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/settings.ini` & `domolibrary-0.1.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.04
+version = 0.1.05
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.4/setup.py` & `domolibrary-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/Base.py` & `domolibrary-0.1.5/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/DictDot.py` & `domolibrary-0.1.5/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/Exceptions.py` & `domolibrary-0.1.5/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/LoggerClass.py` & `domolibrary-0.1.5/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/chunk_execution.py` & `domolibrary-0.1.5/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/consol_get_creds.py` & `domolibrary-0.1.5/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/convert.py` & `domolibrary-0.1.5/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.5/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.4/utils/upload_data.py` & `domolibrary-0.1.5/utils/upload_data.py`

 * *Files identical despite different names*

