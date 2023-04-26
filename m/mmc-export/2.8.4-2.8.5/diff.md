# Comparing `tmp/mmc_export-2.8.4.tar.gz` & `tmp/mmc_export-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmc_export-2.8.4.tar", max compression
+gzip compressed data, was "mmc_export-2.8.5.tar", max compression
```

## Comparing `mmc_export-2.8.4.tar` & `mmc_export-2.8.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2022-05-10 23:10:38.982236 mmc_export-2.8.4/LICENSE
--rw-r--r--   0        0        0     5545 2022-11-03 07:21:41.102451 mmc_export-2.8.4/README.md
--rw-r--r--   0        0        0     2816 2023-04-20 09:34:24.580816 mmc_export-2.8.4/mmc_export/Formats/curseforge.py
--rw-r--r--   0        0        0     4094 2022-11-06 06:15:03.483584 mmc_export-2.8.4/mmc_export/Formats/modrinth.py
--rw-r--r--   0        0        0     4984 2023-04-20 09:34:42.212054 mmc_export-2.8.4/mmc_export/Formats/packwiz.py
--rw-r--r--   0        0        0    15932 2023-04-20 16:10:37.743561 mmc_export-2.8.4/mmc_export/Helpers/resourceAPI.py
--rw-r--r--   0        0        0     2396 2022-08-24 18:47:04.717746 mmc_export-2.8.4/mmc_export/Helpers/structures.py
--rw-r--r--   0        0        0    11689 2023-04-20 16:06:45.308995 mmc_export-2.8.4/mmc_export/Helpers/utils.py
--rw-r--r--   0        0        0       63 2022-07-09 03:47:00.282736 mmc_export-2.8.4/mmc_export/__init__.py
--rw-r--r--   0        0        0       61 2022-05-10 23:10:38.982236 mmc_export-2.8.4/mmc_export/__main__.py
--rw-r--r--   0        0        0      648 2022-09-12 09:19:59.859818 mmc_export-2.8.4/mmc_export/config.py
--rw-r--r--   0        0        0     2788 2023-04-20 09:36:05.218485 mmc_export-2.8.4/mmc_export/main.py
--rw-r--r--   0        0        0     3069 2023-01-23 19:06:35.936606 mmc_export-2.8.4/mmc_export/parser.py
--rw-r--r--   0        0        0      844 2023-04-20 16:10:48.241135 mmc_export-2.8.4/pyproject.toml
--rw-r--r--   0        0        0     6834 1970-01-01 00:00:00.000000 mmc_export-2.8.4/setup.py
--rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 mmc_export-2.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-05-10 23:10:38.982236 mmc_export-2.8.5/LICENSE
+-rw-r--r--   0        0        0     5435 2023-04-26 13:05:21.095903 mmc_export-2.8.5/README.md
+-rw-r--r--   0        0        0     2816 2023-04-20 09:34:24.580816 mmc_export-2.8.5/mmc_export/Formats/curseforge.py
+-rw-r--r--   0        0        0     4094 2023-04-20 16:30:01.736035 mmc_export-2.8.5/mmc_export/Formats/modrinth.py
+-rw-r--r--   0        0        0     4984 2023-04-20 09:34:42.212054 mmc_export-2.8.5/mmc_export/Formats/packwiz.py
+-rw-r--r--   0        0        0    15932 2023-04-26 13:10:29.841306 mmc_export-2.8.5/mmc_export/Helpers/resourceAPI.py
+-rw-r--r--   0        0        0     2396 2022-08-24 18:47:04.717746 mmc_export-2.8.5/mmc_export/Helpers/structures.py
+-rw-r--r--   0        0        0    11823 2023-04-26 13:12:23.197893 mmc_export-2.8.5/mmc_export/Helpers/utils.py
+-rw-r--r--   0        0        0       63 2022-07-09 03:47:00.282736 mmc_export-2.8.5/mmc_export/__init__.py
+-rw-r--r--   0        0        0       61 2022-05-10 23:10:38.982236 mmc_export-2.8.5/mmc_export/__main__.py
+-rw-r--r--   0        0        0      648 2022-09-12 09:19:59.859818 mmc_export-2.8.5/mmc_export/config.py
+-rw-r--r--   0        0        0     2788 2023-04-20 09:36:05.218485 mmc_export-2.8.5/mmc_export/main.py
+-rw-r--r--   0        0        0     3069 2023-01-23 19:06:35.936606 mmc_export-2.8.5/mmc_export/parser.py
+-rw-r--r--   0        0        0      844 2023-04-26 13:10:19.440150 mmc_export-2.8.5/pyproject.toml
+-rw-r--r--   0        0        0     6722 1970-01-01 00:00:00.000000 mmc_export-2.8.5/setup.py
+-rw-r--r--   0        0        0     6459 1970-01-01 00:00:00.000000 mmc_export-2.8.5/PKG-INFO
```

### Comparing `mmc_export-2.8.4/LICENSE` & `mmc_export-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/README.md` & `mmc_export-2.8.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -129,16 +129,14 @@
 This can be defined to delete any file that isn't downloadable from CurseForge/Modrinth, e.g. mod config or metadata file.
 ```
 [[File]]
 name = "Useless file.txt"
 action = "remove"
 ```
 
-> Also specifying both name and filename is optional but recommended, you can always leave only one of these
-
 ## Scheme Formatting
 
 Must be used as `--scheme "{keyword}_Literally any text"` without file extension, follows python's [format string syntax](https://docs.python.org/3/library/string.html#format-string-syntax)
 
 #### Available keywords: 
 - `abbr` - provider abbreviation, usually 2 capitals, e.g. `MR`, `CF`
 - `format` - full format name, e.g. `CurseForge`, `Packwiz`
```

### Comparing `mmc_export-2.8.4/mmc_export/Formats/curseforge.py` & `mmc_export-2.8.5/mmc_export/Formats/curseforge.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/Formats/modrinth.py` & `mmc_export-2.8.5/mmc_export/Formats/modrinth.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/Formats/packwiz.py` & `mmc_export-2.8.5/mmc_export/Formats/packwiz.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/Helpers/resourceAPI.py` & `mmc_export-2.8.5/mmc_export/Helpers/resourceAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     excluded_providers: list[str]
 
     def __init__(self, session: CachedSession, intermediate: Intermediate) -> None:
 
         self.session = session
         self.intermediate = intermediate
 
-        self.session.headers["User-Agent"] = "RozeFound/mmc-export/2.8.4"
+        self.session.headers["User-Agent"] = "RozeFound/mmc-export/2.8.5"
         self.session.headers["X-Api-Key"] = config.CURSEFORGE_API_TOKEN
         self.session.headers["Content-Type"] = "application/json"
         self.session.headers["Accept"] = "application/json"
 
         self.github = "https://api.github.com"
         self.modrinth = "https://api.modrinth.com/v2"
         self.curseforge = "https://api.curseforge.com/v1"
```

### Comparing `mmc_export-2.8.4/mmc_export/Helpers/structures.py` & `mmc_export-2.8.5/mmc_export/Helpers/structures.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/Helpers/utils.py` & `mmc_export-2.8.5/mmc_export/Helpers/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,17 @@
                     return
 
 def delete_github_token() -> None:
     try: secret_store.delete_password("mmc-export", "github-token")
     except secret_store.core.backend.errors.PasswordDeleteError: return
 
 def get_github_token() -> str | None:
-    return secret_store.get_password("mmc-export", "github-token")
+    try: return secret_store.get_password("mmc-export", "github-token")
+    except secret_store.core.backend.errors.NoKeyringError: return
+    except secret_store.core.backend.errors.InitError: return
 
 def parse_args() -> Namespace:
 
     formats = ('packwiz', 'Modrinth', 'CurseForge', 'Intermediate')
     mr_search = ('exact', 'accurate', 'loose')
     providers = ('GitHub', 'CurseForge', 'Modrinth', 'Other')
```

### Comparing `mmc_export-2.8.4/mmc_export/config.py` & `mmc_export-2.8.5/mmc_export/config.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/main.py` & `mmc_export-2.8.5/mmc_export/main.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/mmc_export/parser.py` & `mmc_export-2.8.5/mmc_export/parser.py`

 * *Files identical despite different names*

### Comparing `mmc_export-2.8.4/pyproject.toml` & `mmc_export-2.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mmc-export"
-version = "2.8.4"
+version = "2.8.5"
 description = "Export MMC modpack to other modpack formats"
 authors = ["RozeFound"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/RozeFound/mmc-export"
 
 keywords = [
```

### Comparing `mmc_export-2.8.4/setup.py` & `mmc_export-2.8.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,17 @@
  'xxhash>=3.1.0,<4.0.0']
 
 entry_points = \
 {'console_scripts': ['mmc-export = mmc_export:main']}
 
 setup_kwargs = {
     'name': 'mmc-export',
-    'version': '2.8.4',
+    'version': '2.8.5',
     'description': 'Export MMC modpack to other modpack formats',
-    'long_description': '# MultiMC advanced exporter\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mmc-export)](https://www.python.org)\n[![PyPI version](https://img.shields.io/pypi/v/mmc-export?label=mmc-export&color=%2347a637)](https://pypi.org/project/mmc-export)\n[![PyPI downloads](https://img.shields.io/pypi/dm/mmc-export?color=%23894bbf)](https://pypistats.org/packages/mmc-export)\n[![GitHub license](https://img.shields.io/github/license/RozeFound/mmc-export)](/LICENSE)\n\nSince MultiMC export features are very limited, I created a script that solves this problem, with this script you can export MultiMC pack to any popular format (e.g. curseforge, modrinth, packwiz). MultiMC forks which didn\'t changed export format much also supported.\n\n# Features\n\n- Support conversion to:\n    - CurseForge\n    - Modrinth\n    - packwiz\n- Detects downloadable resourcepacks and shaders\n- Supports github parsing[¹](#github-rate-limits)\n- Loose modrinth search\n- User friendly toml config\n- Multiple output formats at once\n\n---\n### GitHub rate limits\n\nGitHub has limited requests per hour (up to 60), this means that if you have more than 60 mods, the rest will be excluded from github search. \nIf you authenticate with GitHub using `mmc-export gh-login`, the limit will be removed and requests will be faster. You can always log out with `mmc-export gh-logout`.\n\nIf you don\'t want to use github search by some reason, you can specify `--exclude-providers GitHub` as argument.\n\n# How to Use\n```\nmmc-export -i modpack.zip -c config.toml -f Modrinth packwiz -o converted_modpacks\n```\nIt\'s recommended to fill config at least with basic info like name and version, some launchers can fail import if these values are empty.\n\n## Sub-commands\n\n`gh-login` - to authrize GitHub \\\n`gh-logout` - to get info how to deauthorize GitHub \n\n`purge-cache` - to purge cache. Available arguments:\n```\n--web: to delete requests cache and downloaded mods\n--files: to delete hashes cache\n--all: equivalent to --web --files, deletes all cache (default)\n```\n\n## Syntax\n```\nmmc-export [sub-command] [-h] [-c CONFIG] -i INPUT -f FORMAT [-o OUTPUT] [-v VERSION] [--modrinth-search SEARCH_TYPE] [--exclude-providers PROVIDERS]\n```\n\n### Explanation\n```\n-h --help: prints help\n-i --input: path to modpack, must be zip file exported from MultiMC.\n-c --config: path to config, used to fill the gaps like description or lost mods.\n-f --format: output formats, must be separated by spaces.\n-o --output: directory where converted zip files will be stored.\n-v --version: specify modpack version, will be overriden by config\'s value if exists\n--modrinth-search: modrinth search accuracy\n--exclude-providers: providers you wish to exclude from search\n--provider-priority: providers priority used for packwiz\n--skip-cache: don\'t use web cache in this run\n--scheme: output filename formatting scheme, more info in #scheme-formatting\n```\n> All paths can be relative to current working directory or absolute.\n\n`--format` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `packwiz`\n- `Intermediate` (only for debugging, may contain sensitive data like username)\n\n`--exclude-providers` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `GitHub`\n\n`--provider-priority` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `Other` or `GitHub`\n\n`--modrinth-search` options:\n- `exact` - by hash (default)\n- `accurate` - by hash or slug\n- `loose` - by hash, slug or long name\n\nThe example for the optional `--config` file [can be found here](example_config.toml). \n\nFor example, if the script says\n\n> No config entry found for resource: ModName\n\nThen you should add **one** of the following entries to the end of the config:\n\n#### Specify source URL\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \nurl = "https://cdn.modrinth.com/data/abcdefg/versions/1.0.0/the_name_of_the.jar"\n```\n#### Hide the warning\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "ignore"\n```\n#### Explicitly move to overrides\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "override"\n```\n#### Delete the file altogether\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "remove"\n```\n#### Make the mod optional\nAppend `optional = true` to any of above\n\n#### Delete any file\nThis can be defined to delete any file that isn\'t downloadable from CurseForge/Modrinth, e.g. mod config or metadata file.\n```\n[[File]]\nname = "Useless file.txt"\naction = "remove"\n```\n\n> Also specifying both name and filename is optional but recommended, you can always leave only one of these\n\n## Scheme Formatting\n\nMust be used as `--scheme "{keyword}_Literally any text"` without file extension, follows python\'s [format string syntax](https://docs.python.org/3/library/string.html#format-string-syntax)\n\n#### Available keywords: \n- `abbr` - provider abbreviation, usually 2 capitals, e.g. `MR`, `CF`\n- `format` - full format name, e.g. `CurseForge`, `Packwiz`\n- `name` same as `pack.name` - modpack name\n- `version` same as `pack.version` - modpack version\n- `pack` - pointer to [Intermediate](mmc_export/Helpers/structures.py#L50-L66) structure\n\nDefault scheme is as simple as `{abbr}_{name}`\n\n***Caution: if you don\'t use any format specifc keywords, output files will overwrite the same file several times***, can be ignored if you output to only one format.\nAlso, be aware of your filesystem limitations, unsupported characters may lead to an error, or inaccesible file.\n\n# How to Install / Update\n```\npip install -U mmc-export\n```\n',
+    'long_description': '# MultiMC advanced exporter\n[![PyPI pyversions](https://img.shields.io/pypi/pyversions/mmc-export)](https://www.python.org)\n[![PyPI version](https://img.shields.io/pypi/v/mmc-export?label=mmc-export&color=%2347a637)](https://pypi.org/project/mmc-export)\n[![PyPI downloads](https://img.shields.io/pypi/dm/mmc-export?color=%23894bbf)](https://pypistats.org/packages/mmc-export)\n[![GitHub license](https://img.shields.io/github/license/RozeFound/mmc-export)](/LICENSE)\n\nSince MultiMC export features are very limited, I created a script that solves this problem, with this script you can export MultiMC pack to any popular format (e.g. curseforge, modrinth, packwiz). MultiMC forks which didn\'t changed export format much also supported.\n\n# Features\n\n- Support conversion to:\n    - CurseForge\n    - Modrinth\n    - packwiz\n- Detects downloadable resourcepacks and shaders\n- Supports github parsing[¹](#github-rate-limits)\n- Loose modrinth search\n- User friendly toml config\n- Multiple output formats at once\n\n---\n### GitHub rate limits\n\nGitHub has limited requests per hour (up to 60), this means that if you have more than 60 mods, the rest will be excluded from github search. \nIf you authenticate with GitHub using `mmc-export gh-login`, the limit will be removed and requests will be faster. You can always log out with `mmc-export gh-logout`.\n\nIf you don\'t want to use github search by some reason, you can specify `--exclude-providers GitHub` as argument.\n\n# How to Use\n```\nmmc-export -i modpack.zip -c config.toml -f Modrinth packwiz -o converted_modpacks\n```\nIt\'s recommended to fill config at least with basic info like name and version, some launchers can fail import if these values are empty.\n\n## Sub-commands\n\n`gh-login` - to authrize GitHub \\\n`gh-logout` - to get info how to deauthorize GitHub \n\n`purge-cache` - to purge cache. Available arguments:\n```\n--web: to delete requests cache and downloaded mods\n--files: to delete hashes cache\n--all: equivalent to --web --files, deletes all cache (default)\n```\n\n## Syntax\n```\nmmc-export [sub-command] [-h] [-c CONFIG] -i INPUT -f FORMAT [-o OUTPUT] [-v VERSION] [--modrinth-search SEARCH_TYPE] [--exclude-providers PROVIDERS]\n```\n\n### Explanation\n```\n-h --help: prints help\n-i --input: path to modpack, must be zip file exported from MultiMC.\n-c --config: path to config, used to fill the gaps like description or lost mods.\n-f --format: output formats, must be separated by spaces.\n-o --output: directory where converted zip files will be stored.\n-v --version: specify modpack version, will be overriden by config\'s value if exists\n--modrinth-search: modrinth search accuracy\n--exclude-providers: providers you wish to exclude from search\n--provider-priority: providers priority used for packwiz\n--skip-cache: don\'t use web cache in this run\n--scheme: output filename formatting scheme, more info in #scheme-formatting\n```\n> All paths can be relative to current working directory or absolute.\n\n`--format` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `packwiz`\n- `Intermediate` (only for debugging, may contain sensitive data like username)\n\n`--exclude-providers` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `GitHub`\n\n`--provider-priority` options (case-sensitive): \n- `CurseForge`\n- `Modrinth`\n- `Other` or `GitHub`\n\n`--modrinth-search` options:\n- `exact` - by hash (default)\n- `accurate` - by hash or slug\n- `loose` - by hash, slug or long name\n\nThe example for the optional `--config` file [can be found here](example_config.toml). \n\nFor example, if the script says\n\n> No config entry found for resource: ModName\n\nThen you should add **one** of the following entries to the end of the config:\n\n#### Specify source URL\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \nurl = "https://cdn.modrinth.com/data/abcdefg/versions/1.0.0/the_name_of_the.jar"\n```\n#### Hide the warning\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "ignore"\n```\n#### Explicitly move to overrides\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "override"\n```\n#### Delete the file altogether\n```\n[[Resource]]\nname = "ModName"\nfilename = "the_name_of_the.jar" \naction = "remove"\n```\n#### Make the mod optional\nAppend `optional = true` to any of above\n\n#### Delete any file\nThis can be defined to delete any file that isn\'t downloadable from CurseForge/Modrinth, e.g. mod config or metadata file.\n```\n[[File]]\nname = "Useless file.txt"\naction = "remove"\n```\n\n## Scheme Formatting\n\nMust be used as `--scheme "{keyword}_Literally any text"` without file extension, follows python\'s [format string syntax](https://docs.python.org/3/library/string.html#format-string-syntax)\n\n#### Available keywords: \n- `abbr` - provider abbreviation, usually 2 capitals, e.g. `MR`, `CF`\n- `format` - full format name, e.g. `CurseForge`, `Packwiz`\n- `name` same as `pack.name` - modpack name\n- `version` same as `pack.version` - modpack version\n- `pack` - pointer to [Intermediate](mmc_export/Helpers/structures.py#L50-L66) structure\n\nDefault scheme is as simple as `{abbr}_{name}`\n\n***Caution: if you don\'t use any format specifc keywords, output files will overwrite the same file several times***, can be ignored if you output to only one format.\nAlso, be aware of your filesystem limitations, unsupported characters may lead to an error, or inaccesible file.\n\n# How to Install / Update\n```\npip install -U mmc-export\n```\n',
     'author': 'RozeFound',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/RozeFound/mmc-export',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `mmc_export-2.8.4/PKG-INFO` & `mmc_export-2.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmc-export
-Version: 2.8.4
+Version: 2.8.5
 Summary: Export MMC modpack to other modpack formats
 Home-page: https://github.com/RozeFound/mmc-export
 License: MIT
 Keywords: minecraft,mods,modpack,converter,MultiMC
 Author: RozeFound
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -155,16 +155,14 @@
 This can be defined to delete any file that isn't downloadable from CurseForge/Modrinth, e.g. mod config or metadata file.
 ```
 [[File]]
 name = "Useless file.txt"
 action = "remove"
 ```
 
-> Also specifying both name and filename is optional but recommended, you can always leave only one of these
-
 ## Scheme Formatting
 
 Must be used as `--scheme "{keyword}_Literally any text"` without file extension, follows python's [format string syntax](https://docs.python.org/3/library/string.html#format-string-syntax)
 
 #### Available keywords: 
 - `abbr` - provider abbreviation, usually 2 capitals, e.g. `MR`, `CF`
 - `format` - full format name, e.g. `CurseForge`, `Packwiz`
```

