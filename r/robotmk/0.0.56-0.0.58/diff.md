# Comparing `tmp/robotmk-0.0.56.tar.gz` & `tmp/robotmk-0.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.56.tar", last modified: Tue Apr 25 14:31:26 2023, max compression
+gzip compressed data, was "robotmk-0.0.58.tar", last modified: Wed Apr 26 18:41:27 2023, max compression
```

## Comparing `robotmk-0.0.56.tar` & `robotmk-0.0.58.tar`

### file list

```diff
@@ -1,58 +1,62 @@
--rw-r--r--   0        0        0      110 2023-04-25 14:30:31.577495 robotmk-0.0.56/.bumpversion.cfg
--rw-r--r--   0        0        0      284 2023-04-04 11:07:18.122518 robotmk-0.0.56/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.56/README.md
--rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.56/pyproject.toml
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.56/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.56/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-25 14:30:31.577495 robotmk-0.0.56/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5528 2023-04-25 08:43:45.469873 robotmk-0.0.56/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.56/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.56/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.56/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.56/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.56/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.56/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0      681 2023-04-13 13:22:33.639789 robotmk-0.0.56/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.56/src/robotmk/context/local/__init__.py
--rw-r--r--   0        0        0     1491 2023-04-13 11:46:06.562610 robotmk-0.0.56/src/robotmk/context/local/cli.py
--rw-r--r--   0        0        0     2052 2023-04-13 11:47:44.173586 robotmk-0.0.56/src/robotmk/context/local/local.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.56/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.56/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.56/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.56/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-04 10:17:56.403169 robotmk-0.0.56/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.56/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.56/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3825 2023-04-13 11:46:27.306392 robotmk-0.0.56/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.56/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     7380 2023-04-25 13:50:39.300240 robotmk-0.0.56/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     4366 2023-04-14 13:05:12.951814 robotmk-0.0.56/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      136 2023-04-01 18:27:58.571962 robotmk-0.0.56/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     5446 2023-04-25 13:50:20.160423 robotmk-0.0.56/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0      315 2023-03-30 05:55:28.600317 robotmk-0.0.56/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6558 2023-04-25 13:56:25.732927 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4878 2023-04-25 14:28:49.598467 robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     2980 2023-04-25 13:50:11.588505 robotmk-0.0.56/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.56/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.56/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.56/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.56/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.56/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.56/src/robotmk/logger.py
--rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.56/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.56/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.56/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.56/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.56/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.56/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.56/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.56/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.56/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.56/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.56/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.56/tests/context/test_cli.py
--rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.56/tests/test_robotmk.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.56/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.56/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-26 18:41:17.217259 robotmk-0.0.58/.bumpversion.cfg
+-rw-r--r--   0        0        0      279 2023-04-25 15:17:21.816448 robotmk-0.0.58/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.58/README.md
+-rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.58/pyproject.toml
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.58/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.58/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-26 18:41:17.217259 robotmk-0.0.58/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-26 09:17:32.607360 robotmk-0.0.58/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.58/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.58/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.58/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.58/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.58/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.58/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.58/src/robotmk/context/agent/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-26 12:58:54.634165 robotmk-0.0.58/src/robotmk/context/agent/agent.py
+-rw-r--r--   0        0        0     1580 2023-04-26 12:34:36.526163 robotmk-0.0.58/src/robotmk/context/agent/cli.py
+-rw-r--r--   0        0        0      681 2023-04-26 12:37:20.188228 robotmk-0.0.58/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.58/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.58/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.58/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.58/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-26 12:27:48.266927 robotmk-0.0.58/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.58/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.58/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-26 10:06:25.887510 robotmk-0.0.58/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.58/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     7380 2023-04-25 13:50:39.300240 robotmk-0.0.58/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     2849 2023-04-26 13:44:29.789250 robotmk-0.0.58/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      135 2023-04-26 13:29:57.729591 robotmk-0.0.58/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     1432 2023-04-26 17:05:40.456944 robotmk-0.0.58/src/robotmk/context/suite/target/abstract.py
+-rw-r--r--   0        0        0     1604 2023-04-26 13:40:32.915503 robotmk-0.0.58/src/robotmk/context/suite/target/factory.py
+-rw-r--r--   0        0        0     2686 2023-04-26 16:31:12.211225 robotmk-0.0.58/src/robotmk/context/suite/target/local.py
+-rw-r--r--   0        0        0     5628 2023-04-26 13:29:57.729591 robotmk-0.0.58/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0     2208 2023-04-26 17:23:25.018107 robotmk-0.0.58/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6339 2023-04-26 13:35:01.378678 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4877 2023-04-26 18:10:20.939058 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     3878 2023-04-26 13:32:58.143863 robotmk-0.0.58/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0     3932 2023-04-26 18:38:03.011146 robotmk-0.0.58/src/robotmk/emitter.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.58/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.58/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.58/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.58/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.58/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.58/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.58/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.58/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.58/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.58/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.58/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.58/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.58/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.58/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.58/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.58/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.58/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.58/tests/context/test_cli.py
+-rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.58/tests/test_robotmk.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.58/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.58/PKG-INFO
```

### Comparing `robotmk-0.0.56/pyproject.toml` & `robotmk-0.0.58/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/categories.json` & `robotmk-0.0.58/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/click_tutorial.py` & `robotmk-0.0.58/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/cli/cli.py` & `robotmk-0.0.58/src/robotmk/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 import pkgutil
 import os.path
 import warnings
 
 
 # CMD1        CMD2     OPTION                                    CMD3            # Description
 # ---------------------------------------------------------------------------------------------
-# # LOCAL CONTEXT
+# # FS CONTEXT
 # robotmk                                                                        # no arg = print output
 
-# robotmk     local                                              output          # print output
-# robotmk     local    --yml /etc/checkmk/another_robotmk.yml    output          # print output with yml
-# robotmk     local    --vars /var/robotmk_local.env             output          # print output, load env from file (instead of env)
-
-# robotmk     local                                              scheduler       # start scheduler
-# robotmk     local    --yml /etc/checkmk/another_robotmk.yml    scheduler       # start scheduler with yml
-# robotmk     local    --vars /var/robotmk_local.env             scheduler       # start scheduler, load env from file  (instead of env)
+# robotmk     fs                                              output          # print output
+# robotmk     fs       --yml /etc/checkmk/another_robotmk.yml    output          # print output with yml
+# robotmk     fs       --vars /var/robotmk_local.env             output          # print output, load env from file (instead of env)
+
+# robotmk     fs                                                 scheduler       # start scheduler
+# robotmk     fs       --yml /etc/checkmk/another_robotmk.yml    scheduler       # start scheduler with yml
+# robotmk     fs       --vars /var/robotmk_local.env             scheduler       # start scheduler, load env from file  (instead of env)
 # ---------------------------------------------------------------------------------------------
 # # SUITE CONTEXT
 # robotmk                                                                        # no arg = exec suite as configured in env
 # robotmk     suite    --vars /var/rmk/foosuiteA_8bb36c3.env                     # exec suite with env from file and suite = yml -> common: suite)
 # robotmk     suite    --vars /var/rmk/foosuiteA_8bb36c3.env     bazsuite        # exec suite with env from file and suite = bazsuite
 # robotmk     suite                                              vardump  foobarsuiteA   # just dump the vars for foobarsuiteA
 # ---------------------------------------------------------------------------------------------
@@ -44,16 +44,16 @@
     Each sub-PACKAGE of pkg is considered a sub-COMMAND. This function recursively traverses the
     package tree and returns all function objects which have the same name as the package.
 
     This allows to maintain the CLI logic within the context packages, while still having a single
     entry point for the CLI.
 
     Example:
-    robotmk.context.local.cli.py contains a function called local(), decorated with @click.group()
-    and connected with subcomands "output()" and "scheduler()". The discovered subcommand is "local()".
+    robotmk.context.agent.cli.py contains a function called agent(), decorated with @click.group()
+    and connected with subcomands "output()" and "scheduler()". The discovered subcommand is "agent()".
     """
     pkg_obj = importlib.import_module(pkg)
     pkg_path = os.path.dirname(pkg_obj.__file__)
     commands = {}
     for module in pkgutil.iter_modules([pkg_path]):
         module_obj = importlib.import_module(f"{pkg}.{module.name}")
         if module.ispkg:
@@ -83,17 +83,17 @@
     type=click.Choice(LOG_LEVELS),
 )
 @click.pass_context
 def main(ctx, loglevel):
     if ctx.invoked_subcommand is None:
         # robotmk was called without argument. Try to detect the context from the default
         # config and/or environment variables.
-        # After that run the default subcommand of the context:
-        # - local: produce output
-        # - specialagent: produce output + call sequencer
+        # After that run the default subcommand of the specific context:
+        # - agent: produce output
+        # - specialagent: run 1 sequence + produce output
         # - suite: run a single suite
         ctx.robotmk = Robotmk(
             contextname=None, log_level=loglevel, ymlfile=None, varfile=None
         )
         ctx.robotmk.run_default()
     else:
         # Robotmk was executed with a context subcommand, whose logic is defined within the context.
```

### Comparing `robotmk-0.0.56/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.58/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/config/config.py` & `robotmk-0.0.58/src/robotmk/config/config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/config/yml.py` & `robotmk-0.0.58/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/context/abstract.py` & `robotmk-0.0.58/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/context/context.py` & `robotmk-0.0.58/src/robotmk/context/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 class ContextFactory:
     def __init__(self, contextname: str, log_level: str) -> None:
         self.contextname = contextname
         self._log_level = log_level
 
     def get_context(self) -> None:
-        if self.contextname == "local":
-            from .local.local import LocalContext
+        if self.contextname == "agent":
+            from .agent.agent import AgentContext
 
-            return LocalContext()
+            return AgentContext()
         elif self.contextname == "specialagent":
             from .specialagent.specialagent import SpecialAgentContext
 
             return SpecialAgentContext()
         elif self.contextname == "suite":
             from .suite.suite import SuiteContext
```

### Comparing `robotmk-0.0.56/src/robotmk/context/local/local.py` & `robotmk-0.0.58/src/robotmk/context/agent/agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from pathlib import Path
 from ..abstract import AbstractContext
 
 from robotmk.config import Config, RobotmkConfigSchema
-
 from robotmk.executor.scheduler import Scheduler
+from robotmk.emitter import Emitter
 
 
-class LocalContext(AbstractContext):
+class AgentContext(AbstractContext):
     def __init__(self):
         super().__init__()
         self.ymlschema = RobotmkConfigSchema
 
     @property
     def logger(self):
         if not self._logger:
             self._logger = RobotmkLogger(
                 Path(self.config.common.logdir).joinpath("robotmk.log"),
                 self.config.common.log_level,
             )
         return self._logger
 
     def load_config(self, defaults, **kwargs) -> None:
-        """Load the config for local context.
+        """Load the config for agent context.
 
-        Local context can merge the config from
+        Agent context can merge the config from
         - OS defaults
         - + YML file (default/custom = --yml)
         - + environment variables
         """
         # self.config = Config()
         self.config.set_defaults(defaults)
         self.config.read_yml_cfg(path=kwargs["ymlfile"], must_exist=True)
@@ -40,23 +40,22 @@
         config_copy = copy.deepcopy(self.configdict)
         # re-initializes the config object
         super().__init__(envvar_prefix=self.envvar_prefix)
         config_changed = config_copy != self.configdict
         return config_changed
 
     def run_default(self):
-        """Implements the default action for local context."""
+        """Implements the default action for agent context."""
         # TODO: how do I call the coutputter here?
-        print("Local context default action = output")
+        print("Agent context default action = output")
         pass
 
     def execute(self, *args, **kwargs):
         """Starts the scheduler."""
         self.executor = Scheduler(self.config)
         self.executor.run()
         pass
 
     def output(self):
-        """Implements the agent output for local context."""
-        print("Local context agent output")
-        self.outputter = LocalOutput(self.config)
-        pass
+        """Gathers the results of all scheduled suites and returns CMK agent output from it."""
+        self.emitter = Emitter(self.config)
+        self.emitter.run()
```

### Comparing `robotmk-0.0.56/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.58/src/robotmk/context/specialagent/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-"""CLI commands for the specialagent context.
-
-Executes Robotmk in specialagent context. This CLI is rather used to debug the 
-specialagent than to run it in production."""
+"""CLI commands for the specialagent context."""
 import sys
 import click
 from robotmk.main import Robotmk, DEFAULTS
 
 
 # use module docstring as help text
 @click.group(help=__doc__, invoke_without_command=True)
@@ -18,22 +15,22 @@
 
     pass
 
 
 @specialagent.command()
 @click.pass_context
 def sequencer(ctx):
-    click.secho("sequencer", fg="green")
+    """Start the sequencer to execute tests once, respecting their interval."""
     ctx.obj.execute()
 
 
 @specialagent.command()
 @click.pass_context
 def output(ctx):
-    click.secho("output", fg="green")
+    """Produces Checkmk Agent output for all suite results."""
     ctx.obj.output()
     pass
 
 
 @specialagent.command(help="Dump the config as YML to STDOUT or FILE")
 # add file arg
 @click.argument("file", required=False, type=click.Path(exists=False))
```

### Comparing `robotmk-0.0.56/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.58/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/cli.py` & `robotmk-0.0.58/src/robotmk/context/suite/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """CLI commands for execution of a single suite."""
 
 import sys
 import click
+import json
 from robotmk.cli.defaultgroup import DefaultGroup
 from robotmk.main import Robotmk, DEFAULTS
 
 # TODO: Refine the defaultgroup usage
 
 #             _ _
 #            (_) |
@@ -38,34 +39,39 @@
     """Trigger the start of a Robot Framework SUITE.
 
     SUITE must be a configuration subkey of the "suites" section.
     (can also be set by env:ROBOTMK_common_suiteuname.)
     """
     if suite:
         ctx.obj.config.set("common.suiteuname", suite)
-    if ctx.obj.config.get("common.suiteuname", None):
+    if bool(ctx.obj.config.get("common.suiteuname", None)):
         ctx.obj.execute()
     else:
         click.secho("Suite '%s' not found in configuration" % suite, fg="red")
 
 
 @suite.command()
 @click.argument("suite", required=False)
 @click.pass_context
-def output(ctx, suite):
-    """Print the CMK agent output of SUITE on STDOUT.
+def result(ctx, suite):
+    """Print the result JSON of a SUITE on STDOUT.
 
-    SUITEID is eiher equal to the suite dir or a combination of suite dir and its unique tag as set in the configuration.
-    Examples are: suite1, suite2_tagfoo, suite3_tagbaz
+    SUITE must be a configuration subkey of the "suites" section.
     (can also be set by env:ROBOTMK_common_suiteuname.)
+
+    To get the Checkmk Agent output, use "agent output" instead.
     """
-    click.secho("output of suite %s" % suite, fg="green")
-    # TODO: to be implemented
-    ctx.obj.output()
-    pass
+    if suite:
+        ctx.obj.config.set("common.suiteuname", suite)
+    if bool(ctx.obj.config.get("common.suiteuname", None)):
+        data = ctx.obj.output()
+        click.secho(json.dumps(data, indent=4), fg="bright_white")
+
+    else:
+        click.secho("Suite '%s' not found in configuration" % suite, fg="red")
 
 
 @suite.command()
 @click.argument("suite", required=True)
 @click.option(
     "--number",
     "-n",
```

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.58/src/robotmk/context/suite/strategies/run.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/suite.py` & `robotmk-0.0.58/src/robotmk/context/suite/suite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,51 @@
 """This module encapsulates everyhting related so a single suite 
-execution, either locally or remotely."""
+execution, either against a local target (RCC/RF) or against a remote one (API)."""
 
+from uuid import uuid4
 from pathlib import Path
 from ..abstract import AbstractContext
 
 from robotmk.config import Config, RobotmkConfigSchema
 
-from .target import Target, RobotFrameworkTarget, RCCTarget, RemoteTarget
+# from .target import Target, RobotFrameworkTarget, RCCTarget, RemoteTarget
+from .target import Target
+from .target.factory import TargetFactory
 import time, os
 
 
 class SuiteContext(AbstractContext):
     def __init__(self):
         super().__init__()
-        self._target = None
+        # the target object
+        self._otarget = None
         self._ymlschema = RobotmkConfigSchema
 
     @property
     def suiteuname(self):
         """suiteuname under "common" sets the suite to start (suitename + tag)"""
         try:
             suiteuname = self.config.get("common.suiteuname")
         except AttributeError:
             pass
             # TODO: What if suite is not found?
         return suiteuname
 
-    def get_target(self) -> Target:
-        """Returns a Target object using the Bridge pattern which combines
-        - Local Targets (Shared Python/RCC)   with
-        - Head Strategies (Headless/Headed, Win/linux)"""
-        # TODO: notify the logger initialization as soon as there is config loaded
-        # to prevent this call
-        if not self._target:
-            self.init_logger()
-            # get the dotmap config for the suite to run
-            # TODO: what if suite is not part of the config?
-            suitecfg = self.config.get("suites.%s" % self.suiteuname)
-            if suitecfg == None:
-                self.error("Suite '%s' is not part of the config!" % self.suiteuname)
-
-            # Depending on the target, create a local or a remote suite
-            target = suitecfg.get("run.target")
-            rcc = suitecfg.get("run.rcc")
-            if target == "local":
-                path = Path(self.config.get("common.robotdir")).joinpath(
-                    suitecfg.get("path")
-                )
-                if path.exists():
-                    if rcc is True:
-                        self._target = RCCTarget(
-                            self.suiteuname, self.config, self.logger
-                        )
-                    else:
-                        self._target = RobotFrameworkTarget(
-                            self.suiteuname, self.config, self.logger
-                        )
-                else:
-                    # TBD: check this if this gets logged...
-                    self.error("Suite path does not exist: " + str(path))
-            elif target == "remote":
-                self._target = RemoteTarget(self.suiteuname, self.config, self.logger)
-            else:
-                self.error("Unknown target type for suite %s!" % self.suiteuname)
-        return self._target
-
     @property
     def target(self) -> Target:
-        return self._target
+        # singleton
+        return self._otarget
+
+    def get_target(self) -> Target:
+        if not self._otarget:
+            self.init_logger()
+            self._otarget = TargetFactory(
+                self.suiteuname, self.config, self.logger
+            ).create()
+        return self._otarget
 
     def load_config(self, defaults, **kwargs) -> None:
         """Load the config for suite context.
 
         Suite context can merge the config from
         - OS defaults
         - + YML file (default/custom = --yml)
@@ -98,17 +72,14 @@
     def run_default(self):
         """Implements the default action for suite context."""
         # TODO: execute one single suite
         print("Suite context default action = execute single suite ")
         pass
 
     def execute(self):
-        """Runs a single suite, either locally or remotely (via API call)."""
+        """Runs a single suite, either fs/remote."""
         # TODO: is it better to pass the suitename to get_target()?
         self.get_target().run()
 
     def output(self):
-        # TODO: make this possible in CLI
-        """Implements the agent output for local context."""
-        print("Local context agent output")
-        self.outputter = SuiteOutput(self.config)
-        pass
+        """Gathers the result of the given suite (fs/remote) and returns it"""
+        return self.get_target().output()
```

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.58/src/robotmk/context/suite/target/rcc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import math
-from .target import LocalTarget
+from .local import LocalTarget
 from ..strategies import RunStrategy
 from robotmk.logger import RobotmkLogger
 from robotmk.config import Config
 
 
 # TODO: make RCC binary path configurabe
 
@@ -16,15 +16,23 @@
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
     @staticmethod
     def worker_count():
-        """Determines the number of RCC worker processes by the total CPU cores available"""
+        """Determines the number of RCC worker processes by the total CPU cores available.
+
+        Example:
+        - 4 cores: 2 workers
+        - 5 cores: 2 workers
+        - 6 cores: 3 workers
+        - 7 cores: 3 workers
+        - 8 cores: 4 workers
+        """
         return max(min(math.floor(os.cpu_count() / 2), 2), 6)
 
     def __str__(self) -> str:
         return "rcc"
 
     @property
     def pre_command(self) -> list:
@@ -60,15 +68,15 @@
             "-t",
             "robotmk",
             "-r",
             str(self.path.joinpath("robot.yaml")),
         ]
 
     def prepare_environment(self) -> dict:
-        """Sets up the environment for a subsequent run.
+        """Sets up the environment for a subsequent RCC robot run.
 
         If Robotmk calls itself in a RCC task, the inner call of Robotmk needs
         some special settings, e.g. NOT to use RCC again, to log into the default
         logdir, etc.
         This function first exports the current config to the environment and
         then adds the special settings on top.
         """
```

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from abc import ABC, abstractmethod
 import os
 from pathlib import Path
+import robot
+import mergedeep
 
 from .retry import RetryStrategyFactory, CompleteRetry, IncrementalRetry
 from .state import RFState
-from ..target import LocalTarget
+from ..local import LocalTarget
 from ...strategies import RunStrategy
 
 from robotmk.logger import RobotmkLogger
 from robotmk.config import Config
 
-import robot
-import mergedeep
-
 
 from datetime import datetime
 
 local_tz = datetime.utcnow().astimezone().tzinfo
 
 # This is the "heavy" part of the code. It contains the logic to run RF.
 # Here I place all the Robotmk v1 shit.
@@ -27,25 +26,14 @@
         self,
         suiteuname: str,
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
 
-        self.retry_strategy = RetryStrategyFactory(self).create()
-
-        self.shortuuid = self.uuid[:8]
-        # this timestamp is used to keep all result files in order; it is used
-        # for all target executions
-        self._timestamp = self.get_now_as_epoch()
-        self._state = RFState(self)
-        # params for RF: global ones & re-execution
-        # self.robot_params = {"console": "NONE", "report": "NONE"}
-        self.robot_params = {"report": "NONE"}
-
     def __str__(self) -> str:
         return "robotframework"
 
     @property
     def main_command(self) -> list:
         """The command will be used by the Run strategy (self.target.command).
 
@@ -91,33 +79,44 @@
                 else:
                     arglist.extend([arg, value])
         # the path of the robot suite is the very last argument
         arglist.append(str(self.path))
         return arglist
 
     def run(self):
+        self.retry_strategy = RetryStrategyFactory(self).create()
+
+        self.shortuuid = self.uuid[:8]
+        # this timestamp is used to keep all result files in order; it is used
+        # for all target executions
+        self._timestamp = self.get_now_as_epoch()
+        self._state = RFState(self)
+        # params for RF: global ones & re-execution
+        # self.robot_params = {"console": "NONE", "report": "NONE"}
+        self.robot_params = {"report": "NONE"}
+
         # Do not run if the suite dir contains a DISABLED file
         if self.is_disabled_by_flagfile:
             # TODO: Log skipped
             # reason = self.get_disabled_reason()
             return
         else:
             # RF "outputdir" = logdir + robotframework (store HTML, XML and console logs)
             self.robot_params.update({"outputdir": self.outputdir})
             self._state.timer_start()
             self.rc = self.retry_strategy.run()
             self._state.timer_stop()
             self._state.write()
             pass
 
-    def get_now_as_dt(self):
+    def _get_now_as_dt(self):
         return datetime.now(local_tz)
 
     def get_now_as_epoch(self):
-        return int(self.get_now_as_dt().timestamp())
+        return int(self._get_now_as_dt().timestamp())
 
     @property
     def timestamp(self):
         """Returns the timestamp the suite execution was started. This is
         used for all executions of the suite, including retries in order
         to group the result files."""
         return self._timestamp
@@ -131,22 +130,14 @@
                     if len(reason) > 0:
                         return "Reason: " + reason
                     else:
                         return ""
             except:
                 return ""
 
-    @property
-    def resultdir(self):
-        return Path(self.logdir).joinpath("results")
-
-    @property
-    def statefile_fullpath(self):
-        return str(Path(self.resultdir).joinpath(self.suiteuname + ".json"))
-
     # OUTPUT
 
     @property
     def outputdir(self):
         return str(Path(self.logdir).joinpath("robotframework"))
 
     @property
```

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         return {
             "suiteuname": self.target.suiteuname,
             "uuid": self.target.uuid,
             "rc": self.target.rc,
             "start_time": self._start_time.isoformat(),
             "end_time": self._end_time.isoformat(),
             "runtime": self._runtime.total_seconds(),
-            "piggybackhost": self.target.config.get("suiteconfig.piggybackhost", None),
+            "piggybackhost": self.target.config.get("suitecfg.piggybackhost", None),
             "output": {
                 "html": {
                     "path": self.target.log_html_fullpath,
                 },
                 "xml": {
                     "path": self.target.output_xml_fullpath,
                     "base64": self.encode(
@@ -36,18 +36,18 @@
 
     def write(self) -> None:
         """Writes the console output to logdir and result JSON file to outputdir."""
         self.write_console_log()
         self.write_result_json()
 
     def timer_start(self) -> None:
-        self._start_time = self.target.get_now_as_dt()
+        self._start_time = self.target._get_now_as_dt()
 
     def timer_stop(self) -> None:
-        self._end_time = self.target.get_now_as_dt()
+        self._end_time = self.target._get_now_as_dt()
         self._runtime = self._end_time - self._start_time
 
     def write_console_log(self) -> None:
         for k, result in self.target.console_results.items():
             # HEREIWAS:
             data = json.dumps(result, indent=4)
             filename = (
```

### Comparing `robotmk-0.0.56/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.58/src/robotmk/context/suite/target/local.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,103 +1,86 @@
 from abc import ABC, abstractmethod
 from pathlib import Path
 from uuid import uuid4
-from ..strategies import RunStrategy, RunStrategyFactory
+import json
 
+from .abstract import Target
+from ..strategies import RunStrategy, RunStrategyFactory
 from robotmk.logger import RobotmkLogger
 
 
-class Target(ABC):
-    """A Target defines the environment where a suite gets executed.
-
-    It's the abstraction of either
-    - a local Robot suite or ("target: local")
-    - an API call to an external platform ("target: remote") like Robocorp or Kubernetes
-    """
-
-    def __init__(self, suiteuname: str, config, logger: RobotmkLogger):
-        self.suiteuname = suiteuname
-        self.config = config
-
-        self.commoncfg = self.config.get("common")
-
-        self._logger = logger
-        # TODO: Boilerplate alarm
-        self.debug = self._logger.debug
-        self.info = self._logger.info
-        self.warning = self._logger.warning
-        self.error = self._logger.error
-        self.critical = self._logger.critical
-
-    @abstractmethod
-    def run(self):
-        """Abstract method to run a suite/target."""
-        pass
-
-    @abstractmethod
-    def output(self):
-        """Abstract method to get the output of a suite/target."""
-        pass
-
-
 class LocalTarget(Target):
-    """A local target is a single Robot Framework suite or a RCC task for this suite.
+    """A FS target is a single RF suite or a RCC task, ready to run from the local filesystem.
 
     It also encapsulates the implementation details of the RUN strategy, which is
     either a headless or a headed execution (RDP, XVFB, Scheduled Task)."""
 
     def __init__(
         self,
         suiteuname: str,
         config: dict,
         logger: RobotmkLogger,
     ):
         super().__init__(suiteuname, config, logger)
-
-        # Store RCC and RF logs in separate folders
-        # TODO: relly needed?
-        # self.config.set(
-        #     "common.logdir",
-        #     "%s/%s" % (self.config.get("basic_cfg.common.logdir"), str(self)),
-        # )
-
         self.path = Path(self.config.get("common.robotdir")).joinpath(
             self.config.get("suitecfg.path")
         )
+        # TODO: run strategy should not be set in init, because output() always reads results from filesystem
         self.run_strategy = RunStrategyFactory(self).create()
         # list of subprocess' results and console output
         self.console_results = {}
 
+    @abstractmethod
+    def run(self):
+        """Implementation in subclasses RCCTarget and RobotFrameworkTarget"""
+        pass
+
+    def output(self):
+        """Read the result artifacts from the filesystem."""
+        try:
+            with open(self.statefile_fullpath) as f:
+                data = json.load(f)
+                return data
+        except FileNotFoundError:
+            # return an empty dict to indicate that the file is not present
+            return {}
+
     @property
     def pre_command(self):
         return None
 
     @property
     def main_command(self):
         return None
 
     @property
     def post_command(self):
         return None
 
     @property
     def uuid(self):
-        return self.config.get("suitecfg.uuid", uuid4().hex)
+        """If a UUID is already part of the suite config, use this. Otherwise generate a new one.
+
+        The idea is that the UUID is handed over between all robotmk calls and lastly part of the
+        result JSON."""
+        uuid_ = self.config.get("suitecfg.uuid", False)
+        if not uuid_:
+            uuid_ = uuid4().hex
+        return uuid_
 
     @property
     def logdir(self):
         return self.config.get("common.logdir")
 
     @property
+    def resultdir(self):
+        return Path(self.logdir).joinpath("results")
+
+    @property
+    def statefile_fullpath(self):
+        return str(Path(self.resultdir).joinpath(self.suiteuname + ".json"))
+
+    @property
     def is_disabled_by_flagfile(self):
         """The presence of a file DISABLED inside of a Robot suite will prevent
         Robotmk to execute the suite, either by RCC or RobotFramework."""
         return self.path.joinpath("DISABLED").exists()
-
-    @abstractmethod
-    def run(self):
-        pass
-
-    def output(self):
-        # None of the run strategies used for "run" are needed to get the output,
-        # so we can just read the result artifacts from the filesystem.
-        pass
```

### Comparing `robotmk-0.0.56/src/robotmk/executor/scheduler.py` & `robotmk-0.0.58/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.58/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/logger.py` & `robotmk-0.0.58/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/src/robotmk/main.py` & `robotmk-0.0.58/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/config/robotmk.yml` & `robotmk-0.0.58/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/config/test_config.py` & `robotmk-0.0.58/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/context/local/test_local_cli.py` & `robotmk-0.0.58/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.58/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/context/suite/robotmk.yml` & `robotmk-0.0.58/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.58/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/context/test_cli.py` & `robotmk-0.0.58/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/test_robotmk.py` & `robotmk-0.0.58/tests/test_robotmk.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/tests/yml/robotmk.yml` & `robotmk-0.0.58/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.56/PKG-INFO` & `robotmk-0.0.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.56
+Version: 0.0.58
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

