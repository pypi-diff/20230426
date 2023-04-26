# Comparing `tmp/commitizen-3.0.1.tar.gz` & `tmp/commitizen-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitizen-3.0.1.tar", max compression
+gzip compressed data, was "commitizen-3.1.0.tar", max compression
```

## Comparing `commitizen-3.0.1.tar` & `commitizen-3.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1065 2023-04-23 07:23:07.112274 commitizen-3.0.1/LICENSE
--rw-r--r--   0        0        0      593 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__init__.py
--rw-r--r--   0        0        0       71 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__main__.py
--rw-r--r--   0        0        0       22 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/__version__.py
--rw-r--r--   0        0        0     8613 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/bump.py
--rw-r--r--   0        0        0    11909 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/changelog.py
--rw-r--r--   0        0        0     3431 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/changelog_parser.py
--rw-r--r--   0        0        0    16605 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cli.py
--rw-r--r--   0        0        0     1112 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cmd.py
--rw-r--r--   0        0        0      420 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/__init__.py
--rw-r--r--   0        0        0    13755 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/bump.py
--rw-r--r--   0        0        0     6845 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/changelog.py
--rw-r--r--   0        0        0     5067 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/check.py
--rw-r--r--   0        0        0     3059 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/commit.py
--rw-r--r--   0        0        0      364 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/example.py
--rw-r--r--   0        0        0      350 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/info.py
--rw-r--r--   0        0        0    12935 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/init.py
--rw-r--r--   0        0        0      325 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/list_cz.py
--rw-r--r--   0        0        0      341 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/schema.py
--rw-r--r--   0        0        0     1488 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/commands/version.py
--rw-r--r--   0        0        0     1229 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/__init__.py
--rw-r--r--   0        0        0      915 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/base_config.py
--rw-r--r--   0        0        0     1384 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/json_config.py
--rw-r--r--   0        0        0     1753 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/toml_config.py
--rw-r--r--   0        0        0     1438 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/config/yaml_config.py
--rw-r--r--   0        0        0     1226 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/__init__.py
--rw-r--r--   0        0        0     2951 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/base.py
--rw-r--r--   0        0        0       64 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/__init__.py
--rw-r--r--   0        0        0     7043 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits.py
--rw-r--r--   0        0        0     1285 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits_info.txt
--rw-r--r--   0        0        0       50 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/__init__.py
--rw-r--r--   0        0        0     2801 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/customize.py
--rw-r--r--   0        0        0        0 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/customize/customize_info.txt
--rw-r--r--   0        0        0       88 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/exceptions.py
--rw-r--r--   0        0        0       57 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/__init__.py
--rw-r--r--   0        0        0     2678 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/jira.py
--rw-r--r--   0        0        0     1940 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/jira/jira_info.txt
--rw-r--r--   0        0        0      272 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/cz/utils.py
--rw-r--r--   0        0        0     3253 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/defaults.py
--rw-r--r--   0        0        0     4575 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/exceptions.py
--rw-r--r--   0        0        0      639 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/factory.py
--rw-r--r--   0        0        0     6916 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/git.py
--rw-r--r--   0        0        0      951 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/hooks.py
--rw-r--r--   0        0        0      745 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/out.py
--rw-r--r--   0        0        0     6657 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/providers.py
--rw-r--r--   0        0        0      405 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/templates/keep_a_changelog_template.j2
--rw-r--r--   0        0        0     2400 2023-04-23 07:23:07.112274 commitizen-3.0.1/commitizen/version_types.py
--rw-r--r--   0        0        0     5800 2023-04-23 07:23:07.116274 commitizen-3.0.1/docs/README.md
--rw-r--r--   0        0        0     3959 2023-04-23 07:23:07.124274 commitizen-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-25 17:05:02.037353 commitizen-3.1.0/LICENSE
+-rw-r--r--   0        0        0      593 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__init__.py
+-rw-r--r--   0        0        0       71 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__main__.py
+-rw-r--r--   0        0        0       22 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/__version__.py
+-rw-r--r--   0        0        0     8613 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/bump.py
+-rw-r--r--   0        0        0    11909 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/changelog.py
+-rw-r--r--   0        0        0     3431 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/changelog_parser.py
+-rw-r--r--   0        0        0    16605 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/cli.py
+-rw-r--r--   0        0        0     1112 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/cmd.py
+-rw-r--r--   0        0        0      420 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/__init__.py
+-rw-r--r--   0        0        0    13932 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/bump.py
+-rw-r--r--   0        0        0     6845 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/changelog.py
+-rw-r--r--   0        0        0     5067 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/check.py
+-rw-r--r--   0        0        0     3059 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/commit.py
+-rw-r--r--   0        0        0      364 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/example.py
+-rw-r--r--   0        0        0      350 2023-04-25 17:05:02.037353 commitizen-3.1.0/commitizen/commands/info.py
+-rw-r--r--   0        0        0    12935 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/init.py
+-rw-r--r--   0        0        0      325 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/list_cz.py
+-rw-r--r--   0        0        0      341 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/schema.py
+-rw-r--r--   0        0        0     1488 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/commands/version.py
+-rw-r--r--   0        0        0     1229 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/__init__.py
+-rw-r--r--   0        0        0      915 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/base_config.py
+-rw-r--r--   0        0        0     1384 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/json_config.py
+-rw-r--r--   0        0        0     1753 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/toml_config.py
+-rw-r--r--   0        0        0     1438 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/config/yaml_config.py
+-rw-r--r--   0        0        0     1226 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/__init__.py
+-rw-r--r--   0        0        0     3016 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/base.py
+-rw-r--r--   0        0        0       64 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits.py
+-rw-r--r--   0        0        0     1285 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits_info.txt
+-rw-r--r--   0        0        0       50 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/__init__.py
+-rw-r--r--   0        0        0     3125 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/customize.py
+-rw-r--r--   0        0        0        0 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/customize/customize_info.txt
+-rw-r--r--   0        0        0       88 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/exceptions.py
+-rw-r--r--   0        0        0       57 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/__init__.py
+-rw-r--r--   0        0        0     2678 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/jira.py
+-rw-r--r--   0        0        0     1940 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/jira/jira_info.txt
+-rw-r--r--   0        0        0      272 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/cz/utils.py
+-rw-r--r--   0        0        0     3310 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/defaults.py
+-rw-r--r--   0        0        0     4575 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/exceptions.py
+-rw-r--r--   0        0        0      639 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/factory.py
+-rw-r--r--   0        0        0     6916 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/git.py
+-rw-r--r--   0        0        0      951 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/hooks.py
+-rw-r--r--   0        0        0      745 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/out.py
+-rw-r--r--   0        0        0     6657 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/providers.py
+-rw-r--r--   0        0        0      405 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/templates/keep_a_changelog_template.j2
+-rw-r--r--   0        0        0     2400 2023-04-25 17:05:02.041354 commitizen-3.1.0/commitizen/version_types.py
+-rw-r--r--   0        0        0     5800 2023-04-25 17:05:02.041354 commitizen-3.1.0/docs/README.md
+-rw-r--r--   0        0        0     3959 2023-04-25 17:05:02.053353 commitizen-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7633 1970-01-01 00:00:00.000000 commitizen-3.1.0/PKG-INFO
```

### Comparing `commitizen-3.0.1/LICENSE` & `commitizen-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/__init__.py` & `commitizen-3.1.0/commitizen/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/bump.py` & `commitizen-3.1.0/commitizen/bump.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/changelog.py` & `commitizen-3.1.0/commitizen/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/changelog_parser.py` & `commitizen-3.1.0/commitizen/changelog_parser.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cli.py` & `commitizen-3.1.0/commitizen/cli.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cmd.py` & `commitizen-3.1.0/commitizen/cmd.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/commands/bump.py` & `commitizen-3.1.0/commitizen/commands/bump.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from logging import getLogger
 from typing import List, Optional
 
 import questionary
 from packaging.version import InvalidVersion, Version
 
-from commitizen import bump, cmd, defaults, factory, git, hooks, out, version_types
+from commitizen import bump, cmd, factory, git, hooks, out, version_types
 from commitizen.commands.changelog import Changelog
 from commitizen.config import BaseConfig
 from commitizen.exceptions import (
     BumpCommitFailedError,
     BumpTagFailedError,
     DryRunExit,
     ExpectedExit,
@@ -82,16 +82,24 @@
                         "- tag_format is missing, check them using 'git tag --list'\n"
                     )
                 )
                 is_initial = questionary.confirm("Is this the first tag created?").ask()
         return is_initial
 
     def find_increment(self, commits: List[git.GitCommit]) -> Optional[str]:
+        # Update the bump map to ensure major version doesn't increment.
+        is_major_version_zero: bool = self.bump_settings["major_version_zero"]
+        # self.cz.bump_map = defaults.bump_map_major_version_zero
+        bump_map = (
+            self.cz.bump_map_major_version_zero
+            if is_major_version_zero
+            else self.cz.bump_map
+        )
         bump_pattern = self.cz.bump_pattern
-        bump_map = self.cz.bump_map
+
         if not bump_map or not bump_pattern:
             raise NoPatternMapError(
                 f"'{self.config.settings['name']}' rule does not support bump"
             )
         increment = bump.find_increment(
             commits, regex=bump_pattern, increments_map=bump_map
         )
@@ -149,17 +157,14 @@
 
         if major_version_zero:
             if not current_version.startswith("0."):
                 raise NotAllowed(
                     f"--major-version-zero is meaningless for current version {current_version}"
                 )
 
-            # Update the bump map to ensure major version doesn't increment.
-            self.cz.bump_map = defaults.bump_map_major_version_zero
-
         current_tag_version: str = bump.normalize_tag(
             current_version,
             tag_format=tag_format,
             version_type_cls=self.version_type,
         )
 
         is_initial = self.is_initial_tag(current_tag_version, is_yes)
```

### Comparing `commitizen-3.0.1/commitizen/commands/changelog.py` & `commitizen-3.1.0/commitizen/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/commands/check.py` & `commitizen-3.1.0/commitizen/commands/check.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/commands/commit.py` & `commitizen-3.1.0/commitizen/commands/commit.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/commands/init.py` & `commitizen-3.1.0/commitizen/commands/init.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/commands/version.py` & `commitizen-3.1.0/commitizen/commands/version.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/config/__init__.py` & `commitizen-3.1.0/commitizen/config/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/config/base_config.py` & `commitizen-3.1.0/commitizen/config/base_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/config/json_config.py` & `commitizen-3.1.0/commitizen/config/json_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/config/toml_config.py` & `commitizen-3.1.0/commitizen/config/toml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/config/yaml_config.py` & `commitizen-3.1.0/commitizen/config/yaml_config.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cz/__init__.py` & `commitizen-3.1.0/commitizen/cz/__init__.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cz/base.py` & `commitizen-3.1.0/commitizen/cz/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from commitizen.config.base_config import BaseConfig
 from commitizen.defaults import Questions
 
 
 class BaseCommitizen(metaclass=ABCMeta):
     bump_pattern: Optional[str] = None
     bump_map: Optional[Dict[str, str]] = None
+    bump_map_major_version_zero: Optional[Dict[str, str]] = None
     default_style_config: List[Tuple[str, str]] = [
         ("qmark", "fg:#ff9d00 bold"),
         ("question", "bold"),
         ("answer", "fg:#ff9d00 bold"),
         ("pointer", "fg:#ff9d00 bold"),
         ("highlighted", "fg:#ff9d00 bold"),
         ("selected", "fg:#cc5454"),
```

### Comparing `commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits.py` & `commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     return required_validator(text, msg="Subject is required.")
 
 
 class ConventionalCommitsCz(BaseCommitizen):
     bump_pattern = defaults.bump_pattern
     bump_map = defaults.bump_map
+    bump_map_major_version_zero = defaults.bump_map_major_version_zero
     commit_parser = defaults.commit_parser
     version_parser = defaults.version_parser
     change_type_map = {
         "feat": "Feat",
         "fix": "Fix",
         "refactor": "Refactor",
         "perf": "Perf",
```

### Comparing `commitizen-3.0.1/commitizen/cz/conventional_commits/conventional_commits_info.txt` & `commitizen-3.1.0/commitizen/cz/conventional_commits/conventional_commits_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cz/customize/customize.py` & `commitizen-3.1.0/commitizen/cz/customize/customize.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 __all__ = ["CustomizeCommitsCz"]
 
 
 class CustomizeCommitsCz(BaseCommitizen):
     bump_pattern = defaults.bump_pattern
     bump_map = defaults.bump_map
+    bump_map_major_version_zero = defaults.bump_map_major_version_zero
     change_type_order = defaults.change_type_order
 
     def __init__(self, config: BaseConfig):
         super(CustomizeCommitsCz, self).__init__(config)
 
         if "customize" not in self.config.settings:
             raise MissingCzCustomizeConfigError()
@@ -30,14 +31,20 @@
         if custom_bump_pattern:
             self.bump_pattern = custom_bump_pattern
 
         custom_bump_map = self.custom_settings.get("bump_map")
         if custom_bump_map:
             self.bump_map = custom_bump_map
 
+        custom_bump_map_major_version_zero = self.custom_settings.get(
+            "bump_map_major_version_zero"
+        )
+        if custom_bump_map_major_version_zero:
+            self.bump_map_major_version_zero = custom_bump_map_major_version_zero
+
         custom_change_type_order = self.custom_settings.get("change_type_order")
         if custom_change_type_order:
             self.change_type_order = custom_change_type_order
 
         commit_parser = self.custom_settings.get("commit_parser")
         if commit_parser:
             self.commit_parser = commit_parser
```

### Comparing `commitizen-3.0.1/commitizen/cz/jira/jira.py` & `commitizen-3.1.0/commitizen/cz/jira/jira.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/cz/jira/jira_info.txt` & `commitizen-3.1.0/commitizen/cz/jira/jira_info.txt`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/defaults.py` & `commitizen-3.1.0/commitizen/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # Type
 Questions = Iterable[MutableMapping[str, Any]]
 
 
 class CzSettings(TypedDict, total=False):
     bump_pattern: str
     bump_map: "OrderedDict[str, str]"
+    bump_map_major_version_zero: "OrderedDict[str, str]"
     change_type_order: List[str]
 
     questions: Questions
     example: Optional[str]
     schema_pattern: Optional[str]
     schema: Optional[str]
     info_path: Union[str, pathlib.Path]
```

### Comparing `commitizen-3.0.1/commitizen/exceptions.py` & `commitizen-3.1.0/commitizen/exceptions.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/factory.py` & `commitizen-3.1.0/commitizen/factory.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/git.py` & `commitizen-3.1.0/commitizen/git.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/hooks.py` & `commitizen-3.1.0/commitizen/hooks.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/out.py` & `commitizen-3.1.0/commitizen/out.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/providers.py` & `commitizen-3.1.0/commitizen/providers.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/commitizen/version_types.py` & `commitizen-3.1.0/commitizen/version_types.py`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/docs/README.md` & `commitizen-3.1.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `commitizen-3.0.1/pyproject.toml` & `commitizen-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.commitizen]
-version = "3.0.1"
+version = "3.1.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "commitizen/__version__.py",
   ".pre-commit-config.yaml:rev:.+Commitizen"
 ]
 
 [tool.poetry]
 name = "commitizen"
-version = "3.0.1"
+version = "3.1.0"
 description = "Python commitizen client tool"
 authors = ["Santiago Fraire <santiwilly@gmail.com>"]
 license = "MIT"
 keywords = ["commitizen", "conventional", "commits", "git"]
 readme = "docs/README.md"
 homepage = "https://github.com/commitizen-tools/commitizen"
 # See also: https://pypi.org/classifiers/
```

### Comparing `commitizen-3.0.1/PKG-INFO` & `commitizen-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitizen
-Version: 3.0.1
+Version: 3.1.0
 Summary: Python commitizen client tool
 Home-page: https://github.com/commitizen-tools/commitizen
 License: MIT
 Keywords: commitizen,conventional,commits,git
 Author: Santiago Fraire
 Author-email: santiwilly@gmail.com
 Requires-Python: >=3.7,<4.0
```

