# Comparing `tmp/flaggie-0.99.3.tar.gz` & `tmp/flaggie-0.99.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaggie-0.99.3.tar", last modified: Wed Feb 15 16:48:30 2023, max compression
+gzip compressed data, was "flaggie-0.99.4.tar", last modified: Wed Apr 26 13:12:33 2023, max compression
```

## Comparing `flaggie-0.99.3.tar` & `flaggie-0.99.4.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.3/COPYING
--rw-r--r--   0        0        0       84 2023-02-15 16:46:37.841431 flaggie-0.99.3/flaggie/__init__.py
--rw-r--r--   0        0        0    12734 2023-01-20 18:33:51.144880 flaggie-0.99.3/flaggie/__main__.py
--rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.3/flaggie/config.py
--rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.3/flaggie/mangle.py
--rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.3/flaggie/pm.py
--rw-r--r--   0        0        0     1058 2023-01-18 16:52:52.021732 flaggie-0.99.3/pyproject.toml
--rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-01-15 07:39:45.197204 flaggie-0.99.4/COPYING
+-rw-r--r--   0        0        0       84 2023-04-26 13:10:44.388852 flaggie-0.99.4/flaggie/__init__.py
+-rw-r--r--   0        0        0    12830 2023-04-26 13:10:43.098826 flaggie-0.99.4/flaggie/__main__.py
+-rw-r--r--   0        0        0     6739 2023-01-15 07:39:45.200537 flaggie-0.99.4/flaggie/config.py
+-rw-r--r--   0        0        0    14319 2023-01-20 19:03:37.545724 flaggie-0.99.4/flaggie/mangle.py
+-rw-r--r--   0        0        0     7288 2023-02-15 16:46:20.320855 flaggie-0.99.4/flaggie/pm.py
+-rw-r--r--   0        0        0     1118 2023-04-26 13:10:43.742172 flaggie-0.99.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-15 07:39:45.200537 flaggie-0.99.4/test/__init__.py
+-rw-r--r--   0        0        0     4723 2023-01-15 07:39:45.200537 flaggie-0.99.4/test/test_config.py
+-rw-r--r--   0        0        0     1845 2023-01-15 16:47:15.640493 flaggie-0.99.4/test/test_main.py
+-rw-r--r--   0        0        0    16203 2023-01-20 19:03:53.062748 flaggie-0.99.4/test/test_mangle.py
+-rw-r--r--   0        0        0     7205 2023-02-15 16:46:20.320855 flaggie-0.99.4/test/test_pm.py
+-rw-r--r--   0        0        0      464 2023-01-15 07:39:45.200537 flaggie-0.99.4/tox.ini
+-rw-r--r--   0        0        0      550 1970-01-01 00:00:00.000000 flaggie-0.99.4/PKG-INFO
```

### Comparing `flaggie-0.99.3/COPYING` & `flaggie-0.99.4/COPYING`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.3/flaggie/__main__.py` & `flaggie-0.99.4/flaggie/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,28 +175,32 @@
                    "disambiguate")
     return next(iter(matched_types))[0]
 
 
 def main(prog_name: str, *argv: str) -> int:
     # same as argparse default, enforce for consistency
     help_width = shutil.get_terminal_size().columns - 2
+    if help_width > 10:
+        epilog = "\n".join(textwrap.fill(x,
+                                         width=help_width,
+                                         drop_whitespace=False,
+                                         replace_whitespace=False)
+                           for x in REQUEST_HELP.splitlines())
+    else:
+        epilog = REQUEST_HELP
 
     if shutil.which("git"):
         diff_default = "git --no-pager diff --no-index --word-diff --"
     else:
         diff_default = "diff -d -u --"
 
     argp = argparse.ArgumentParser(
         prog=os.path.basename(prog_name),
         usage="%(prog)s [options] request ...",
-        epilog="\n".join(textwrap.fill(x,
-                                       width=help_width,
-                                       drop_whitespace=False,
-                                       replace_whitespace=False)
-                         for x in REQUEST_HELP.splitlines()),
+        epilog=epilog,
         formatter_class=partial(argparse.RawDescriptionHelpFormatter,
                                 width=help_width),
         )
     argp.add_argument("--config-root",
                       type=Path,
                       default=Path("/"),
                       help="Root directory relative to which configuration "
```

### Comparing `flaggie-0.99.3/flaggie/config.py` & `flaggie-0.99.4/flaggie/config.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.3/flaggie/mangle.py` & `flaggie-0.99.4/flaggie/mangle.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.3/flaggie/pm.py` & `flaggie-0.99.4/flaggie/pm.py`

 * *Files identical despite different names*

### Comparing `flaggie-0.99.3/pyproject.toml` & `flaggie-0.99.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,20 @@
 
 [project.scripts]
 flaggie = "flaggie.__main__:entry_point"
 
 [project.urls]
 Homepage = "https://github.com/projg2/flaggie/"
 
+[tool.flit.sdist]
+include = [
+    "test",
+    "tox.ini",
+]
+
 [tool.mypy]
 disallow_untyped_defs = true
 no_implicit_optional = true
 
 [[tool.mypy.overrides]]
 module = [
     "test.*",
```

### Comparing `flaggie-0.99.3/PKG-INFO` & `flaggie-0.99.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaggie
-Version: 0.99.3
+Version: 0.99.4
 Summary: CLI mangler for Portage package.* configuration files
 Author-email: Michał Górny <mgorny@gentoo.org>
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: more-itertools
 Requires-Dist: gentoopm >= 0.5 ; extra == "package-manager"
 Requires-Dist: rich ; extra == "pretty-log"
```

