# Comparing `tmp/pdm_conda-0.9.2b1.tar.gz` & `tmp/pdm_conda-0.9.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_conda-0.9.2b1.tar", last modified: Fri Apr 21 18:27:35 2023, max compression
+gzip compressed data, was "pdm_conda-0.9.3b0.tar", last modified: Wed Apr 26 21:30:37 2023, max compression
```

## Comparing `pdm_conda-0.9.2b1.tar` & `pdm_conda-0.9.3b0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.2b1/LICENSE
--rw-r--r--   0        0        0     5649 2023-04-19 19:04:02.148249 pdm_conda-0.9.2b1/README.md
--rw-r--r--   0        0        0     1979 2023-04-21 18:27:35.124240 pdm_conda-0.9.2b1/pyproject.toml
--rw-r--r--   0        0        0      595 2023-04-21 18:27:32.161644 pdm_conda-0.9.2b1/src/pdm_conda/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.2b1/src/pdm_conda/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/__init__.py
--rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/add.py
--rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/remove.py
--rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.2b1/src/pdm_conda/cli/utils.py
--rw-r--r--   0        0        0    15662 2023-04-21 18:19:33.532039 pdm_conda-0.9.2b1/src/pdm_conda/conda.py
--rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.2b1/src/pdm_conda/installers/__init__.py
--rw-r--r--   0        0        0     2613 2023-04-21 15:54:37.431271 pdm_conda-0.9.2b1/src/pdm_conda/installers/manager.py
--rw-r--r--   0        0        0     2307 2023-04-19 19:04:02.152461 pdm_conda-0.9.2b1/src/pdm_conda/installers/synchronizers.py
--rw-r--r--   0        0        0     3043 2023-04-19 19:04:02.153381 pdm_conda-0.9.2b1/src/pdm_conda/mapping.py
--rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.2b1/src/pdm_conda/models/__init__.py
--rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.2b1/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
--rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.2b1/src/pdm_conda/models/candidates.py
--rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.2b1/src/pdm_conda/models/conda.py
--rw-r--r--   0        0        0     8612 2023-04-19 19:04:02.155447 pdm_conda-0.9.2b1/src/pdm_conda/models/config.py
--rw-r--r--   0        0        0     3095 2023-04-19 19:04:02.155978 pdm_conda-0.9.2b1/src/pdm_conda/models/environment.py
--rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.2b1/src/pdm_conda/models/repositories.py
--rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.2b1/src/pdm_conda/models/requirements.py
--rw-r--r--   0        0        0      900 2023-04-09 20:29:55.611942 pdm_conda-0.9.2b1/src/pdm_conda/models/setup.py
--rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.2b1/src/pdm_conda/project.py
--rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.2b1/src/pdm_conda/resolver/__init__.py
--rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.2b1/src/pdm_conda/resolver/providers.py
--rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.2b1/src/pdm_conda/resolvers.py
--rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.2b1/src/pdm_conda/utils.py
--rw-r--r--   0        0        0     7497 1970-01-01 00:00:00.000000 pdm_conda-0.9.2b1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-16 23:52:20.043514 pdm_conda-0.9.3b0/LICENSE
+-rw-r--r--   0        0        0     5701 2023-04-26 21:23:52.333777 pdm_conda-0.9.3b0/README.md
+-rw-r--r--   0        0        0      110 2023-04-26 21:12:13.255162 pdm_conda-0.9.3b0/data/mapping_fixes.json
+-rw-r--r--   0        0        0     1998 2023-04-26 21:30:37.087628 pdm_conda-0.9.3b0/pyproject.toml
+-rw-r--r--   0        0        0      595 2023-04-26 21:30:00.405870 pdm_conda-0.9.3b0/src/pdm_conda/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:28.238706 pdm_conda-0.9.3b0/src/pdm_conda/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-06 20:52:59.837399 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/__init__.py
+-rw-r--r--   0        0        0     3087 2023-04-19 19:04:02.150645 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/add.py
+-rw-r--r--   0        0        0     1681 2023-04-19 16:32:57.025189 pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/remove.py
+-rw-r--r--   0        0        0     3009 2023-04-21 15:54:37.429042 pdm_conda-0.9.3b0/src/pdm_conda/cli/utils.py
+-rw-r--r--   0        0        0    15836 2023-04-26 21:23:23.198612 pdm_conda-0.9.3b0/src/pdm_conda/conda.py
+-rw-r--r--   0        0        0        0 2023-01-05 20:40:25.652497 pdm_conda-0.9.3b0/src/pdm_conda/installers/__init__.py
+-rw-r--r--   0        0        0     2444 2023-04-26 21:20:39.055538 pdm_conda-0.9.3b0/src/pdm_conda/installers/manager.py
+-rw-r--r--   0        0        0     2304 2023-04-26 21:18:03.786553 pdm_conda-0.9.3b0/src/pdm_conda/installers/synchronizers.py
+-rw-r--r--   0        0        0     3343 2023-04-26 21:12:20.058679 pdm_conda-0.9.3b0/src/pdm_conda/mapping.py
+-rw-r--r--   0        0        0        0 2023-01-02 22:45:44.891129 pdm_conda-0.9.3b0/src/pdm_conda/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-30 01:53:52.844040 pdm_conda-0.9.3b0/src/pdm_conda/models/__pycache__/candidates.cpython-310.pyc.281473776611248
+-rw-r--r--   0        0        0     7575 2023-04-21 15:54:37.432253 pdm_conda-0.9.3b0/src/pdm_conda/models/candidates.py
+-rw-r--r--   0        0        0     1818 2023-04-19 19:04:02.154757 pdm_conda-0.9.3b0/src/pdm_conda/models/conda.py
+-rw-r--r--   0        0        0     8846 2023-04-26 21:15:12.881202 pdm_conda-0.9.3b0/src/pdm_conda/models/config.py
+-rw-r--r--   0        0        0     3795 2023-04-26 21:19:38.356166 pdm_conda-0.9.3b0/src/pdm_conda/models/environment.py
+-rw-r--r--   0        0        0     6740 2023-04-21 15:54:37.432966 pdm_conda-0.9.3b0/src/pdm_conda/models/repositories.py
+-rw-r--r--   0        0        0    11368 2023-04-21 15:54:37.434138 pdm_conda-0.9.3b0/src/pdm_conda/models/requirements.py
+-rw-r--r--   0        0        0     1123 2023-04-26 21:17:17.574104 pdm_conda-0.9.3b0/src/pdm_conda/models/setup.py
+-rw-r--r--   0        0        0     8311 2023-04-19 19:04:02.158361 pdm_conda-0.9.3b0/src/pdm_conda/project.py
+-rw-r--r--   0        0        0        0 2023-02-18 20:09:32.663574 pdm_conda-0.9.3b0/src/pdm_conda/resolver/__init__.py
+-rw-r--r--   0        0        0     2418 2023-04-19 19:04:02.159092 pdm_conda-0.9.3b0/src/pdm_conda/resolver/providers.py
+-rw-r--r--   0        0        0     8601 2023-04-19 19:04:02.159990 pdm_conda-0.9.3b0/src/pdm_conda/resolvers.py
+-rw-r--r--   0        0        0      784 2023-01-10 16:37:32.674613 pdm_conda-0.9.3b0/src/pdm_conda/utils.py
+-rw-r--r--   0        0        0     7549 1970-01-01 00:00:00.000000 pdm_conda-0.9.3b0/PKG-INFO
```

### Comparing `pdm_conda-0.9.2b1/LICENSE` & `pdm_conda-0.9.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/README.md` & `pdm_conda-0.9.3b0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # pdm-conda
 
 A PDM plugin to resolve/install/uninstall project dependencies with Conda.
 
 ## Configuration
 
-| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
-|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
-| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
-| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `CONDA_SOLVER`              |
-| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
-| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
-| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
-| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
-| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
-| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
-| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
-| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
+| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable            |
+|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|---------------------------------|
+| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `PDM_CONDA_RUNNER`              |
+| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `PDM_CONDA_SOLVER`              |
+| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                                 |
+| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `PDM_CONDA_AS_DEFAULT_MANAGER`  |
+| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `PDM_CONDA_BATCHED_COMMANDS`    |
+| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                                 |
+| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `PDM_CONDA_INSTALLATION_METHOD` |
+| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                                 |
+| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                                 |
+| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                                 |
+| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PDM_CONDA_PYPI_MAPPING_DIR`    |
 
 All configuration items use prefix `pdm.tool`, this is a viable configuration:
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
```

### Comparing `pdm_conda-0.9.2b1/pyproject.toml` & `pdm_conda-0.9.3b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "pdm~=2.4.0",
     "requests>=2.28.1",
 ]
-version = "0.9.2b1"
+version = "0.9.3b0"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://github.com/macro128/pdm-conda"
 Changelog = "https://github.com/macro128/pdm-conda/blob/main/CHANGELOG.md"
@@ -52,14 +52,15 @@
 source = "file"
 path = "src/pdm_conda/__init__.py"
 
 [tool.pdm.build]
 package-dir = "src"
 includes = [
     "src",
+    "data/*.json",
 ]
 excludes = [
     "tests",
 ]
 
 [tool.pdm.scripts]
 test = "pytest --cov=src/pdm_conda/ tests/ --cov-report xml --cov-report term"
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/__init__.py` & `pdm_conda-0.9.3b0/src/pdm_conda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     core.register_command(AddCommand)
     core.register_command(RemoveCommand)
 
     for name, config in CONFIGS:
         core.add_config(name, config)
 
 
-__version__ = "0.9.2b1"
+__version__ = "0.9.3b0"
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/add.py` & `pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/cli/commands/remove.py` & `pdm_conda-0.9.3b0/src/pdm_conda/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/cli/utils.py` & `pdm_conda-0.9.3b0/src/pdm_conda/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/conda.py` & `pdm_conda-0.9.3b0/src/pdm_conda/conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,26 +81,33 @@
                         for v in options:
                             f.write(f"  - {v}\n")
             f.seek(0)
             cmd = cmd + ["--file", f.name]
         logger.debug(f"cmd: {' '.join(cmd)}")
         if environment:
             logger.debug(f"env: {environment}")
-        process = subprocess.run(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, encoding="utf-8")
+        process = subprocess.run(cmd, capture_output=True, encoding="utf-8")
     if "--json" in cmd:
         try:
             response = json.loads(process.stdout)
         except:
             response = {}
     else:
-        response = {"message": f"{process.stdout}\n{process.stderr}"}
+        response = {}
+        msg = f"{process.stdout}\n" if process.stdout else ""
+        if process.stderr:
+            msg += process.stderr
+        if msg:
+            response["message"] = msg
     try:
         process.check_returncode()
     except subprocess.CalledProcessError as e:
-        msg = f"{exception_msg}\n"
+        msg = ""
+        if exception_msg:
+            msg = f"{exception_msg}\n"
         if isinstance(response, dict) and not response.get("success", False):
             if err := response.get("solver_problems", response.get("error", response.get("message", process.stderr))):
                 if isinstance(err, str):
                     err = [err]
                 msg += "\n".join(err)
         else:
             msg += process.stderr
@@ -241,15 +248,15 @@
     _requirement = requirement
     if isinstance(_requirement, CondaRequirement):
         channel = channel or _requirement.channel
         _requirement = _requirement.as_line(with_build_string=True, conda_compatible=True).replace(" ", "=")
     if "::" in _requirement:
         channel, _requirement = _requirement.split("::", maxsplit=1)
     if isinstance(requirement, str):
-        requirement = parse_requirement(f"conda::{requirement}")
+        requirement = parse_requirement(f"conda:{requirement}")
     channels = _ensure_channels(
         project,
         [channel] if channel else [],
         f"No channel specified for searching [req]{requirement}[/] using defaults if exist.",
     )
     packages = _conda_search(project, _requirement, tuple(channels))
     return _parse_candidates(project, packages, requirement)
@@ -356,15 +363,15 @@
     else:
         command.extend(packages)
     if dry_run:
         command.append("--dry-run")
     kwargs: dict = dict()
     if explicit:
         kwargs["lockfile"] = packages
-    run_conda(command + ["--json"], **kwargs)
+    run_conda(command + ["--json"], exception_cls=exception_cls, exception_msg="", **kwargs)
 
 
 def conda_install(
     project: CondaProject,
     packages: str | list[str],
     dry_run: bool = False,
     no_deps: bool = False,
@@ -403,19 +410,15 @@
     :param project: PDM project
     :param packages: resolved packages
     :param dry_run: don't uninstall if dry run
     :param no_deps: don't uninstall dependencies if true
     """
     config = project.conda_config
 
-    with config.with_config(
-        runner=CondaRunner.CONDA if no_deps and config.runner == CondaRunner.MAMBA else config.runner,
-    ):
-        command = config.command("remove")
-
+    command = config.command("remove")
     if no_deps:
         if config.runner == CondaRunner.MICROMAMBA:
             command.append("--no-prune")
         command.append("--force")
 
     _conda_install(command, packages, dry_run=dry_run, exception_cls=UninstallError)
 
@@ -456,14 +459,16 @@
     :return: packages distribution
     """
     config = project.conda_config
     distributions = dict()
     if config.is_initialized:
         packages = run_conda(config.command("list") + ["--json"])
         for package in packages:
+            if config.runner != CondaRunner.MICROMAMBA and package.get("platform", "") == "pypi":
+                continue
             name, version = package["name"], package["version"]
             distributions[normalize_name(name)] = CondaSetupDistribution(
                 Setup(
                     name=name,
                     summary="",
                     version=parse_conda_version(version),
                 ),
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/installers/manager.py` & `pdm_conda-0.9.3b0/src/pdm_conda/installers/manager.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 from importlib.metadata import Distribution
 from typing import cast
 
-from installer.exceptions import InstallerError
-from pdm.exceptions import RequirementError, UninstallError
 from pdm.installers import InstallManager
 
 from pdm_conda.conda import conda_install, conda_uninstall
 from pdm_conda.models.candidates import Candidate, CondaCandidate
 from pdm_conda.models.environment import CondaEnvironment, Environment
 from pdm_conda.models.setup import CondaSetupDistribution
 
 
 class CondaInstallManager(InstallManager):
     def __init__(self, environment: Environment, *, use_install_cache: bool = False) -> None:
         super().__init__(environment, use_install_cache=use_install_cache)
         self.environment = cast(CondaEnvironment, environment)
         self._num_install = 0
         self._num_remove = 0
-        self._batch_install: list[CondaCandidate] = []
-        self._batch_remove: list[CondaSetupDistribution] = []
+        self._batch_install: list[str] = []
+        self._batch_remove: list[str] = []
 
     def prepare_batch_operations(self, num_install: int, num_remove: int):
         self._num_install = num_install
         self._num_remove = num_remove
 
+    def _run_with_conda(self, conda_func, new_requirement: str, requirements: list[str], min_requirements: int):
+        requirements.append(new_requirement)
+        if len(requirements) >= min_requirements:
+            try:
+                conda_func(
+                    self.environment.project,
+                    list(requirements),
+                    no_deps=True,
+                )
+                requirements.clear()
+            except:
+                if min_requirements == 0:
+                    requirements.clear()
+                raise
+
     def install(self, candidate: Candidate) -> None:
         """
         Install candidate, use conda if conda package else default installer
         :param candidate: candidate to install
         """
         if isinstance(candidate, CondaCandidate):
-            try:
-                self._batch_install.append(candidate)
-                if len(self._batch_install) >= self._num_install:
-                    conda_install(
-                        self.environment.project,
-                        [f"{c.link.url_without_fragment}#{c.link.hash}" for c in self._batch_install],
-                        no_deps=True,
-                    )
-                    self._batch_install.clear()
-            except (RequirementError, ValueError) as e:
-                raise InstallerError(e) from e
+            self._run_with_conda(
+                conda_install,
+                f"{candidate.link.url_without_fragment}#{candidate.link.hash}",
+                self._batch_install,
+                self._num_install,
+            )
         else:
             super().install(candidate)
 
     def uninstall(self, dist: Distribution) -> None:
         """
         Uninstall distribution, use conda if conda package else default uninstaller
         :param dist: distribution to uninstall
         """
         if isinstance(dist, CondaSetupDistribution):
-            try:
-                self._batch_remove.append(dist)
-                if len(self._batch_remove) >= self._num_remove:
-                    conda_uninstall(self.environment.project, [d.name for d in self._batch_remove], no_deps=True)
-                    self._batch_remove.clear()
-            except RequirementError as e:
-                raise UninstallError(e) from e
+            self._run_with_conda(conda_uninstall, dist.name, self._batch_remove, self._num_remove)
         else:
             super().uninstall(dist)
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/installers/synchronizers.py` & `pdm_conda-0.9.3b0/src/pdm_conda/installers/synchronizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
     def compare_with_working_set(self) -> tuple[list[str], list[str], list[str]]:
         to_add, to_update, to_remove = super().compare_with_working_set()
 
         # deactivate parallel execution if uninstall
         self.parallel = self.environment.project.config["install.parallel"]
         if to_remove:
-            to_remove = [p for p in to_remove if p not in self.environment.python_dependencies]
+            to_remove = [p for p in to_remove if p not in self.environment.env_dependencies]
 
         num_update, num_remove = (
             len([p for p in pks if isinstance(self.working_set[p], CondaSetupDistribution)])
             for pks in (to_update, to_remove)
         )
         if self.parallel and (num_update + num_remove > 0):
             self.environment.project.core.ui.echo("Deactivating parallel uninstall.")
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/mapping.py` & `pdm_conda-0.9.3b0/src/pdm_conda/mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from datetime import datetime, timedelta
 from functools import lru_cache
 from pathlib import Path
 
 import requests
 
 MAPPINGS_URL = "https://github.com/regro/cf-graph-countyfair/raw/master/mappings/pypi/grayskull_pypi_mapping.yaml"
-DOWNLOAD_DIR_ENV_VAR = "PYPI_MAPPING_DIR"
+DOWNLOAD_DIR_ENV_VAR = "PDM_CONDA_PYPI_MAPPING_DIR"
 
 
 def process_mapping(yaml_path: Path, dict_path: Path):
     """
     Create json mapping from yaml mapping
     :param yaml_path: yaml path
     :param dict_path: json path
@@ -55,18 +55,28 @@
                 f.write(chunk)
         process_mapping(yaml_path, dict_path)
 
     with dict_path.open() as f:
         return json.load(f)
 
 
+def get_mapping_fixes() -> dict:
+    fixes = dict()
+    if (fixes_file := Path(__file__).parents[2] / "data/mapping_fixes.json").exists():
+        with fixes_file.open() as f:
+            fixes = json.load(f)
+    return fixes
+
+
 @lru_cache
 def get_pypi_mapping() -> dict[str, str]:
     download_dir = os.getenv(DOWNLOAD_DIR_ENV_VAR)
-    return download_mapping(Path(str(download_dir)))
+    mapping = download_mapping(Path(str(download_dir)))
+    mapping.update(get_mapping_fixes())
+    return mapping
 
 
 @lru_cache
 def get_conda_mapping() -> dict[str, str]:
     return {v: k for k, v in get_pypi_mapping().items()}
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/candidates.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/conda.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/conda.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/config.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,31 +23,31 @@
     MAMBA = "libmamba"
 
 
 _CONFIG_MAP = {"pypi-mapping.download-dir": "mapping_download_dir"}
 _CONFIG_MAP |= {v: k for k, v in _CONFIG_MAP.items()}
 
 CONFIGS = [
-    ("runner", ConfigItem("Conda runner executable", CondaRunner.CONDA.value, env_var="CONDA_RUNNER")),
-    ("solver", ConfigItem("Solver to use for Conda resolution", CondaSolver.CONDA.value, env_var="CONDA_SOLVER")),
+    ("runner", ConfigItem("Conda runner executable", CondaRunner.CONDA.value, env_var="PDM_CONDA_RUNNER")),
+    ("solver", ConfigItem("Solver to use for Conda resolution", CondaSolver.CONDA.value, env_var="PDM_CONDA_SOLVER")),
     ("channels", ConfigItem("Conda channels to use")),
     (
         "as-default-manager",
-        ConfigItem("Use Conda to install all possible requirements", False, env_var="CONDA_AS_DEFAULT_MANAGER"),
+        ConfigItem("Use Conda to install all possible requirements", False, env_var="PDM_CONDA_AS_DEFAULT_MANAGER"),
     ),
     (
         "batched-commands",
-        ConfigItem("Execute batched install and remove commands", False, env_var="CONDA_BATCHED_COMMANDS"),
+        ConfigItem("Execute batched install and remove commands", False, env_var="PDM_CONDA_BATCHED_COMMANDS"),
     ),
     (
         "installation-method",
         ConfigItem(
             "Whether to use hard-link or copy when installing",
             "hard-link",
-            env_var="CONDA_INSTALLATION_METHOD",
+            env_var="PDM_CONDA_INSTALLATION_METHOD",
         ),
     ),
     ("dependencies", ConfigItem("Dependencies to install with Conda")),
     ("optional-dependencies", ConfigItem("Optional dependencies to install with Conda")),
     ("dev-dependencies", ConfigItem("Development dependencies to install with Conda")),
     ("excludes", ConfigItem("Excluded dependencies from Conda")),
     (
@@ -208,18 +208,24 @@
 
     def command(self, cmd="install"):
         """
         Get runner command args
         :param cmd: command, install by default
         :return: args list
         """
-        _command = [self.runner, *cmd.split(" ")]
+        runner = self.runner
+        if cmd == "remove" and runner == CondaRunner.MAMBA:
+            runner = CondaRunner.CONDA
+        if isinstance(runner, CondaRunner):
+            runner = runner.value
+
+        _command = [runner, *cmd.split(" ")]
+
         if self.runner != CondaRunner.CONDA and cmd == "search":
             _command.insert(1, "repoquery")
-
         if cmd in ("install", "remove", "create"):
             _command.append("-y")
         if cmd in ("install", "create") or (cmd == "search" and self.runner == CondaRunner.MICROMAMBA):
             _command.append("--strict-channel-priority")
         if self.runner == CondaRunner.CONDA and self.solver == CondaSolver.MAMBA and cmd in ("create", "install"):
-            _command.extend(["--solver", self.solver])
+            _command.extend(["--solver", CondaSolver.MAMBA.value])
         return _command
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/environment.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import functools
 import os
 import sysconfig
+import uuid
 from copy import copy
 from pathlib import Path
 from typing import cast
 
 from pdm.exceptions import ProjectError
 from pdm.models.environment import Environment, PrefixEnvironment
 from pdm.models.requirements import Requirement
 from pdm.models.specifiers import PySpecSet
 from pdm.models.working_set import WorkingSet
 from pdm.project import Project
 
-from pdm_conda.conda import conda_list, conda_search
+from pdm_conda.conda import conda_create, conda_list, conda_search
 from pdm_conda.mapping import pypi_to_conda
+from pdm_conda.models.config import CondaRunner, CondaSolver
 from pdm_conda.project import CondaProject
 from pdm_conda.utils import normalize_name
 
 _patched = False
 
 
 def ensure_conda_env():
@@ -26,15 +28,15 @@
     return packages_path
 
 
 class CondaEnvironment(Environment):
     def __init__(self, project: Project) -> None:
         super().__init__(project)
         self.project = cast(CondaProject, project)
-        self._python_dependencies: dict[str, Requirement] | None = None
+        self._env_dependencies: dict[str, Requirement] | None = None
         self.python_requires &= PySpecSet(f"=={self.interpreter.version}")
 
     @property
     def packages_path(self) -> Path:
         return Path(ensure_conda_env())
 
     def get_paths(self) -> dict[str, str]:
@@ -50,30 +52,45 @@
         working_set = super().get_working_set()
         working_set._dist_map = conda_list(self.project) | {
             normalize_name(pypi_to_conda(dist.metadata["Name"])): dist for dist in working_set._dist_map.values()
         }
         return working_set
 
     @property
-    def python_dependencies(self) -> dict[str, Requirement]:
-        if self._python_dependencies is None:
-            self._python_dependencies = dict()
+    def env_dependencies(self) -> dict[str, Requirement]:
+        if self._env_dependencies is None:
+            self._env_dependencies = dict()
 
             def load_dependencies(name: str, packages: dict, dependencies: dict):
                 if name not in packages and name not in dependencies:
                     return
-                package = packages[name].as_line().replace(" ", "=")
-                candidate = conda_search(self.project, package)[0]
+                candidate = conda_search(self.project, packages[name].req)[0]
                 dependencies[name] = candidate.req
                 for d in candidate.dependencies:
                     load_dependencies(d.name, packages, dependencies)
 
-            load_dependencies("python", conda_list(self.project), self._python_dependencies)
+            working_set = conda_list(self.project)
+            dependencies = ["python"]
+            if (runner := self.project.conda_config.runner) in working_set:
+                dependencies.append(runner)
+            if (
+                runner in (CondaRunner.MAMBA, CondaRunner.MICROMAMBA)
+                or self.project.conda_config.solver == CondaSolver.MAMBA
+            ):
+                self._env_dependencies = conda_create(
+                    self.project,
+                    [working_set[d].req for d in dependencies],
+                    prefix=f"/tmp/{uuid.uuid4()}",
+                    dry_run=True,
+                )
+            else:
+                for dep in dependencies:
+                    load_dependencies(dep, working_set, self._env_dependencies)
 
-        return self._python_dependencies
+        return self._env_dependencies
 
 
 def wrap_init(func):
     @functools.wraps(func)
     def wrapper(self, *args, **kwargs):
         res = func(self, *args, **kwargs)
         if isinstance(self.project, CondaProject):
```

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/repositories.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/models/requirements.py` & `pdm_conda-0.9.3b0/src/pdm_conda/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/project.py` & `pdm_conda-0.9.3b0/src/pdm_conda/project.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/resolver/providers.py` & `pdm_conda-0.9.3b0/src/pdm_conda/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/resolvers.py` & `pdm_conda-0.9.3b0/src/pdm_conda/resolvers.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/src/pdm_conda/utils.py` & `pdm_conda-0.9.3b0/src/pdm_conda/utils.py`

 * *Files identical despite different names*

### Comparing `pdm_conda-0.9.2b1/PKG-INFO` & `pdm_conda-0.9.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-conda
-Version: 0.9.2b1
+Version: 0.9.3b0
 Summary: A PDM plugin to resolve/install/uninstall project dependencies with Conda
 Keywords: pdm plugin conda
 Author: Marcos Pastorini
 License: MIT License
         
         Copyright (c) 2022 macro128
         
@@ -37,27 +37,27 @@
 
 # pdm-conda
 
 A PDM plugin to resolve/install/uninstall project dependencies with Conda.
 
 ## Configuration
 
-| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable        |
-|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|-----------------------------|
-| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `CONDA_RUNNER`              |
-| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `CONDA_SOLVER`              |
-| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                             |
-| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `CONDA_AS_DEFAULT_MANAGER`  |
-| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `CONDA_BATCHED_COMMANDS`    |
-| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                             |
-| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `CONDA_INSTALLATION_METHOD` |
-| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                             |
-| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                             |
-| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                             |
-| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PYPI_MAPPING_DIR`          |
+| Config item                       | Description                                                                                          | Default value       | Possible values                | Environment variable            |
+|-----------------------------------|------------------------------------------------------------------------------------------------------|---------------------|--------------------------------|---------------------------------|
+| `conda.runner`                    | Conda runner executable                                                                              | `conda`             | `conda`, `mamba`, `micromamba` | `PDM_CONDA_RUNNER`              |
+| `conda.solver`                    | Solver to use for Conda resolution                                                                   | `conda`             | `conda`, `libmamba`            | `PDM_CONDA_SOLVER`              |
+| `conda.channels`                  | Conda channels to use, order will be enforced                                                        | `[]`                |                                |                                 |
+| `conda.as-default-manager`        | Use Conda to install all possible requirements                                                       | `False`             |                                | `PDM_CONDA_AS_DEFAULT_MANAGER`  |
+| `conda.batched-commands`          | Execute batched install and remove Conda commands, when True the command is executed only at the end | `False`             |                                | `PDM_CONDA_BATCHED_COMMANDS`    |
+| `conda.excludes`                  | Array of dependencies to exclude from Conda resolution                                               | `[]`                |                                |                                 |
+| `conda.installation-method`       | Installation method to use when installing dependencies with Conda                                   | `hard-link`         | `hard-link`, `copy`            | `PDM_CONDA_INSTALLATION_METHOD` |
+| `conda.dependencies`              | Array of dependencies to install with Conda, analogue to `project.dependencies`                      | `[]`                |                                |                                 |
+| `conda.optional-dependencies`     | Groups of optional dependencies to install with Conda, analogue to `project.optional-dependencies`   | `{}`                |                                |                                 |
+| `conda.dev-dependencies`          | Groups of development dependencies to install with Conda, analogue to `tool.pdm.dev-dependencies`    | `{}`                |                                |                                 |
+| `conda.pypi-mapping.download-dir` | PyPI-Conda mapping download directory                                                                | `$HOME/.pdm-conda/` |                                | `PDM_CONDA_PYPI_MAPPING_DIR`    |
 
 All configuration items use prefix `pdm.tool`, this is a viable configuration:
 
 ```toml
 [tool.pdm.conda]
 runner = "micromamba"
 channels = ["conda-forge/noarch", "conda-forge", "anaconda"]
```

