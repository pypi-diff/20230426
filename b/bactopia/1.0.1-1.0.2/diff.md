# Comparing `tmp/bactopia-1.0.1.tar.gz` & `tmp/bactopia-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bactopia-1.0.1.tar", max compression
+gzip compressed data, was "bactopia-1.0.2.tar", max compression
```

## Comparing `bactopia-1.0.1.tar` & `bactopia-1.0.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1065 2023-04-06 01:21:18.917662 bactopia-1.0.1/LICENSE
--rw-r--r--   0        0        0    24569 2023-04-06 01:21:18.917662 bactopia-1.0.1/README.md
--rw-r--r--   0        0        0      113 2023-04-06 01:21:18.917662 bactopia-1.0.1/bactopia/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 01:21:18.917662 bactopia-1.0.1/bactopia/cli/__init__.py
--rw-r--r--   0        0        0     2652 2023-04-06 01:21:18.917662 bactopia-1.0.1/bactopia/cli/citations.py
--rw-r--r--   0        0        0    19341 2023-04-06 01:21:18.917662 bactopia-1.0.1/bactopia/cli/download.py
--rw-r--r--   0        0        0     2416 2023-04-06 01:21:18.917662 bactopia-1.0.1/bactopia/cli/jsonify.py
--rw-r--r--   0        0        0    16397 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/cli/prepare.py
--rw-r--r--   0        0        0    20687 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/cli/search.py
--rw-r--r--   0        0        0    15430 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/cli/summary.py
--rw-r--r--   0        0        0     1398 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parse.py
--rw-r--r--   0        0        0      267 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/__init__.py
--rw-r--r--   0        0        0      484 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/amrfinderplus.py
--rw-r--r--   0        0        0     1000 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/annotator.py
--rw-r--r--   0        0        0     2783 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/ariba.py
--rw-r--r--   0        0        0      664 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/assembler.py
--rw-r--r--   0        0        0     4673 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/blast.py
--rw-r--r--   0        0        0     1365 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/error.py
--rw-r--r--   0        0        0      372 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/gather.py
--rw-r--r--   0        0        0     1492 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/generic.py
--rw-r--r--   0        0        0     2683 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/mapping.py
--rw-r--r--   0        0        0      640 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/mlst.py
--rw-r--r--   0        0        0     1599 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/parsables.py
--rw-r--r--   0        0        0     3093 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/qc.py
--rw-r--r--   0        0        0     5014 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/sketcher.py
--rw-r--r--   0        0        0     2574 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/variants.py
--rw-r--r--   0        0        0      874 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/parsers/versions.py
--rw-r--r--   0        0        0     5292 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/summary.py
--rw-r--r--   0        0        0     4496 2023-04-06 01:21:18.921662 bactopia-1.0.1/bactopia/utils.py
--rw-r--r--   0        0        0     1004 2023-04-06 01:21:18.921662 bactopia-1.0.1/pyproject.toml
--rw-r--r--   0        0        0    26065 1970-01-01 00:00:00.000000 bactopia-1.0.1/setup.py
--rw-r--r--   0        0        0    25523 1970-01-01 00:00:00.000000 bactopia-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-25 18:04:35.882807 bactopia-1.0.2/LICENSE
+-rw-r--r--   0        0        0    27493 2023-04-25 18:04:35.886807 bactopia-1.0.2/README.md
+-rw-r--r--   0        0        0      113 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/__init__.py
+-rw-r--r--   0        0        0     2667 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/citations.py
+-rw-r--r--   0        0        0     5118 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/datasets.py
+-rw-r--r--   0        0        0    19341 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/download.py
+-rw-r--r--   0        0        0     2416 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/jsonify.py
+-rw-r--r--   0        0        0    16397 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/prepare.py
+-rw-r--r--   0        0        0    20687 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/search.py
+-rw-r--r--   0        0        0    15455 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/cli/summary.py
+-rw-r--r--   0        0        0     1398 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parse.py
+-rw-r--r--   0        0        0      267 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/__init__.py
+-rw-r--r--   0        0        0      484 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/amrfinderplus.py
+-rw-r--r--   0        0        0     1000 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/annotator.py
+-rw-r--r--   0        0        0     2783 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/ariba.py
+-rw-r--r--   0        0        0      664 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/assembler.py
+-rw-r--r--   0        0        0     4673 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/blast.py
+-rw-r--r--   0        0        0     1365 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/error.py
+-rw-r--r--   0        0        0      372 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/gather.py
+-rw-r--r--   0        0        0     1492 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/generic.py
+-rw-r--r--   0        0        0     2683 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/mapping.py
+-rw-r--r--   0        0        0      640 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/mlst.py
+-rw-r--r--   0        0        0     1599 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/parsables.py
+-rw-r--r--   0        0        0     3093 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/qc.py
+-rw-r--r--   0        0        0     5014 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/sketcher.py
+-rw-r--r--   0        0        0     2574 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/variants.py
+-rw-r--r--   0        0        0      874 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/parsers/versions.py
+-rw-r--r--   0        0        0     5292 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/summary.py
+-rw-r--r--   0        0        0     4496 2023-04-25 18:04:35.886807 bactopia-1.0.2/bactopia/utils.py
+-rw-r--r--   0        0        0     1053 2023-04-25 18:04:35.886807 bactopia-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    29090 1970-01-01 00:00:00.000000 bactopia-1.0.2/setup.py
+-rw-r--r--   0        0        0    28447 1970-01-01 00:00:00.000000 bactopia-1.0.2/PKG-INFO
```

### Comparing `bactopia-1.0.1/LICENSE` & `bactopia-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/README.md` & `bactopia-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ## Bactopia Subcommands
 
 There are many subcommands available in Bactopia. Here is a brief description of each command:
 
 | Command              | Description                                                                |
 |----------------------|----------------------------------------------------------------------------|
 | `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |
+| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |
 | `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |
 | `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |
 | `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |
 | `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |
 
 Below is the `--help` output for each subcommand.
 
@@ -23,22 +24,51 @@
 
 ```{bash}
  Usage: bactopia-citations [OPTIONS]
 
  Print out tools and citations used throughout Bactopia
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────╮
-│    --version     -V        Show the version and exit.                                │
-│ *  --bactopia    -b  TEXT  Directory where Bactopia repository is stored [required]  │
-│    --name        -n  TEXT  Only print citation matching a given name                 │
-│    --plain-text  -p        Disable rich formatting                                   │
-│    --help                  Show this message and exit.                               │
+│    --version        -V        Show the version and exit.                             │
+│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │
+│                               [required]                                             │
+│    --name           -n  TEXT  Only print citation matching a given name              │
+│    --plain-text     -p        Disable rich formatting                                │
+│    --help                     Show this message and exit.                            │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+### `bactopia-datasets`
+
+```{bash}
+ Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...
+
+ Download optional datasets to supplement your analyses with Bactopia
+
+╭─ Required Options ───────────────────────────────────────────────────────────────────╮
+│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Download Related Options ───────────────────────────────────────────────────────────╮
+│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │
+│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │
+│                              will be created)                                        │
+│                              [default: ${HOME}/.bactopia]                 │
+│ --force                      Force overwrite of existing pre-built environments.     │
+│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │
+│                              (Default: 3)                                            │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Additional Options ─────────────────────────────────────────────────────────────────╮
+│ --verbose      Print debug related text.                                             │
+│ --silent       Only critical errors will be printed.                                 │
+│ --version      Show the version and exit.                                            │
+│ --help         Show this message and exit.                                           │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+
+```
+
 ### `bactopia-download`
 
 ```{bash}
  Usage: bactopia-download [OPTIONS] [UNKNOWN]...
 
  Builds Bactopia environments for use with Nextflow.
 
@@ -183,15 +213,15 @@
 
 ```{bash}
  Usage: bactopia-summary [OPTIONS]
 
  Generate a summary table from the Bactopia results.
 
 ╭─ Required Options ───────────────────────────────────────────────────────────────────╮
-│ *  --bactopia  -b  TEXT  Directory where Bactopia results are stored [required]      │
+│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮
 │ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │
 │                                         status                                       │
 │                                         [default: 100]                               │
 │ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │
 │                                         for Gold status                              │
```

### Comparing `bactopia-1.0.1/bactopia/cli/citations.py` & `bactopia-1.0.2/bactopia/cli/citations.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,25 @@
                 module_citations[ref.lower()] = vals
         return [citations, module_citations]
 
 
 @click.command()
 @click.version_option(bactopia.__version__, "--version", "-V")
 @click.option(
-    "--bactopia",
+    "--bactopia-path",
     "-b",
     required=True,
     help="Directory where Bactopia repository is stored",
 )
 @click.option("--name", "-n", help="Only print citation matching a given name")
 @click.option("--plain-text", "-p", is_flag=True, help="Disable rich formatting")
-def citations(bactopia: str, name: str, plain_text: bool) -> None:
+def citations(bactopia_path: str, name: str, plain_text: bool) -> None:
     """Print out tools and citations used throughout Bactopia"""
 
-    citations_yml = validate_file(f"{bactopia}/citations.yml")
+    citations_yml = validate_file(f"{bactopia_path}/citations.yml")
     citations, module_citations = parse_citations(citations_yml)
 
     markdown = []
     if name:
         if name.lower() in module_citations:
             markdown.append(f"{module_citations[name.lower()]['name']}  ")
             markdown.append(module_citations[name.lower()]["cite"].rstrip())
```

### Comparing `bactopia-1.0.1/bactopia/cli/download.py` & `bactopia-1.0.2/bactopia/cli/download.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/cli/jsonify.py` & `bactopia-1.0.2/bactopia/cli/jsonify.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/cli/prepare.py` & `bactopia-1.0.2/bactopia/cli/prepare.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/cli/search.py` & `bactopia-1.0.2/bactopia/cli/search.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/cli/summary.py` & `bactopia-1.0.2/bactopia/cli/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # Set up Rich
 stderr = rich.console.Console(stderr=True)
 rich.traceback.install(console=stderr, width=200, word_wrap=True, extra_lines=1)
 click.rich_click.USE_RICH_MARKUP = True
 click.rich_click.OPTION_GROUPS = {
     "bactopia-summary": [
-        {"name": "Required Options", "options": ["--bactopia"]},
+        {"name": "Required Options", "options": ["--bactopia-path"]},
         {
             "name": "Gold Cutoffs",
             "options": [
                 "--gold-coverage",
                 "--gold-quality",
                 "--gold-read-length",
                 "--gold-contigs",
@@ -140,15 +140,15 @@
 
     return [rank, reason]
 
 
 @click.command()
 @click.version_option(bactopia.__version__, "--version", "-V")
 @click.option(
-    "--bactopia",
+    "--bactopia-path",
     "-b",
     required=True,
     help="Directory where Bactopia results are stored",
 )
 @click.option(
     "--gold-coverage",
     "-gcov",
@@ -270,15 +270,15 @@
     show_default=True,
     help="Prefix to use for output files",
 )
 @click.option("--force", is_flag=True, help="Overwrite existing reports")
 @click.option("--verbose", is_flag=True, help="Increase the verbosity of output")
 @click.option("--silent", is_flag=True, help="Only critical errors will be printed")
 def summary(
-    bactopia,
+    bactopia_path,
     gold_coverage,
     gold_quality,
     gold_read_length,
     gold_contigs,
     silver_coverage,
     silver_quality,
     silver_read_length,
@@ -343,16 +343,16 @@
     else:
         logging.debug(f"Creating output directory: {outdir}")
         Path(outdir).mkdir(parents=True, exist_ok=True)
 
     processed_samples = {}
     versions = []
     dfs = []
-    samples = parse_bactopia_directory(bactopia)
-    logging.info(f"Found {len(samples)} samples in {bactopia} to process")
+    samples = parse_bactopia_directory(bactopia_path)
+    logging.info(f"Found {len(samples)} samples in {bactopia_path} to process")
     if samples:
         for sample in samples:
             if sample["is_bactopia"]:
                 COUNTS["total"] += 1
                 logging.debug(f"Processing {sample['id']} ({sample['path']})")
 
                 # Get the versions files to parse
```

### Comparing `bactopia-1.0.1/bactopia/parse.py` & `bactopia-1.0.2/bactopia/parse.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/annotator.py` & `bactopia-1.0.2/bactopia/parsers/annotator.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/ariba.py` & `bactopia-1.0.2/bactopia/parsers/ariba.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/assembler.py` & `bactopia-1.0.2/bactopia/parsers/assembler.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/blast.py` & `bactopia-1.0.2/bactopia/parsers/blast.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/error.py` & `bactopia-1.0.2/bactopia/parsers/error.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/generic.py` & `bactopia-1.0.2/bactopia/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/mapping.py` & `bactopia-1.0.2/bactopia/parsers/mapping.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/mlst.py` & `bactopia-1.0.2/bactopia/parsers/mlst.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/parsables.py` & `bactopia-1.0.2/bactopia/parsers/parsables.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/qc.py` & `bactopia-1.0.2/bactopia/parsers/qc.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/sketcher.py` & `bactopia-1.0.2/bactopia/parsers/sketcher.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/variants.py` & `bactopia-1.0.2/bactopia/parsers/variants.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/parsers/versions.py` & `bactopia-1.0.2/bactopia/parsers/versions.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/summary.py` & `bactopia-1.0.2/bactopia/summary.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/bactopia/utils.py` & `bactopia-1.0.2/bactopia/utils.py`

 * *Files identical despite different names*

### Comparing `bactopia-1.0.1/pyproject.toml` & `bactopia-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "bactopia"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Python package for working with Bactopia"
 authors = [
     "Robert A. Petit III <robbie.petit@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://bactopia.github.io/"
 repository = "https://github.com/bactopia/bactopia-py"
 keywords = ["bioinformatics", "bacteria", "bactopia", "SRA", "ENA"]
 
 [tool.poetry.scripts]
 bactopia-citations = "bactopia.cli.citations:main"
+bactopia-datasets = "bactopia.cli.datasets:main"
 bactopia-download = "bactopia.cli.download:main"
 bactopia-prepare = "bactopia.cli.prepare:main"
 bactopia-search = "bactopia.cli.search:main"
 bactopia-summary = "bactopia.cli.summary:main"
 
 [tool.poetry.dependencies]
 python = "^3.8.0"
```

### Comparing `bactopia-1.0.1/setup.py` & `bactopia-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,24 +13,25 @@
  'pysradb>=1.4.2,<2.0.0',
  'requests>=2.28.2,<3.0.0',
  'rich-click>=1.6.1,<2.0.0',
  'rich>=13.3.1,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['bactopia-citations = bactopia.cli.citations:main',
+                     'bactopia-datasets = bactopia.cli.datasets:main',
                      'bactopia-download = bactopia.cli.download:main',
                      'bactopia-prepare = bactopia.cli.prepare:main',
                      'bactopia-search = bactopia.cli.search:main',
                      'bactopia-summary = bactopia.cli.summary:main']}
 
 setup_kwargs = {
     'name': 'bactopia',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'A Python package for working with Bactopia',
-    'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version     -V        Show the version and exit.                                │\n│ *  --bactopia    -b  TEXT  Directory where Bactopia repository is stored [required]  │\n│    --name        -n  TEXT  Only print citation matching a given name                 │\n│    --plain-text  -p        Disable rich formatting                                   │\n│    --help                  Show this message and exit.                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia  -b  TEXT  Directory where Bactopia results are stored [required]      │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
+    'long_description': "[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-908a85?logo=gitpod)](https://gitpod.io/#https://github.com/bactopia/bactopia-py)\n\n![Bactopia Logo](https://raw.githubusercontent.com/bactopia/bactopia/master/data/bactopia-logo.png)\n\n# bactopia-py\nA Python package for working with [Bactopia](https://bactopia.github.io/)\n\n## Bactopia Subcommands\n\nThere are many subcommands available in Bactopia. Here is a brief description of each command:\n\n| Command              | Description                                                                |\n|----------------------|----------------------------------------------------------------------------|\n| `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |\n| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |\n| `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |\n| `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |\n| `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |\n| `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |\n\nBelow is the `--help` output for each subcommand.\n\n### `bactopia-citations`\n\n```{bash}\n Usage: bactopia-citations [OPTIONS]\n\n Print out tools and citations used throughout Bactopia\n\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│    --version        -V        Show the version and exit.                             │\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │\n│                               [required]                                             │\n│    --name           -n  TEXT  Only print citation matching a given name              │\n│    --plain-text     -p        Disable rich formatting                                │\n│    --help                     Show this message and exit.                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-datasets`\n\n```{bash}\n Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...\n\n Download optional datasets to supplement your analyses with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Download Related Options ───────────────────────────────────────────────────────────╮\n│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │\n│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │\n│                              will be created)                                        │\n│                              [default: ${HOME}/.bactopia]                 │\n│ --force                      Force overwrite of existing pre-built environments.     │\n│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │\n│                              (Default: 3)                                            │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n\n```\n\n### `bactopia-download`\n\n```{bash}\n Usage: bactopia-download [OPTIONS] [UNKNOWN]...\n\n Builds Bactopia environments for use with Nextflow.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path    TEXT  Directory where Bactopia results are stored [required]   │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Build Related Options ──────────────────────────────────────────────────────────────╮\n│ --envtype                     [conda|docker|singularity|  The type of environment to │\n│                               all]                        build.                     │\n│                                                           [default: conda]           │\n│ --wf                          TEXT                        Build a environment for a  │\n│                                                           the given workflow         │\n│                                                           [default: bactopia]        │\n│ --condadir                    TEXT                        Directory to create Conda  │\n│                                                           environments               │\n│                                                           (NXF_CONDA_CACHEDIR env    │\n│                                                           variable takes precedence) │\n│ --use_conda                                               Use Conda for building     │\n│                                                           Conda environments instead │\n│                                                           of Mamba                   │\n│ --singularity_cache           TEXT                        Directory to download      │\n│                                                           Singularity images         │\n│                                                           (NXF_SINGULARITY_CACHEDIR  │\n│                                                           env variable takes         │\n│                                                           precedence)                │\n│ --singularity_pull_docker…                                Force conversion of Docker │\n│                                                           containers, instead        │\n│                                                           downloading Singularity    │\n│                                                           images directly            │\n│ --force_rebuild                                           Force overwrite of         │\n│                                                           existing pre-built         │\n│                                                           environments.              │\n│ --max_retry                   INTEGER                     Maximum times to attempt   │\n│                                                           creating Conda             │\n│                                                           environment. (Default: 3)  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --verbose      Print debug related text.                                             │\n│ --silent       Only critical errors will be printed.                                 │\n│ --version      Show the version and exit.                                            │\n│ --help         Show this message and exit.                                           │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Options ────────────────────────────────────────────────────────────────────────────╮\n│ --build-all         Builds all environments for Bactopia workflows                   │\n│ --build-nfcore      Builds all nf-core related environments                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-prepare`\n\n```{bash}\n Usage: bactopia-prepare [OPTIONS]\n\n Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --path  -p  TEXT  Directory where FASTQ files are stored [required]               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Matching Options ───────────────────────────────────────────────────────────────────╮\n│ --assembly-ext     -a  TEXT  Extension of the FASTA assemblies [default: .fna.gz]    │\n│ --fastq-ext        -f  TEXT  Extension of the FASTQs [default: .fastq.gz]            │\n│ --fastq-separator      TEXT  Split FASTQ name on the last occurrence of the          │\n│                              separator                                               │\n│                              [default: _]                                            │\n│ --pe1-pattern          TEXT  Designates difference first set of paired-end reads     │\n│                              [default: [Aa]|[Rr]1|1]                                 │\n│ --pe2-pattern          TEXT  Designates difference second set of paired-end reads    │\n│                              [default: [Bb]|[Rr]2|2]                                 │\n│ --merge                      Flag samples with multiple read sets to be merged by    │\n│                              Bactopia                                                │\n│ --ont                        Single-end reads should be treated as Oxford Nanopore   │\n│                              reads                                                   │\n│ --recursive        -r        Directories will be traversed recursively               │\n│ --prefix               TEXT  Prefix to add to the path                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Sample Information Options ─────────────────────────────────────────────────────────╮\n│ --metadata             TEXT     Metadata per sample with genome size and species     │\n│                                 information                                          │\n│ --genome-size  -gsize  INTEGER  Genome size to use for all samples                   │\n│ --species      -s      TEXT     Species to use for all samples (If available, can be │\n│                                 used to determine genome size)                       │\n│ --taxid                TEXT     Use the genome size of the Taxon ID for all samples  │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --examples        Print example usage                                                │\n│ --verbose         Increase the verbosity of output                                   │\n│ --silent          Only critical errors will be printed                               │\n│ --version   -V    Show the version and exit.                                         │\n│ --help            Show this message and exit.                                        │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-search`\n\n```{bash}\n Usage: bactopia-search [OPTIONS]\n\n Query against ENA and SRA for public accessions to process with Bactopia\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --query  -q  TEXT  Taxon ID or Study, BioSample, or Run accession (can also be    │\n│                       comma separated or a file of accessions)                       │\n│                       [required]                                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Query Options ──────────────────────────────────────────────────────────────────────╮\n│ --exact-taxon                     Exclude Taxon ID descendants                       │\n│ --limit             -l   INTEGER  Maximum number of results (per query) to return    │\n│                                   [default: 1000000]                                 │\n│ --accession-limit   -al  INTEGER  Maximum number of accessions to query at once      │\n│                                   [default: 5000]                                    │\n│ --biosample-subset       INTEGER  If a BioSample has multiple Experiments, maximum   │\n│                                   number to randomly select (0 = disabled)           │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Filtering Options ──────────────────────────────────────────────────────────────────╮\n│ --min-base-count   -mbc  INTEGER  Filters samples based on minimum base pair count   │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-read-length  -mrl  INTEGER  Filters samples based on minimum mean read length  │\n│                                   (0 = disabled)                                     │\n│                                   [default: 0]                                       │\n│ --min-coverage     -mc   INTEGER  Filter samples based on minimum coverage (requires │\n│                                   --genome_size, 0 = disabled)                       │\n│                                   [default: 0]                                       │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --genome-size  -gsize  INTEGER  Genome size to be used for all samples, and for      │\n│                                 calculating min coverage                             │\n│                                 [default: 0]                                         │\n│ --outdir       -o      TEXT     Directory to write output [default: ./]              │\n│ --prefix       -p      TEXT     Prefix to use for output file names                  │\n│                                 [default: bactopia]                                  │\n│ --force                         Overwrite existing reports                           │\n│ --verbose                       Increase the verbosity of output                     │\n│ --silent                        Only critical errors will be printed                 │\n│ --version      -V               Show the version and exit.                           │\n│ --help                          Show this message and exit.                          │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n### `bactopia-summary`\n\n```{bash}\n Usage: bactopia-summary [OPTIONS]\n\n Generate a summary table from the Bactopia results.\n\n╭─ Required Options ───────────────────────────────────────────────────────────────────╮\n│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │\n│                                         status                                       │\n│                                         [default: 100]                               │\n│ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │\n│                                         for Gold status                              │\n│                                         [default: 30]                                │\n│ --gold-read-length  -glen      INTEGER  Minimum mean read length required for Gold   │\n│                                         status                                       │\n│                                         [default: 95]                                │\n│ --gold-contigs      -gcontigs  INTEGER  Maximum contig count required for Gold       │\n│                                         status                                       │\n│                                         [default: 100]                               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Silver Cutoffs ─────────────────────────────────────────────────────────────────────╮\n│ --silver-coverage     -scov      INTEGER  Minimum amount of coverage required for    │\n│                                           Silver status                              │\n│                                           [default: 50]                              │\n│ --silver-quality      -squal     INTEGER  Minimum per-read mean quality score        │\n│                                           required for Silver status                 │\n│                                           [default: 20]                              │\n│ --silver-read-length  -slen      INTEGER  Minimum mean read length required for      │\n│                                           Silver status                              │\n│                                           [default: 75]                              │\n│ --silver-contigs      -scontigs  INTEGER  Maximum contig count required for Silver   │\n│                                           status                                     │\n│                                           [default: 200]                             │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Fail Cutoffs ───────────────────────────────────────────────────────────────────────╮\n│ --min-coverage        -mincov   INTEGER  Minimum amount of coverage required to pass │\n│                                          [default: 20]                               │\n│ --min-quality         -minqual  INTEGER  Minimum per-read mean quality score         │\n│                                          required to pass                            │\n│                                          [default: 12]                               │\n│ --min-read-length     -minlen   INTEGER  Minimum mean read length required to pass   │\n│                                          [default: 49]                               │\n│ --max-contigs                   INTEGER  Maximum contig count required to pass       │\n│                                          [default: 500]                              │\n│ --min-assembled-size            INTEGER  Minimum assembled genome size               │\n│ --max-assembled-size            INTEGER  Maximum assembled genome size               │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Additional Options ─────────────────────────────────────────────────────────────────╮\n│ --outdir   -o  PATH  Directory to write output [default: ./]                         │\n│ --prefix   -p  TEXT  Prefix to use for output files [default: bactopia]              │\n│ --force              Overwrite existing reports                                      │\n│ --verbose            Increase the verbosity of output                                │\n│ --silent             Only critical errors will be printed                            │\n│ --version  -V        Show the version and exit.                                      │\n│ --help               Show this message and exit.                                     │\n╰──────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n# Feedback\nYour feedback is very valuable! If you run into any issues using Bactopia, have questions, or have some ideas to improve Bactopia, I highly encourage you to submit it to the [Issue Tracker](https://github.com/bactopia/bactopia/issues).\n\n# License\n[MIT License](https://raw.githubusercontent.com/bactopia/bactopia/master/LICENSE)\n\n# Citation\n\nPetit III RA, Read TD, *Bactopia: a flexible pipeline for complete analysis of bacterial genomes.* __mSystems__. 5 (2020), https://doi.org/10.1128/mSystems.00190-20.\n\n# Author\n\n* Robert A. Petit III\n* Twitter: [@rpetit3](https://twitter.com/rpetit3)\n",
     'author': 'Robert A. Petit III',
     'author_email': 'robbie.petit@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://bactopia.github.io/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `bactopia-1.0.1/PKG-INFO` & `bactopia-1.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bactopia
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python package for working with Bactopia
 Home-page: https://bactopia.github.io/
 License: MIT
 Keywords: bioinformatics,bacteria,bactopia,SRA,ENA
 Author: Robert A. Petit III
 Author-email: robbie.petit@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
@@ -33,14 +33,15 @@
 ## Bactopia Subcommands
 
 There are many subcommands available in Bactopia. Here is a brief description of each command:
 
 | Command              | Description                                                                |
 |----------------------|----------------------------------------------------------------------------|
 | `bactopia-citations` | Print out tools and citations used throughout Bactopia                     |
+| `bactopia-datasets`  | Download optional datasets to supplement your analyses with Bactopia       |
 | `bactopia-download`  | Builds Bactopia environments for use with Nextflow.                        |
 | `bactopia-prepare`   | Create a 'file of filenames' (FOFN) of samples to be processed by Bactopia |
 | `bactopia-search`    | Query against ENA and SRA for public accessions to process with Bactopia   |
 | `bactopia-summary`   | Generate a summary table from the Bactopia results.                        |
 
 Below is the `--help` output for each subcommand.
 
@@ -48,22 +49,51 @@
 
 ```{bash}
  Usage: bactopia-citations [OPTIONS]
 
  Print out tools and citations used throughout Bactopia
 
 ╭─ Options ────────────────────────────────────────────────────────────────────────────╮
-│    --version     -V        Show the version and exit.                                │
-│ *  --bactopia    -b  TEXT  Directory where Bactopia repository is stored [required]  │
-│    --name        -n  TEXT  Only print citation matching a given name                 │
-│    --plain-text  -p        Disable rich formatting                                   │
-│    --help                  Show this message and exit.                               │
+│    --version        -V        Show the version and exit.                             │
+│ *  --bactopia-path  -b  TEXT  Directory where Bactopia repository is stored          │
+│                               [required]                                             │
+│    --name           -n  TEXT  Only print citation matching a given name              │
+│    --plain-text     -p        Disable rich formatting                                │
+│    --help                     Show this message and exit.                            │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
+### `bactopia-datasets`
+
+```{bash}
+ Usage: bactopia-datasets [OPTIONS] [UNKNOWN]...
+
+ Download optional datasets to supplement your analyses with Bactopia
+
+╭─ Required Options ───────────────────────────────────────────────────────────────────╮
+│ *  --bactopia-path    TEXT  Directory where Bactopia repository is stored [required] │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Download Related Options ───────────────────────────────────────────────────────────╮
+│ --datasets_cache    TEXT     Base directory to download datasets to (Defaults to env │
+│                              variable BACTOPIA_CACHEDIR, a subfolder called datasets │
+│                              will be created)                                        │
+│                              [default: ${HOME}/.bactopia]                 │
+│ --force                      Force overwrite of existing pre-built environments.     │
+│ --max_retry         INTEGER  Maximum times to attempt creating Conda environment.    │
+│                              (Default: 3)                                            │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+╭─ Additional Options ─────────────────────────────────────────────────────────────────╮
+│ --verbose      Print debug related text.                                             │
+│ --silent       Only critical errors will be printed.                                 │
+│ --version      Show the version and exit.                                            │
+│ --help         Show this message and exit.                                           │
+╰──────────────────────────────────────────────────────────────────────────────────────╯
+
+```
+
 ### `bactopia-download`
 
 ```{bash}
  Usage: bactopia-download [OPTIONS] [UNKNOWN]...
 
  Builds Bactopia environments for use with Nextflow.
 
@@ -208,15 +238,15 @@
 
 ```{bash}
  Usage: bactopia-summary [OPTIONS]
 
  Generate a summary table from the Bactopia results.
 
 ╭─ Required Options ───────────────────────────────────────────────────────────────────╮
-│ *  --bactopia  -b  TEXT  Directory where Bactopia results are stored [required]      │
+│ *  --bactopia-path  -b  TEXT  Directory where Bactopia results are stored [required] │
 ╰──────────────────────────────────────────────────────────────────────────────────────╯
 ╭─ Gold Cutoffs ───────────────────────────────────────────────────────────────────────╮
 │ --gold-coverage     -gcov      INTEGER  Minimum amount of coverage required for Gold │
 │                                         status                                       │
 │                                         [default: 100]                               │
 │ --gold-quality      -gqual     INTEGER  Minimum per-read mean quality score required │
 │                                         for Gold status                              │
```

