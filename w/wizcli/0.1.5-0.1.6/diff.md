# Comparing `tmp/wizcli-0.1.5.tar.gz` & `tmp/wizcli-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizcli-0.1.5.tar", max compression
+gzip compressed data, was "wizcli-0.1.6.tar", max compression
```

## Comparing `wizcli-0.1.5.tar` & `wizcli-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      281 2023-04-23 23:26:05.956812 wizcli-0.1.5/README.md
--rw-r--r--   0        0        0      530 2023-04-23 23:26:05.956812 wizcli-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2332 2023-04-23 23:26:05.956812 wizcli-0.1.5/wizcli/cli.py
--rw-r--r--   0        0        0     2392 2023-04-23 23:26:05.956812 wizcli-0.1.5/wizcli/wiz.py
--rw-r--r--   0        0        0      878 1970-01-01 00:00:00.000000 wizcli-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      891 2023-04-25 18:05:32.944945 wizcli-0.1.6/README.md
+-rw-r--r--   0        0        0      530 2023-04-25 18:05:32.944945 wizcli-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2334 2023-04-25 18:05:32.944945 wizcli-0.1.6/wizcli/cli.py
+-rw-r--r--   0        0        0     2392 2023-04-25 18:05:32.944945 wizcli-0.1.6/wizcli/wiz.py
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 wizcli-0.1.6/PKG-INFO
```

### Comparing `wizcli-0.1.5/pyproject.toml` & `wizcli-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wizcli"
-version = "0.1.5"
+version = "0.1.6"
 description = "control WiZ bulbs from the CLI"
 authors = ["Agustin B <redraw@sdf.org>"]
 readme = "README.md"
 repository = "https://github.com/redraw/wizcli"
 
 [tool.poetry.scripts]
 wiz = 'wizcli.cli:run'
```

### Comparing `wizcli-0.1.5/wizcli/cli.py` & `wizcli-0.1.6/wizcli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     port: int = typer.Option(38899, "--port", "-p", envvar="WIZ_PORT", help="WiZ bulb port"),
     timeout: int = typer.Option(5, "--timeout", "-t", envvar="WIZ_TIMEOUT", help="Timeout in seconds"),
     verbose: bool = typer.Option(False, "--verbose", "-v"),
 ):
     logging.basicConfig(level=logging.DEBUG if verbose else logging.ERROR)
 
     if not host:
-        logger.info("Missing host.")
+        logger.error("Missing host.")
         raise typer.Abort()
 
     logger.info(f"WiZ {host=} {port=}")
 
     ctx.obj = State(
         wiz=Wiz(host, port, timeout=timeout),
     )
@@ -102,8 +102,8 @@
 
 
 @run.command()
 def get(
     ctx: typer.Context
 ):
     state = ctx.obj.wiz.get_state()
-    json.dump(state, sys.stdout, indent=2)
+    json.dump(state, sys.stdout, indent=2)
```

### Comparing `wizcli-0.1.5/wizcli/wiz.py` & `wizcli-0.1.6/wizcli/wiz.py`

 * *Files identical despite different names*

