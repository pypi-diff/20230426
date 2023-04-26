# Comparing `tmp/xeno-6.0.2.tar.gz` & `tmp/xeno-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xeno-6.0.2.tar", last modified: Tue Apr 25 23:15:45 2023, max compression
+gzip compressed data, was "xeno-6.0.3.tar", last modified: Wed Apr 26 00:40:21 2023, max compression
```

## Comparing `xeno-6.0.2.tar` & `xeno-6.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-25 23:15:45.948836 xeno-6.0.2/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.0.2/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.0.2/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-25 23:15:45.945503 xeno-6.0.2/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.0.2/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-25 23:15:45.948836 xeno-6.0.2/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-25 23:15:28.000000 xeno-6.0.2/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-25 23:15:45.945503 xeno-6.0.2/xeno/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/__init__.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/abstract.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/async_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/attributes.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    17991 2023-04-25 23:15:19.000000 xeno-6.0.2/xeno/build.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-04-25 22:04:51.000000 xeno-6.0.2/xeno/color.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-04-25 17:49:47.000000 xeno-6.0.2/xeno/cookbook.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/decorators.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.0.2/xeno/errors.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/events.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.0.2/xeno/namespaces.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.0.2/xeno/pkg_config.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26055 2023-04-25 17:49:47.000000 xeno-6.0.2/xeno/recipe.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-04-25 17:49:47.000000 xeno-6.0.2/xeno/shell.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-04-25 22:05:30.000000 xeno-6.0.2/xeno/spinner.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/sync_injector.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/testing.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.0.2/xeno/utils.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-25 23:15:45.945503 xeno-6.0.2/xeno.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-25 23:15:45.000000 xeno-6.0.2/xeno.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-25 23:15:45.000000 xeno-6.0.2/xeno.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-25 23:15:45.000000 xeno-6.0.2/xeno.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-25 23:15:45.000000 xeno-6.0.2/xeno.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1567 2023-02-22 19:19:33.000000 xeno-6.0.3/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       18 2023-02-22 19:19:33.000000 xeno-6.0.3/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-26 00:40:21.344179 xeno-6.0.3/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9195 2023-02-22 19:19:33.000000 xeno-6.0.3/README.md
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-04-26 00:40:21.344179 xeno-6.0.3/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1160 2023-04-26 00:40:02.000000 xeno-6.0.3/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/xeno/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/__init__.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10174 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/abstract.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13407 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/async_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7094 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/attributes.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19114 2023-04-26 00:33:27.000000 xeno-6.0.3/xeno/build.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5004 2023-04-25 22:04:51.000000 xeno-6.0.3/xeno/color.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10217 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/cookbook.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4465 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/decorators.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2677 2023-02-22 19:19:33.000000 xeno-6.0.3/xeno/errors.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7250 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/events.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3018 2023-02-22 19:19:33.000000 xeno-6.0.3/xeno/namespaces.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1321 2023-03-04 18:15:00.000000 xeno-6.0.3/xeno/pkg_config.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26055 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/recipe.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7140 2023-04-25 17:49:47.000000 xeno-6.0.3/xeno/shell.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2056 2023-04-25 22:05:30.000000 xeno-6.0.3/xeno/spinner.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7505 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/sync_injector.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1362 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/testing.py
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3258 2023-04-25 17:49:02.000000 xeno-6.0.3/xeno/utils.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-04-26 00:40:21.344179 xeno-6.0.3/xeno.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9816 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      455 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        5 2023-04-26 00:40:21.000000 xeno-6.0.3/xeno.egg-info/top_level.txt
```

### Comparing `xeno-6.0.2/LICENSE` & `xeno-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/PKG-INFO` & `xeno-6.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.0.2
+Version: 6.0.3
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xeno-6.0.2/README.md` & `xeno-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/setup.py` & `xeno-6.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="xeno",
-    version="6.0.2",
+    version="6.0.3",
     description="The Python dependency injector from outer space.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/xeno",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `xeno-6.0.2/xeno/__init__.py` & `xeno-6.0.3/xeno/__init__.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/abstract.py` & `xeno-6.0.3/xeno/abstract.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/async_injector.py` & `xeno-6.0.3/xeno/async_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/attributes.py` & `xeno-6.0.3/xeno/attributes.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/build.py` & `xeno-6.0.3/xeno/build.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,20 +55,22 @@
     class SortingHelpFormatter(HelpFormatter):
         def add_arguments(self, actions):
             actions = sorted(actions, key=lambda a: a.option_strings)
             super().add_arguments(actions)
 
     def __init__(self):
         self.cleanup_mode = self.CleanupMode.NONE
-        self.debug = False
         self.color = "auto"
+        self.debug = False
         self.jobs = multiprocessing.cpu_count()
         self.mode = self.Mode.BUILD
+        self.quiet = False
         self.targets: list[str] = []
         self.tasks: list[str] = []
+        self.to_stdout = False
         self.verbose = 0
 
     def _argparser(self):
         parser = ArgumentParser(
             add_help=False,
             formatter_class=Config.SortingHelpFormatter,
         )
@@ -112,14 +114,26 @@
         parser.add_argument(
             "--verbose",
             "-v",
             action="count",
             help="Print additional diagnostic or help info.",
         )
         parser.add_argument(
+            "--quiet",
+            "-q",
+            action="store_true",
+            help="Only print info/warning/error event contents to stderr, nothing else.",
+        )
+        parser.add_argument(
+            "--to-stdout",
+            "-s",
+            action="store_true",
+            help="Print info event contents to stdout, all else to stderr.",
+        )
+        parser.add_argument(
             "--list",
             "-l",
             dest="mode",
             action="store_const",
             const=self.Mode.LIST,
             help="List all top-level tasks targets.",
         )
@@ -180,15 +194,15 @@
 
     def __init__(self, name="Build Script"):
         self.name = name
         self.bus_hooks: list[EngineHook] = list()
         self.env = Environment.context()
         self.injector = AsyncInjector()
         self.scan = Recipe.Scanner()
-        self.txt = TextDecorator()
+        self.txt = TextDecorator(outfile=sys.stderr)
 
     def add_hook(self, hook: EngineHook):
         self.bus_hooks.append(hook)
 
     async def tasks(self, *, parent: Optional[Recipe] = None) -> list[Recipe]:
         tasks = []
         if parent is None:
@@ -415,14 +429,15 @@
                     return self._list_tasks(config, await self.tasks())
                 case Config.Mode.LIST_ALL:
                     return self._list_tasks(
                         config, (await self.addressable_task_map()).values()
                     )
 
                 case Config.Mode.REBUILD:
+                    tasks = await self._resolve_tasks(config)
                     await self._clean_tasks(config, tasks)
                     return await self._make_tasks(config, tasks)
                 case Config.Mode.TREE:
                     return self._list_task_tree(await self.tasks())
                 case _:
                     raise RuntimeError("Unknown mode encountered.")
 
@@ -458,14 +473,16 @@
 
 
 # --------------------------------------------------------------------
 class DefaultEngineHook:
     def __init__(self):
         self.spinner = Spinner("resolving")
         self.txt: Optional[TextDecorator] = None
+        self.quiet = False
+        self.to_stdout = False
 
     def embrace(self, *content, **kwargs):
         assert self.txt
         return self.txt.embrace(*content, **kwargs)
 
     def print(self, *content, **kwargs):
         assert self.txt
@@ -473,49 +490,69 @@
 
     def sigil(self, event):
         return event.context.sigil().replace(
             Recipe.SIGIL_DELIMITER, event.context.fmt.symbols.target
         )
 
     async def on_frame(self, event):
+        if self.quiet:
+            return
         assert self.txt
         self.spinner.message = f"resolving [{len(Recipe.active)}]"
         self.txt.wipe = await self.spinner.spin()
 
     def on_clean(self, event):
+        if self.quiet:
+            return
         self.embrace(self.sigil(event), fg="green", render="bold")
         self.print(event.context.fmt.clean(event.context))
 
     def on_error(self, event):
-        self.embrace(self.sigil(event), fg="red", render="bold")
+        if not self.quiet:
+            self.embrace(self.sigil(event), fg="red", render="bold")
         self.print(event.data)
 
     def on_fail(self, event):
+        if self.quiet:
+            return
         self.embrace(self.sigil(event), fg="white", bg="red", render="bold")
         self.print(event.context.fmt.fail(event.context))
 
     def on_info(self, event: Event):
-        self.embrace(self.sigil(event), fg="white", render="dim")
-        self.print(event.data, fg="white", render="dim")
+        if not self.quiet and not self.to_stdout:
+            self.embrace(self.sigil(event), fg="white", render="dim")
+        if self.to_stdout:
+            print(event.data)
+        else:
+            self.print(event.data, fg="white", render="dim")
 
     def on_start(self, event: Event):
+        if self.quiet:
+            return
         self.embrace(self.sigil(event), fg="cyan", render="bold")
         self.print(event.context.fmt.start(event.context))
 
     def on_success(self, event: Event):
+        if self.quiet:
+            return
         self.embrace(self.sigil(event), fg="green", render="bold")
         self.print(event.context.fmt.ok(event.context))
 
     def on_warning(self, event: Event):
-        self.embrace(self.sigil(event), fg="yellow", render="bold")
-        self.print(event.data, fg="yellow", render="dim")
+        if not self.quiet:
+            self.embrace(self.sigil(event), fg="yellow", render="bold")
+            self.print(event.data, fg="yellow", render="dim")
+        else:
+            self.print(event.data)
 
     def __call__(self, config: Config, engine: Engine, bus: EventBus):
         self.txt = engine.txt
         self.spinner.colorized = is_color_enabled()
+        self.quiet = config.quiet
+        self.to_stdout = config.to_stdout
         bus.subscribe(Events.CLEAN, self.on_clean)
         bus.subscribe(Events.ERROR, self.on_error)
         bus.subscribe(Events.FAIL, self.on_fail)
         bus.subscribe(Events.INFO, self.on_info)
         bus.subscribe(Events.START, self.on_start)
         bus.subscribe(Events.SUCCESS, self.on_success)
         bus.subscribe(Events.WARNING, self.on_warning)
```

### Comparing `xeno-6.0.2/xeno/color.py` & `xeno-6.0.3/xeno/color.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/cookbook.py` & `xeno-6.0.3/xeno/cookbook.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/decorators.py` & `xeno-6.0.3/xeno/decorators.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/errors.py` & `xeno-6.0.3/xeno/errors.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/events.py` & `xeno-6.0.3/xeno/events.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/namespaces.py` & `xeno-6.0.3/xeno/namespaces.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/pkg_config.py` & `xeno-6.0.3/xeno/pkg_config.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/recipe.py` & `xeno-6.0.3/xeno/recipe.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/shell.py` & `xeno-6.0.3/xeno/shell.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/spinner.py` & `xeno-6.0.3/xeno/spinner.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/sync_injector.py` & `xeno-6.0.3/xeno/sync_injector.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/testing.py` & `xeno-6.0.3/xeno/testing.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno/utils.py` & `xeno-6.0.3/xeno/utils.py`

 * *Files identical despite different names*

### Comparing `xeno-6.0.2/xeno.egg-info/PKG-INFO` & `xeno-6.0.3/xeno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xeno
-Version: 6.0.2
+Version: 6.0.3
 Summary: The Python dependency injector from outer space.
 Home-page: https://github.com/lainproliant/xeno
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: IOC dependency injector
 Classifier: Development Status :: 5 - Production/Stable
```

