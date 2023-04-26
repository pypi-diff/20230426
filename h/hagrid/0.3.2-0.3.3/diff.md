# Comparing `tmp/hagrid-0.3.2.tar.gz` & `tmp/hagrid-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.2.tar", last modified: Fri Apr 21 03:26:01 2023, max compression
+gzip compressed data, was "hagrid-0.3.3.tar", last modified: Wed Apr 26 05:54:05 2023, max compression
```

## Comparing `hagrid-0.3.2.tar` & `hagrid-0.3.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 03:26:01.325923 hagrid-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-21 03:23:42.000000 hagrid-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134691 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 03:23:57.000000 hagrid-0.3.2/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 03:23:57.000000 hagrid-0.3.2/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:26:01.325923 hagrid-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-21 03:23:57.000000 hagrid-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 05:54:05.928377 hagrid-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-26 05:51:49.000000 hagrid-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.924377 hagrid-0.3.3/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134776 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-26 05:52:04.000000 hagrid-0.3.3/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-26 05:52:04.000000 hagrid-0.3.3/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-26 05:51:49.000000 hagrid-0.3.3/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 05:54:05.000000 hagrid-0.3.3/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 05:54:05.928377 hagrid-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-26 05:52:04.000000 hagrid-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:54:05.928377 hagrid-0.3.3/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-26 05:51:49.000000 hagrid-0.3.3/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.2/README.md` & `hagrid-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/__init__.py` & `hagrid-0.3.3/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/art.py` & `hagrid-0.3.3/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/auth.py` & `hagrid-0.3.3/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/azure.py` & `hagrid-0.3.3/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/cache.py` & `hagrid-0.3.3/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/cli.py` & `hagrid-0.3.3/hagrid/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,17 +289,17 @@
 )
 @click.option(
     "--no-vpn",
     is_flag=True,
     help="Disable tailscale vpn container",
 )
 @click.option(
-    "--silent",
+    "--verbose",
     is_flag=True,
-    help="Suppress extra launch outputs",
+    help="Show verbose output",
 )
 @click.option(
     "--trace",
     required=False,
     type=str,
     help="Optional: allow trace to be turned on or off",
 )
@@ -354,15 +354,18 @@
 
     dry_run = bool(kwargs["cmd"])
 
     health_checks = not bool(kwargs["no_health_checks"])
 
     try:
         tail = bool(kwargs["tail"])
-        silent = not tail
+        verbose = bool(kwargs["verbose"])
+        silent = not verbose
+        if tail:
+            silent = False
 
         from_rendered_dir = bool(kwargs["from_template"]) and EDITABLE_MODE
 
         node_type = verb.get_named_term_type(name="node_type").input
         execute_commands(
             cmds,
             dry_run=dry_run,
@@ -1124,15 +1127,15 @@
 
     parsed_kwargs["oblv"] = bool(kwargs["oblv"])
 
     parsed_kwargs["tls"] = bool(kwargs["tls"])
     parsed_kwargs["test"] = bool(kwargs["test"])
     parsed_kwargs["dev"] = bool(kwargs["dev"])
 
-    parsed_kwargs["silent"] = bool(kwargs["silent"])
+    parsed_kwargs["silent"] = not bool(kwargs["verbose"])
     parsed_kwargs["from_template"] = bool(kwargs["from_template"])
 
     parsed_kwargs["trace"] = False
     if ("trace" not in kwargs or kwargs["trace"] is None) and parsed_kwargs["dev"]:
         # default to trace on in dev mode
         parsed_kwargs["trace"] = True
     elif "trace" in kwargs:
```

### Comparing `hagrid-0.3.2/hagrid/deps.py` & `hagrid-0.3.3/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/grammar.py` & `hagrid-0.3.3/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/land.py` & `hagrid-0.3.3/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/launch.py` & `hagrid-0.3.3/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/lib.py` & `hagrid-0.3.3/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/manifest_template.yml` & `hagrid-0.3.3/hagrid/manifest_template.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.2
-syft_version: 0.8.0-beta.8
-dockerTag: 0.8.0-beta.8
+hagrid_version: 0.3.3
+syft_version: 0.8.0-beta.9
+dockerTag: 0.8.0-beta.9
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: 1c8d04be94dbcf5f9db7e288073dd811ce56f183
+hash: b1396848e85f6e0332983ac9007db3461f81b826
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.2/hagrid/mode.py` & `hagrid-0.3.3/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/names.py` & `hagrid-0.3.3/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/orchestra.py` & `hagrid-0.3.3/hagrid/orchestra.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 
 class NodeType(Enum):
     GATEWAY = "gateway"
     DOMAIN = "domain"
     WORKER = "worker"
     ENCLAVE = "enclave"
     PYTHON = "python"
+    VM = "vm"
 
 
 class NodeHandle:
     def __init__(
         self,
         node_type: NodeType,
         name: str,
@@ -81,15 +82,15 @@
         self.python_node = python_node
         self.shutdown = shutdown
 
     @property
     def client(self) -> Any:
         if self.port:
             sy = get_syft_client()
-            return sy.login(port=self.port)  # type: ignore
+            return sy.login(url=self.url, port=self.port)  # type: ignore
         elif self.node_type == NodeType.PYTHON:
             return self.python_node.guest_client  # type: ignore
 
     def login(
         self, email: Optional[str] = None, password: Optional[str] = None
     ) -> Optional[Any]:
         client = self.client
@@ -97,14 +98,16 @@
             return client.login(email=email, password=password)
         return None
 
     def land(self) -> None:
         if self.node_type == NodeType.PYTHON:
             if self.shutdown:
                 self.shutdown()
+        elif self.node_type == NodeType.VM:
+            pass
         else:
             Orchestra.land(self.name, node_type=self.node_type.value)
 
 
 def get_node_type(node_type: Optional[str]) -> Optional[NodeType]:
     if node_type is None:
         node_type = os.environ.get("ORCHESTRA_NODE_TYPE", NodeType.PYTHON)
@@ -158,14 +161,19 @@
                 )
             else:
                 worker = sy.Domain.named(name, processes=processes, reset=reset, local_db=local_db)  # type: ignore
                 return NodeHandle(
                     node_type=node_type_enum, name=name, python_node=worker
                 )
 
+        if node_type_enum == NodeType.VM:
+            return NodeHandle(
+                node_type=node_type_enum, name=name, port=80, url="http://192.168.56.2"
+            )
+
         # Currently by default we launch in dev mode
         if reset:
             Orchestra.reset(name, node_type)
         else:
             _port = default_port if port is None else port
             if container_exists_with(name=name, port=_port):
                 return NodeHandle(
```

### Comparing `hagrid-0.3.2/hagrid/parse_template.py` & `hagrid-0.3.3/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/quickstart_ui.py` & `hagrid-0.3.3/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/rand_sec.py` & `hagrid-0.3.3/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/style.py` & `hagrid-0.3.3/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/util.py` & `hagrid-0.3.3/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/win_bootstrap.py` & `hagrid-0.3.3/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid/wizard_ui.py` & `hagrid-0.3.3/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.3/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.2/setup.py` & `hagrid-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.2/tests/hagrid/cli_test.py` & `hagrid-0.3.3/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

