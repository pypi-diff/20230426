# Comparing `tmp/robotmk-0.0.54.tar.gz` & `tmp/robotmk-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.54.tar", last modified: Fri Apr 14 12:44:34 2023, max compression
+gzip compressed data, was "robotmk-0.0.56.tar", last modified: Tue Apr 25 14:31:26 2023, max compression
```

## Comparing `robotmk-0.0.54.tar` & `robotmk-0.0.56.tar`

### file list

```diff
@@ -1,74 +1,58 @@
--rw-r--r--   0        0        0      110 2023-04-14 12:44:31.988345 robotmk-0.0.54/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.54/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.54/README.md
--rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.54/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-28 07:41:38.789867 robotmk-0.0.54/src/_confitree/__init__.py
--rw-r--r--   0        0        0     5092 2023-03-02 13:49:11.086894 robotmk-0.0.54/src/_confitree/confitree.py
--rw-r--r--   0        0        0      512 2023-03-04 11:44:09.697687 robotmk-0.0.54/src/_confitree/robotmk.yml
--rwxr-xr-x   0        0        0      635 2023-02-24 13:10:55.692823 robotmk-0.0.54/src/_robotmk/__init__.py
--rwxr-xr-x   0        0        0      533 2023-02-24 13:10:55.692823 robotmk-0.0.54/src/_robotmk/__main__.py
--rwxr-xr-x   0        0        0     2249 2023-03-03 09:34:49.997849 robotmk-0.0.54/src/_robotmk/cli.py
--rwxr-xr-x   0        0        0      754 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/__init__.py
--rwxr-xr-x   0        0        0    11155 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/agent.py
--rwxr-xr-x   0        0        0     1152 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/agent/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/output/__init__.py
--rwxr-xr-x   0        0        0      100 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/output/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robot/__init__.py
--rwxr-xr-x   0        0        0       99 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robot/cli.py
--rwxr-xr-x   0        0        0      308 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/robotmk.py
--rwxr-xr-x   0        0        0        0 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/specialagent/__init__.py
--rwxr-xr-x   0        0        0      106 2023-02-24 13:10:55.696823 robotmk-0.0.54/src/_robotmk/modes/specialagent/cli.py
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.54/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.54/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-14 12:44:31.988345 robotmk-0.0.54/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5514 2023-03-30 06:57:58.218217 robotmk-0.0.54/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.54/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.54/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.54/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.54/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.54/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.54/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.54/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.54/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.54/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.54/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.54/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.54/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.54/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.54/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.54/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1899 2023-03-29 11:50:21.439532 robotmk-0.0.54/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.54/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.54/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.54/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     6793 2023-04-14 12:43:34.356917 robotmk-0.0.54/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4506 2023-04-14 10:30:06.489439 robotmk-0.0.54/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.54/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     4732 2023-04-14 11:14:59.168198 robotmk-0.0.54/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.54/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5635 2023-04-14 12:31:44.104026 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6474 2023-04-14 11:50:43.784189 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4818 2023-04-14 11:43:33.303934 robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2793 2023-04-14 11:13:48.468830 robotmk-0.0.54/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.54/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.54/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.54/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.54/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.54/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2027 2023-04-04 10:56:24.192653 robotmk-0.0.54/src/robotmk/logger.py
--rw-r--r--   0        0        0     3643 2023-04-14 10:22:44.709931 robotmk-0.0.54/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.54/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.54/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.54/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.54/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.54/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.54/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.54/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.54/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.54/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.54/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.54/tests/context/test_cli.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.54/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.54/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-25 14:30:31.577495 robotmk-0.0.56/.bumpversion.cfg
+-rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.56/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.56/README.md
+-rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.56/pyproject.toml
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.56/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.56/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-25 14:30:31.577495 robotmk-0.0.56/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5528 2023-04-25 08:43:45.469873 robotmk-0.0.56/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.56/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.56/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.56/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.56/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.56/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.56/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.56/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.56/src/robotmk/context/local/__init__.py
+-rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.56/src/robotmk/context/local/cli.py
+-rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.56/src/robotmk/context/local/local.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.56/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.56/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.56/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.56/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.56/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.56/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.56/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.56/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.56/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     7380 2023-04-25 13:50:39.300240 robotmk-0.0.56/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     4366 2023-04-14 13:05:12.951814 robotmk-0.0.56/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.56/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     5446 2023-04-25 13:50:20.160423 robotmk-0.0.56/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.56/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6558 2023-04-25 13:56:25.732927 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4878 2023-04-25 14:28:49.598467 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     2980 2023-04-25 13:50:11.588505 robotmk-0.0.56/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.56/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.56/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.56/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.56/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.56/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.56/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.56/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.56/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.56/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.56/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.56/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.56/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.56/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.56/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.56/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.56/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.56/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.56/tests/context/test_cli.py
+-rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.56/tests/test_robotmk.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.56/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.56/PKG-INFO
```

### Comparing `robotmk-0.0.54/pyproject.toml` & `robotmk-0.0.56/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/categories.json` & `robotmk-0.0.56/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/click_tutorial.py` & `robotmk-0.0.56/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/cli/cli.py` & `robotmk-0.0.56/src/robotmk/cli/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # # LOCAL CONTEXT
 # robotmk                                                                        # no arg = print output
 
 # robotmk     local                                              output          # print output
 # robotmk     local    --yml /etc/checkmk/another_robotmk.yml    output          # print output with yml
 # robotmk     local    --vars /var/robotmk_local.env             output          # print output, load env from file (instead of env)
 
-# robotmk     local    scheduler                                                 # start scheduler
+# robotmk     local                                              scheduler       # start scheduler
 # robotmk     local    --yml /etc/checkmk/another_robotmk.yml    scheduler       # start scheduler with yml
 # robotmk     local    --vars /var/robotmk_local.env             scheduler       # start scheduler, load env from file  (instead of env)
 # ---------------------------------------------------------------------------------------------
 # # SUITE CONTEXT
 # robotmk                                                                        # no arg = exec suite as configured in env
 # robotmk     suite    --vars /var/rmk/foosuiteA_8bb36c3.env                     # exec suite with env from file and suite = yml -> common: suite)
 # robotmk     suite    --vars /var/rmk/foosuiteA_8bb36c3.env     bazsuite        # exec suite with env from file and suite = bazsuite
@@ -83,19 +83,21 @@
     type=click.Choice(LOG_LEVELS),
 )
 @click.pass_context
 def main(ctx, loglevel):
     if ctx.invoked_subcommand is None:
         # robotmk was called without argument. Try to detect the context from the default
         # config and/or environment variables.
-        # After that run the default command of the context:
-        # - output() for local context
-        # - specialagent() for specialagent context (output + sequencer)
-        # - run() for suite context
-        ctx.robotmk = Robotmk(contextname=None, log_level=loglevel, yml=None, vars=None)
+        # After that run the default subcommand of the context:
+        # - local: produce output
+        # - specialagent: produce output + call sequencer
+        # - suite: run a single suite
+        ctx.robotmk = Robotmk(
+            contextname=None, log_level=loglevel, ymlfile=None, varfile=None
+        )
         ctx.robotmk.run_default()
     else:
         # Robotmk was executed with a context subcommand, whose logic is defined within the context.
         pass
 
 
 @main.command()
```

### Comparing `robotmk-0.0.54/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.56/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/config/config.py` & `robotmk-0.0.56/src/robotmk/config/config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/config/yml.py` & `robotmk-0.0.56/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/abstract.py` & `robotmk-0.0.56/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/context.py` & `robotmk-0.0.56/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/local/cli.py` & `robotmk-0.0.56/src/robotmk/context/local/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/local/local.py` & `robotmk-0.0.56/src/robotmk/context/local/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.56/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.56/src/robotmk/context/specialagent/specialagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
         if not self._logger:
             self._logger = RobotmkLogger(
                 Path(self.config.common.logdir).joinpath("robotmk.log"),
                 self.config.common.log_level,
             )
         return self._logger
 
-    def load_config(self, defaults, ymlfile: str, varfile: str) -> None:
+    def load_config(self, defaults, **kwargs) -> None:
         """Load the config for specialagent context.
 
         This context can merge the config from
         - OS defaults
         - + var file (= --vars)
         - + environment variables
 
         (There is no YML file for specialagent context!)
         """
         self.config.set_defaults(defaults)
-        self.config.read_cfg_vars(path=varfile)
+        self.config.read_cfg_vars(path=kwargs.get("path"))
         # TODO: validate later so that config can be dumped
         # self.config.validate(self.ymlschema)
 
     def refresh_config(self) -> bool:
         """Re-loads the config and returns True if it changed"""
         # TODO: implement this
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/cli.py` & `robotmk-0.0.56/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.56/src/robotmk/context/suite/strategies/run.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 from abc import ABC, abstractmethod
 import platform
 from robotmk.logger import RobotmkLogger
 import subprocess
 import os
+from dataclasses import dataclass, field, asdict
+from typing import List
+
+# TODO: split this into modules
+# TODO:
+
+
+@dataclass
+class Result:
+    """Result of a subprocess execution."""
+
+    args: List[str] = field(default_factory=list)
+    returncode: int = 0
+    stdout: List[str] = field(default_factory=list)
+    stderr: List[str] = field(default_factory=list)
 
 
 class RunStrategy(ABC):
     def __init__(self, target) -> None:
         self.target = target
 
         # self.suiteuname = suiteuname
@@ -19,172 +34,172 @@
         # self.critical = self._logger.critical
 
     def run(self, *args, **kwargs):
         """Template method which bundles the linked methods to run.
 
         The concrete strategy selectivly overrides the methods to implement."""
         rc = max(
-            self.prepare(*args, **kwargs),
-            self.execute(*args, **kwargs),
-            self.cleanup(*args, **kwargs),
+            self.exec_pre(*args, **kwargs),
+            self.exec_main(*args, **kwargs),
+            self.exec_post(*args, **kwargs),
         )
         return rc
 
     @abstractmethod
-    def prepare(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
         """Prepares the given suite."""
         pass
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> int:
+    def exec_main(self, *args, **kwargs) -> int:
         """Execute the the given suite."""
         pass
 
     @abstractmethod
-    def cleanup(self, *args, **kwargs) -> int:
+    def exec_post(self, *args, **kwargs) -> int:
         """Cleans up the given suite."""
         pass
 
 
 class Runner(RunStrategy):
     """This Strategy is the only one which executes a 'job' in fact.
 
     - run a Robot Framework Suite
     - run a RCC task
     """
 
     def __init__(self, target) -> None:
         super().__init__(target)
 
-    def prepare(self, *args, **kwargs) -> int:
-        # nothing to do
-        return 0
+    def run_subprocess(self, command, environ) -> Result:
+        """If command was given, run the subprocess and return the result object."""
+        if command:
+            res = subprocess.run(command, capture_output=True, env=environ)
+            return Result(
+                args=res.args,
+                returncode=res.returncode,
+                stdout=res.stdout.decode("utf-8").splitlines(),
+                stderr=res.stderr.decode("utf-8").splitlines(),
+            )
+        else:
+            return Result()
 
-    def execute(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
+        result = self.run_subprocess(self.target.pre_command, os.environ)
+        return result.returncode
+
+    def exec_main(self, *args, **kwargs) -> int:
         # DEBUG: " ".join(self.target.command)
         # DEBUG: [f"{k}={v}" for (k,v) in environment.items()  if k.startswith("RO")]
-        if kwargs.get("env"):
-            environment = kwargs["env"]
-        else:
-            environment = os.environ
-        result = subprocess.run(
-            self.target.command, capture_output=True, env=environment
+        result = self.run_subprocess(
+            self.target.main_command, kwargs.get("env", os.environ)
         )
-        stdout_str = result.stdout.decode("utf-8").splitlines()
-        stderr_str = result.stderr.decode("utf-8").splitlines()
-        result_dict = {
-            "args": result.args,
-            "returncode": result.returncode,
-            "stdout": stdout_str,
-            "stderr": stderr_str,
-        }
+
         # TODO: log console output? Save it anyway because a a fatal RF error must be tracable.
         # RCC does not re.execute...
         if getattr(self.target, "attempt", None) is None:
             self.target.attempt = 1
-        self.target.console_results[self.target.attempt] = result_dict
+        self.target.console_results[self.target.attempt] = asdict(result)
         return result.returncode
 
-    def cleanup(self, *args, **kwargs) -> int:
-        # nothing to do
-        return 0
-
-    # def _write_console_output(self, result):
+    def exec_post(self, *args, **kwargs) -> int:
+        result = self.run_subprocess(self.target.post_command, os.environ)
+        return result.returncode
 
 
 class WindowsTask(RunStrategy):
     """Parent class for Single and Multi desktop strategies.
 
     Both have in common that they need to create a scheduled task."""
 
     def __init__(self, target) -> None:
         super().__init__(target)
 
     @abstractmethod
-    def prepare(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
         pass
 
     @abstractmethod
-    def execute(self, *args, **kwargs) -> int:
+    def exec_main(self, *args, **kwargs) -> int:
         pass
 
     @abstractmethod
-    def cleanup(self, *args, **kwargs) -> int:
+    def exec_post(self, *args, **kwargs) -> int:
         pass
 
 
 class WindowsSingleDesktop(WindowsTask):
     """Concrete class to run a suite with UI on Windows.
 
     ....
     """
 
     def __init__(self, target) -> None:
         super().__init__(target)
 
-    def prepare(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
         # create the scheduled task for the given user
         pass
 
-    def execute(self, *args, **kwargs) -> int:
+    def exec_main(self, *args, **kwargs) -> int:
         # run schtask.exe to run the task
         pass
 
-    def cleanup(self, *args, **kwargs) -> int:
+    def exec_post(self, *args, **kwargs) -> int:
         pass
 
 
 class WindowsMultiDesktop(WindowsTask):
     """Concrete class to run a suite in a loopback RDP session.
 
     This will require a Windows Server with RDP enabled and a proper
     MSTC license. Although there is https://github.com/stascorp/rdpwrap
     (https://www.anyviewer.com/how-to/windows-10-pro-remote-desktop-multiple-users-0427.html)
     """
 
     def __init__(self, target) -> None:
         super().__init__(target)
 
-    def prepare(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
         # create RDP file:
         # rdp_file = "loopback.rdp"
         # with open(rdp_file, "w") as f:
         #     f.write(f"""\
         # username:s:{username}
         # password 51:b:{password}
         # full address:s:127.0.0.2
         # """)
         pass
 
-    def execute(self, *args, **kwargs) -> int:
+    def exec_main(self, *args, **kwargs) -> int:
         # Launch the RDP session with the specified command
         # os.system(f"mstsc /v:127.0.0.2 /f /w:800 /h:600 /v:127.0.0.2 /u:{username} /p:{password} /v:{rdp_file} /start:{command}")
         # os.system(f'mstsc /v:127.0.0.1 /f /w:800 /h:600 /u:{username} /p:{password} /v:127.0.0.1 /w:800 /h:600 /v:127.0.0.1 /w:800 /h:600 /admin /restrictedAdmin cmd /c "{command}"')
 
         pass
 
-    def cleanup(self, *args, **kwargs) -> int:
+    def exec_post(self, *args, **kwargs) -> int:
         # Close the RDP session
         # os.system(f'tscon /dest:console')
         pass
 
 
 class LinuxMultiDesktop(RunStrategy):
     """Executes a suite with a user interface on Linux."""
 
     def __init__(self, target) -> None:
         super().__init__(target)
 
-    def prepare(self, *args, **kwargs) -> int:
+    def exec_pre(self, *args, **kwargs) -> int:
         pass
 
-    def execute(self, *args, **kwargs) -> int:
+    def exec_main(self, *args, **kwargs) -> int:
         pass
 
-    def cleanup(self, *args, **kwargs) -> int:
+    def exec_post(self, *args, **kwargs) -> int:
         pass
 
 
 #    __           _
 #   / _|         | |
 #  | |_ __ _  ___| |_ ___  _ __ _   _
 #  |  _/ _` |/ __| __/ _ \| '__| | | |
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/suite.py` & `robotmk-0.0.56/src/robotmk/context/suite/suite.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,18 +100,14 @@
         # TODO: execute one single suite
         print("Suite context default action = execute single suite ")
         pass
 
     def execute(self):
         """Runs a single suite, either locally or remotely (via API call)."""
         # TODO: is it better to pass the suitename to get_target()?
-        # pid = os.getpid()
-        # print(f"Suite start (PID: {pid})")
-        # time.sleep(1)
-        # print(f"Suite end (PID: {pid})")
         self.get_target().run()
 
     def output(self):
         # TODO: make this possible in CLI
         """Implements the agent output for local context."""
         print("Local context agent output")
         self.outputter = SuiteOutput(self.config)
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.56/src/robotmk/context/suite/target/rcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,54 @@
 import os
+import math
 from .target import LocalTarget
 from ..strategies import RunStrategy
 from robotmk.logger import RobotmkLogger
 from robotmk.config import Config
 
 
+# TODO: make RCC binary path configurabe
+
+
 class RCCTarget(LocalTarget):
     def __init__(
         self,
         suiteuname: str,
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
+    @staticmethod
+    def worker_count():
+        """Determines the number of RCC worker processes by the total CPU cores available"""
+        return max(min(math.floor(os.cpu_count() / 2), 2), 6)
+
     def __str__(self) -> str:
         return "rcc"
 
     @property
-    def command(self):
+    def pre_command(self) -> list:
+        """Runs just before the command, executed by the Run strategy"""
+        return [
+            "rcc",
+            "holotree",
+            "vars",
+            "--controller",
+            "robotmk",
+            "--space",
+            self.suiteuname,
+            "--workers",
+            str(self.worker_count()),
+            "-r",
+            str(self.path.joinpath("robot.yaml")),
+        ]
+
+    @property
+    def main_command(self) -> list:
         """The command will be used by the Run strategy (self.target.command).
 
         In RCC target, the commandline gets buuilt to execute a RCC task (=Robotmk inside of RCC)
         """
         return [
             "rcc",
             "task",
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,32 +97,30 @@
         # for f in filenames:
         #     self.suite._runner.logdebug(" - %s" % f)
 
         # rebot wants to print out the generated file names on stdout; write to devnull
         devnull = open(os.devnull, "w")
         rebot(
             *outputfiles,
-            outputdir=self.target.robot_params["outputdir"],
+            outputdir=self.target.outputdir,
             output=self.target.output_xml,
             log=self.target.log_html,
             report=None,
             merge=True,
             stdout=devnull,
         )
         # self.suite._runner.loginfo("Merged results of all reexecutions into:")
         # self.suite._runner.loginfo(" - %s" % self.suite.output)
         # self.suite._runner.loginfo(" - %s" % self.suite.log)
 
     def _glob_target_outputfiles(self):
         """Returns the list of XML output files of the target execution attempts 1..n"""
         glob_pattern = "%s-*.xml" % self.target.output_filename.rsplit("-", 1)[0]
         outputfiles = sorted(
-            glob.glob(
-                str(Path(self.target.robot_params["outputdir"]).joinpath(glob_pattern))
-            )
+            glob.glob(str(Path(self.target.outputdir).joinpath(glob_pattern)))
         )
         return outputfiles
 
 
 class CompleteRetry(RetryStrategy):
     """Execution strategy for suites with complete re-execution"""
 
@@ -144,13 +142,13 @@
 
     def _reparametrize(self):
         """Reparametrize the suite for the next attempt.
 
         The next attempt needs the XML file of the last attempt as input.
         From there it will read failed tests and re-execute them only."""
         # Chance for next try. Attempt gets increased, output files get bumped
-        failed_xml = Path(self.target.logdir).joinpath(self.target.output_xml)
+        failed_xml = Path(self.target.outputdir).joinpath(self.target.output_xml)
         self.target.robot_params.update({"rerunfailed": str(failed_xml)})
         rerun_selection = self.target.config.get(
             "suitecfg.retry_failed.rerun_selection", asdict=True, default={}
         )
         self.target.robot_params.update(rerun_selection)
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,24 +42,24 @@
         # self.robot_params = {"console": "NONE", "report": "NONE"}
         self.robot_params = {"report": "NONE"}
 
     def __str__(self) -> str:
         return "robotframework"
 
     @property
-    def command(self):
+    def main_command(self) -> list:
         """The command will be used by the Run strategy (self.target.command).
 
         In RF target, the complete commandline must be built to execute the RF suite.
         (See https://robot-framework.readthedocs.io/en/latest/autodoc/robot.html#robot.run.run_cli)
         TODO: Logging"""
         self.robot_params.update(
             {
-                "log": self.log_html,
-                "output": self.output_xml,
+                "log": self.log_html,  #'rf_suite_default_1682429039_10559086-1.html'
+                "output": self.output_xml,  #'rf_suite_default_1682429039_10559086-1.xml'
             }
         )
 
         suite_params = mergedeep.merge(
             {}, self.config.get("suitecfg.params").asdict(), self.robot_params
         )
         arglist = ["robot"]
@@ -97,36 +97,29 @@
     def run(self):
         # Do not run if the suite dir contains a DISABLED file
         if self.is_disabled_by_flagfile:
             # TODO: Log skipped
             # reason = self.get_disabled_reason()
             return
         else:
-            # Tell Robot Framework to write its "output" files into the log dir.
-            # The "outputdir" is where RMK produces files later for the agent.
-            self.robot_params.update(
-                {"outputdir": str(Path(self.logdir).joinpath("robotframework"))}
-            )
+            # RF "outputdir" = logdir + robotframework (store HTML, XML and console logs)
+            self.robot_params.update({"outputdir": self.outputdir})
             self._state.timer_start()
             self.rc = self.retry_strategy.run()
             self._state.timer_stop()
             self._state.write()
             pass
 
     def get_now_as_dt(self):
         return datetime.now(local_tz)
 
     def get_now_as_epoch(self):
         return int(self.get_now_as_dt().timestamp())
 
     @property
-    def outdir(self):
-        return self.config.get("common.outdir")
-
-    @property
     def timestamp(self):
         """Returns the timestamp the suite execution was started. This is
         used for all executions of the suite, including retries in order
         to group the result files."""
         return self._timestamp
 
     def get_disabled_reason(self) -> str:
@@ -139,14 +132,28 @@
                         return "Reason: " + reason
                     else:
                         return ""
             except:
                 return ""
 
     @property
+    def resultdir(self):
+        return Path(self.logdir).joinpath("results")
+
+    @property
+    def statefile_fullpath(self):
+        return str(Path(self.resultdir).joinpath(self.suiteuname + ".json"))
+
+    # OUTPUT
+
+    @property
+    def outputdir(self):
+        return str(Path(self.logdir).joinpath("robotframework"))
+
+    @property
     def output_filename(self):
         """Returns the output filename string, including the retry number.
 
         Example:
             rf_suite1_978741fb_1680335851
             rf_suite1_978741fb_1680335851-1"""
         if self.attempt is None:
@@ -160,35 +167,31 @@
                 self.suiteuname,
                 self.timestamp,
                 self.shortuuid,
                 int(self.attempt),
             )
         return suite_filename
 
-    @property
-    def statefile_fullpath(self):
-        return str(Path(self.outdir).joinpath(self.suiteuname + ".json"))
-
-    # XML ---
+    # XML Output---
     @property
     def output_xml(self):
         return self.output_filename + ".xml"
 
     @property
     def output_xml_fullpath(self):
-        return str(Path(self.robot_params["outputdir"]).joinpath(self.output_xml))
+        return str(Path(self.outputdir).joinpath(self.output_xml))
 
-    # HTML ---
+    # HTML Output ---
     @property
     def log_html(self):
         return self.output_filename + ".html"
 
     @property
     def log_html_fullpath(self):
-        return str(Path(self.robot_params["outputdir"]).joinpath(self.log_html))
+        return str(Path(self.outputdir).joinpath(self.log_html))
 
     # Suite timestamp for filenames
     @property
     def timestamp(self):
         return self._timestamp
 
     @timestamp.setter
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 from pathlib import Path
 import base64
 import zlib
+from robotmk import __version__
 
 
 class RFState:
     def __init__(self, target) -> None:
         self.target = target
 
     @property
@@ -26,14 +27,15 @@
                     "path": self.target.output_xml_fullpath,
                     "base64": self.encode(
                         self.read_file(self.target.output_xml_fullpath)
                     ),
                 },
                 "console": self.target.console_results,
             },
+            "robotmk_version": __version__,
         }
 
     def write(self) -> None:
         """Writes the console output to logdir and result JSON file to outputdir."""
         self.write_console_log()
         self.write_result_json()
 
@@ -45,15 +47,15 @@
         self._runtime = self._end_time - self._start_time
 
     def write_console_log(self) -> None:
         for k, result in self.target.console_results.items():
             # HEREIWAS:
             data = json.dumps(result, indent=4)
             filename = (
-                Path(self.target.robot_params["outputdir"])
+                Path(self.target.outputdir)
                 / f"{self.target.output_filename}-{int(k)}.txt"
             )
             self.write_data2file(data, filename)
             pass
 
     def write_result_json(self) -> None:
         """ """
```

### Comparing `robotmk-0.0.54/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.56/src/robotmk/context/suite/target/target.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from uuid import uuid4
 from ..strategies import RunStrategy, RunStrategyFactory
 
-
 from robotmk.logger import RobotmkLogger
 
 
 class Target(ABC):
     """A Target defines the environment where a suite gets executed.
 
     It's the abstraction of either
@@ -65,14 +64,26 @@
             self.config.get("suitecfg.path")
         )
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
 
     @property
+    def pre_command(self):
+        return None
+
+    @property
+    def main_command(self):
+        return None
+
+    @property
+    def post_command(self):
+        return None
+
+    @property
     def uuid(self):
         return self.config.get("suitecfg.uuid", uuid4().hex)
 
     @property
     def logdir(self):
         return self.config.get("common.logdir")
```

### Comparing `robotmk-0.0.54/src/robotmk/executor/scheduler.py` & `robotmk-0.0.56/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.56/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/src/robotmk/logger.py` & `robotmk-0.0.56/src/robotmk/logger.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import loguru
 from abc import ABC, abstractmethod
 from datetime import datetime
 
 
+# TODO: concurrent writes to the log file
+# e.g. RCC -> RF
+
+
 class AbstractLogger(ABC):
     def __init__(self, log_level):
         self.log_level = log_level
         if not getattr(self, "logger", None):
             self.logger = loguru.logger
             # Disable the logger completely if log level is not set
             if self.log_level is None:
```

### Comparing `robotmk-0.0.54/src/robotmk/main.py` & `robotmk-0.0.56/src/robotmk/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,73 +28,70 @@
         # "cache_time": 960,
         # "execution_interval": 900,
     },
     # Default values for the "common" config section (Windows)
     "nt": {
         "robotdir": "C:/ProgramData/checkmk/agent/robot",
         "cfgdir": "C:/ProgramData/checkmk/agent/config",
-        "logdir": "C:/ProgramData/checkmk/agent/log/robotmk",
-        "outdir": "C:/ProgramData/checkmk/agent/log/robotmk/results",
+        "logdir": "C:/ProgramData/checkmk/agent/log/robotmk/",
         "tmpdir": "C:/ProgramData/checkmk/agent/tmp/robotmk",
     },
     # Default values for the "common" config section (Linux)
     "posix": {
         "robotdir": "/usr/lib/check_mk_agent/robot",
         "cfgdir": "/etc/check_mk",
         "logdir": "/var/log/robotmk",
-        "outdir": "/var/log/robotmk/results",
         "tmpdir": "/tmp/robotmk",
     },
 }
 
 
 class Robotmk:
     """This is the main class of the robotmk package. It is used to create a
     Robotmk instance with a specific context.
 
     Configuration loading (yml, var, env) depends on the context and is only
-    done when not config object is passed to the init method."""
+    done when no config object is passed to the init method."""
 
     def __init__(
         self,
         log_level=None,
         contextname=None,
         ymlfile: str = None,
         varfile: str = None,
         default_cfg: dict = {},
     ) -> None:
         """context is the strategy to use and in fact a set of factory methods.
         If called from the CLI without context argument, the default context
         will be read from environment variable ROBOTMK_common_context."""
 
-        self.__set_context(contextname, log_level)
+        self._set_context(contextname, log_level)
         self._context.load_config(
             DEFAULTS, ymlfile=ymlfile, varfile=varfile, default_cfg=default_cfg
         )
-        self.config.set("common.context", contextname)
 
         self.run_default = self._context.run_default
         # execute and output are the two main functions of each context:
         self.execute = self._context.execute
         self.output = self._context.output
 
     @property
     def config(self):
         return self._context.config
 
-    def __set_context(self, contextname: str, log_level: str = None) -> None:
+    def _set_context(self, contextname: str, log_level: str = None) -> None:
         """Sets the context of the Robotmk instance (=strategy)."""
         if contextname is None:
-            contextname = os.environ.get("ROBOTMK_common_context", "not set")
-        if contextname == "not set":
+            contextname = os.environ.get("ROBOTMK_common_context", None)
+        if contextname is None:
             raise ValueError(
                 "No context given on CLI or set by environment variable ROBOTMK_common_context."
             )
-
         self._context = ContextFactory(contextname, log_level).get_context()
+        self.config.set("common.context", contextname)
 
         # TODO: Setup Logging here
 
 
 # print('Press Ctrl+{0} to exit'.format('Break' if os.name == 'nt' else 'C'))
 
 # try:
```

### Comparing `robotmk-0.0.54/tests/config/robotmk.yml` & `robotmk-0.0.56/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/config/test_config.py` & `robotmk-0.0.56/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/context/local/test_local_cli.py` & `robotmk-0.0.56/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.56/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/context/suite/robotmk.yml` & `robotmk-0.0.56/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.56/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/context/test_cli.py` & `robotmk-0.0.56/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/tests/yml/robotmk.yml` & `robotmk-0.0.56/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.54/PKG-INFO` & `robotmk-0.0.56/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.54
+Version: 0.0.56
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

