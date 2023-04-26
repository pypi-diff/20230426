# Comparing `tmp/aaz-dev-1.2.0.tar.gz` & `tmp/aaz-dev-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aaz-dev-1.2.0.tar", last modified: Wed Apr 26 03:24:13 2023, max compression
+gzip compressed data, was "aaz-dev-1.2.1.tar", last modified: Wed Apr 26 07:05:27 2023, max compression
```

## Comparing `aaz-dev-1.2.0.tar` & `aaz-dev-1.2.1.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.613742 aaz-dev-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-26 03:24:13.613742 aaz-dev-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 03:24:13.613742 aaz-dev-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.553741 aaz-dev-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.561741 aaz-dev-1.2.0/src/aaz_dev/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.565741 aaz-dev-1.2.0/src/aaz_dev/app/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/app/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/app/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/app/url_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.565741 aaz-dev-1.2.0/src/aaz_dev/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.565741 aaz-dev-1.2.0/src/aaz_dev/cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/api/az.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/api/portal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.569742 aaz-dev-1.2.0/src/aaz_dev/cli/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_arg_group_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_module_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    38422 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_operation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_profile_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_selector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/controller/portal_cli_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.569742 aaz-dev-1.2.0/src/aaz_dev/cli/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.569742 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.569742 aaz-dev-1.2.0/src/aaz_dev/cli/model/common/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/common/_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.569742 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/command/
--rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/group/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.573742 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/setup.cfg.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/setup.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/_help.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/_params.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/commands.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/custom.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/tests/profile/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/cli/templates/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/command/api/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/api/_cmds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/api/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.577741 aaz-dev-1.2.0/src/aaz_dev/command/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/cfg_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/cfg_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/specs_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    67823 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/workspace_cfg_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/controller/workspace_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.581742 aaz-dev-1.2.0/src/aaz_dev/command/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.585742 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_command_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_content.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_format.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_help.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http_request_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http_response_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_selector_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_subresource_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.585742 aaz-dev-1.2.0/src/aaz_dev/command/model/editor/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/editor/_workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.589742 aaz-dev-1.2.0/src/aaz_dev/command/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/specs/_command_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/model/specs/_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.589742 aaz-dev-1.2.0/src/aaz_dev/command/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/command.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/group.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/resource_ref.md.j2
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/command/templates/tree.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.589742 aaz-dev-1.2.0/src/aaz_dev/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.589742 aaz-dev-1.2.0/src/aaz_dev/swagger/api/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/api/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.593742 aaz-dev-1.2.0/src/aaz_dev/swagger/controller/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/controller/command_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/controller/specs_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.593742 aaz-dev-1.2.0/src/aaz_dev/swagger/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.601742 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/cmd_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/external_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    17557 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/items.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/path_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    28604 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/security_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/swagger.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.601742 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_resource_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.601742 aaz-dev-1.2.0/src/aaz_dev/swagger/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/swagger/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.601742 aaz-dev-1.2.0/src/aaz_dev/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-26 03:23:41.000000 aaz-dev-1.2.0/src/aaz_dev/ui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-26 03:23:41.000000 aaz-dev-1.2.0/src/aaz_dev/ui/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-26 03:23:41.000000 aaz-dev-1.2.0/src/aaz_dev/ui/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 03:23:41.000000 aaz-dev-1.2.0/src/aaz_dev/ui/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 03:23:41.000000 aaz-dev-1.2.0/src/aaz_dev/ui/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.561741 aaz-dev-1.2.0/src/aaz_dev/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.605742 aaz-dev-1.2.0/src/aaz_dev/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.609742 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   574621 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  2235009 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   146530 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)   473250 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-26 03:24:12.000000 aaz-dev-1.2.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.613742 aaz-dev-1.2.0/src/aaz_dev/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/error_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/plane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/portal_file_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/src/aaz_dev/utils/stage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 03:24:13.561741 aaz-dev-1.2.0/src/aaz_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 03:24:13.000000 aaz-dev-1.2.0/src/aaz_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 03:23:22.000000 aaz-dev-1.2.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:27.002711 aaz-dev-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-04-26 07:05:27.002711 aaz-dev-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 07:05:27.002711 aaz-dev-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.926710 aaz-dev-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.942710 aaz-dev-1.2.1/src/aaz_dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.946710 aaz-dev-1.2.1/src/aaz_dev/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/app/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/app/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/app/url_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.946710 aaz-dev-1.2.1/src/aaz_dev/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.946710 aaz-dev-1.2.1/src/aaz_dev/cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/api/az.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/api/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.950710 aaz-dev-1.2.1/src/aaz_dev/cli/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18344 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_arg_group_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_atomic_profile_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27518 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_module_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38422 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_operation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_profile_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_selector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/controller/portal_cli_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.950710 aaz-dev-1.2.1/src/aaz_dev/cli/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.954710 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.954710 aaz-dev-1.2.1/src/aaz_dev/cli/model/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/common/_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.954710 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/command/
+-rw-r--r--   0 runner    (1001) docker     (123)    31868 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/group/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/profile/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.958710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/HISTORY.rst.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.962710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.962710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.962710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/setup.cfg.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/setup.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.966710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/_help.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/_params.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/commands.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/custom.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.966710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/tests/__init__.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.966710 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/tests/profile/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/tests/profile/test_.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/cli/templates/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.966710 aaz-dev-1.2.1/src/aaz_dev/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.966710 aaz-dev-1.2.1/src/aaz_dev/command/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/api/_cmds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24148 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/api/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.970710 aaz-dev-1.2.1/src/aaz_dev/command/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41315 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/cfg_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/cfg_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/specs_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67823 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/workspace_cfg_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40663 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/controller/workspace_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.970710 aaz-dev-1.2.1/src/aaz_dev/command/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.982710 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16344 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16261 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_command_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10501 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http_response_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_selector_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_subresource_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.982710 aaz-dev-1.2.1/src/aaz_dev/command/model/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/editor/_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.982710 aaz-dev-1.2.1/src/aaz_dev/command/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/specs/_command_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/model/specs/_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.986710 aaz-dev-1.2.1/src/aaz_dev/command/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/command.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/group.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/resource_ref.md.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/command/templates/tree.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.986710 aaz-dev-1.2.1/src/aaz_dev/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.986710 aaz-dev-1.2.1/src/aaz_dev/swagger/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/api/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.986710 aaz-dev-1.2.1/src/aaz_dev/swagger/controller/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23496 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/controller/command_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/controller/specs_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.986710 aaz-dev-1.2.1/src/aaz_dev/swagger/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.994711 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25842 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/cmd_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/external_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18051 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11258 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/path_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28691 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/security_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5933 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_odata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_pageable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.994711 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_resource_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.994711 aaz-dev-1.2.1/src/aaz_dev/swagger/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/swagger/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.994711 aaz-dev-1.2.1/src/aaz_dev/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-26 07:05:02.000000 aaz-dev-1.2.1/src/aaz_dev/ui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-04-26 07:05:02.000000 aaz-dev-1.2.1/src/aaz_dev/ui/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-26 07:05:02.000000 aaz-dev-1.2.1/src/aaz_dev/ui/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-04-26 07:05:02.000000 aaz-dev-1.2.1/src/aaz_dev/ui/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 07:05:02.000000 aaz-dev-1.2.1/src/aaz_dev/ui/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.938710 aaz-dev-1.2.1/src/aaz_dev/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.994711 aaz-dev-1.2.1/src/aaz_dev/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.998711 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   574621 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2235009 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   146530 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)   473250 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.998711 aaz-dev-1.2.1/src/aaz_dev/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/error_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/portal_file_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/src/aaz_dev/utils/stage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 07:05:26.942710 aaz-dev-1.2.1/src/aaz_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8674 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8475 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-26 07:05:26.000000 aaz-dev-1.2.1/src/aaz_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-26 07:04:49.000000 aaz-dev-1.2.1/version.py
```

### Comparing `aaz-dev-1.2.0/HISTORY.rst` & `aaz-dev-1.2.1/HISTORY.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 .. :changelog:
 
 Release History
 ===============
 
+1.2.1
+++++++
+* Support x-typespec-name and x-typespec-generated in swagger (#243)
+
 1.2.0
 ++++++
 * Support argument prompt input (#238)
 * Setup Github Pages, move content into docs and link docs to Github Pages in aaz-dev-tools (#240)
 
 1.1.1
 ++++++
```

### Comparing `aaz-dev-1.2.0/LICENSE` & `aaz-dev-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/PKG-INFO` & `aaz-dev-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.2.0
+Version: 1.2.1
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [Doc](./src/aaz_dev/docs/Docs#introduction-to-aazdev) or [Video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9)
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-1.2.0/README.md` & `aaz-dev-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [Doc](./src/aaz_dev/docs/Docs#introduction-to-aazdev) or [Video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9)
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-1.2.0/setup.py` & `aaz-dev-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/app/app.py` & `aaz-dev-1.2.1/src/aaz_dev/app/app.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/app/run.py` & `aaz-dev-1.2.1/src/aaz_dev/app/run.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/app/url_converters.py` & `aaz-dev-1.2.1/src/aaz_dev/app/url_converters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/api/_cmds.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/api/az.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/api/az.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/api/portal.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/api/portal.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_arg_group_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_arg_group_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_atomic_profile_builder.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_atomic_profile_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_command_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_module_manager.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_module_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_operation_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_operation_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_output_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_output_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_profile_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_profile_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/az_selector_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/az_selector_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/controller/portal_cli_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/controller/portal_cli_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_command.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_command_group.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/atomic/_help.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/atomic/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/common/_fields.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/common/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_command.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_command_group.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_module.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/model/view/_profile.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/model/view/_profile.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/__init__.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/_filters.py` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/command/_cmd.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/aaz/group/__cmd_group.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/azext_/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/extension/setup.py.j2` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/extension/setup.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/cli/templates/main/__init__.py.j2` & `aaz-dev-1.2.1/src/aaz_dev/cli/templates/main/__init__.py.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/api/_cmds.py` & `aaz-dev-1.2.1/src/aaz_dev/command/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/api/editor.py` & `aaz-dev-1.2.1/src/aaz_dev/command/api/editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/api/specs.py` & `aaz-dev-1.2.1/src/aaz_dev/command/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/controller/cfg_reader.py` & `aaz-dev-1.2.1/src/aaz_dev/command/controller/cfg_reader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/controller/specs_manager.py` & `aaz-dev-1.2.1/src/aaz_dev/command/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/controller/workspace_cfg_editor.py` & `aaz-dev-1.2.1/src/aaz_dev/command/controller/workspace_cfg_editor.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/controller/workspace_manager.py` & `aaz-dev-1.2.1/src/aaz_dev/command/controller/workspace_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/__init__.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg_builder.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_arg_group.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_arg_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_command.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_command.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_command_group.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_command_group.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_condition.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_condition.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_configuration.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_content.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_content.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_fields.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_fields.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_format.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_help.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_help.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http_request_body.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http_request_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_http_response_body.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_http_response_body.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_create.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_create.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_delete.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_delete.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_instance_update.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_instance_update.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_operation.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_output.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_output.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_resource.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_schema.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_selector_index.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_selector_index.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_subresource_selector.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_subresource_selector.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/configuration/_xml.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/configuration/_xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/editor/_workspace.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/editor/_workspace.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/model/specs/_command_tree.py` & `aaz-dev-1.2.1/src/aaz_dev/command/model/specs/_command_tree.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/templates/__init__.py` & `aaz-dev-1.2.1/src/aaz_dev/command/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/templates/_filters.py` & `aaz-dev-1.2.1/src/aaz_dev/command/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/templates/command.md.j2` & `aaz-dev-1.2.1/src/aaz_dev/command/templates/command.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/command/templates/group.md.j2` & `aaz-dev-1.2.1/src/aaz_dev/command/templates/group.md.j2`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/api/specs.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/api/specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/controller/command_generator.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/controller/command_generator.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/controller/specs_manager.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/controller/specs_manager.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/cmd_builder.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/cmd_builder.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/contact.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/contact.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/fields.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,25 @@
             default=False,
             serialized_name="x-cadl-generated",
             deserialize_from="x-cadl-generated",
             **kwargs
         )
 
 
+class XTypespecGeneratedField(BaseType):
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            default=False,
+            serialized_name="x-typespec-generated",
+            deserialize_from="x-typespec-generated",
+            **kwargs
+        )
+
+
 class XmsSkipURLEncodingField(BooleanType):
     """
     skips URL encoding for path and query parameters.
 
     https://github.com/Azure/autorest/tree/main/docs/extensions#x-ms-skip-url-encoding
     """
 
@@ -380,14 +391,24 @@
         super().__init__(
             serialized_name='x-cadl-name',
             deserialize_from='x-cadl-name',
             **kwargs
         )
 
 
+class XTypespecNameField(StringType):
+
+    def __init__(self, **kwargs):
+        super().__init__(
+            serialized_name='x-typespec-name',
+            deserialize_from='x-typespec-name',
+            **kwargs
+        )
+
+
 class XmsHeaderCollectionPrefix(StringType):
     """ only used in Storage Data plane """
 
     def __init__(self, **kwargs):
         super().__init__(
             serialized_name='x-ms-header-collection-prefix',
             deserialize_from='x-ms-header-collection-prefix',
```

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/info.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from schematics.models import Model
 from schematics.types import StringType, ModelType
 from .contact import Contact
 from .license import License
-from .fields import XmsCodeGenerationSettingsField, XcadlGeneratedField
+from .fields import XmsCodeGenerationSettingsField, XcadlGeneratedField, XTypespecGeneratedField
 
 
 class Info(Model):
     """The object provides metadata about the API. The metadata can be used by the clients if needed, and can be presented in the Swagger-UI for convenience."""
 
     title = StringType(required=True)       # The title of the application.
     version = StringType(required=True)     # Provides the version of the application API (not to be confused with the specification version)
@@ -17,7 +17,8 @@
     )  # The Terms of Service for the API.
     contact = ModelType(Contact)  # The contact information for the exposed API.
     license = ModelType(License)  # The license information for the exposed API.
 
     # specific properties
     _x_ms_code_generation_settings = XmsCodeGenerationSettingsField()  # Deprecated
     _x_cadl_generated = XcadlGeneratedField()
+    _x_typespec_generated = XTypespecGeneratedField()
```

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/items.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/items.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/operation.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/parameter.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/parameter.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/path_item.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/path_item.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/reference.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/reference.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/response.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/response.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/schema.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from command.model.configuration import CMDSchemaEnum, CMDSchemaEnumItem, CMDSchema, CMDSchemaBase
 from swagger.utils import exceptions
 from .external_documentation import ExternalDocumentation
 from .fields import DataTypeFormatEnum, RegularExpressionField, XmsClientNameField, XmsExternalField, \
     XmsDiscriminatorValueField, XmsClientFlattenField, XmsMutabilityField, XmsClientDefaultField, XNullableField, \
     XmsAzureResourceField, MutabilityEnum, XmsArmIdDetailsField
 from .fields import XmsSecretField, XAccessibilityField, XAzSearchDeprecatedField, XSfClientLibField, \
-    XApimCodeNillableField, XCommentField, XAbstractField, XADLNameField, XCadlNameField
+    XApimCodeNillableField, XCommentField, XAbstractField, XADLNameField, XCadlNameField, XTypespecNameField
 from .reference import ReferenceField, Linkable
 from .x_ms_enum import XmsEnumField
 from .xml import XML
 
 logger = logging.getLogger('backend')
 
 
@@ -254,14 +254,15 @@
     _x_abstract = XAbstractField()  # Only used in Logic Mgmt Plane and Web Mgmt Plane
     _x_adl_name = XADLNameField()  # Only used in FluidRelay Mgmt Plane
     _x_enum_Names = ListType(BaseType(), serialized_name="x-enumNames", deserialize_from="x-enumNames")  # Only used in Marketplane Catalog Data Plane
     _x_enum_flags = BooleanType(serialized_name="x-enumFlags", deserialize_from="x-enumFlags")  # Only used in Marketplane Catalog Data Plane
     _x_dictionary_key = ModelType(ReferenceSchema, serialized_name="x-dictionaryKey", deserialize_from="x-dictionaryKey")  # Only used in Marketplane Catalog Data Plane
 
     _x_cadl_name = XCadlNameField()  # Cadl field name
+    _x_typespec_name = XTypespecNameField()  # Typespec field name
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.ref_instance = None
         self.disc_parent = None
         self.disc_children = {}
```

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/security_scheme.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/security_scheme.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/swagger.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/swagger.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/tag.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/tag.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_enum.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_enum.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_long_running_operation.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_odata.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_odata.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_pageable.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_pageable.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_parameter_grouping.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/x_ms_parameterized_host.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/schema/xml.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/schema/xml.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_resource.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_resource.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_resource_provider.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_resource_provider.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_loader.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_loader.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_module.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_module.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_swagger_specs.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_swagger_specs.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/model/specs/_utils.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/model/specs/_utils.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/swagger/utils/tools.py` & `aaz-dev-1.2.1/src/aaz_dev/swagger/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/asset-manifest.json` & `aaz-dev-1.2.1/src/aaz_dev/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/favicon.ico` & `aaz-dev-1.2.1/src/aaz_dev/ui/favicon.ico`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/index.html` & `aaz-dev-1.2.1/src/aaz_dev/ui/index.html`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/logo192.png` & `aaz-dev-1.2.1/src/aaz_dev/ui/logo192.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/logo512.png` & `aaz-dev-1.2.1/src/aaz_dev/ui/logo512.png`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/css/main.6dea0f05.chunk.css.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/2.2736f8c1.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js.map` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/main.e3fb8aee.chunk.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map` & `aaz-dev-1.2.1/src/aaz_dev/ui/static/js/runtime-main.f7313c7c.js.map`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/config.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/config.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/error_format.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/error_format.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/exceptions.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/plane.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/plane.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/portal_file_schema.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/portal_file_schema.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev/utils/stage.py` & `aaz-dev-1.2.1/src/aaz_dev/utils/stage.py`

 * *Files identical despite different names*

### Comparing `aaz-dev-1.2.0/src/aaz_dev.egg-info/PKG-INFO` & `aaz-dev-1.2.1/src/aaz_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aaz-dev
-Version: 1.2.0
+Version: 1.2.1
 Summary: Microsoft Atomic Azure CLI Commands Developer Tools
 Home-page: https://github.com/Azure/aaz-dev-tools
 Author: Microsoft Corporation
 Author-email: azpycli@microsoft.com
 License: MIT
 Keywords: azure
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Microsoft Atomic Azure CLI Dev Tools
 
-The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [Doc](./src/aaz_dev/docs/Docs#introduction-to-aazdev) or [Video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9)
+The *aaz-dev* tool is designed to generate atomic Azure CLI commands from OpenAPI specifications. For more information, please refer to [document](https://azure.github.io/aaz-dev-tools/) and [video](https://msit.microsoftstream.com/video/d8c50840-98dc-a27a-806a-f1ed2daa33a9).
 
 ## Installation
 Currently, we can install it with a [.whl file](https://github.com/Azure/aaz-dev-tools/releases). Later on, we'll publish it to PyPI to support *pip install* way of installation.
 
 ## Setting up your development environment
 
 ### 1 Code repos
```

### Comparing `aaz-dev-1.2.0/src/aaz_dev.egg-info/SOURCES.txt` & `aaz-dev-1.2.1/src/aaz_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

