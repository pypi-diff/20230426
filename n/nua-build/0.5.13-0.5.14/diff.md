# Comparing `tmp/nua_build-0.5.13.tar.gz` & `tmp/nua_build-0.5.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nua_build-0.5.13.tar", max compression
+gzip compressed data, was "nua_build-0.5.14.tar", max compression
```

## Comparing `nua_build-0.5.13.tar` & `nua_build-0.5.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3241 2023-04-24 21:25:56.860904 nua_build-0.5.13/README.md
--rw-r--r--   0        0        0     1810 2023-04-24 21:27:54.721199 nua_build-0.5.13/pyproject.toml
--rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.13/src/nua/build/__init__.py
--rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.13/src/nua/build/__main__.py
--rw-r--r--   0        0        0     2864 2023-04-08 16:30:34.934589 nua_build-0.5.13/src/nua/build/archive_search.py
--rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.13/src/nua/build/builders/__init__.py
--rw-r--r--   0        0        0     3074 2023-04-24 21:25:56.862074 nua_build-0.5.13/src/nua/build/builders/base.py
--rw-r--r--   0        0        0     7471 2023-04-24 21:25:56.862204 nua_build-0.5.13/src/nua/build/builders/docker.py
--rw-r--r--   0        0        0     2455 2023-04-24 21:25:56.862424 nua_build-0.5.13/src/nua/build/builders/factory.py
--rw-r--r--   0        0        0     2489 2023-04-24 21:25:56.862526 nua_build-0.5.13/src/nua/build/builders/wrap.py
--rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.13/src/nua/build/config.py
--rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.13/src/nua/build/default_conf/__init__.py
--rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.13/src/nua/build/default_conf/config.toml
--rw-r--r--   0        0        0      151 2023-01-19 17:57:22.672446 nua_build-0.5.13/src/nua/build/defaults/Dockerfile
--rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.13/src/nua/build/defaults/__init__.py
--rw-r--r--   0        0        0     1883 2023-04-24 21:25:56.862754 nua_build-0.5.13/src/nua/build/main.py
--rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.13/src/nua/build/scripts/__init__.py
--rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.13/src/nua/build/scripts/test_replace_domain.py
--rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.13/src/nua/build/version.py
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 nua_build-0.5.13/PKG-INFO
+-rw-r--r--   0        0        0     3241 2023-04-24 21:25:56.860904 nua_build-0.5.14/README.md
+-rw-r--r--   0        0        0     1784 2023-04-26 06:46:51.584593 nua_build-0.5.14/pyproject.toml
+-rw-r--r--   0        0        0      208 2022-11-17 17:42:00.898773 nua_build-0.5.14/src/nua/build/__init__.py
+-rw-r--r--   0        0        0       86 2023-01-06 12:47:38.576197 nua_build-0.5.14/src/nua/build/__main__.py
+-rw-r--r--   0        0        0     2864 2023-04-08 16:30:34.934589 nua_build-0.5.14/src/nua/build/archive_search.py
+-rw-r--r--   0        0        0      323 2023-04-16 17:02:10.325031 nua_build-0.5.14/src/nua/build/builders/__init__.py
+-rw-r--r--   0        0        0     3166 2023-04-26 06:41:08.602266 nua_build-0.5.14/src/nua/build/builders/base.py
+-rw-r--r--   0        0        0     7447 2023-04-26 06:41:08.602485 nua_build-0.5.14/src/nua/build/builders/docker.py
+-rw-r--r--   0        0        0     2580 2023-04-26 06:41:08.602708 nua_build-0.5.14/src/nua/build/builders/factory.py
+-rw-r--r--   0        0        0     2465 2023-04-26 06:41:08.602900 nua_build-0.5.14/src/nua/build/builders/wrap.py
+-rw-r--r--   0        0        0      178 2022-12-20 18:49:45.395907 nua_build-0.5.14/src/nua/build/config.py
+-rw-r--r--   0        0        0        0 2022-12-20 18:49:45.396072 nua_build-0.5.14/src/nua/build/default_conf/__init__.py
+-rw-r--r--   0        0        0       65 2022-12-20 18:49:45.396131 nua_build-0.5.14/src/nua/build/default_conf/config.toml
+-rw-r--r--   0        0        0      151 2023-01-19 17:57:22.672446 nua_build-0.5.14/src/nua/build/defaults/Dockerfile
+-rw-r--r--   0        0        0       76 2022-12-03 19:23:00.336307 nua_build-0.5.14/src/nua/build/defaults/__init__.py
+-rw-r--r--   0        0        0     2497 2023-04-26 06:41:08.603124 nua_build-0.5.14/src/nua/build/main.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:42:00.899795 nua_build-0.5.14/src/nua/build/scripts/__init__.py
+-rw-r--r--   0        0        0     1750 2023-04-08 16:32:16.237367 nua_build-0.5.14/src/nua/build/scripts/test_replace_domain.py
+-rw-r--r--   0        0        0       81 2022-11-17 17:42:00.900100 nua_build-0.5.14/src/nua/build/version.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 nua_build-0.5.14/PKG-INFO
```

### Comparing `nua_build-0.5.13/README.md` & `nua_build-0.5.14/README.md`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.13/pyproject.toml` & `nua_build-0.5.14/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 [tool.poetry]
 name = "nua-build"
-version = "0.5.13"
+version = "0.5.14"
 description = "Nua build package (currently: build, core build, agent)"
 authors = [
     "Stefane Fermigier <sf@abilian.com>",
     "Jerome Dumonteil <jd@abilian.com>",
 ]
 license = "AGPL"
 readme = "README.md"
 packages = [
   { include = "nua", from = "src" }
 ]
 
-
 [tool.poetry.scripts]
 nua-build = "nua.build.main:app"
 nua_test_replace_domain = "nua.build.scripts.test_replace_domain:main"
 
-
 [tool.poetry.dependencies]
 python = "^3.10"
-nua-lib = "=0.5.13"
-nua-agent = "=0.5.13"
-nua-autobuild = "=0.5.13"
+nua-lib = "=0.5.14"
+nua-agent = "=0.5.14"
+nua-autobuild = "=0.5.14"
 tomli = "^2.0.1"
-pyyaml = "^6"
 snoop = "^0.4.3"
-typer = {version = "^0.7.0", extras = ["all"]}
-docker = {version = "^6", extras = ["ssh"]}
+cleez = "^0.1.8"
+pyyaml = "^6.0"
+docker = {version = "^6.0.1", extras = ["ssh"]}
 
 [tool.poetry.group.dev.dependencies]
 abilian-devtools = "*"
 nox = "*"
+devtools = "^0.11.0"
 
 types-setuptools = "*"
 types-pyyaml = "*"
 
 # To please poetry
 platformdirs = "<3.0.0"
-devtools = "^0.11.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # ------------------------------------------------------------------------------
```

### Comparing `nua_build-0.5.13/src/nua/build/archive_search.py` & `nua_build-0.5.14/src/nua/build/archive_search.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.13/src/nua/build/builders/base.py` & `nua_build-0.5.14/src/nua/build/builders/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,21 +31,25 @@
 
     config: NuaConfig
     container_type: str
     build_dir: Path
     nua_folder: Path
     nua_base: str
 
-    def __init__(self, config: NuaConfig):
+    save_image: bool = True
+
+    def __init__(self, config: NuaConfig, save_image: bool = True):
         assert isinstance(config, NuaConfig)
 
         self.config = config
         self.nua_base = ""
         self.build_dir = self.make_build_dir()
 
+        self.save_image = save_image
+
     @abstractmethod
     def run(self):
         raise NotImplementedError()
 
     def post_build_notices(self):
         """Post build analysis and possible usefull information."""
         self._notice_local_volumes()
```

### Comparing `nua_build-0.5.13/src/nua/build/builders/docker.py` & `nua_build-0.5.14/src/nua/build/builders/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         (self.build_dir / "nua").mkdir(mode=0o755)
         self._copy_local_code()
         self._copy_manifest_files()
         self._copy_nua_folder()
         self._copy_default_files()
 
     @docker_build_log_error
-    def build_with_docker_stream(self, save: bool = True):
+    def build_with_docker_stream(self):
         with chdir(self.build_dir):
             with suppress(IOError):
                 copy2(
                     self.build_dir / "nua" / "Dockerfile",
                     self.build_dir,
                 )
             nua_tag = self.config.nua_tag
@@ -130,18 +130,18 @@
             }
             info(f"Building image {nua_tag}")
             image_id = docker_stream_build(".", nua_tag, buildargs, labels)
 
             with verbosity(1):
                 display_docker_img(nua_tag)
 
-            if save:
-                client = docker.from_env(timeout=CLIENT_TIMEOUT)
-                image = client.images.get(image_id)
-                self.save(image, nua_tag)
+        if self.save_image:
+            client = docker.from_env(timeout=CLIENT_TIMEOUT)
+            image = client.images.get(image_id)
+            self.save(image, nua_tag)
 
     def _copy_local_code(self):
         if any((self.config.src_url, self.config.git_url)):
             return
         files = [
             item
             for item in self.config.root_dir.glob("*")
```

### Comparing `nua_build-0.5.13/src/nua/build/builders/factory.py` & `nua_build-0.5.14/src/nua/build/builders/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 """Builder factory: create a Builder instance based on the nua-config.
 """
 from __future__ import annotations
 
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 from pprint import pformat
+from typing import Any
 
 from nua.agent.nua_config import NuaConfig
 from nua.lib.panic import info, vprint
 from nua.lib.tool.state import verbosity
 
 from .base import Builder, BuilderError
 from .docker import DockerBuilder
 from .wrap import DockerWrapBuilder
 
 
-def get_builder(config_path: str | Path | None = None) -> Builder:
+def get_builder(config_path: str | Path | None = None, **opts) -> Builder:
     config = NuaConfig(config_path)
-    factory = BuilderFactory(config)
+    factory = BuilderFactory(config, opts)
     return factory.get_builder()
 
 
 @dataclass(frozen=True)
 class BuilderFactory:
     """Factory to create a Builder instance."""
 
     config: NuaConfig
+    opts: dict[str, Any] = field(default_factory=dict)
 
     def __post_init__(self) -> None:
         assert isinstance(self.config, NuaConfig)
 
     def get_builder(self) -> Builder:
         with verbosity(4):
             vprint(pformat(self.config.as_dict()))
 
         # Not used at this stage
         # container_type = self.detect_container_type()
         build_method = self.detect_build_method()
 
         if build_method == "build":
-            return DockerBuilder(self.config)
+            return DockerBuilder(self.config, **self.opts)
 
         if build_method == "wrap":
-            return DockerWrapBuilder(self.config)
+            return DockerWrapBuilder(self.config, **self.opts)
 
         raise ValueError(f"Unknown build strategy '{build_method}'")
 
     # XXX: not used
     def detect_container_type(self) -> str:
         """Placeholder for future container technology detection.
```

### Comparing `nua_build-0.5.13/src/nua/build/builders/wrap.py` & `nua_build-0.5.14/src/nua/build/builders/wrap.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 "FROM ${nua_wrap_tag}\n\n"
                 "RUN mkdir -p /nua/metadata\n"
                 "COPY nua-config.json /nua/metadata/\n"
             )
         docker_file.write_text(content, encoding="utf8")
 
     @docker_build_log_error
-    def build_wrap_with_docker_stream(self, save: bool = True):
+    def build_wrap_with_docker_stream(self):
         with chdir(self.build_dir):
             nua_tag = self.config.nua_tag
             buildargs = {
                 "nua_wrap_tag": self.config.wrap_image,
             }
             labels = {
                 "APP_ID": self.config.app_id,
@@ -68,11 +68,11 @@
             }
             info(f"Building (wrap) image {nua_tag}")
             image_id = docker_stream_build(".", nua_tag, buildargs, labels)
 
             with verbosity(1):
                 display_docker_img(nua_tag)
 
-            if save:
-                client = docker.from_env(timeout=CLIENT_TIMEOUT)
-                image = client.images.get(image_id)
-                self.save(image, nua_tag)
+        if self.save_image:
+            client = docker.from_env(timeout=CLIENT_TIMEOUT)
+            image = client.images.get(image_id)
+            self.save(image, nua_tag)
```

### Comparing `nua_build-0.5.13/src/nua/build/scripts/test_replace_domain.py` & `nua_build-0.5.14/src/nua/build/scripts/test_replace_domain.py`

 * *Files identical despite different names*

### Comparing `nua_build-0.5.13/PKG-INFO` & `nua_build-0.5.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: nua-build
-Version: 0.5.13
+Version: 0.5.14
 Summary: Nua build package (currently: build, core build, agent)
 License: AGPL
 Author: Stefane Fermigier
 Author-email: sf@abilian.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: docker[ssh] (>=6,<7)
-Requires-Dist: nua-agent (==0.5.13)
-Requires-Dist: nua-autobuild (==0.5.13)
-Requires-Dist: nua-lib (==0.5.13)
-Requires-Dist: pyyaml (>=6,<7)
+Requires-Dist: cleez (>=0.1.8,<0.2.0)
+Requires-Dist: docker[ssh] (>=6.0.1,<7.0.0)
+Requires-Dist: nua-agent (==0.5.14)
+Requires-Dist: nua-autobuild (==0.5.14)
+Requires-Dist: nua-lib (==0.5.14)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: snoop (>=0.4.3,<0.5.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown
 
 # Nua-build
 
 Build system for Nua packages.
 
 [Nua](https://nua.rocks/) is an open source, self-hosted cloud platform project (a PaaS - platform as a service).
```

