# Comparing `tmp/robotmk-0.0.58.tar.gz` & `tmp/robotmk-0.0.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotmk-0.0.58.tar", last modified: Wed Apr 26 18:41:27 2023, max compression
+gzip compressed data, was "robotmk-0.0.59.tar", last modified: Wed Apr 26 19:15:47 2023, max compression
```

## Comparing `robotmk-0.0.58.tar` & `robotmk-0.0.59.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0      110 2023-04-26 18:41:17.217259 robotmk-0.0.58/.bumpversion.cfg
--rw-r--r--   0        0        0      279 2023-04-25 15:17:21.816448 robotmk-0.0.58/.cli.env
--rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.58/README.md
--rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.58/pyproject.toml
--rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.58/src/categories.json
--rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.58/src/click_tutorial.py
--rw-r--r--   0        0        0       92 2023-04-26 18:41:17.217259 robotmk-0.0.58/src/robotmk/__init__.py
--rw-r--r--   0        0        0     5531 2023-04-26 09:17:32.607360 robotmk-0.0.58/src/robotmk/cli/cli.py
--rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.58/src/robotmk/cli/defaultgroup.py
--rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.58/src/robotmk/config/__init__.py
--rw-r--r--   0        0        0    17973 2023-04-14 12:38:42.931817 robotmk-0.0.58/src/robotmk/config/config.py
--rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.58/src/robotmk/config/yml.py
--rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.58/src/robotmk/context/__init__.py
--rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.58/src/robotmk/context/abstract.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.58/src/robotmk/context/agent/__init__.py
--rw-r--r--   0        0        0     2086 2023-04-26 12:58:54.634165 robotmk-0.0.58/src/robotmk/context/agent/agent.py
--rw-r--r--   0        0        0     1580 2023-04-26 12:34:36.526163 robotmk-0.0.58/src/robotmk/context/agent/cli.py
--rw-r--r--   0        0        0      681 2023-04-26 12:37:20.188228 robotmk-0.0.58/src/robotmk/context/context.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.58/src/robotmk/context/server/__init__.py
--rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.58/src/robotmk/context/server/cli.py
--rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.58/src/robotmk/context/server/server.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.58/src/robotmk/context/specialagent/__init__.py
--rw-r--r--   0        0        0     1112 2023-04-26 12:27:48.266927 robotmk-0.0.58/src/robotmk/context/specialagent/cli.py
--rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.58/src/robotmk/context/specialagent/specialagent.py
--rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.58/src/robotmk/context/suite/__init__.py
--rw-r--r--   0        0        0     3995 2023-04-26 10:06:25.887510 robotmk-0.0.58/src/robotmk/context/suite/cli.py
--rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.58/src/robotmk/context/suite/strategies/__init__.py
--rw-r--r--   0        0        0     7380 2023-04-25 13:50:39.300240 robotmk-0.0.58/src/robotmk/context/suite/strategies/run.py
--rw-r--r--   0        0        0     2849 2023-04-26 13:44:29.789250 robotmk-0.0.58/src/robotmk/context/suite/suite.py
--rw-r--r--   0        0        0      135 2023-04-26 13:29:57.729591 robotmk-0.0.58/src/robotmk/context/suite/target/__init__.py
--rw-r--r--   0        0        0     1432 2023-04-26 17:05:40.456944 robotmk-0.0.58/src/robotmk/context/suite/target/abstract.py
--rw-r--r--   0        0        0     1604 2023-04-26 13:40:32.915503 robotmk-0.0.58/src/robotmk/context/suite/target/factory.py
--rw-r--r--   0        0        0     2686 2023-04-26 16:31:12.211225 robotmk-0.0.58/src/robotmk/context/suite/target/local.py
--rw-r--r--   0        0        0     5628 2023-04-26 13:29:57.729591 robotmk-0.0.58/src/robotmk/context/suite/target/rcc.py
--rw-r--r--   0        0        0     2208 2023-04-26 17:23:25.018107 robotmk-0.0.58/src/robotmk/context/suite/target/remote.py
--rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/__init__.py
--rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/retry.py
--rw-r--r--   0        0        0     6339 2023-04-26 13:35:01.378678 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/robotframework.py
--rw-r--r--   0        0        0     4877 2023-04-26 18:10:20.939058 robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/state.py
--rw-r--r--   0        0        0     3878 2023-04-26 13:32:58.143863 robotmk-0.0.58/src/robotmk/context/suite/target/target.py
--rw-r--r--   0        0        0     3932 2023-04-26 18:38:03.011146 robotmk-0.0.58/src/robotmk/emitter.py
--rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.58/src/robotmk/executor/__init__.py
--rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.58/src/robotmk/executor/abstract.py
--rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.58/src/robotmk/executor/scheduler.py
--rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.58/src/robotmk/executor/sequencer.py
--rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.58/src/robotmk/executor/suiterunner.py
--rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.58/src/robotmk/logger.py
--rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.58/src/robotmk/main.py
--rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.58/tests/__init__.py
--rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.58/tests/config/robotmk.env
--rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.58/tests/config/robotmk.yml
--rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.58/tests/config/test_config.py
--rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.58/tests/context/local/robotmk.yml
--rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.58/tests/context/local/test_local_cli.py
--rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.58/tests/context/specialagent/test_specialagent_cli.py
--rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.58/tests/context/suite/robotmk.yml
--rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.58/tests/context/suite/test_suite.py
--rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.58/tests/context/suite/test_suite_cli.py
--rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.58/tests/context/test_cli.py
--rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.58/tests/test_robotmk.py
--rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.58/tests/yml/robotmk.yml
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.58/PKG-INFO
+-rw-r--r--   0        0        0      110 2023-04-26 19:15:34.684949 robotmk-0.0.59/.bumpversion.cfg
+-rw-r--r--   0        0        0      279 2023-04-25 15:17:21.816448 robotmk-0.0.59/.cli.env
+-rw-r--r--   0        0        0       40 2023-02-24 13:10:55.692823 robotmk-0.0.59/README.md
+-rw-r--r--   0        0        0      755 2023-04-14 12:23:02.253430 robotmk-0.0.59/pyproject.toml
+-rw-r--r--   0        0        0    25966 2023-03-09 10:38:47.105752 robotmk-0.0.59/src/categories.json
+-rw-r--r--   0        0        0     2161 2023-03-09 11:10:22.787194 robotmk-0.0.59/src/click_tutorial.py
+-rw-r--r--   0        0        0       92 2023-04-26 19:15:34.684949 robotmk-0.0.59/src/robotmk/__init__.py
+-rw-r--r--   0        0        0     5531 2023-04-26 09:17:32.607360 robotmk-0.0.59/src/robotmk/cli/cli.py
+-rw-r--r--   0        0        0     3033 2023-03-16 11:52:36.253603 robotmk-0.0.59/src/robotmk/cli/defaultgroup.py
+-rw-r--r--   0        0        0       64 2023-03-30 15:36:25.625426 robotmk-0.0.59/src/robotmk/config/__init__.py
+-rw-r--r--   0        0        0    18059 2023-04-26 18:46:09.822405 robotmk-0.0.59/src/robotmk/config/config.py
+-rw-r--r--   0        0        0     2498 2023-03-30 14:32:11.107185 robotmk-0.0.59/src/robotmk/config/yml.py
+-rw-r--r--   0        0        0      178 2023-03-14 15:49:36.083594 robotmk-0.0.59/src/robotmk/context/__init__.py
+-rw-r--r--   0        0        0     2306 2023-04-13 11:26:21.934600 robotmk-0.0.59/src/robotmk/context/abstract.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:26.579374 robotmk-0.0.59/src/robotmk/context/agent/__init__.py
+-rw-r--r--   0        0        0     2086 2023-04-26 12:58:54.634165 robotmk-0.0.59/src/robotmk/context/agent/agent.py
+-rw-r--r--   0        0        0     1579 2023-04-26 18:42:24.872602 robotmk-0.0.59/src/robotmk/context/agent/cli.py
+-rw-r--r--   0        0        0      681 2023-04-26 12:37:20.188228 robotmk-0.0.59/src/robotmk/context/context.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:31.416463 robotmk-0.0.59/src/robotmk/context/server/__init__.py
+-rw-r--r--   0        0        0      501 2023-04-04 10:17:35.143381 robotmk-0.0.59/src/robotmk/context/server/cli.py
+-rw-r--r--   0        0        0        0 2023-03-16 12:36:40.036375 robotmk-0.0.59/src/robotmk/context/server/server.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:27.895361 robotmk-0.0.59/src/robotmk/context/specialagent/__init__.py
+-rw-r--r--   0        0        0     1112 2023-04-26 12:27:48.266927 robotmk-0.0.59/src/robotmk/context/specialagent/cli.py
+-rw-r--r--   0        0        0     1892 2023-04-25 09:19:43.794680 robotmk-0.0.59/src/robotmk/context/specialagent/specialagent.py
+-rw-r--r--   0        0        0        0 2023-03-10 09:07:29.079350 robotmk-0.0.59/src/robotmk/context/suite/__init__.py
+-rw-r--r--   0        0        0     3995 2023-04-26 10:06:25.887510 robotmk-0.0.59/src/robotmk/context/suite/cli.py
+-rw-r--r--   0        0        0      125 2023-04-01 20:18:16.209113 robotmk-0.0.59/src/robotmk/context/suite/strategies/__init__.py
+-rw-r--r--   0        0        0     7380 2023-04-25 13:50:39.300240 robotmk-0.0.59/src/robotmk/context/suite/strategies/run.py
+-rw-r--r--   0        0        0     2849 2023-04-26 13:44:29.789250 robotmk-0.0.59/src/robotmk/context/suite/suite.py
+-rw-r--r--   0        0        0      135 2023-04-26 13:29:57.729591 robotmk-0.0.59/src/robotmk/context/suite/target/__init__.py
+-rw-r--r--   0        0        0     1432 2023-04-26 17:05:40.456944 robotmk-0.0.59/src/robotmk/context/suite/target/abstract.py
+-rw-r--r--   0        0        0     1604 2023-04-26 13:40:32.915503 robotmk-0.0.59/src/robotmk/context/suite/target/factory.py
+-rw-r--r--   0        0        0     2686 2023-04-26 16:31:12.211225 robotmk-0.0.59/src/robotmk/context/suite/target/local.py
+-rw-r--r--   0        0        0     5628 2023-04-26 13:29:57.729591 robotmk-0.0.59/src/robotmk/context/suite/target/rcc.py
+-rw-r--r--   0        0        0     2245 2023-04-26 18:48:30.732980 robotmk-0.0.59/src/robotmk/context/suite/target/remote.py
+-rw-r--r--   0        0        0       49 2023-04-03 17:11:56.923310 robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/__init__.py
+-rw-r--r--   0        0        0     5576 2023-04-25 14:21:05.706886 robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/retry.py
+-rw-r--r--   0        0        0     6339 2023-04-26 13:35:01.378678 robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/robotframework.py
+-rw-r--r--   0        0        0     4877 2023-04-26 18:10:20.939058 robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/state.py
+-rw-r--r--   0        0        0     3878 2023-04-26 13:32:58.143863 robotmk-0.0.59/src/robotmk/context/suite/target/target.py
+-rw-r--r--   0        0        0     3932 2023-04-26 18:38:03.011146 robotmk-0.0.59/src/robotmk/emitter.py
+-rw-r--r--   0        0        0        0 2023-03-16 16:00:58.422756 robotmk-0.0.59/src/robotmk/executor/__init__.py
+-rw-r--r--   0        0        0      438 2023-03-21 06:35:39.773943 robotmk-0.0.59/src/robotmk/executor/abstract.py
+-rw-r--r--   0        0        0     4287 2023-04-14 12:18:48.728192 robotmk-0.0.59/src/robotmk/executor/scheduler.py
+-rw-r--r--   0        0        0      287 2023-03-20 12:52:46.348308 robotmk-0.0.59/src/robotmk/executor/sequencer.py
+-rw-r--r--   0        0        0      552 2023-03-21 11:00:25.331460 robotmk-0.0.59/src/robotmk/executor/suiterunner.py
+-rw-r--r--   0        0        0     2088 2023-04-25 12:24:30.689639 robotmk-0.0.59/src/robotmk/logger.py
+-rw-r--r--   0        0        0     3514 2023-04-25 12:30:37.990565 robotmk-0.0.59/src/robotmk/main.py
+-rw-r--r--   0        0        0        0 2023-03-04 11:04:47.025603 robotmk-0.0.59/tests/__init__.py
+-rw-r--r--   0        0        0       25 2023-04-12 14:35:21.918852 robotmk-0.0.59/tests/config/robotmk.env
+-rw-r--r--   0        0        0     2075 2023-04-04 09:03:29.524056 robotmk-0.0.59/tests/config/robotmk.yml
+-rw-r--r--   0        0        0    10489 2023-04-13 09:43:10.811649 robotmk-0.0.59/tests/config/test_config.py
+-rw-r--r--   0        0        0      300 2023-03-14 15:05:35.715975 robotmk-0.0.59/tests/context/local/robotmk.yml
+-rw-r--r--   0        0        0     1265 2023-03-16 08:41:25.311423 robotmk-0.0.59/tests/context/local/test_local_cli.py
+-rw-r--r--   0        0        0      746 2023-03-14 15:06:49.651217 robotmk-0.0.59/tests/context/specialagent/test_specialagent_cli.py
+-rw-r--r--   0        0        0     2075 2023-04-04 10:39:17.810567 robotmk-0.0.59/tests/context/suite/robotmk.yml
+-rw-r--r--   0        0        0      427 2023-04-04 10:41:57.860986 robotmk-0.0.59/tests/context/suite/test_suite.py
+-rw-r--r--   0        0        0      842 2023-04-03 10:50:55.769100 robotmk-0.0.59/tests/context/suite/test_suite_cli.py
+-rw-r--r--   0        0        0      991 2023-03-14 11:06:07.698634 robotmk-0.0.59/tests/context/test_cli.py
+-rw-r--r--   0        0        0     1143 2023-04-25 09:15:14.565152 robotmk-0.0.59/tests/test_robotmk.py
+-rw-r--r--   0        0        0      945 2023-03-20 10:00:06.880076 robotmk-0.0.59/tests/yml/robotmk.yml
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 robotmk-0.0.59/PKG-INFO
```

### Comparing `robotmk-0.0.58/pyproject.toml` & `robotmk-0.0.59/pyproject.toml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/categories.json` & `robotmk-0.0.59/src/categories.json`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/click_tutorial.py` & `robotmk-0.0.59/src/click_tutorial.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/cli/cli.py` & `robotmk-0.0.59/src/robotmk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/cli/defaultgroup.py` & `robotmk-0.0.59/src/robotmk/cli/defaultgroup.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/config/config.py` & `robotmk-0.0.59/src/robotmk/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,17 +458,19 @@
             print(f"{varname} = {d}")
             if environ is None:
                 os.environ[varname] = str(d)
             else:
                 environ[varname] = str(d)
 
     def to_yml(self, file=None) -> Union[str, None]:
-        """Dumps the config to a file returns it."""
+        """Dumps the config to a file or returns it."""
         if file:
             try:
                 with open(file, "w") as f:
                     yaml.dump(self.configdict, f)
             except Exception as e:
                 print(f"Could not write to file {file}: {e}")
                 return None
         else:
-            return yaml.dump(self.configdict)
+            return yaml.dump(
+                self.configdict, sort_keys=False, indent=4, default_flow_style=False
+            )
```

### Comparing `robotmk-0.0.58/src/robotmk/config/yml.py` & `robotmk-0.0.59/src/robotmk/config/yml.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/abstract.py` & `robotmk-0.0.59/src/robotmk/context/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/agent/agent.py` & `robotmk-0.0.59/src/robotmk/context/agent/agent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/agent/cli.py` & `robotmk-0.0.59/src/robotmk/context/agent/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,26 +28,26 @@
         click.secho("No subcommand given. Use --help for help.", fg="red")
         sys.exit(1)
 
 
 @agent.command()
 @click.pass_context
 def scheduler(ctx):
-    """Start the scheduler to execute tests repeatedly."""
+    """Starts the scheduler to execute tests repeatedly."""
     ctx.obj.execute()
 
 
 @agent.command()
 @click.pass_context
 def output(ctx):
-    """Produces Checkmk Agent output for all suite results."""
+    """Emits Checkmk Agent output for all suite results."""
     data = ctx.obj.output()
     click.secho(data, fg="bright_white")
 
 
-@agent.command(help="Dump the config as YML to STDOUT or FILE")
+@agent.command(help="Dumps the config as YML to STDOUT or FILE")
 # add file arg
 @click.argument("file", required=False, type=click.Path(exists=False))
 @click.pass_context
 def ymldump(ctx, file):
     click.secho(ctx.obj.config.to_yml(file), fg="bright_white")
     sys.exit(0)
```

### Comparing `robotmk-0.0.58/src/robotmk/context/context.py` & `robotmk-0.0.59/src/robotmk/context/context.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/specialagent/cli.py` & `robotmk-0.0.59/src/robotmk/context/specialagent/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/specialagent/specialagent.py` & `robotmk-0.0.59/src/robotmk/context/specialagent/specialagent.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/cli.py` & `robotmk-0.0.59/src/robotmk/context/suite/cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/strategies/run.py` & `robotmk-0.0.59/src/robotmk/context/suite/strategies/run.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/suite.py` & `robotmk-0.0.59/src/robotmk/context/suite/suite.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/abstract.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/abstract.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/factory.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/factory.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/local.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/local.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/rcc.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/rcc.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/remote.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/remote.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class RemoteTarget(Target):
     def __init__(self, suiteuname: str, config: dict, logger: RobotmkLogger):
         super().__init__(suiteuname, config, logger)
 
     def run(self):
+        print("NOT YET IMPLEMENTED")
         pass
 
     def output(self):
         # return a dummy dict from a dummy REST API call
         # TODO: implement REST API Call to Robocorp to fetch the output
         return {
             "suiteuname": self.suiteuname,
```

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/retry.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/retry.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/robotframework.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/robotframework.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/robotframework/state.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/robotframework/state.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/context/suite/target/target.py` & `robotmk-0.0.59/src/robotmk/context/suite/target/target.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/emitter.py` & `robotmk-0.0.59/src/robotmk/emitter.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/executor/scheduler.py` & `robotmk-0.0.59/src/robotmk/executor/scheduler.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/executor/suiterunner.py` & `robotmk-0.0.59/src/robotmk/executor/suiterunner.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/logger.py` & `robotmk-0.0.59/src/robotmk/logger.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/src/robotmk/main.py` & `robotmk-0.0.59/src/robotmk/main.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/config/robotmk.yml` & `robotmk-0.0.59/tests/config/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/config/test_config.py` & `robotmk-0.0.59/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/context/local/test_local_cli.py` & `robotmk-0.0.59/tests/context/local/test_local_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/context/specialagent/test_specialagent_cli.py` & `robotmk-0.0.59/tests/context/specialagent/test_specialagent_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/context/suite/robotmk.yml` & `robotmk-0.0.59/tests/context/suite/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/context/suite/test_suite_cli.py` & `robotmk-0.0.59/tests/context/suite/test_suite_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/context/test_cli.py` & `robotmk-0.0.59/tests/context/test_cli.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/test_robotmk.py` & `robotmk-0.0.59/tests/test_robotmk.py`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/tests/yml/robotmk.yml` & `robotmk-0.0.59/tests/yml/robotmk.yml`

 * *Files identical despite different names*

### Comparing `robotmk-0.0.58/PKG-INFO` & `robotmk-0.0.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotmk
-Version: 0.0.58
+Version: 0.0.59
 Summary: Robot Framework test execution and result parsing for Check_MK
 Keywords: robotmk,checkmk,robotframework,automation,monitoring
 Author-email: Simon Meggle <simon.meggle@elabit.de>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: click
 Requires-Dist: psutil
```

