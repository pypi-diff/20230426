# Comparing `tmp/datature-1.0.0.tar.gz` & `tmp/datature-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-kbibbuc8/datature-1.0.0.tar", last modified: Fri Apr 14 09:08:20 2023, max compression
+gzip compressed data, was "/home/runner/work/Puppeteer/Puppeteer/pypi/puppeteer/dist/.tmp-9vsg8_24/datature-1.0.1.tar", last modified: Wed Apr 26 10:54:28 2023, max compression
```

## Comparing `datature-1.0.0.tar` & `datature-1.0.1.tar`

### file list

```diff
@@ -1,80 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-14 09:08:09.000000 datature-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-14 09:08:09.000000 datature-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 09:08:20.000000 datature-1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 09:08:09.000000 datature-1.0.0/datature/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-14 09:08:09.000000 datature-1.0.0/datature/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-14 09:08:09.000000 datature-1.0.0/datature/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-14 09:08:09.000000 datature-1.0.0/datature/http/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-14 09:08:09.000000 datature-1.0.0/datature/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-14 09:08:09.000000 datature-1.0.0/datature/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/base_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/dicom_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-04-14 09:08:09.000000 datature-1.0.0/datature/processor/nii_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/artifact.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/rest/asset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/__int__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/asset/upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-04-14 09:08:09.000000 datature-1.0.0/datature/rest/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/datature/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-14 09:08:09.000000 datature-1.0.0/datature/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 09:08:20.000000 datature-1.0.0/datature.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-14 09:08:09.000000 datature-1.0.0/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 09:08:20.000000 datature-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-04-14 09:08:09.000000 datature-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/fixture/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/fixture/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/error_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/operation_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/data/upload_session_fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-14 09:08:09.000000 datature-1.0.0/test/fixture/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-14 09:08:09.000000 datature-1.0.0/test/http/test_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:20.000000 datature-1.0.0/test/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_asset_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-14 09:08:09.000000 datature-1.0.0/test/rest/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 09:08:09.000000 datature-1.0.0/test/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-14 09:08:09.000000 datature-1.0.0/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-04-26 10:54:17.000000 datature-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-26 10:54:17.000000 datature-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 10:54:28.000000 datature-1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-26 10:54:17.000000 datature-1.0.1/datature/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17392 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-04-26 10:54:17.000000 datature-1.0.1/datature/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-26 10:54:17.000000 datature-1.0.1/datature/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-26 10:54:17.000000 datature-1.0.1/datature/http/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-26 10:54:17.000000 datature-1.0.1/datature/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-26 10:54:17.000000 datature-1.0.1/datature/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/base_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/dicom_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-26 10:54:17.000000 datature-1.0.1/datature/processor/nii_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/artifact.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/rest/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/__int__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8823 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/asset/upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7066 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-04-26 10:54:17.000000 datature-1.0.1/datature/rest/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/datature/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-26 10:54:17.000000 datature-1.0.1/datature/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-26 10:54:28.000000 datature-1.0.1/datature.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 10:54:17.000000 datature-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-04-26 10:54:17.000000 datature-1.0.1/docs/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-26 10:54:17.000000 datature-1.0.1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 10:54:28.000000 datature-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 10:54:17.000000 datature-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/fixture/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/fixture/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/error_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/operation_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/data/upload_session_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-26 10:54:17.000000 datature-1.0.1/test/fixture/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-26 10:54:17.000000 datature-1.0.1/test/http/test_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:28.000000 datature-1.0.1/test/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6865 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_asset_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-26 10:54:17.000000 datature-1.0.1/test/rest/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-26 10:54:17.000000 datature-1.0.1/test/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-26 10:54:17.000000 datature-1.0.1/test/test_logger.py
```

### Comparing `datature-1.0.0/LICENSE` & `datature-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/PKG-INFO` & `datature-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 # Datatue Python SDK
 
 ## Get started
 
 - [Documentation](#documentation)
```

### Comparing `datature-1.0.0/datature/__init__.py` & `datature-1.0.1/datature/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   init module, include global configuration
 '''
 
 # Global Configuration
 API_BASE_URL = "https://api.datature.io/v1"
-SDK_VERSION = "1.0.0"
+SDK_VERSION = "1.0.1"
 
 # Constant environment
 OPERATION_LOOPING_TIMES = 20
 ASSET_UPLOAD_BATCH_SIZE = 5000
 SHOW_PROGRESS = False
 OPERATION_LOOPING_DELAY_SECONDS = 5
 HTTP_TIMEOUT_SECONDS = 120
```

### Comparing `datature-1.0.0/datature/cli/commands.py` & `datature-1.0.1/datature/cli/commands.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/cli/config.py` & `datature-1.0.1/datature/cli/config.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/cli/functions.py` & `datature-1.0.1/datature/cli/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,16 +197,15 @@
         print(messages.NO_ASSETS_FOUND_MESSAGE)
         sys.exit(1)
 
     nii_orientation = None
     if '.nii' in ",".join(str(file_path).lower() for file_path in file_paths):
         nii_orientation = inquirer.text(
             messages.ASSETS_NIFTI_DIRECTION_CHOICE_MESSAGE,
-            default="x",
-            validate=lambda _, x: x in ["x", "y", "z"],
+            validate=lambda _, x: x in ["", "x", "y", "z"],
         )
 
     if not groups:
         groups_res = inquirer.text(
             messages.ASSETS_GROUPS_MESSAGE,
             default="main",
             validate=lambda _, x: re.match("^[A-Za-z0-9,]*$", x),
@@ -240,15 +239,15 @@
                 title_length=12,
         ) as progress_bar:
             for file_path in batch:
                 upload_session.add(file_path, orientation=nii_orientation)
                 progress_bar()
 
         operation = upload_session.start(groups)
-        cli_loop_operation(operation.get("op_link"), len(batch))
+        cli_loop_operation(operation.get("op_link"), upload_session.size())
 
 
 def upload_annotations(path: Optional[Path] = None,
                        annotation_format: Optional[str] = None):
     """
     Upload annotations from path.
```

### Comparing `datature-1.0.0/datature/cli/main.py` & `datature-1.0.1/datature/cli/main.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/error.py` & `datature-1.0.1/datature/error.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/http/requester.py` & `datature-1.0.1/datature/http/requester.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,21 @@
         response = request(method,
                            absolute_url,
                            headers=headers,
                            data=post_data,
                            files=post_files,
                            timeout=datature.HTTP_TIMEOUT_SECONDS)
 
+        self._interpret_response(response)
+
         logger.log_info("API response:",
                         path=absolute_url,
                         response_code=response.status_code)
-        logger.log_debug("API response headers:", headers=headers)
         logger.log_debug("API response body:", body=response.json())
 
-        self._interpret_response(response)
-
         snake_case_response = self._snake_case_response(response)
 
         return snake_case_response
 
     def _make_headers(self, method, request_headers):
         """Make request headers
 
@@ -142,12 +141,12 @@
             if response_code == 429:
                 raise error.TooManyRequestsError(error_message, response_data)
 
             raise error.InternalServerError("Internal Server Error",
                                             response_data)
 
     def _snake_case_response(self, response: Response):
-        """Convert camelcase response to snake_case
+        """Convert CamelCase response to snake_case
 
         :param response: The request response
         """
         return humps.decamelize(response.json())
```

### Comparing `datature-1.0.0/datature/http/resource.py` & `datature-1.0.1/datature/http/resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/logger.py` & `datature-1.0.1/datature/logger.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/messages.py` & `datature-1.0.1/datature/messages.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 UNKNOWN_ERROR_SUPPORT_MESSAGE = "\nCommunication failed, contact support at support@datature.io."
 CONNECTION_ERROR_MESSAGE = "\nConnection failed, please check your network."
 UNKNOWN_ERROR_MESSAGE = "\nUnknown error occurred, contact support at support@datature.io."
 ANNOTATION_DOWNLOAD_MESSAGE = "Processing annotations for download."
 ACTIVE_PROJECT_MESSAGE = "Your active project is now"
 NO_ASSETS_FOUND_MESSAGE = "No allowable assets found in folders, please change the folder path."
 ASSETS_NIFTI_DIRECTION_CHOICE_MESSAGE = (
-    "Select axis of orientation, ['x','y','z']")
+    "Select the axis of orientation, if not provided, we will save videos for each axis. ['x','y','z']"
+)
```

### Comparing `datature-1.0.0/datature/processor/__init__.py` & `datature-1.0.1/datature/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/processor/base_processor.py` & `datature-1.0.1/datature/processor/base_processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 @Author  :   Raighne.Weng
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Base Processor module
 '''
 
+from typing import List
 from abc import ABC, abstractmethod
 
 
 class BaseProcessor(ABC):
     """Base processor class"""
 
     @abstractmethod
     def valid(self, request_data):
         """Valid the input file if a valid file"""
 
     @abstractmethod
-    def process(self, request_data):
+    def process(self, request_data) -> List[str]:
         """Function to process input file to assets"""
```

### Comparing `datature-1.0.0/datature/processor/dicom_processor.py` & `datature-1.0.1/datature/processor/dicom_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Dicom Processor
 '''
 
 import tempfile
+from typing import List
 from pathlib import Path
 from os import makedirs, path
 
 import cv2
 from pydicom import config, dcmread
 
 from datature import error
@@ -39,15 +40,15 @@
         :return: None.
         """
         file_path = request_data.get("file")
 
         if not file_path:
             raise error.BadRequestError("Required field")
 
-    def process(self, request_data):
+    def process(self, request_data) -> List[str]:
         """Start process file to asset video
 
         :param request_data: The request data, include file path.
         :return: str: The generate video path.
         """
         out_path = tempfile.mkdtemp()
         file_path = request_data.get("file")
@@ -57,29 +58,29 @@
         video_output = path.join(out_path, file_name)
 
         if not path.exists(video_output):
             makedirs(video_output)
 
         dicom_data = dcmread(file_path)
 
-        four_cc = cv2.VideoWriter_fourcc(*'avc1')
+        four_cc = cv2.VideoWriter_fourcc(*"mp4v")
 
         number_of_frames = int(dicom_data.get('NumberOfFrames', 1))
 
         # if only contain one image, convert to image.
         if number_of_frames == 1:
             cv2.imwrite(f"{video_output}/{file_name}.png",
                         dicom_data.pixel_array)
 
-            return f"{video_output}/{file_name}.png"
+            return [f"{video_output}/{file_name}.png"]
 
         video_writer = cv2.VideoWriter(f"{video_output}/{file_name}.mp4",
                                        four_cc, 30.0,
                                        (dicom_data.Rows, dicom_data.Columns))
 
         for _, image in enumerate(dicom_data.pixel_array):
             new_image = cv2.cvtColor(image, cv2.COLOR_GRAY2RGB)
             video_writer.write(new_image)
 
         video_writer.release()
 
-        return f"{video_output}/{file_name}.mp4"
+        return [f"{video_output}/{file_name}.mp4"]
```

### Comparing `datature-1.0.0/datature/processor/nii_processor.py` & `datature-1.0.1/datature/processor/nii_processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,17 @@
 @Version :   0.7.3
 @Contact :   raighne@datature.io
 @License :   Apache License 2.0
 @Desc    :   Nii Processor
 '''
 
 import tempfile
-from os import makedirs, path
+from typing import List
 from pathlib import Path
+from os import makedirs, path
 
 import cv2
 import numpy as np
 import nibabel as nib
 from datature import error
 from datature.processor.base_processor import BaseProcessor
 
@@ -32,60 +33,75 @@
     def valid(self, request_data):
         """Valid the input
 
         :param request_data: The request data, include file path.
         :return: None.
         """
         file_path = request_data.get("file")
-        options = request_data.get("options")
 
         if not file_path:
             raise error.BadRequestError(
                 "Required field, must include file path")
 
-        if not options.get("orientation") or options.get(
-                "orientation") not in ["x", "y", "z"]:
-            raise error.BadRequestError(
-                "NIfTI file must have an orientation of choice: [x, y, z]")
-
-    def process(self, request_data):
+    def process(self, request_data) -> List[str]:
         """Start process file to asset video
 
         :param request_data: The request data, include file path.
         :return: str: The generate video path.
         """
         out_path = tempfile.mkdtemp()
 
         file_path = request_data.get("file")
-        direction = request_data.get("options").get("direction")
+        orientation = request_data.get("options").get("orientation")
 
         file_name = Path(file_path).stem
 
         video_output = path.join(out_path, file_name)
 
         if not path.exists(video_output):
             makedirs(video_output)
 
         scan = nib.load(file_path)
 
         # Read data and get scan's shape
         scan_array = scan.get_fdata()
-        scan_array_shape = scan_array.shape
 
-        four_cc = cv2.VideoWriter_fourcc(*'avc1')
-        video_writer = cv2.VideoWriter(f"{video_output}/{file_name}.mp4",
-                                       four_cc, 30.0, (1024, 1024))
+        # if client provide the orientation
+        if orientation and orientation in ["x", "y", "z"]:
+            output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
+
+            self.__write_video(scan_array, orientation, output_file_path)
+
+            return [output_file_path]
+
+        # if not then save all orientations
+        output_file_paths = []
+        for orientation in ["x", "y", "z"]:
+            output_file_path = f"{video_output}/{file_name}-{orientation}.mp4"
+
+            self.__write_video(scan_array, orientation, output_file_path)
 
-        axis = 0 if direction == 'x' else 1 if direction == 'y' else 2
+            output_file_paths.append(output_file_path)
 
-        for i in range(scan_array_shape[axis]):
+        return output_file_paths
+
+    def __write_video(self, scan_array, orientation, saved_path):
+        """Write video to file
+
+        :param scan_array: The NIfTI scan array data.
+        :param axis: The orientation of the pics.
+        :param saved_path: The saved file path.
+        """
+        four_cc = cv2.VideoWriter_fourcc(*"mp4v")
+        video_writer = cv2.VideoWriter(saved_path, four_cc, 30.0, (1024, 1024))
+
+        axis = {'x': 0, 'y': 1, 'z': 2}[orientation]
+
+        for i in range(scan_array.shape[axis]):
             # Get slice along the correct axis and resize
             slice_axis = scan_array.take(i, axis=axis)
             image = cv2.resize(slice_axis, (1024, 1024))
 
             # Convert to RGB and write to video file
             new_image = cv2.cvtColor(np.uint8(image), cv2.COLOR_GRAY2RGB)
             video_writer.write(new_image)
-
         video_writer.release()
-
-        return f"{video_output}/{file_name}.mp4"
```

### Comparing `datature-1.0.0/datature/rest/__init__.py` & `datature-1.0.1/datature/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature/rest/asset/upload_session.py` & `datature-1.0.1/datature/rest/asset/upload_session.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,98 +50,21 @@
         """Add asset to upload."""
         if len(self.assets) >= datature.ASSET_UPLOAD_BATCH_SIZE:
             raise error.Error("One upload session allow max 5000 assets.")
 
         if not path.exists(file_path):
             raise error.Error("Cannot find the Asset file")
 
-        # Prepare filename size and mime type
-        filename = path.basename(file_path)
-
         # Convert DICOM and NII file to video asset
-        if file_path.lower().endswith(('.dcm', '.nii')):
-            processor = get_processor(file_path)
-
-            process_data = {"file": file_path, "options": kwargs}
-            processor.valid(process_data)
-            resp = processor.process(process_data)
-
-            if resp:
-                # change the converted file_path and filename
-                file_path = resp
-                filename = Path(file_path).stem
-
-        with open(file_path, 'rb') as file:
-            contents = file.read()
-
-            # calculate file crc32
-            file_hash = google_crc32c.Checksum()
-            file_hash.update(contents)
+        processed_files = self.__process_medical_file(file_path, kwargs)
 
-            # To fix the wrong crc32 caused by mac M1 clip
-            crc32 = struct.unpack(">l", file_hash.digest())[0]
-
-            size = path.getsize(file_path)
-
-            mime_kind = filetype.guess(file_path)
-
-            file.close()
-
-            if self.file_name_map.get(filename) is not None:
-                raise error.Error(
-                    f"Cannot add multiple files with the same name, {filename}"
-                )
-
-            if (filename and size and crc32 and mime_kind):
-                if mime_kind.mime in ["image/jpeg", "image/png"]:
-                    asset_metadata = {
-                        "filename": filename,
-                        "size": size,
-                        "crc32c": crc32,
-                        "mime": mime_kind.mime
-                    }
-                elif mime_kind.mime == "video/mp4":
-                    cap = cv2.VideoCapture(file_path)
-                    frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-                    four_c_c = int(cap.get(cv2.CAP_PROP_FOURCC))
-                    codec = chr(four_c_c
-                                & 0xff) + chr((four_c_c >> 8) & 0xff) + chr(
-                                    (four_c_c >> 16)
-                                    & 0xff) + chr((four_c_c >> 24) & 0xff)
-                    if not codec.startswith('avc1'):
-                        raise error.Error("UnSupported asset file")
-
-                    asset_metadata = {
-                        "filename": filename,
-                        "size": size,
-                        "crc32c": crc32,
-                        "mime": mime_kind.mime,
-                        "frames": frames,
-                        "encoder": {
-                            "profile": "h264Saver",
-                            "everyNthFrame": 1
-                        },
-                    }
-                else:
-                    raise error.Error("UnSupported asset file")
-
-                self.assets.append(asset_metadata)
-                self.file_name_map[filename] = {"path": file_path}
-
-                if custom_metadata is not None:
-                    if len(json.dumps(custom_metadata)) > self.metadata_limit:
-                        raise error.Error(
-                            f"Your tier only allow upload {self.metadata_limit} bytes metadata."
-                        )
-
-                    self.custom_metadata_map[filename] = custom_metadata
-
-                logger.log_info("Add asset:", metadata=asset_metadata)
-            else:
-                raise error.Error("UnSupported asset file")
+        for processed_file in processed_files:
+            self.__generate_metadata(processed_file.get("filename"),
+                                     processed_file.get("file_path"),
+                                     custom_metadata)
 
     def start(self, groups: [str] = None, background: bool = False) -> dict:
         """Request server to get signed ur and upload file to gcp."""
 
         # Set default groups
         if groups is None:
             groups = ["main"]
@@ -192,23 +115,23 @@
         for asset_upload in response["assets"]:
             file_name = asset_upload["metadata"]["filename"]
             file_path = self.file_name_map.get(file_name)["path"]
 
             with open(file_path, 'rb') as file:
                 contents = file.read()
 
-                logger.log_info("Start Uploading" + file_path)
+                logger.log_info("Start Uploading:" + file_path)
 
                 # upload asset to GCP one by one
                 request("PUT",
                         asset_upload["upload"]["url"],
                         headers=asset_upload["upload"]["headers"],
                         data=contents,
                         timeout=10)
-                logger.log_info("Done Uploading" + file_path)
+                logger.log_info("Done Uploading:" + file_path)
 
         if background:
             return {"op_link": op_link}
 
         # Wait server finish generate thumbnail
         Operation.loop_retrieve(op_link)
 
@@ -216,7 +139,105 @@
         for filename in self.custom_metadata_map:
             datature.Asset.modify(filename, {
                 "custom_metadata":
                 self.custom_metadata_map.get(filename, {})
             })
 
         return {"op_link": op_link}
+
+    def size(self) -> int:
+        """Get upload session size."""
+        return len(self.assets)
+
+    def __process_medical_file(self, file_path: str, options: dict = None):
+        """Pre process the file, if medical file convert to MP4 first."""
+        # Convert DICOM and NII file to video asset
+        if file_path.lower().endswith(('.dcm', '.nii')):
+            processor = get_processor(file_path)
+
+            process_data = {"file": file_path, "options": options}
+            processor.valid(process_data)
+            resp = processor.process(process_data)
+
+            if resp:
+                # change the converted file_path and filename
+                return [{
+                    "filename": Path(file_path).stem,
+                    "file_path": file_path
+                } for file_path in resp]
+
+        return [{"filename": path.basename(file_path), "file_path": file_path}]
+
+    def __generate_metadata(self,
+                            filename: str,
+                            file_path: str,
+                            custom_metadata: dict = None):
+        """process the file to asset metadata."""
+        with open(file_path, 'rb') as file:
+            contents = file.read()
+
+            # calculate file crc32
+            file_hash = google_crc32c.Checksum()
+            file_hash.update(contents)
+
+            # To fix the wrong crc32 caused by mac M1 clip
+            crc32 = struct.unpack(">l", file_hash.digest())[0]
+
+            size = path.getsize(file_path)
+
+            mime_kind = filetype.guess(file_path)
+
+            file.close()
+
+            if self.file_name_map.get(filename) is not None:
+                raise error.Error(
+                    f"Cannot add multiple files with the same name, {filename}"
+                )
+
+            if (filename and size and crc32 and mime_kind):
+                if mime_kind.mime in ["image/jpeg", "image/png"]:
+                    asset_metadata = {
+                        "filename": filename,
+                        "size": size,
+                        "crc32c": crc32,
+                        "mime": mime_kind.mime
+                    }
+                elif mime_kind.mime == "video/mp4":
+                    cap = cv2.VideoCapture(file_path)
+                    frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+                    four_c_c = int(cap.get(cv2.CAP_PROP_FOURCC))
+                    codec = chr(four_c_c
+                                & 0xff) + chr((four_c_c >> 8) & 0xff) + chr(
+                                    (four_c_c >> 16)
+                                    & 0xff) + chr((four_c_c >> 24) & 0xff)
+                    if not (codec.startswith('avc1')
+                            or codec.startswith('mp4v')):
+                        raise error.Error("UnSupported asset file")
+
+                    asset_metadata = {
+                        "filename": filename,
+                        "size": size,
+                        "crc32c": crc32,
+                        "mime": mime_kind.mime,
+                        "frames": frames,
+                        "encoder": {
+                            "profile": "h264Saver",
+                            "everyNthFrame": 1
+                        },
+                    }
+                else:
+                    raise error.Error("UnSupported asset file")
+
+                self.assets.append(asset_metadata)
+                self.file_name_map[filename] = {"path": file_path}
+
+                if custom_metadata is not None:
+                    if len(json.dumps(custom_metadata)) > self.metadata_limit:
+                        raise error.Error(
+                            f"Your tier only allow upload {self.metadata_limit} bytes metadata."
+                        )
+
+                    self.custom_metadata_map[filename] = custom_metadata
+
+                logger.log_info("Add asset:", metadata=asset_metadata)
+            else:
+                raise error.Error("UnSupported asset file")
```

### Comparing `datature-1.0.0/datature/utils/utils.py` & `datature-1.0.1/datature/utils/utils.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/datature.egg-info/PKG-INFO` & `datature-1.0.1/datature.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: datature
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python bindings for the Datature API
 Author: Raighne Weng
 Author-email: raighne@datature.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: docs
 License-File: LICENSE
 
 # Datatue Python SDK
 
 ## Get started
 
 - [Documentation](#documentation)
```

### Comparing `datature-1.0.0/datature.egg-info/SOURCES.txt` & `datature-1.0.1/datature.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 datature/rest/types.py
 datature/rest/workflow.py
 datature/rest/asset/__int__.py
 datature/rest/asset/asset.py
 datature/rest/asset/upload_session.py
 datature/utils/__init__.py
 datature/utils/utils.py
+docs/upload.py
+docs/source/conf.py
 test/__init__.py
 test/test_error.py
 test/test_logger.py
 test/fixture/__init__.py
 test/fixture/mock.py
 test/fixture/data/__init__.py
 test/fixture/data/error_fixture.py
```

### Comparing `datature-1.0.0/readme.md` & `datature-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/setup.py` & `datature-1.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,11 +41,14 @@
         "filetype", "opencv-python", "alive-progress", "pydicom", "nibabel",
         "pillow"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License"
     ],
+    extras_require={
+        'docs': ["sphinx", "sphinx-rtd-theme", "sphinx_markdown_builder"]
+    },
     entry_points={
         'console_scripts': ['datature=datature.cli.main:main'],
     },
 )
```

### Comparing `datature-1.0.0/test/fixture/data/error_fixture.py` & `datature-1.0.1/test/fixture/data/error_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/fixture/data/operation_fixture.py` & `datature-1.0.1/test/fixture/data/operation_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/fixture/data/upload_session_fixture.py` & `datature-1.0.1/test/fixture/data/upload_session_fixture.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/fixture/mock.py` & `datature-1.0.1/test/fixture/mock.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/http/test_requester.py` & `datature-1.0.1/test/http/test_requester.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/http/test_resource.py` & `datature-1.0.1/test/http/test_resource.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_annotation.py` & `datature-1.0.1/test/rest/test_annotation.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_artifact.py` & `datature-1.0.1/test/rest/test_artifact.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_asset.py` & `datature-1.0.1/test/rest/test_asset.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_asset_upload_session.py` & `datature-1.0.1/test/rest/test_asset_upload_session.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_deploy.py` & `datature-1.0.1/test/rest/test_deploy.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_operation.py` & `datature-1.0.1/test/rest/test_operation.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_project.py` & `datature-1.0.1/test/rest/test_project.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_run.py` & `datature-1.0.1/test/rest/test_run.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_tag.py` & `datature-1.0.1/test/rest/test_tag.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/rest/test_workflow.py` & `datature-1.0.1/test/rest/test_workflow.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/test_error.py` & `datature-1.0.1/test/test_error.py`

 * *Files identical despite different names*

### Comparing `datature-1.0.0/test/test_logger.py` & `datature-1.0.1/test/test_logger.py`

 * *Files identical despite different names*

