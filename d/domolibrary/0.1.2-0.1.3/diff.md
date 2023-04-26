# Comparing `tmp/domolibrary-0.1.2.tar.gz` & `tmp/domolibrary-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-0.1.2.tar", last modified: Wed Apr 26 13:37:55 2023, max compression
+gzip compressed data, was "domolibrary-0.1.3.tar", last modified: Wed Apr 26 16:43:11 2023, max compression
```

## Comparing `domolibrary-0.1.2.tar` & `domolibrary-0.1.3.tar`

### file list

```diff
@@ -1,145 +1,145 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.063516 domolibrary-0.1.2/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.895516 domolibrary-0.1.2/Automation/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/Automation/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.2/Automation/automation.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.907516 domolibrary-0.1.2/DataOcean/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/Transport.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_athena_highbandwidth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_pgsql.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_s3.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DataOcean/cnfg_snowflake.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.951516 domolibrary-0.1.2/DomoClasses/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoAppDb.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.2/DomoClasses/DomoApplication.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoCard.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoCertification.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.2/DomoClasses/DomoJob.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoLineage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.2/DomoClasses/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoSandbox.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/DomoStream.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoTag.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:54.999516 domolibrary-0.1.2/DomoClasses/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.2/DomoClasses/routes/account_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/activity_log_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/appdb_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/application_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/auth_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/bootstrap_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/card_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/datacenter_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/dataflow_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/dataset_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.2/DomoClasses/routes/get_data.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/grant_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/group_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/instance_config_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.2/DomoClasses/routes/job_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.2/DomoClasses/routes/page_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/pdp_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/publish_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/role_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/sandbox_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/stream_routes.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.2/DomoClasses/routes/user_routes.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.003516 domolibrary-0.1.2/GitHub/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/GitHub/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.2/GitHub/get_github_file.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.2/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.2/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 13:37:55.063516 domolibrary-0.1.2/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.2/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.007516 domolibrary-0.1.2/domolibrary/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)   147817 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/_modidx.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/classes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17100 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoAccount.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoActivityLog.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoBootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDatacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoDataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoGrant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoGroup.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoInstanceConfig.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPDP.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPage.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoPublish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoRole.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/classes/DomoUser.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/classes/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/client/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/DomoAuth.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/DomoError.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/Logger.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/client/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/client/get_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.027516 domolibrary-0.1.2/domolibrary/integrations/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/DomoJupyter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/RoleHierarchy.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/integrations/__init__.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.035516 domolibrary-0.1.2/domolibrary/routes/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8202 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/account.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/activity_log.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/bootstrap.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/card.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/datacenter.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/dataflow.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/dataset.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/grant.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/group.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/instance_config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/page.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/pdp.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 13:37:41.000000 domolibrary-0.1.2/domolibrary/routes/publish.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/role.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/routes/user.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.039516 domolibrary-0.1.2/domolibrary/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      865 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 13:37:42.000000 domolibrary-0.1.2/domolibrary/utils/upload_data.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.019516 domolibrary-0.1.2/domolibrary.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.2/domolibrary.egg-info/not-zip-safe
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 13:37:54.000000 domolibrary-0.1.2/domolibrary.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 13:37:50.000000 domolibrary-0.1.2/settings.ini
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 13:37:55.063516 domolibrary-0.1.2/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.2/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 13:37:55.059516 domolibrary-0.1.2/utils/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/Base.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/DictDot.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.2/utils/Exceptions.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.2/utils/LoggerClass.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/ResponseGetData.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/chunk_execution.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/consol_get_creds.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/convert.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.2/utils/read_creds_from_dotenv.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.2/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.407911 domolibrary-0.1.3/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.295911 domolibrary-0.1.3/Automation/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/Automation/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6580 2023-01-05 15:38:44.000000 domolibrary-0.1.3/Automation/automation.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.303911 domolibrary-0.1.3/DataOcean/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2534 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/Transport.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2263 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/cnfg_athena_highbandwidth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3060 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/cnfg_pgsql.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3402 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/cnfg_s3.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3514 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DataOcean/cnfg_snowflake.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.343911 domolibrary-0.1.3/DomoClasses/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9543 2023-01-17 21:03:25.000000 domolibrary-0.1.3/DomoClasses/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2504 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1904 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoAppDb.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4514 2023-03-02 20:34:40.000000 domolibrary-0.1.3/DomoClasses/DomoApplication.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5125 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1680 2023-01-17 21:03:25.000000 domolibrary-0.1.3/DomoClasses/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1643 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoCard.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      767 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoCertification.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8511 2023-01-17 21:03:25.000000 domolibrary-0.1.3/DomoClasses/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1789 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    19304 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      727 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8797 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8972 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12851 2023-04-03 12:48:28.000000 domolibrary-0.1.3/DomoClasses/DomoJob.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8279 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoLineage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3950 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15635 2023-02-08 21:41:51.000000 domolibrary-0.1.3/DomoClasses/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10879 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4464 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2963 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoSandbox.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7127 2023-01-17 21:03:25.000000 domolibrary-0.1.3/DomoClasses/DomoStream.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3073 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoTag.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8118 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.359911 domolibrary-0.1.3/DomoClasses/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6391 2023-01-17 21:03:25.000000 domolibrary-0.1.3/DomoClasses/routes/account_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1469 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/activity_log_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1359 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/appdb_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1294 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/application_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1763 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/auth_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      889 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/bootstrap_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2638 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/card_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3711 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/datacenter_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      830 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/dataflow_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13688 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/dataset_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6044 2023-04-03 12:48:28.000000 domolibrary-0.1.3/DomoClasses/routes/get_data.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      977 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/grant_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4523 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/group_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2697 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/instance_config_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6434 2023-03-02 20:34:40.000000 domolibrary-0.1.3/DomoClasses/routes/job_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3183 2023-01-31 17:52:06.000000 domolibrary-0.1.3/DomoClasses/routes/page_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2470 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/pdp_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4670 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/publish_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3836 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/role_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2204 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/sandbox_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1633 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/stream_routes.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4371 2023-01-05 15:38:44.000000 domolibrary-0.1.3/DomoClasses/routes/user_routes.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.359911 domolibrary-0.1.3/GitHub/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/GitHub/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-01-05 15:38:44.000000 domolibrary-0.1.3/GitHub/get_github_file.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11337 2023-01-05 15:38:44.000000 domolibrary-0.1.3/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      111 2023-01-05 15:38:44.000000 domolibrary-0.1.3/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 16:43:11.407911 domolibrary-0.1.3/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8248 2023-04-25 19:47:17.000000 domolibrary-0.1.3/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.359911 domolibrary-0.1.3/domolibrary/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       23 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)   147817 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/_modidx.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.363911 domolibrary-0.1.3/domolibrary/classes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17116 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoAccount.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4070 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoActivityLog.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3015 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoBootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4119 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoDatacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2706 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoDataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    25103 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoDataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1255 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoGrant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    17403 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoGroup.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6174 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoInstanceConfig.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9145 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoPDP.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4432 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoPage.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6985 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoPublish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15572 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoRole.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    13908 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/DomoUser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/classes/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.363911 domolibrary-0.1.3/domolibrary/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12655 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/DomoAuth.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2069 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/DomoError.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5929 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/Logger.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6189 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    12027 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/client/get_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.363911 domolibrary-0.1.3/domolibrary/integrations/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15484 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/integrations/DomoJupyter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3207 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/integrations/RoleHierarchy.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/integrations/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.371911 domolibrary-0.1.3/domolibrary/routes/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8202 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/account.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2035 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/activity_log.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2039 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/bootstrap.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3425 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/card.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6442 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/datacenter.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      769 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/dataflow.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15254 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/dataset.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1682 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/grant.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    10945 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/group.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4807 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/instance_config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2488 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/page.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     7214 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/pdp.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4174 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/publish.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8584 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/role.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9473 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/routes/user.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.383911 domolibrary-0.1.3/domolibrary/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1660 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      865 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1732 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1184 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4519 2023-04-26 16:42:55.000000 domolibrary-0.1.3/domolibrary/utils/upload_data.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.363911 domolibrary-0.1.3/domolibrary.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9024 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3842 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       65 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-02-17 20:52:42.000000 domolibrary-0.1.3/domolibrary.egg-info/not-zip-safe
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      105 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       58 2023-04-26 16:43:11.000000 domolibrary-0.1.3/domolibrary.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1083 2023-04-26 15:03:46.000000 domolibrary-0.1.3/settings.ini
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-04-26 16:43:11.407911 domolibrary-0.1.3/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2539 2023-01-06 02:41:16.000000 domolibrary-0.1.3/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-04-26 16:43:11.403911 domolibrary-0.1.3/utils/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      540 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/Base.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      759 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/DictDot.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1220 2023-01-09 21:38:41.000000 domolibrary-0.1.3/utils/Exceptions.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2578 2023-01-17 21:03:25.000000 domolibrary-0.1.3/utils/LoggerClass.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      273 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/ResponseGetData.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1145 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/chunk_execution.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1133 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/consol_get_creds.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      522 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/convert.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1476 2023-01-05 15:38:44.000000 domolibrary-0.1.3/utils/read_creds_from_dotenv.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3671 2023-03-06 14:03:40.000000 domolibrary-0.1.3/utils/upload_data.py
```

### Comparing `domolibrary-0.1.2/Automation/automation.py` & `domolibrary-0.1.3/Automation/automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DataOcean/Transport.py` & `domolibrary-0.1.3/DataOcean/Transport.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DataOcean/cnfg_athena_highbandwidth.py` & `domolibrary-0.1.3/DataOcean/cnfg_athena_highbandwidth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DataOcean/cnfg_pgsql.py` & `domolibrary-0.1.3/DataOcean/cnfg_pgsql.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DataOcean/cnfg_s3.py` & `domolibrary-0.1.3/DataOcean/cnfg_s3.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DataOcean/cnfg_snowflake.py` & `domolibrary-0.1.3/DataOcean/cnfg_snowflake.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoAccount.py` & `domolibrary-0.1.3/DomoClasses/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoActivityLog.py` & `domolibrary-0.1.3/DomoClasses/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoAppDb.py` & `domolibrary-0.1.3/DomoClasses/DomoAppDb.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoApplication.py` & `domolibrary-0.1.3/DomoClasses/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoAuth.py` & `domolibrary-0.1.3/DomoClasses/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoBootstrap.py` & `domolibrary-0.1.3/DomoClasses/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoCard.py` & `domolibrary-0.1.3/DomoClasses/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoCertification.py` & `domolibrary-0.1.3/DomoClasses/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoDatacenter.py` & `domolibrary-0.1.3/DomoClasses/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoDataflow.py` & `domolibrary-0.1.3/DomoClasses/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoDataset.py` & `domolibrary-0.1.3/DomoClasses/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoGrant.py` & `domolibrary-0.1.3/DomoClasses/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoGroup.py` & `domolibrary-0.1.3/DomoClasses/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoInstanceConfig.py` & `domolibrary-0.1.3/DomoClasses/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoJob.py` & `domolibrary-0.1.3/DomoClasses/DomoJob.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoLineage.py` & `domolibrary-0.1.3/DomoClasses/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoPDP.py` & `domolibrary-0.1.3/DomoClasses/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoPage.py` & `domolibrary-0.1.3/DomoClasses/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoPublish.py` & `domolibrary-0.1.3/DomoClasses/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoRole.py` & `domolibrary-0.1.3/DomoClasses/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoSandbox.py` & `domolibrary-0.1.3/DomoClasses/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoStream.py` & `domolibrary-0.1.3/DomoClasses/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoTag.py` & `domolibrary-0.1.3/DomoClasses/DomoTag.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/DomoUser.py` & `domolibrary-0.1.3/DomoClasses/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/account_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/account_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/activity_log_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/activity_log_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/appdb_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/appdb_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/application_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/application_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/auth_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/auth_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/bootstrap_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/bootstrap_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/card_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/card_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/datacenter_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/datacenter_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/dataflow_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/dataflow_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/dataset_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/dataset_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/get_data.py` & `domolibrary-0.1.3/DomoClasses/routes/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/grant_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/grant_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/group_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/group_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/instance_config_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/instance_config_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/job_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/job_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/page_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/page_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/pdp_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/pdp_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/publish_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/publish_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/role_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/role_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/sandbox_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/sandbox_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/stream_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/stream_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/DomoClasses/routes/user_routes.py` & `domolibrary-0.1.3/DomoClasses/routes/user_routes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/LICENSE` & `domolibrary-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/PKG-INFO` & `domolibrary-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.2/README.md` & `domolibrary-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/_modidx.py` & `domolibrary-0.1.3/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoAccount.py` & `domolibrary-0.1.3/domolibrary/classes/DomoAccount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/classes/50_DomoAccount.ipynb.
 
 # %% auto 0
 __all__ = ['DomoAccount_Config', 'DomoAccount_Config_AbstractCredential', 'DomoAccount_Config_DatasetCopy',
-           'DomoAccount_Config_Governance', 'DomoAccount_Config_HighBandwidthConnector', 'DomoAccount_Config_AmazonS3',
-           'DomoAccount_Config_AwsAthena', 'AccountConfig', 'DomoAccount',
+           'DomoAccount_Config_Governance', 'DomoAccount_Config_AmazonS3', 'DomoAccount_Config_AwsAthena',
+           'DomoAccount_Config_HighBandwidthConnector', 'AccountConfig', 'DomoAccount',
            'DomoAccount_DataProviderType_ConfigNotDefined', 'DomoAccount_UpdateName_Error',
            'DomoAccount_CreateAccount_Error', 'DomoAccount_DeleteAccount_Error', 'ShareAccount_AccessLevel',
            'DomoAccounts']
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 3
 from enum import Enum
 from dataclasses import dataclass, field
@@ -43,15 +43,15 @@
 
     @abstractmethod
     def to_json(self):
         """convert class object into a format the accounts API expects"""
         pass
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 6
+# %% ../../nbs/classes/50_DomoAccount.ipynb 7
 @dataclass
 class DomoAccount_Config_AbstractCredential(DomoAccount_Config):
     data_provider_type = "abstract-credential-store"
     credentials: dict
 
     @classmethod
     def _from_json(cls, obj):
@@ -62,15 +62,15 @@
             credentials=dd.credentials,
         )
 
     def to_json(self):
         return {"credentials": self.credentials}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 7
+# %% ../../nbs/classes/50_DomoAccount.ipynb 8
 @dataclass
 class DomoAccount_Config_DatasetCopy(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
     data_provider_type = "dataset-copy"
 
@@ -81,15 +81,15 @@
 
         return cls(access_token=dd.accessToken, domo_instance=dd.instance)
 
     def to_json(self):
         return {"accessToken": self.access_token, "instance": self.domo_instance}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 8
+# %% ../../nbs/classes/50_DomoAccount.ipynb 9
 @dataclass
 class DomoAccount_Config_Governance(DomoAccount_Config):
     domo_instance: str
     access_token: str = field(repr=False)
 
     data_provider_type = "domo-governance-d14c2fef-49a8-4898-8ddd-f64998005600"
 
@@ -100,113 +100,114 @@
 
         return cls(access_token=dd.apikey, domo_instance=dd.customer)
 
     def to_json(self):
         return {"apikey": self.access_token, "customer": self.domo_instance}
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 9
+# %% ../../nbs/classes/50_DomoAccount.ipynb 11
 @dataclass
-class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
-    aws_access_key: str
-    aws_secret_key: str = field(repr=False)
-    s3_staging_dir: str
-
+class DomoAccount_Config_AmazonS3(DomoAccount_Config):
+    access_key: str
+    secret_key: str = field(repr=False)
+    bucket: str
     region: str = "us-west-2"
-    data_provider_type = "amazon-athena-high-bandwidth"
+    data_provider_type = "amazon-s3"
 
+    
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
         return cls(
-            aws_access_key=dd.awsAccessKey,
-            aws_secret_key=dd.awsSecretKey,
-            s3_staging_dir=dd.s3StagingDir,
+            access_key=dd.accessKey,
+            secret_key=dd.secretKey,
+            bucket=dd.bucket,
             region=dd.region,
         )
 
     def to_json(self):
+        if self.bucket.lower().startswith("s3://"):
+            bucket = self.bucket[5:]
+            print(f"🤦‍♀️- Domo bucket expects string without s3:// prefix. Trimming to '{bucket}' for the output")
         return {
-            "awsAccessKey": self.aws_access_key,
-            "awsSecretKey": self.aws_secret_key,
-            "s3StagingDir": self.s3_staging_dir,
+            "accessKey": self.access_key,
+            "secretKey": self.secret_key,
+            "bucket": bucket,
             "region": self.region,
         }
 
-
-# %% ../../nbs/classes/50_DomoAccount.ipynb 10
+# %% ../../nbs/classes/50_DomoAccount.ipynb 12
 @dataclass
-class DomoAccount_Config_AmazonS3(DomoAccount_Config):
-    access_key: str
-    secret_key: str = field(repr=False)
-    bucket: str
+class DomoAccount_Config_AwsAthena(DomoAccount_Config):
+    aws_access_key: str
+    aws_secret_key: str = field(repr=False)
+    s3_staging_dir: str
+    workgroup: str
+
     region: str = "us-west-2"
-    data_provider_type = "amazon-s3"
+    data_provider_type = "aws-athena"
 
-    
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
         return cls(
             aws_access_key=dd.awsAccessKey,
             aws_secret_key=dd.awsSecretKey,
             s3_staging_dir=dd.s3StagingDir,
             region=dd.region,
             workgroup=dd.workgroup,
         )
 
     def to_json(self):
-        if self.bucket.lower().startswith("s3://"):
-            bucket = self.bucket[5:]
-            print(f"🤦‍♀️- Domo bucket expects string without s3:// prefix. Trimming to '{bucket}' for the output")
         return {
-            "accessKey": self.access_key,
-            "secretKey": self.secret_key,
-            "bucket": bucket,
+            "awsAccessKey": self.aws_access_key,
+            "awsSecretKey": self.aws_secret_key,
+            "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
+            "workgroup": self.workgroup,
         }
 
 # %% ../../nbs/classes/50_DomoAccount.ipynb 13
 @dataclass
-class DomoAccount_Config_AwsAthena(DomoAccount_Config):
+class DomoAccount_Config_HighBandwidthConnector(DomoAccount_Config):
+    """ this connector is not enabled by default contact your CSM / AE"""
+    
     aws_access_key: str
     aws_secret_key: str = field(repr=False)
     s3_staging_dir: str
-    workgroup: str
 
     region: str = "us-west-2"
-    data_provider_type = "aws-athena"
+    data_provider_type = "amazon-athena-high-bandwidth"
 
     @classmethod
     def _from_json(cls, obj):
 
         dd = util_dd.DictDot(obj)
 
         return cls(
             aws_access_key=dd.awsAccessKey,
             aws_secret_key=dd.awsSecretKey,
             s3_staging_dir=dd.s3StagingDir,
             region=dd.region,
-            workgroup=dd.workgroup,
         )
 
     def to_json(self):
         return {
             "awsAccessKey": self.aws_access_key,
             "awsSecretKey": self.aws_secret_key,
             "s3StagingDir": self.s3_staging_dir,
             "region": self.region,
-            "workgroup": self.workgroup,
         }
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 14
+
+# %% ../../nbs/classes/50_DomoAccount.ipynb 16
 class AccountConfig(Enum):
     """
     Enum provides appropriate spelling for data_provider_type and config object.
     The name of the enum should correspond with the data_provider_type with hyphens replaced with underscores.
     """
 
     amazon_athena_high_bandwidth = DomoAccount_Config_HighBandwidthConnector
@@ -218,15 +219,15 @@
     domo_governance_d14c2fef_49a8_4898_8ddd_f64998005600 = DomoAccount_Config_Governance
 
     aws_athena = DomoAccount_Config_AwsAthena
 
     amazon_s3 = DomoAccount_Config_AmazonS3
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 16
+# %% ../../nbs/classes/50_DomoAccount.ipynb 18
 @dataclass
 class DomoAccount:
     name: str
     data_provider_type: str
 
     id: int = None
     created_dt: dt.datetime = None
@@ -246,15 +247,15 @@
             name=dd.displayName,
             data_provider_type=dd.dataProviderType,
             created_dt=cd.convert_epoch_millisecond_to_datetime(dd.createdAt),
             modified_dt=cd.convert_epoch_millisecond_to_datetime(dd.modifiedAt),
             auth=auth,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 17
+# %% ../../nbs/classes/50_DomoAccount.ipynb 19
 class DomoAccount_DataProviderType_ConfigNotDefined(de.DomoError):
     def __init__(
         self, account_id, data_provider_type, domo_instance, function_name="_get_config"
     ):
 
         message = f"🛑 data provider type {data_provider_type} for account_id {account_id} not defined yet.  Extend the AccountConfig class"
 
@@ -295,15 +296,15 @@
             function_name = '_get_config'
         )
 
     self.config = AccountConfig[enum_clean].value._from_json(res_config.response)
 
     return self.config
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 18
+# %% ../../nbs/classes/50_DomoAccount.ipynb 20
 @patch_to(DomoAccount, cls_method=True)
 async def get_from_id(
     cls,
     auth: dmda.DomoAuth,
     account_id: int,
     session: httpx.AsyncClient = None,
     return_raw: bool = False,
@@ -333,15 +334,15 @@
     
     except Exception as e:
         print(e)
 
     finally:
         return acc
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 22
+# %% ../../nbs/classes/50_DomoAccount.ipynb 24
 @patch_to(DomoAccount)
 async def update_config(
     self: DomoAccount,
     auth: dmda.DomoAuth = None,
     debug_api: bool = False,
     config: DomoAccount_Config = None,
     session: httpx.AsyncClient = None,
@@ -365,15 +366,15 @@
         return res
 
     await self._get_config(session=session, debug_api=debug_api)
 
     return self
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 25
+# %% ../../nbs/classes/50_DomoAccount.ipynb 27
 class DomoAccount_UpdateName_Error(de.DomoError):
     def __init__(
         self,
         domo_instance,
         status,
         message,
         entity_id,
@@ -422,15 +423,15 @@
             message=res.response,
         )
 
     self = await self.get_from_id(auth=auth, account_id=self.id)
 
     return self
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 29
+# %% ../../nbs/classes/50_DomoAccount.ipynb 31
 class DomoAccount_CreateAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -441,15 +442,15 @@
             function_name=function_name,
             entity_id=entity_id,
             domo_instance=domo_instance,
             status=status,
             message=message,
         )
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 30
+# %% ../../nbs/classes/50_DomoAccount.ipynb 32
 @patch_to(DomoAccount, cls_method=True)
 def generate_create_body(cls, account_name, config):
     return {
         "displayName": account_name,
         "dataProviderType": config.data_provider_type,
         "name": config.data_provider_type,
         "configurations": config.to_json(),
@@ -478,15 +479,15 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return await cls.get_from_id(auth=auth, account_id=res.response.get("id"))
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 31
+# %% ../../nbs/classes/50_DomoAccount.ipynb 33
 class DomoAccount_DeleteAccount_Error(de.DomoError):
     def __init__(
         self,
         entity_id,
         domo_instance,
         status,
         message,
@@ -523,15 +524,15 @@
             domo_instance=auth.domo_instance,
             status=res.status,
             message=res.response,
         )
 
     return True
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 32
+# %% ../../nbs/classes/50_DomoAccount.ipynb 34
 class ShareAccount_AccessLevel(Enum):
     "enumerates access levels for Domo Users and Domo Accounts"
     CAN_VIEW = "CAN_VIEW"
     CAN_EDIT = "CAN_EDIT" # only available with accounts_v2 feature switch (group ownership beta)
     CAN_SHARE = "CAN_SHARE" # only available with accounts_v2 feature switch (group ownership beta)
 
 
@@ -567,20 +568,20 @@
         account_id=self.id,
         share_payload=share_payload,
         debug_api=debug_api,
         session=session,
     )
 
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 34
+# %% ../../nbs/classes/50_DomoAccount.ipynb 36
 @dataclass
 class DomoAccounts:
     auth: dmda.DomoAuth
 
-# %% ../../nbs/classes/50_DomoAccount.ipynb 35
+# %% ../../nbs/classes/50_DomoAccount.ipynb 37
 @patch_to(DomoAccounts, cls_method=True)
 async def get_accounts(
     cls: DomoAccounts,
     auth: dmda.DomoAuth,
     account_name: str = None, # account string to search for, must be an exact match in spelling.  case insensitive
     account_type: AccountConfig = None, #to retrieve a specific account type
     debug_api: bool = False,
```

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoActivityLog.py` & `domolibrary-0.1.3/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoBootstrap.py` & `domolibrary-0.1.3/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoDatacenter.py` & `domolibrary-0.1.3/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoDataflow.py` & `domolibrary-0.1.3/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoDataset.py` & `domolibrary-0.1.3/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoGrant.py` & `domolibrary-0.1.3/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoGroup.py` & `domolibrary-0.1.3/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-0.1.3/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoPDP.py` & `domolibrary-0.1.3/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoPage.py` & `domolibrary-0.1.3/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoPublish.py` & `domolibrary-0.1.3/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoRole.py` & `domolibrary-0.1.3/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/classes/DomoUser.py` & `domolibrary-0.1.3/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/client/DomoAuth.py` & `domolibrary-0.1.3/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/client/DomoError.py` & `domolibrary-0.1.3/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/client/Logger.py` & `domolibrary-0.1.3/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/client/ResponseGetData.py` & `domolibrary-0.1.3/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/client/get_data.py` & `domolibrary-0.1.3/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/integrations/DomoJupyter.py` & `domolibrary-0.1.3/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-0.1.3/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/account.py` & `domolibrary-0.1.3/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/activity_log.py` & `domolibrary-0.1.3/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/bootstrap.py` & `domolibrary-0.1.3/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/card.py` & `domolibrary-0.1.3/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/datacenter.py` & `domolibrary-0.1.3/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/dataflow.py` & `domolibrary-0.1.3/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/dataset.py` & `domolibrary-0.1.3/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/grant.py` & `domolibrary-0.1.3/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/group.py` & `domolibrary-0.1.3/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/instance_config.py` & `domolibrary-0.1.3/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/page.py` & `domolibrary-0.1.3/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/pdp.py` & `domolibrary-0.1.3/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/publish.py` & `domolibrary-0.1.3/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/role.py` & `domolibrary-0.1.3/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/routes/user.py` & `domolibrary-0.1.3/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/utils/DictDot.py` & `domolibrary-0.1.3/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/utils/chunk_execution.py` & `domolibrary-0.1.3/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/utils/convert.py` & `domolibrary-0.1.3/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.3/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary/utils/upload_data.py` & `domolibrary-0.1.3/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/domolibrary.egg-info/PKG-INFO` & `domolibrary-0.1.3/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 0.1.2
+Version: 0.1.3
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-0.1.2/domolibrary.egg-info/SOURCES.txt` & `domolibrary-0.1.3/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/settings.ini` & `domolibrary-0.1.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 0.1.02
+version = 0.1.03
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-0.1.2/setup.py` & `domolibrary-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/Base.py` & `domolibrary-0.1.3/utils/Base.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/DictDot.py` & `domolibrary-0.1.3/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/Exceptions.py` & `domolibrary-0.1.3/utils/Exceptions.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/LoggerClass.py` & `domolibrary-0.1.3/utils/LoggerClass.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/chunk_execution.py` & `domolibrary-0.1.3/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/consol_get_creds.py` & `domolibrary-0.1.3/utils/consol_get_creds.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/convert.py` & `domolibrary-0.1.3/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/read_creds_from_dotenv.py` & `domolibrary-0.1.3/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-0.1.2/utils/upload_data.py` & `domolibrary-0.1.3/utils/upload_data.py`

 * *Files identical despite different names*

