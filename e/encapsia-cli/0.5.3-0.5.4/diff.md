# Comparing `tmp/encapsia_cli-0.5.3.tar.gz` & `tmp/encapsia_cli-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encapsia_cli-0.5.3.tar", max compression
+gzip compressed data, was "encapsia_cli-0.5.4.tar", max compression
```

## Comparing `encapsia_cli-0.5.3.tar` & `encapsia_cli-0.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1078 2022-01-07 06:44:24.119730 encapsia_cli-0.5.3/LICENSE
--rw-r--r--   0        0        0     1388 2023-01-03 16:16:53.715217 encapsia_cli-0.5.3/README.md
--rw-r--r--   0        0        0       90 2023-01-11 07:37:30.655978 encapsia_cli-0.5.3/encapsia_cli/__init__.py
--rw-r--r--   0        0        0     1495 2022-01-07 06:44:24.119730 encapsia_cli-0.5.3/encapsia_cli/completion.py
--rw-r--r--   0        0        0     1638 2022-10-05 14:03:11.428246 encapsia_cli-0.5.3/encapsia_cli/config.py
--rw-r--r--   0        0        0     1681 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/database.py
--rw-r--r--   0        0        0     4095 2022-11-22 14:49:47.724708 encapsia_cli-0.5.3/encapsia_cli/encapsia.py
--rw-r--r--   0        0        0     1883 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/fixtures.py
--rw-r--r--   0        0        0     1145 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/help.py
--rw-r--r--   0        0        0      564 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/httpie.py
--rw-r--r--   0        0        0     8204 2023-01-11 07:37:30.655978 encapsia_cli-0.5.3/encapsia_cli/lib.py
--rw-r--r--   0        0        0    16224 2022-11-22 14:49:47.724708 encapsia_cli-0.5.3/encapsia_cli/plugininfo.py
--rw-r--r--   0        0        0    26879 2023-01-10 15:57:32.885572 encapsia_cli-0.5.3/encapsia_cli/plugins.py
--rw-r--r--   0        0        0     4296 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/run.py
--rw-r--r--   0        0        0     1156 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/s3.py
--rw-r--r--   0        0        0     2218 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/schedule.py
--rw-r--r--   0        0        0      520 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/shell.py
--rw-r--r--   0        0        0     3749 2023-01-11 07:37:30.655978 encapsia_cli-0.5.3/encapsia_cli/token.py
--rw-r--r--   0        0        0     4189 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/users.py
--rw-r--r--   0        0        0      300 2022-01-07 06:44:24.123731 encapsia_cli-0.5.3/encapsia_cli/version.py
--rw-r--r--   0        0        0     1577 2023-01-11 07:37:30.659978 encapsia_cli-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2704 1970-01-01 00:00:00.000000 encapsia_cli-0.5.3/setup.py
--rw-r--r--   0        0        0     2738 1970-01-01 00:00:00.000000 encapsia_cli-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-01-07 06:44:24.119730 encapsia_cli-0.5.4/LICENSE
+-rw-r--r--   0        0        0     1515 2023-04-24 06:40:03.716923 encapsia_cli-0.5.4/README.md
+-rw-r--r--   0        0        0       90 2023-04-24 06:37:39.700477 encapsia_cli-0.5.4/encapsia_cli/__init__.py
+-rw-r--r--   0        0        0     1495 2022-01-07 06:44:24.119730 encapsia_cli-0.5.4/encapsia_cli/completion.py
+-rw-r--r--   0        0        0     1930 2023-04-24 06:27:52.898295 encapsia_cli-0.5.4/encapsia_cli/config.py
+-rw-r--r--   0        0        0     1928 2023-04-24 06:49:10.547106 encapsia_cli-0.5.4/encapsia_cli/database.py
+-rw-r--r--   0        0        0     4224 2023-04-24 06:27:52.898295 encapsia_cli-0.5.4/encapsia_cli/encapsia.py
+-rw-r--r--   0        0        0     2377 2023-04-24 06:49:28.555269 encapsia_cli-0.5.4/encapsia_cli/fixtures.py
+-rw-r--r--   0        0        0     1145 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/help.py
+-rw-r--r--   0        0        0      564 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/httpie.py
+-rw-r--r--   0        0        0     8320 2023-04-24 06:27:52.898295 encapsia_cli-0.5.4/encapsia_cli/lib.py
+-rw-r--r--   0        0        0    18109 2023-04-25 08:55:32.373899 encapsia_cli-0.5.4/encapsia_cli/plugininfo.py
+-rw-r--r--   0        0        0    31423 2023-04-25 08:39:10.483092 encapsia_cli-0.5.4/encapsia_cli/plugins.py
+-rw-r--r--   0        0        0     4296 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/run.py
+-rw-r--r--   0        0        0     1156 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/s3.py
+-rw-r--r--   0        0        0     2218 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/schedule.py
+-rw-r--r--   0        0        0      520 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/shell.py
+-rw-r--r--   0        0        0     3749 2023-02-02 13:22:51.981788 encapsia_cli-0.5.4/encapsia_cli/token.py
+-rw-r--r--   0        0        0     4391 2023-04-24 06:27:52.898295 encapsia_cli-0.5.4/encapsia_cli/users.py
+-rw-r--r--   0        0        0      300 2022-01-07 06:44:24.123731 encapsia_cli-0.5.4/encapsia_cli/version.py
+-rw-r--r--   0        0        0     1577 2023-04-24 06:36:19.352201 encapsia_cli-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2835 1970-01-01 00:00:00.000000 encapsia_cli-0.5.4/setup.py
+-rw-r--r--   0        0        0     2865 1970-01-01 00:00:00.000000 encapsia_cli-0.5.4/PKG-INFO
```

### Comparing `encapsia_cli-0.5.3/LICENSE` & `encapsia_cli-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/README.md` & `encapsia_cli-0.5.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,29 @@
 
 Run:
 
     poetry run pytest
 
 ### Walkthrough Tests
 
+Prerequisite: an instance of ice must be running on your localhost, and valid token for
+it must be present in your key store.
+
 See the `walkthrough_tests` directory for bash scripts which exercise the CLI.
 
 Run them e.g. with:
 
     poetry run bash walkthrough_tests/all.sh
 
 or test specific subcommands with:
 
     poetry run bash walkthrough_tests/token.sh
 
-Note that these tests are *not* self-verifying; they just provide helpful coverage, assurance, and working documentation.
+Note that these tests are *not* self-verifying; they just provide helpful coverage,
+assurance, and working documentation.
 
 ## Release checklist
 
 * Run: `poetry run black .`
 * Run: `poetry run isort .`
 * Run: `poetry run flake8 .`
 * Run: `poetry run mypy .`
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/completion.py` & `encapsia_cli-0.5.4/encapsia_cli/completion.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/config.py` & `encapsia_cli-0.5.4/encapsia_cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,24 +21,26 @@
 @click.argument("output", type=click.File("w"))
 @click.pass_obj
 def save(obj, output):
     """Save entire configuration to given file."""
     api = lib.get_api(**obj)
     config = api.get_all_config()
     lib.pretty_print(config, "json", output=output)
+    lib.log_output(f"Configuration saved to {output.name}")
 
 
 @main.command()
 @click.argument("input", type=click.File("r"))
 @click.pass_obj
 def load(obj, input):
     """Load (merge) configuration from given file."""
     api = lib.get_api(**obj)
     data = lib.parse(input.read(), "json")
     api.set_config_multi(data)
+    lib.log_output(f"Configuration loaded from {input.name}")
 
 
 @main.command()
 @click.argument("key")
 @click.pass_obj
 def get(obj, key):
     """Retrieve value against given key."""
@@ -57,16 +59,19 @@
 @click.argument("value")
 @click.pass_obj
 def set(obj, key, value):
     """Store value against given key."""
     api = lib.get_api(**obj)
     value = lib.parse(value, "json")
     api.set_config(key, value)
+    new_value = api.get_config(key)
+    lib.log_output(f"Configuration entry {key} has been set to {new_value}")
 
 
 @main.command()
 @click.argument("key")
 @click.pass_obj
 def delete(obj, key):
     """Delete value against given key."""
     api = lib.get_api(**obj)
     api.delete_config(key)
+    lib.log_output(f"Configuration entry {key} deleted")
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/database.py` & `encapsia_cli-0.5.4/encapsia_cli/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,20 +25,27 @@
     )
     filename = api.dbctl_download_data(handle, filename)
     lib.log(f"Downloaded {filename.stat().st_size} bytes to {filename}")
 
 
 @main.command()
 @click.argument("filename", type=click.Path(exists=True))
-@click.option("--force", is_flag=True, help="Don't prompt the user for confirmation.")
+@click.option(
+    "--force", is_flag=True, help="[DEPRECATED] Don't prompt the user for confirmation."
+)
+@click.option("--yes", is_flag=True, help="Don't prompt the user for confirmation.")
 @click.pass_obj
-def restore(obj, filename, force):
+def restore(obj, filename, force, yes):
     """Restore database from given backup file."""
+    if force:
+        lib.log_error(
+            "Warning: --force option is deprecated, please use the --yes option."
+        )
     filename = pathlib.Path(filename)
-    if not force:
+    if not (force or yes):
         click.confirm(
             f'Are you sure you want to restore the database from "{filename}"?',
             abort=True,
         )
     api = lib.get_api(**obj)
     handle = api.dbctl_upload_data(filename)
     # On a restore, the server is temporarily stopped.
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/encapsia.py` & `encapsia_cli-0.5.4/encapsia_cli/encapsia.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,22 @@
     default="auto",
     help="Control colour on stdout.",
 )
 @click.option(
     "--host",
     help="Name to use to lookup credentials in .encapsia/credentials.toml",
 )
+@click.option(
+    "--silent",
+    is_flag=True,
+    default=False,
+    help="Suppress normal output.",
+)
 @click.pass_context
-def main(ctx, colour, host):
+def main(ctx, colour, host, silent):
     """CLI to talk to an encapsia host.
 
     Options can be provided in one of three ways, in this priority order:
 
     \b
     1. On the command line as an --option.
     2. In an environment variable as ENCAPSIA_<OPTION> or ENCAPSIA_<SUBCOMMAND>_<OPTION>.
@@ -111,15 +117,15 @@
     Else abort.
 
     The tool will also abort if instructed to lookup in ~/.encapsia/credentials.toml
     but cannot find a correct entry.
 
     """
     ctx.color = {"always": True, "never": False, "auto": None}[colour]
-    ctx.obj = dict(host=host)
+    ctx.obj = dict(host=host, silent=silent)
 
 
 COMMANDS = [
     encapsia_cli.completion.main,
     encapsia_cli.config.main,
     encapsia_cli.database.main,
     encapsia_cli.fixtures.main,
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/fixtures.py` & `encapsia_cli-0.5.4/encapsia_cli/fixtures.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,36 +35,50 @@
             api, "create_fixture", dict(name=name), f"Creating fixture {name}"
         )
     )
 
 
 @main.command("use")
 @click.argument("name")
-@click.option("--force", is_flag=True, help="Don't prompt the user for confirmation.")
+@click.option(
+    "--force", is_flag=True, help="[DEPRECATED] Don't prompt the user for confirmation."
+)
+@click.option("--yes", is_flag=True, help="Don't prompt the user for confirmation.")
 @click.pass_obj
-def use_fixture(obj, name, force):
+def use_fixture(obj, name, force, yes):
     """Switch to fixture with given name."""
-    if not force:
+    if force:
+        lib.log_error(
+            "Warning: --force option is deprecated, please use the --yes option."
+        )
+    if not (force or yes):
         click.confirm(
             f'Are you sure you want to change the database to fixture "{name}"?',
             abort=True,
         )
     api = lib.get_api(**obj)
     poll, NoTaskResultYet = api.dbctl_action("use_fixture", dict(name=name))
     lib.log(f"Requested change to fixture {name}.")
     lib.log("Please verify by other means (e.g. look at the logs).")
 
 
 @main.command("delete")
 @click.argument("name")
-@click.option("--force", is_flag=True, help="Don't prompt the user for confirmation.")
+@click.option(
+    "--force", is_flag=True, help="[Deprecated] Don't prompt the user for confirmation."
+)
+@click.option("--yes", is_flag=True, help="Don't prompt the user for confirmation.")
 @click.pass_obj
-def delete_fixture(obj, name, force):
+def delete_fixture(obj, name, force, yes):
     """Delete fixture with given name."""
-    if not force:
+    if force:
+        lib.log_error(
+            "Warning: --force option is deprecated, please use the --yes option."
+        )
+    if not (force or yes):
         click.confirm(f'Are you sure you want to delete fixture "{name}"?', abort=True)
     api = lib.get_api(**obj)
     lib.log_output(
         lib.dbctl_action(
             api, "delete_fixture", dict(name=name), f"Deleting fixture {name}"
         )
     )
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/help.py` & `encapsia_cli-0.5.4/encapsia_cli/help.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/httpie.py` & `encapsia_cli-0.5.4/encapsia_cli/httpie.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/lib.py` & `encapsia_cli-0.5.4/encapsia_cli/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,21 @@
         was_auto = ""
     if shell not in SHELL_SET_ENV_TEMPLATES:
         log_error(f"Unsupported shell: {shell}{was_auto}", abort=True)
     return SHELL_SET_ENV_TEMPLATES[shell]
 
 
 def log(message="", nl=True):
-    click.secho(message, fg="yellow", nl=nl)
+    if not click.get_current_context().obj["silent"]:
+        click.secho(message, fg="yellow", nl=nl)
 
 
 def log_output(message=""):
-    click.secho(message, fg="green")
+    if not click.get_current_context().obj["silent"]:
+        click.secho(message, fg="green")
 
 
 def log_error(message="", abort=False):
     click.secho(message, fg="red", err=True)
     if abort:
         raise click.Abort()
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/plugininfo.py` & `encapsia_cli-0.5.4/encapsia_cli/plugininfo.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,62 +232,108 @@
                 ]
             )
         except s3.S3Error as e:
             lib.log_error(str(e), abort=True)
             return None  # Never reached, but keep linters happy
 
     @staticmethod
-    def make_from_encapsia(host: str) -> PluginInfos:
+    def make_from_encapsia(host: str, bad_plugins_bin=None) -> PluginInfos:
         api = lib.get_api(host=host)
         raw_info = api.run_view(
             "pluginsmanager",
             "plugins",
         )
         pis = []
         for i in raw_info:
-            tags = i.get("manifest").get("tags")
+            # keys should be present and non-null
+            MANDATORY_ENTRIES = ("name", "version")
+            missing_mandatory_entries = [
+                key for key in MANDATORY_ENTRIES if i.get(key) is None
+            ]
+            if missing_mandatory_entries:
+                lib.log_error(
+                    f"Invalid plugin info!\nMissing mandatory entries {missing_mandatory_entries} in {i}"
+                )
+                if bad_plugins_bin is not None:
+                    bad_plugins_bin.add(i.get("name"))
+                continue
+
+            # keys should be present and non-null
+            IMPORTANT_ENTRIES = ("manifest", "when")
+            missing_important_entries = [
+                key for key in IMPORTANT_ENTRIES if i.get(key) is None
+            ]
+            if missing_important_entries:
+                lib.log_error(
+                    f"Missing important information {missing_important_entries} for plugin {i}"
+                )
+                if bad_plugins_bin is not None:
+                    bad_plugins_bin.add(i.get("name"))
+
+            manifest = i.get("manifest")
+            tags = manifest.get("tags") if hasattr(manifest, "get") else None
             if not isinstance(tags, list):
                 tags = []
             try:
                 variant = get_variant_from_tags(tags)
             except TooManyVariantTagsError as e:
                 lib.log_error(f"Error in {i['name']} tag list: {e}")
+                if bad_plugins_bin is not None:
+                    bad_plugins_bin.add(i.get("name"))
             pi = PluginInfo.make_from_name_variant_version(
                 i["name"], variant, i["version"]
             )
             pi.extras.update(
                 {
-                    "description": i["description"],
-                    "installed": _format_datetime(i["when"]),
+                    "description": i.get("description"),
+                    "installed": (
+                        _format_datetime(i.get("when")) if "when" in i else "Unknown"
+                    ),
                     "plugin-tags": ", ".join(sorted(tags)),
                 }
             )
             pis.append(pi)
         return PluginInfos(pis)
 
-    def latest(self) -> T.Optional[PluginInfo]:
+    def latest(self, include_prereleases=True) -> T.Optional[PluginInfo]:
         """Returns greatest PluginInfo with in sort order (name, variant, version).
 
         Careful: this has little value when comparing plugins with different name and
         variant!
         """
-        return max(self.pis, default=None)
+        if not include_prereleases:
+            return max(
+                (pi for pi in self.pis if not pi.semver.prerelease), default=None
+            )
+        else:
+            return max(self.pis, default=None)
 
     def filter_to_latest(self) -> PluginInfos:
         groupped_pis = collections.defaultdict(list)
         for pi in self.pis:
             groupped_pis[(pi.name, pi.variant)].append(pi)
         return PluginInfos(
             p
             for pis in groupped_pis.values()
             if (p := PluginInfos(pis).latest()) is not None
         )
 
-    def latest_version_matching_spec(self, spec) -> T.Optional[PluginInfo]:
-        return PluginSpec.make_from_spec_or_string(spec).filter(self).latest()
+    def filter_out_prereleases(self, include_prereleases=False) -> PluginInfos:
+        if not include_prereleases:
+            return PluginInfos(pi for pi in self.pis if not pi.semver.prerelease)
+        return self
+
+    def latest_version_matching_spec(
+        self, spec, include_prereleases=True
+    ) -> T.Optional[PluginInfo]:
+        return (
+            PluginSpec.make_from_spec_or_string(spec)
+            .filter(self)
+            .latest(include_prereleases)
+        )
 
 
 @dataclass
 class PluginSpec:
     name: str
     variant: T_Variant
     version_prefix: str = ""
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/plugins.py` & `encapsia_cli-0.5.4/encapsia_cli/plugins.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,61 +59,70 @@
     lib.log(
         "\n(*) Plugin variant shown in square brackets when defined."
         "\n(**) Equivalent semver versions are shown in brackets when non-semver version is used."
     )
 
 
 def _add_to_local_store_from_uri(
-    plugins_local_dir: Path, uri: str, force: bool = False
+    plugins_local_dir: Path, uri: str, overwrite: bool = False
 ):
     full_name = uri.rsplit("/", 1)[-1]
     try:
         PluginInfo.make_from_filename(full_name)  # Will raise if name is invalid.
     except ValueError:
         lib.log_error("That doesn't look like a plugin. Aborting!", abort=True)
     store_filename = plugins_local_dir / full_name
-    if not force and store_filename.exists():
+    if not overwrite and store_filename.exists():
         lib.log(f"Found: {store_filename} (Skipping)")
     else:
         filename, headers = urllib.request.urlretrieve(uri, tempfile.mkstemp()[1])
         shutil.move(filename, store_filename)
         lib.log(f"Added to local store: {store_filename}")
 
 
 def _add_to_local_store_from_s3(
-    pi: PluginInfo, plugins_local_dir: Path, force: bool = False
+    pi: PluginInfo, plugins_local_dir: Path, overwrite: bool = False
 ):
     target = plugins_local_dir / pi.get_filename()
-    if not force and target.exists():
+    if not overwrite and target.exists():
         lib.log(f"Found: {target} (Skipping)")
     else:
         try:
             s3.download_file(pi.get_s3_bucket(), pi.get_s3_name(), target.as_posix())
         except s3.S3Error as e:
             lib.log_error(str(e))
         else:
             lib.log(
                 f"Downloaded {pi.get_s3_bucket()}/{pi.get_s3_name()} and saved to {target}"
             )
 
 
 def _create_install_plan(
-    candidates, installed, local_store, plugins_s3_buckets, force_install
+    candidates,
+    installed,
+    local_store,
+    plugins_s3_buckets,
+    bad_plugins,
+    allow_reinstall,
+    allow_downgrade,
+    include_prereleases,
 ):
     plan = []
     to_download_from_s3 = []
     s3_versions = None  # For performance, only fetch if/when first needed.
     for spec in candidates:
-        candidate = local_store.latest_version_matching_spec(spec)
+        candidate = local_store.latest_version_matching_spec(spec, include_prereleases)
         will_get_from_s3 = False
         if not candidate:
             if s3_versions is None:
                 s3_versions = PluginInfos.make_from_s3_buckets(plugins_s3_buckets)
             if (
-                candidate := s3_versions.latest_version_matching_spec(spec)
+                candidate := s3_versions.latest_version_matching_spec(
+                    spec, include_prereleases
+                )
             ) is not None:
                 to_download_from_s3.append(candidate)
                 will_get_from_s3 = True
             else:
                 lib.log_error(
                     f"Could not find plugin matching {spec} in local store nor S3",
                     abort=True,
@@ -122,20 +131,22 @@
             PluginSpec(spec.name, spec.variant)
         )
         if current:
             current_version = current.formatted_version()
             if current.semver < candidate.semver:
                 action = "upgrade"
             elif current.semver > candidate.semver:
-                action = "downgrade"
+                action = "downgrade" if allow_downgrade else "skip"
             else:
-                action = "reinstall" if force_install else "skip"
+                action = "reinstall" if allow_reinstall else "skip"
         else:
             current_version = ""
             action = "install"
+        if spec.name in bad_plugins:
+            action = "skip"
         if will_get_from_s3 and action != "skip":
             action = "download from s3 and " + action
         plan.append(
             [
                 candidate,  # keep first for sorting
                 candidate.name_and_variant(),
                 current_version,
@@ -165,15 +176,17 @@
 
 
 def _download_plugins_from_s3(
     plugins_to_download, plugins_local_dir, plugins_force, added_from_file_or_uri=False
 ):
     if plugins_to_download:
         for plugin in plugins_to_download:
-            _add_to_local_store_from_s3(plugin, plugins_local_dir, force=plugins_force)
+            _add_to_local_store_from_s3(
+                plugin, plugins_local_dir, overwrite=plugins_force
+            )
     else:
         if not added_from_file_or_uri:
             lib.log("Nothing to do!")
 
 
 @click.group("plugins")
 @click.option(
@@ -190,33 +203,45 @@
     default="ice-plugins",
     help="Name of AWS S3 bucket (or path) containing plugins (may be provided multiple times).",
 )
 @click.option(
     "--force",
     is_flag=True,
     default=False,
-    help="Always fetch/build/etc again.",
+    help="[DEPRECATED] Always fetch/build/etc again.",
 )
 @click.pass_context
 def main(ctx, force, s3_buckets, local_dir):
     """Install, uninstall, create, and update plugins."""
+    if force:
+        lib.log_error(
+            "Warning: --force option is deprecated, please use the other available options (use --help to find them)."
+        )
     ctx.obj["plugins_local_dir"] = Path(local_dir).expanduser()
     ctx.obj["plugins_local_dir"].mkdir(parents=True, exist_ok=True)
     ctx.obj["plugins_s3_buckets"] = s3_buckets
     ctx.obj["plugins_force"] = force
 
 
 @main.command()
 @click.pass_obj
 def freeze(obj):
     """Print currently installed plugins as versions TOML."""
+    bad_plugins = set()
     versions = PluginSpecs.make_from_plugininfos(
-        PluginInfos.make_from_encapsia(obj["host"])
+        PluginInfos.make_from_encapsia(obj["host"], bad_plugins)
     ).as_version_dict()
-    lib.log_output(toml.dumps(versions))
+    for pl_name in versions.keys():
+        color = "red" if pl_name in bad_plugins else None
+        lib.log_output(click.style(f"{pl_name} = {versions[pl_name]}", fg=color))
+    if bad_plugins:
+        lib.log_error(
+            "There were some errors in the plugin metadata retrieved from server"
+        )
+        raise click.Abort()
 
 
 @main.command()
 @click.argument("plugins", nargs=-1)
 @click.pass_obj
 def logs(obj, plugins):
     """Print the latest install logs for given plugins."""
@@ -266,36 +291,43 @@
 def status(obj, long_format, plugins):
     """Print information about (successfully) installed plugins."""
     host = obj["host"]
     plugins_local_dir = obj["plugins_local_dir"]
     local_versions = PluginInfos.make_from_local_store(
         plugins_local_dir
     ).filter_to_latest()
-    plugin_infos = PluginInfos.make_from_encapsia(host)
+    bad_plugins = set()
+    plugin_infos = PluginInfos.make_from_encapsia(host, bad_plugins)
     if plugins:
         specs = PluginSpecs.make_from_spec_strings(plugins)
         plugin_infos = specs.filter(plugin_infos)
 
     headers = ["name*", "version**", "available**", "installed"]
     if long_format:
         headers.extend(["description", "plugin-tags"])
 
     info = []
     for pi in plugin_infos:
+        print_reverse = pi.name in bad_plugins
         pi_info = [
-            pi.name_and_variant(),
+            click.style(pi.name_and_variant(), reverse=print_reverse, reset=False),
             pi.formatted_version(),
             _get_available_from_local_store(local_versions, pi),
             pi.extras["installed"],
         ]
         if long_format:
             pi_info.extend([pi.extras["description"], pi.extras["plugin-tags"]])
         info.append(pi_info)
     lib.log(tabulate(info, headers=headers))
     _log_message_explaining_headers()
+    if bad_plugins:
+        lib.log_error(
+            "There were some errors in the plugin metadata retrieved from server"
+        )
+        raise click.Abort()
 
 
 @main.command()
 @click.option(
     "--versions", default=None, help="TOML file containing plugin names and versions."
 )
 @click.option(
@@ -309,17 +341,67 @@
 )
 @click.option(
     "--all-available",
     is_flag=True,
     default=False,
     help="Download all available plugins from s3.",
 )
+@click.option(
+    "--yes",
+    is_flag=True,
+    default=False,
+    help="Do not prompt for confirmation after presenting the install plan.",
+)
+@click.option(
+    "--reinstall",
+    is_flag=True,
+    default=False,
+    help="Allow re-installing plugins even if the same version is already installed.",
+)
+@click.option(
+    "--downgrade",
+    is_flag=True,
+    default=False,
+    help="Allow installing plugins even if a newer version is already installed.",
+)
+@click.option(
+    "--overwrite",
+    is_flag=True,
+    default=False,
+    help="Overwrite existing plugins having the same name and version in the local store.",
+)
+@click.option(
+    "--ignore-warnings",
+    is_flag=True,
+    default=False,
+    help="In case of warnings, try to perform the installation of plugins that are deemed to be safe (from the supplied list) - instead of aborting the operation completely.",
+)
+@click.option(
+    "--include-prereleases",
+    "--pre",
+    is_flag=True,
+    default=False,
+    help="Include pre-release builds when looking for the latest available version in the local store.",
+)
 @click.argument("plugins", nargs=-1)
 @click.pass_obj
-def install(obj, versions, show_logs, latest_existing, all_available, plugins):
+def install(
+    obj,
+    versions,
+    show_logs,
+    latest_existing,
+    all_available,
+    yes,
+    reinstall,
+    downgrade,
+    overwrite,
+    ignore_warnings,
+    include_prereleases,
+    plugins,
+):
     """Install/upgrade plugins by name, from files, or from a versions.toml file.
 
     Plugins provided as files are put in the local store before being installed.
 
     When described by name alone, the latest plugin of that name in the local store will be used.
 
     Plugins specified in the versions.toml file will be taken from the local store.
@@ -334,15 +416,15 @@
     to_install_candidates = []
     for plugin in plugins:
         if PluginInfo.looks_like_path_to_plugin(plugin):
             plugin_filename = Path(plugin).resolve()
             if plugin_filename.is_file():
                 # If it looks like a file then just add it.
                 _add_to_local_store_from_uri(
-                    plugins_local_dir, plugin_filename.as_uri(), force=True
+                    plugins_local_dir, plugin_filename.as_uri(), overwrite=True
                 )
                 plugin_info = PluginInfo.make_from_filename(plugin_filename)
                 plugin_spec = PluginSpec.make_from_plugininfo(plugin_info)
                 to_install_candidates.append(plugin_spec)
             else:
                 lib.log_error(
                     f"The requested plugin '{plugin}', which looks like a path to a file, was not found."
@@ -361,49 +443,62 @@
         to_install_candidates.extend(
             PluginSpec(pi.name, pi.variant)
             for pi in PluginInfos.make_from_encapsia(host)
         )
 
     # Get the plugins from S3
     if all_available and plugins_s3_buckets:
-        s3_plugins = PluginInfos.make_from_s3_buckets(plugins_s3_buckets)
+        s3_plugins = PluginInfos.make_from_s3_buckets(
+            plugins_s3_buckets
+        ).filter_out_prereleases(include_prereleases)
         for s3_plugin in s3_plugins:
             _add_to_local_store_from_s3(
-                s3_plugin, plugins_local_dir, force=plugins_force
+                s3_plugin, plugins_local_dir, overwrite=(plugins_force or overwrite)
             )
             to_install_candidates.append(PluginSpec.make_from_plugininfo(s3_plugin))
 
     # Work out and list installation plan.
     # to_install_candidates = sorted(PluginInfos(to_install_candidates))
-    installed = PluginInfos.make_from_encapsia(host)
+    bad_plugins = set()
+    installed = PluginInfos.make_from_encapsia(host, bad_plugins)
+    if bad_plugins and not ignore_warnings:
+        lib.log_error(
+            "There are some plugin metadata errors on the destination server. Use --ignore-warnings to install only the plugins that are not impacted.",
+            abort=True,
+        )
     local_store = PluginInfos.make_from_local_store(plugins_local_dir)
     plan, to_download_from_s3 = _create_install_plan(
         to_install_candidates,
         installed,
         local_store,
         plugins_s3_buckets,
-        force_install=plugins_force,
+        bad_plugins,
+        allow_reinstall=plugins_force or reinstall,
+        allow_downgrade=plugins_force or downgrade,
+        include_prereleases=include_prereleases,
     )
     to_install = [i[0] for i in plan if i[4] != "skip"]
     headers = ["name*", "existing version**", "new version**", "action"]
     lib.log(tabulate([i[1:] for i in plan], headers=headers))
     _log_message_explaining_headers()
 
     # Seek confirmation unless force.
-    if to_install and not plugins_force:
+    if to_install and not (plugins_force or yes):
         click.confirm(
-            "Do you wish to proceed with the above plan?",
+            "Do you wish to proceed?",
             abort=True,
         )
 
     # Install them.
     lib.log("")
     if to_install:
         for pi in to_download_from_s3:
-            _add_to_local_store_from_s3(pi, plugins_local_dir, force=plugins_force)
+            _add_to_local_store_from_s3(
+                pi, plugins_local_dir, overwrite=(plugins_force or overwrite)
+            )
         api = lib.get_api(**obj)
         for pi in to_install:
             success = _install_plugin(
                 api, plugins_local_dir / pi.get_filename(), print_output=show_logs
             )
         if not success:
             lib.log_error("Some plugins failed to install.", abort=True)
@@ -424,19 +519,22 @@
     return len(matching_plugins) > 0
 
 
 @main.command()
 @click.option(
     "--show-logs", is_flag=True, default=False, help="Print installation logs."
 )
+@click.option(
+    "--yes", is_flag=True, default=False, help="Do not prompt for confirmation."
+)
 @click.argument("namespaces", nargs=-1)
 @click.pass_obj
-def uninstall(obj, show_logs, namespaces):
+def uninstall(obj, show_logs, yes, namespaces):
     """Uninstall named plugin(s)."""
-    if namespaces and not obj["plugins_force"]:
+    if namespaces and not (obj["plugins_force"] or yes):
         lib.log("Preparing to uninstall: " + ", ".join(namespaces))
         click.confirm(
             "Are you sure?",
             abort=True,
         )
     api = lib.get_api(**obj)
     for namespace in namespaces:
@@ -507,29 +605,36 @@
                         self.data[name] = datetime.datetime.utcnow()
                 else:
                     yield Path(name)
                     self.data[name] = datetime.datetime.utcnow()
 
 
 @main.command("dev-update")
+@click.option(
+    "--all",
+    "upload_all",
+    is_flag=True,
+    default=False,
+    help="Upload all folders, not just the new or modified ones.",
+)
 @click.argument("directory", default=".")
 @click.pass_obj
-def dev_update(obj, directory):
+def dev_update(obj, upload_all, directory):
     """Update plugin parts which have changed since previous update.
 
     Optionally pass in the DIRECTORY of the plugin (defaults to cwd).
 
     """
     directory = Path(directory)
     plugin_toml_path = directory / "plugin.toml"
     if not plugin_toml_path.exists():
         lib.log_error("Not in a plugin directory.", abort=True)
 
     with _get_modified_plugin_directories(
-        directory, reset=obj["plugins_force"]
+        directory, reset=obj["plugins_force"] or upload_all
     ) as modified_plugin_directories:
         if modified_plugin_directories:
             with lib.temp_directory() as temp_directory:
                 shutil.copy(plugin_toml_path, temp_directory)
                 for modified_directory in modified_plugin_directories:
                     lib.log(f"Including: {modified_directory}")
                     shutil.copytree(
@@ -562,45 +667,60 @@
         "dev_create_namespace",
         dict(namespace=namespace, n_task_workers=n_task_workers),
         "Creating namespace",
     )
 
 
 @main.command("dev-destroy")
-@click.option("--all", is_flag=True, default=False, help="Destroy all namespaces!")
+@click.option(
+    "--all", "destroy_all", is_flag=True, default=False, help="Destroy all namespaces!"
+)
+@click.option(
+    "--yes", is_flag=True, default=False, help="Do not prompt for confirmation."
+)
 @click.argument("namespaces", nargs=-1)
 @click.pass_obj
-def dev_destroy(obj, all, namespaces):
+def dev_destroy(obj, destroy_all, yes, namespaces):
     """Destroy namespace(s) of given name. Only useful during development"""
     api = lib.get_api(**obj)
-    if all:
-        click.confirm(
-            "Are you sure you want to destroy all namespaces?",
-            abort=True,
-        )
+    if destroy_all:
+        plugins_force = obj["plugins_force"]
+        if not (plugins_force or yes):
+            click.confirm(
+                "Are you sure you want to destroy all namespaces?",
+                abort=True,
+            )
         lib.run_plugins_task(
             api,
             "dev_wipe",
             {},
             "Destroying all namespaces",
         )
     else:
+        if len(namespaces) == 0:
+            lib.log("Specify at least one namespace or --all")
         for namespace in namespaces:
             lib.run_plugins_task(
                 api,
                 "dev_destroy_namespace",
                 dict(namespace=namespace),
                 f"Destroying namespace: {namespace}",
             )
 
 
 @main.command()
+@click.option(
+    "--overwrite",
+    is_flag=True,
+    default=False,
+    help="Overwrite any existing plugin with the same name and version in the local store.",
+)
 @click.argument("sources", nargs=-1)
 @click.pass_obj
-def dev_build(obj, sources):
+def dev_build(obj, overwrite, sources):
     """Build plugins from given source directories."""
     plugins_local_dir = obj["plugins_local_dir"]
     plugins_force = obj["plugins_force"]
     for source_directory in sources:
         source_directory = Path(source_directory)
         manifest = lib.read_toml(source_directory / "plugin.toml")
         name = manifest["name"]
@@ -612,15 +732,15 @@
             lib.log_error(str(e), abort=True)
         if variant:
             output_filename = (
                 plugins_local_dir / f"plugin-{name}-variant-{variant}-{version}.tar.gz"
             )
         else:
             output_filename = plugins_local_dir / f"plugin-{name}-{version}.tar.gz"
-        if not plugins_force and output_filename.exists():
+        if not (plugins_force or overwrite) and output_filename.exists():
             lib.log(f"Found: {output_filename} (Skipping)")
         else:
             with lib.temp_directory() as temp_directory:
                 base_dir = temp_directory / f"plugin-{name}-{version}"
                 base_dir.mkdir()
                 for t in (
                     "webfiles",
@@ -640,14 +760,15 @@
                 lib.log(f"Added to local store: {output_filename}")
 
 
 @main.command()
 @click.argument("plugins", nargs=-1)
 @click.option(
     "--all-versions",
+    "--all",
     is_flag=True,
     default=False,
     help="List all versions, not just the latest.",
 )
 @click.pass_obj
 def upstream(obj, plugins, all_versions):
     """Print information about plugins on S3.
@@ -686,47 +807,77 @@
 )
 @click.option(
     "--all-available",
     is_flag=True,
     default=False,
     help="Add to local store all available plugins from s3.",
 )
+@click.option(
+    "--overwrite",
+    is_flag=True,
+    default=False,
+    help="Overwrite if the same plugin version already exists in the local store.",
+)
+@click.option(
+    "--include-prereleases",
+    "--pre",
+    is_flag=True,
+    default=False,
+    help="Include pre-release builds when looking for the latest available version in the S3 buckets.",
+)
+@click.option(
+    "--ignore-warnings",
+    is_flag=True,
+    default=False,
+    help="In case of warnings, try to add only the plugins that are found in S3 buckets - instead of aborting the operation completely.",
+)
 @click.argument("plugins", nargs=-1)
 @click.pass_obj
-def add(obj, versions, latest_existing, all_available, plugins):
+def add(
+    obj,
+    versions,
+    latest_existing,
+    all_available,
+    overwrite,
+    include_prereleases,
+    ignore_warnings,
+    plugins,
+):
     """Add plugin(s) to local store from file, URL, or S3."""
     plugins_local_dir = obj["plugins_local_dir"]
     plugins_s3_buckets = obj["plugins_s3_buckets"]
-    plugins_force = obj["plugins_force"]
+    overwrite = overwrite or obj["plugins_force"]
     host = obj["host"]
 
     specs_to_search_in_s3 = []
     to_download_from_s3 = []
     s3_versions = None  # For performance, only fetch if/when first needed.
     added_from_file_or_uri = False
 
     # Get all available plugins from S3
     if all_available and plugins_s3_buckets:
         _download_plugins_from_s3(
-            PluginInfos.make_from_s3_buckets(plugins_s3_buckets),
+            PluginInfos.make_from_s3_buckets(plugins_s3_buckets).filter_out_prereleases(
+                include_prereleases
+            ),
             plugins_local_dir,
-            plugins_force,
+            overwrite,
         )
         return
 
     for plugin in plugins:
         if Path(plugin).is_file():
             _add_to_local_store_from_uri(
                 plugins_local_dir,
                 Path(plugin).resolve().as_uri(),
-                plugins_force,
+                overwrite,
             )
             added_from_file_or_uri = True
         elif urllib.parse.urlparse(plugin).scheme != "":
-            _add_to_local_store_from_uri(plugins_local_dir, plugin, plugins_force)
+            _add_to_local_store_from_uri(plugins_local_dir, plugin, overwrite)
             added_from_file_or_uri = True
         else:
             specs_to_search_in_s3.append(PluginSpec.make_from_string(plugin))
     if versions:
         specs_to_search_in_s3.extend(
             PluginSpecs.make_from_version_dict(
                 lib.read_toml(Path(versions).expanduser())
@@ -736,27 +887,31 @@
         specs_to_search_in_s3.extend(
             PluginSpecs.make_from_plugininfos(PluginInfos.make_from_encapsia(host))
         )
     if specs_to_search_in_s3:
         s3_versions = PluginInfos.make_from_s3_buckets(plugins_s3_buckets)
         not_found = []
         for spec in specs_to_search_in_s3:
-            if (pi := s3_versions.latest_version_matching_spec(spec)) is not None:
+            if (
+                pi := s3_versions.latest_version_matching_spec(
+                    spec, include_prereleases
+                )
+            ) is not None:
                 to_download_from_s3.append(pi)
             else:
                 not_found.append(spec)
         if not_found:
             lib.log_error(
                 "Some plugins could not be found in S3: {}".format(
                     ", ".join(str(s) for s in not_found)
                 ),
-                abort=True,
+                abort=not ignore_warnings,
             )
     _download_plugins_from_s3(
-        to_download_from_s3, plugins_local_dir, plugins_force, added_from_file_or_uri
+        to_download_from_s3, plugins_local_dir, overwrite, added_from_file_or_uri
     )
 
 
 @main.command()
 @click.option(
     "--all-versions",
     is_flag=True,
```

### Comparing `encapsia_cli-0.5.3/encapsia_cli/run.py` & `encapsia_cli-0.5.4/encapsia_cli/run.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/s3.py` & `encapsia_cli-0.5.4/encapsia_cli/s3.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/schedule.py` & `encapsia_cli-0.5.4/encapsia_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/shell.py` & `encapsia_cli-0.5.4/encapsia_cli/shell.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/token.py` & `encapsia_cli-0.5.4/encapsia_cli/token.py`

 * *Files identical despite different names*

### Comparing `encapsia_cli-0.5.3/encapsia_cli/users.py` & `encapsia_cli-0.5.4/encapsia_cli/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,25 +15,27 @@
 @click.argument("description")
 @click.argument("capabilities")
 @click.pass_obj
 def add_systemuser(obj, description, capabilities):
     """Create system user with suitable user and role."""
     api = lib.get_api(**obj)
     api.add_system_user(description, [x.strip() for x in capabilities.split(",")])
+    lib.log_output(f"System user and role for {description} successfully created")
 
 
 @main.command()
 @click.argument("email", callback=lib.validate_email)
 @click.argument("first_name")
 @click.argument("last_name")
 @click.pass_obj
 def add_superuser(obj, email, first_name, last_name):
     """Create superuser with suitable user and role."""
     api = lib.get_api(**obj)
     api.add_super_user(email, first_name, last_name)
+    lib.log_output(f"Superuser {email} successfully created")
 
 
 @main.command("list")
 @click.option("--super-users/--no-super-users", default=False)
 @click.option("--system-users/--no-system-users", default=False)
 @click.option("--all-users/--no-all-users", default=False)
 @click.pass_obj
@@ -87,14 +89,15 @@
 @main.command("delete")
 @click.argument("email", callback=lib.validate_email)
 @click.pass_obj
 def delete_user(obj, email):
     """Delete user (but *do not* delete any related role)."""
     api = lib.get_api(**obj)
     api.delete_user(email)
+    lib.log_output(f"User {email} successfully deleted")
 
 
 @main.command("export")
 @click.argument(
     "filename", type=click.Path(writable=True, readable=False), required=True
 )
 @click.option("--with-roles/--without-roles", default=True)
```

### Comparing `encapsia_cli-0.5.3/pyproject.toml` & `encapsia_cli-0.5.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encapsia-cli"
-version = "0.5.3"
+version = "0.5.4"
 description = "Client CLI for talking to an Encapsia system."
 readme = "README.md"
 authors = ["Timothy Corbett-Clark <timothy.corbettclark@gmail.com>"]
 maintainers = ["Petre Mierluțiu <pmierlutiu@cmedtechnology.com>"]
 license = "MIT"
 keywords = ["encapsia", "eSource", "EDC", "Clinical Trials"]
 homepage = "https://github.com/Encapsia/encapsia-cli"
```

### Comparing `encapsia_cli-0.5.3/setup.py` & `encapsia_cli-0.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 {'httpie-shell': ['http-prompt>=1.0,<2.0']}
 
 entry_points = \
 {'console_scripts': ['encapsia = encapsia_cli.encapsia:encapsia']}
 
 setup_kwargs = {
     'name': 'encapsia-cli',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Client CLI for talking to an Encapsia system.',
-    'long_description': '# About\n\n[![Known Vulnerabilities](https://snyk.io/test/github/encapsia/encapsia-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/encapsia/encapsia-cli?targetFile=requirements.txt)\n\nThis package provides command line access to Encapsia over the REST API.\n\nAll of these are designed to work with server 1.5 and beyond.\n\n## Autocomplete\n\nSetup autocomplete using the instructions found on <https://github.com/click-contrib/click-completion>\n\n## Tests\n\n### Unit tests\n\nRun:\n\n    poetry run pytest\n\n### Walkthrough Tests\n\nSee the `walkthrough_tests` directory for bash scripts which exercise the CLI.\n\nRun them e.g. with:\n\n    poetry run bash walkthrough_tests/all.sh\n\nor test specific subcommands with:\n\n    poetry run bash walkthrough_tests/token.sh\n\nNote that these tests are *not* self-verifying; they just provide helpful coverage, assurance, and working documentation.\n\n## Release checklist\n\n* Run: `poetry run black .`\n* Run: `poetry run isort .`\n* Run: `poetry run flake8 .`\n* Run: `poetry run mypy .`\n* Ensure "tests" run ok (see above).\n* Capture test output and commit with: `poetry run bash walkthrough_tests/all.sh 2>&1 | poetry run ansi2html -f 80% >WALKTHROUGH.html`\n* Create `requirements.txt` for Snyk scanning with: `poetry export -f requirements.txt >requirements.txt`\n* Ensure git tag, package version, and `encapsia_cli.__version__` are all equal.\n',
+    'long_description': '# About\n\n[![Known Vulnerabilities](https://snyk.io/test/github/encapsia/encapsia-cli/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/encapsia/encapsia-cli?targetFile=requirements.txt)\n\nThis package provides command line access to Encapsia over the REST API.\n\nAll of these are designed to work with server 1.5 and beyond.\n\n## Autocomplete\n\nSetup autocomplete using the instructions found on <https://github.com/click-contrib/click-completion>\n\n## Tests\n\n### Unit tests\n\nRun:\n\n    poetry run pytest\n\n### Walkthrough Tests\n\nPrerequisite: an instance of ice must be running on your localhost, and valid token for\nit must be present in your key store.\n\nSee the `walkthrough_tests` directory for bash scripts which exercise the CLI.\n\nRun them e.g. with:\n\n    poetry run bash walkthrough_tests/all.sh\n\nor test specific subcommands with:\n\n    poetry run bash walkthrough_tests/token.sh\n\nNote that these tests are *not* self-verifying; they just provide helpful coverage,\nassurance, and working documentation.\n\n## Release checklist\n\n* Run: `poetry run black .`\n* Run: `poetry run isort .`\n* Run: `poetry run flake8 .`\n* Run: `poetry run mypy .`\n* Ensure "tests" run ok (see above).\n* Capture test output and commit with: `poetry run bash walkthrough_tests/all.sh 2>&1 | poetry run ansi2html -f 80% >WALKTHROUGH.html`\n* Create `requirements.txt` for Snyk scanning with: `poetry export -f requirements.txt >requirements.txt`\n* Ensure git tag, package version, and `encapsia_cli.__version__` are all equal.\n',
     'author': 'Timothy Corbett-Clark',
     'author_email': 'timothy.corbettclark@gmail.com',
     'maintainer': 'Petre Mierluțiu',
     'maintainer_email': 'pmierlutiu@cmedtechnology.com',
     'url': 'https://github.com/Encapsia/encapsia-cli',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `encapsia_cli-0.5.3/PKG-INFO` & `encapsia_cli-0.5.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encapsia-cli
-Version: 0.5.3
+Version: 0.5.4
 Summary: Client CLI for talking to an Encapsia system.
 Home-page: https://github.com/Encapsia/encapsia-cli
 License: MIT
 Keywords: encapsia,eSource,EDC,Clinical Trials
 Author: Timothy Corbett-Clark
 Author-email: timothy.corbettclark@gmail.com
 Maintainer: Petre Mierluțiu
@@ -50,25 +50,29 @@
 
 Run:
 
     poetry run pytest
 
 ### Walkthrough Tests
 
+Prerequisite: an instance of ice must be running on your localhost, and valid token for
+it must be present in your key store.
+
 See the `walkthrough_tests` directory for bash scripts which exercise the CLI.
 
 Run them e.g. with:
 
     poetry run bash walkthrough_tests/all.sh
 
 or test specific subcommands with:
 
     poetry run bash walkthrough_tests/token.sh
 
-Note that these tests are *not* self-verifying; they just provide helpful coverage, assurance, and working documentation.
+Note that these tests are *not* self-verifying; they just provide helpful coverage,
+assurance, and working documentation.
 
 ## Release checklist
 
 * Run: `poetry run black .`
 * Run: `poetry run isort .`
 * Run: `poetry run flake8 .`
 * Run: `poetry run mypy .`
```

