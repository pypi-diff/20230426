# Comparing `tmp/gitflow-api-0.3.8.tar.gz` & `tmp/gitflow-api-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gitflow-api-0.3.8.tar", last modified: Wed Jul  1 14:01:35 2020, max compression
+gzip compressed data, was "dist/gitflow-api-0.3.9.tar", last modified: Wed Aug 12 18:14:21 2020, max compression
```

## Comparing `gitflow-api-0.3.8.tar` & `gitflow-api-0.3.9.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1005 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/PKG-INFO
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     3593 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/README.md
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)       25 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/__init__.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/api/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      465 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/api.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      835 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/api_merge_request.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      682 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/api_strategy.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      460 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/gitlab_manager.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     5633 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/merge_request.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1028 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/project.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/communicator/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/communicator/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      661 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/communicator/communicator.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      761 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/communicator/communicator_strategy.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2382 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/communicator/slack.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/config/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/config/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     4190 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/config/config.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      590 2020-05-08 13:36:44.000000 gitflow-api-0.3.8/gitflow_api/config/properties.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api/deploy/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/deploy/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      233 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/deploy/deploy.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      878 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/deploy/deploy_strategy.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      366 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/deploy/maven.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      651 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/deploy/pypi.py
--rwxr-xr-x   0 mauyr     (1000) mauyr     (1000)     2691 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/gitflow.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/gitflow_api/project/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1163 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/angular_project.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     4439 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/maven_project.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1058 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/project_manager.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)      656 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/project_manager_strategy.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2114 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/project/python_project.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/gitflow_api/services/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/services/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)    11024 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/services/changelog.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1799 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/services/feature.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1857 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/services/hotfix.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)    14767 2020-05-08 14:03:46.000000 gitflow-api-0.3.8/gitflow_api/services/release.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/gitflow_api/utilities/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/utilities/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     4314 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/gitflow_api/utilities/git_helper.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     3710 2020-05-08 14:07:53.000000 gitflow-api-0.3.8/gitflow_api/utilities/version_utils.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.991786 gitflow-api-0.3.8/gitflow_api.egg-info/
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1005 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/PKG-INFO
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1827 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/SOURCES.txt
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)        1 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/dependency_links.txt
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       54 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/entry_points.txt
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       58 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/requires.txt
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       18 2020-07-01 14:01:35.000000 gitflow-api-0.3.8/gitflow_api.egg-info/top_level.txt
--rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       38 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/setup.cfg
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1783 2020-07-01 13:54:45.000000 gitflow-api-0.3.8/setup.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/tests/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/__init__.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/tests/deploy/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/deploy/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1023 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/deploy/test_deploy.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/tests/project/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/project/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1074 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/project/test_angular_project.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2116 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/project/test_python_project.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/tests/services/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/services/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1952 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/services/test_communicator.py
-drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-07-01 14:01:35.995786 gitflow-api-0.3.8/tests/utilities/
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/utilities/__init__.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1832 2020-05-08 13:30:08.000000 gitflow-api-0.3.8/tests/utilities/test_git_helper.py
--rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1590 2020-05-08 14:07:23.000000 gitflow-api-0.3.8/tests/utilities/test_version_utils.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.851721 gitflow-api-0.3.9/
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1005 2020-08-12 18:14:21.851721 gitflow-api-0.3.9/PKG-INFO
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     3593 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/README.md
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.839721 gitflow-api-0.3.9/gitflow_api/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)       25 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/__init__.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.839721 gitflow-api-0.3.9/gitflow_api/api/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      465 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/api.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      835 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/api_merge_request.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      682 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/api_strategy.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.839721 gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      460 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/gitlab_manager.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     5633 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/merge_request.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1028 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/project.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.843721 gitflow-api-0.3.9/gitflow_api/communicator/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/communicator/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      661 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/communicator/communicator.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      761 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/communicator/communicator_strategy.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2382 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/communicator/slack.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.843721 gitflow-api-0.3.9/gitflow_api/config/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/config/__init__.py
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     4351 2020-08-12 13:58:17.000000 gitflow-api-0.3.9/gitflow_api/config/config.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      590 2020-05-08 13:36:44.000000 gitflow-api-0.3.9/gitflow_api/config/properties.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.843721 gitflow-api-0.3.9/gitflow_api/deploy/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/deploy/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      233 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/deploy/deploy.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      878 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/deploy/deploy_strategy.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      366 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/deploy/maven.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      639 2020-08-12 18:14:16.000000 gitflow-api-0.3.9/gitflow_api/deploy/pypi.py
+-rwxr-xr-x   0 mauyr     (1000) mauyr     (1000)     2691 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/gitflow.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/gitflow_api/project/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1163 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/angular_project.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     4439 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/maven_project.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1058 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/project_manager.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)      656 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/project_manager_strategy.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2114 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/project/python_project.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/gitflow_api/services/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/services/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)    11024 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/services/changelog.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1799 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/services/feature.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1857 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/services/hotfix.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)    14767 2020-05-08 14:03:46.000000 gitflow-api-0.3.9/gitflow_api/services/release.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/gitflow_api/utilities/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/utilities/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     4314 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/gitflow_api/utilities/git_helper.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     3710 2020-05-08 14:07:53.000000 gitflow-api-0.3.9/gitflow_api/utilities/version_utils.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.839721 gitflow-api-0.3.9/gitflow_api.egg-info/
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1005 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/PKG-INFO
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)     1827 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)        1 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       54 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/entry_points.txt
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       58 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/requires.txt
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       18 2020-08-12 18:14:21.000000 gitflow-api-0.3.9/gitflow_api.egg-info/top_level.txt
+-rw-rw-r--   0 mauyr     (1000) mauyr     (1000)       38 2020-08-12 18:14:21.851721 gitflow-api-0.3.9/setup.cfg
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1783 2020-08-12 14:01:36.000000 gitflow-api-0.3.9/setup.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/tests/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/__init__.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/tests/deploy/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/deploy/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1023 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/deploy/test_deploy.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/tests/project/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/project/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1074 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/project/test_angular_project.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     2116 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/project/test_python_project.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.847721 gitflow-api-0.3.9/tests/services/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/services/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1952 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/services/test_communicator.py
+drwxrwxr-x   0 mauyr     (1000) mauyr     (1000)        0 2020-08-12 18:14:21.851721 gitflow-api-0.3.9/tests/utilities/
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)        0 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/utilities/__init__.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1832 2020-05-08 13:30:08.000000 gitflow-api-0.3.9/tests/utilities/test_git_helper.py
+-rw-r--r--   0 mauyr     (1000) mauyr     (1000)     1590 2020-05-08 14:07:23.000000 gitflow-api-0.3.9/tests/utilities/test_version_utils.py
```

### Comparing `gitflow-api-0.3.8/PKG-INFO` & `gitflow-api-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gitflow-api
-Version: 0.3.8
+Version: 0.3.9
 Summary: Gitflow-API library using a API as backend
 Home-page: https://github.com/mauyr/gitflow-api
 Author: Mauyr Alexandre Pereira
 Author-email: mauyr.pereira@inovapro.com.br
 License: GNU GPLv3
 Description: Gitflow-API is a python library used use a gitflow_methodology on development using a API like Gitlab or Github to execute most of process
 Platform: UNKNOWN
```

### Comparing `gitflow-api-0.3.8/README.md` & `gitflow-api-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/api/api_merge_request.py` & `gitflow-api-0.3.9/gitflow_api/api/api_merge_request.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/api/api_strategy.py` & `gitflow-api-0.3.9/gitflow_api/api/api_strategy.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/merge_request.py` & `gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/merge_request.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/api/gitlab_manager/project.py` & `gitflow-api-0.3.9/gitflow_api/api/gitlab_manager/project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/communicator/communicator.py` & `gitflow-api-0.3.9/gitflow_api/communicator/communicator.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/communicator/communicator_strategy.py` & `gitflow-api-0.3.9/gitflow_api/communicator/communicator_strategy.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/communicator/slack.py` & `gitflow-api-0.3.9/gitflow_api/communicator/slack.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/config/config.py` & `gitflow-api-0.3.9/gitflow_api/config/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 import configparser
+import json
 import os
 
 from gitflow_api.config.properties import *
 
 
 class Config:
     # Branches structure
@@ -97,10 +98,13 @@
             try:
                 return os.environ[os_environment]
             except Exception as ex:
                 return default_value
 
     def _get_property(self, group, config_property, default_property):
         try:
-            return self.config_file[group][config_property]
+            if isinstance(default_property, list):
+                return json.loads(self.config_file[group][config_property])
+            else:
+                return self.config_file[group][config_property]
         except Exception as e:
             return default_property
```

### Comparing `gitflow-api-0.3.8/gitflow_api/config/properties.py` & `gitflow-api-0.3.9/gitflow_api/config/properties.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/deploy/deploy_strategy.py` & `gitflow-api-0.3.9/gitflow_api/deploy/deploy_strategy.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/deploy/pypi.py` & `gitflow-api-0.3.9/gitflow_api/deploy/pypi.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,12 +16,12 @@
         # remove dist and build files
         try:
             shutil.rmtree('dist')
             shutil.rmtree('build')
         except FileNotFoundError:
             print('Skipping deleting folder')
 
-        cmd = 'python3 setup.py sdist bdist_wheel'
+        cmd = 'python3 setup.py sdist'
         check_call(cmd, shell=True)
 
         cmd = 'twine upload dist/*'
         check_call(cmd, shell=True)
```

### Comparing `gitflow-api-0.3.8/gitflow_api/gitflow.py` & `gitflow-api-0.3.9/gitflow_api/gitflow.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/project/angular_project.py` & `gitflow-api-0.3.9/gitflow_api/project/angular_project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/project/maven_project.py` & `gitflow-api-0.3.9/gitflow_api/project/maven_project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/project/project_manager.py` & `gitflow-api-0.3.9/gitflow_api/project/project_manager.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/project/project_manager_strategy.py` & `gitflow-api-0.3.9/gitflow_api/project/project_manager_strategy.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/project/python_project.py` & `gitflow-api-0.3.9/gitflow_api/project/python_project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/services/changelog.py` & `gitflow-api-0.3.9/gitflow_api/services/changelog.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/services/feature.py` & `gitflow-api-0.3.9/gitflow_api/services/feature.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/services/hotfix.py` & `gitflow-api-0.3.9/gitflow_api/services/hotfix.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/services/release.py` & `gitflow-api-0.3.9/gitflow_api/services/release.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/utilities/git_helper.py` & `gitflow-api-0.3.9/gitflow_api/utilities/git_helper.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api/utilities/version_utils.py` & `gitflow-api-0.3.9/gitflow_api/utilities/version_utils.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/gitflow_api.egg-info/PKG-INFO` & `gitflow-api-0.3.9/gitflow_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: gitflow-api
-Version: 0.3.8
+Version: 0.3.9
 Summary: Gitflow-API library using a API as backend
 Home-page: https://github.com/mauyr/gitflow-api
 Author: Mauyr Alexandre Pereira
 Author-email: mauyr.pereira@inovapro.com.br
 License: GNU GPLv3
 Description: Gitflow-API is a python library used use a gitflow_methodology on development using a API like Gitlab or Github to execute most of process
 Platform: UNKNOWN
```

### Comparing `gitflow-api-0.3.8/gitflow_api.egg-info/SOURCES.txt` & `gitflow-api-0.3.9/gitflow_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/setup.py` & `gitflow-api-0.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 install_requires = ['GitPython>=2.1.11','python-gitlab>=1.6.0','slackclient>=1.3.0']
 test_requires = []
 # end
 
 setup(
     name="gitflow-api",
-    version="0.3.8",
+    version="0.3.9",
     description="Gitflow-API library using a API as backend",
     author="Mauyr Alexandre Pereira",
     author_email="mauyr.pereira@inovapro.com.br",
     url="https://github.com/mauyr/gitflow-api",
     packages=find_packages('.'),
     entry_points = {
         'console_scripts': ['gitflow=gitflow_api.gitflow:main'],
```

### Comparing `gitflow-api-0.3.8/tests/deploy/test_deploy.py` & `gitflow-api-0.3.9/tests/deploy/test_deploy.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/tests/project/test_angular_project.py` & `gitflow-api-0.3.9/tests/project/test_angular_project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/tests/project/test_python_project.py` & `gitflow-api-0.3.9/tests/project/test_python_project.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/tests/services/test_communicator.py` & `gitflow-api-0.3.9/tests/services/test_communicator.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/tests/utilities/test_git_helper.py` & `gitflow-api-0.3.9/tests/utilities/test_git_helper.py`

 * *Files identical despite different names*

### Comparing `gitflow-api-0.3.8/tests/utilities/test_version_utils.py` & `gitflow-api-0.3.9/tests/utilities/test_version_utils.py`

 * *Files identical despite different names*

