# Comparing `tmp/robocorp_tasks-0.1.4.tar.gz` & `tmp/robocorp_tasks-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.1.4.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.1.5.tar", max compression
```

## Comparing `robocorp_tasks-0.1.4.tar` & `robocorp_tasks-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0      463 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/README.md
--rw-r--r--   0        0        0      944 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      108 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     3472 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1230 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     4991 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0      155 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0      627 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     4531 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2335 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     1699 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0      933 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0     5507 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0      638 2023-04-23 12:19:08.305974 robocorp_tasks-0.1.4/src/robocorp/tasks/decorators.py
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4799 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/README.md
+-rw-r--r--   0        0        0     1214 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     3371 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1230 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5048 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     5284 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0      638 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_decorators.py
+-rw-r--r--   0        0        0      182 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0      599 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     4519 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0     2335 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     1699 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0      933 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      809 2023-04-25 15:08:39.286338 robocorp_tasks-0.1.5/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.5/PKG-INFO
```

### Comparing `robocorp_tasks-0.1.4/pyproject.toml` & `robocorp_tasks-0.1.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.1.4"
+version = "0.1.5"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.0.11"
+robocorp-log = "0.0.12"
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_argdispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
 
     def _create_argparser(self):
         import argparse
 
         parser = argparse.ArgumentParser(
             prog="robocorp.tasks",
             description="Robocorp framework for RPA development using Python.",
-            # TODO: Add a proper epilog once we have an actual url to point to.
-            # epilog="View https://github.com/robocorp/draft-python-framework/ for more information",
+            epilog="View https://github.com/robocorp/robo for more information",
         )
 
         subparsers = parser.add_subparsers(dest="command")
 
         # Run
         run_parser = subparsers.add_parser(
             "run",
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_collect_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -129,15 +129,17 @@
                 task = Task(module, method)
                 if accept_task(task):
                     yield task
 
             del methods_marked_as_tasks_found[:]
 
         else:
-            from ._exceptions import RoboCollectError
+            from ._exceptions import RobocorpTasksCollectError
 
             if not path.exists():
-                raise RoboCollectError(f"Path: {path} does not exist")
+                raise RobocorpTasksCollectError(f"Path: {path} does not exist")
 
-            raise RoboCollectError(f"Expected {path} to map to a directory or file.")
+            raise RobocorpTasksCollectError(
+                f"Expected {path} to map to a directory or file."
+            )
     finally:
         _hooks.on_task_func_found.unregister(methods_marked_as_tasks_found.append)
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_hooks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from robocorp.tasks._callback import Callback
-from robocorp.tasks._protocols import (
+from ._callback import Callback
+from ._protocols import (
     IOnTaskFuncFoundCallback,
     IBeforeCollectTasksCallback,
     IBeforeTaskRunCallback,
     IAfterTaskRunCallback,
 )
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_log_auto_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,14 @@
 
 def _log_before_task_run(task: ITask):
     log.start_task(
         task.name,
         task.module_name,
         task.filename,
         task.method.__code__.co_firstlineno,
-        [],
     )
 
 
 def _log_after_task_run(task: ITask):
     status = task.status
     log.end_task(task.name, task.module_name, status, task.message)
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_log_output_setup.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_log_output_setup.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_protocols.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/_task.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_task.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from typing import Tuple
 
 import json
 import os
 import sys
 import traceback
 
-from ._argdispatch import arg_dispatch
+from ._argdispatch import arg_dispatch as _arg_dispatch
 
 
 # Note: the args must match the 'dest' on the configured argparser.
-@arg_dispatch.register(name="list")
+@_arg_dispatch.register(name="list")
 def list_tasks(
     path: str,
 ) -> int:
     """
     Prints the tasks available at a given path to the stdout in json format.
 
     [
@@ -53,15 +53,15 @@
         )
 
     sys.stdout.write(json.dumps(tasks_found))
     return 0
 
 
 # Note: the args must match the 'dest' on the configured argparser.
-@arg_dispatch.register()
+@_arg_dispatch.register()
 def run(
     output_dir: str,
     path: str,
     task_name: str,
     max_log_files: int = 5,
     max_log_file_size: str = "1MB",
 ) -> int:
@@ -81,15 +81,15 @@
         1 if there was some error running the task.
     """
     from ._collect_tasks import collect_tasks
     from ._hooks import before_task_run, after_task_run
     from ._protocols import ITask
     from ._task import Context
     from ._protocols import Status
-    from ._exceptions import RoboCollectError
+    from ._exceptions import RobocorpTasksCollectError
     from ._log_auto_setup import (
         setup_cli_auto_logging,
         read_filters_from_pyproject_toml,
     )
     from ._log_output_setup import setup_log_output, setup_stdout_logging
 
     # Don't show internal machinery on tracebacks:
@@ -119,66 +119,55 @@
         run_status = "PASS"
         setup_message = ""
 
         run_name = f"{os.path.basename(path)} - {task_name}"
         log.start_run(run_name)
 
         try:
-            log.start_task("Collect tasks", "setup", "", 0, [])
+            log.start_task("Collect tasks", "setup", "", 0)
             try:
                 if not task_name:
                     context.show(f"\nCollecting tasks from: {path}")
                 else:
                     context.show(f"\nCollecting task {task_name} from: {path}")
 
                 tasks: Tuple[ITask, ...] = tuple(collect_tasks(p, task_name))
 
                 if not tasks:
-                    raise RoboCollectError(f"Did not find any tasks in: {path}")
+                    raise RobocorpTasksCollectError(
+                        f"Did not find any tasks in: {path}"
+                    )
                 if len(tasks) > 1:
-                    raise RoboCollectError(
+                    raise RobocorpTasksCollectError(
                         f"Expected only 1 task to be run. Found: {', '.join(t.name for t in tasks)}"
                     )
             except Exception as e:
                 run_status = "ERROR"
                 setup_message = str(e)
                 log.exception()
 
-                if not isinstance(e, RoboCollectError):
+                if not isinstance(e, RobocorpTasksCollectError):
                     traceback.print_exc()
                 else:
                     context.show_error(setup_message)
 
                 return 1
             finally:
                 log.end_task("Collect tasks", "setup", run_status, setup_message)
 
+            returncode = 0
+
             for task in tasks:
                 before_task_run(task)
                 try:
                     task.run()
                     run_status = task.status = Status.PASS
                 except Exception as e:
                     run_status = task.status = Status.ERROR
+                    returncode = 1
                     task.message = str(e)
                 finally:
                     after_task_run(task)
 
-                returncode = 0 if task.status == Status.PASS else 1
-                return returncode
-
-            raise AssertionError("Should never get here.")
+            return returncode
         finally:
             log.end_run(run_name, run_status)
-
-
-def main(args=None, exit: bool = True) -> int:
-    if args is None:
-        args = sys.argv[1:]
-    returncode = arg_dispatch.process_args(args)
-    if exit:
-        sys.exit(returncode)
-    return returncode
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `robocorp_tasks-0.1.4/src/robocorp/tasks/decorators.py` & `robocorp_tasks-0.1.5/src/robocorp/tasks/_decorators.py`

 * *Files identical despite different names*

