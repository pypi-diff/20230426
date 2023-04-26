# Comparing `tmp/autora_core-3.0.0a2.tar.gz` & `tmp/autora-core-3.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora_core-3.0.0a2.tar", max compression
+gzip compressed data, was "autora-core-3.0.0a3.tar", last modified: Wed Apr 26 21:15:31 2023, max compression
```

## Comparing `autora_core-3.0.0a2.tar` & `autora-core-3.0.0a3.tar`

### file list

```diff
@@ -1,20 +1,110 @@
--rw-r--r--   0        0        0     1100 2023-04-04 15:44:49.452496 autora_core-3.0.0a2/LICENSE.md
--rw-r--r--   0        0        0    18766 2023-04-04 15:44:49.452648 autora_core-3.0.0a2/README.md
--rw-r--r--   0        0        0      197 2023-04-04 15:44:49.452860 autora_core-3.0.0a2/autora/cycle/__init__.py
--rw-r--r--   0        0        0    20073 2023-04-04 15:44:49.452973 autora_core-3.0.0a2/autora/cycle/plot_utils.py
--rw-r--r--   0        0        0    21619 2023-04-04 15:44:49.453119 autora_core-3.0.0a2/autora/cycle/simple.py
--rw-r--r--   0        0        0    18310 2023-04-04 15:44:49.453470 autora_core-3.0.0a2/autora/experimentalist/pipeline.py
--rw-r--r--   0        0        0      620 2023-04-04 17:43:02.812363 autora_core-3.0.0a2/autora/experimentalist/pooler/grid.py
--rw-r--r--   0        0        0     1180 2023-04-04 17:43:02.805905 autora_core-3.0.0a2/autora/experimentalist/pooler/random.py
--rw-r--r--   0        0        0     1666 2023-04-04 15:44:49.454174 autora_core-3.0.0a2/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0        0        0      497 2023-04-04 15:44:49.454260 autora_core-3.0.0a2/autora/experimentalist/sampler/random.py
--rw-r--r--   0        0        0     4586 2023-04-04 15:44:49.454425 autora_core-3.0.0a2/autora/experimentalist/utils.py
--rw-r--r--   0        0        0     2649 2023-04-04 15:44:49.455009 autora_core-3.0.0a2/autora/synthetic/__init__.py
--rw-r--r--   0        0        0     7338 2023-04-04 15:44:49.455531 autora_core-3.0.0a2/autora/synthetic/inventory.py
--rw-r--r--   0        0        0        0 2023-04-04 17:30:58.941911 autora_core-3.0.0a2/autora/theorist/.gitkeep
--rw-r--r--   0        0        0       25 2023-04-04 15:44:49.458458 autora_core-3.0.0a2/autora/utils/__init__.py
--rw-r--r--   0        0        0      441 2023-04-04 15:44:49.458541 autora_core-3.0.0a2/autora/utils/dictionary.py
--rw-r--r--   0        0        0     1866 2023-04-04 15:44:49.458699 autora_core-3.0.0a2/autora/variable/__init__.py
--rw-r--r--   0        0        0     2511 2023-04-04 15:44:49.458801 autora_core-3.0.0a2/autora/variable/time.py
--rw-r--r--   0        0        0     1357 2023-04-04 17:45:05.987137 autora_core-3.0.0a2/pyproject.toml
--rw-r--r--   0        0        0    19880 1970-01-01 00:00:00.000000 autora_core-3.0.0a2/PKG-INFO
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.107550 autora-core-3.0.0a3/
+-rw-r--r--   0 jholla10   (503) staff       (20)      291 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.editorconfig
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.088436 autora-core-3.0.0a3/.github/
+-rw-r--r--   0 jholla10   (503) staff       (20)      363 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/dependabot.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)     2095 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/pull_request_template.md
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.089787 autora-core-3.0.0a3/.github/workflows/
+-rw-r--r--   0 jholla10   (503) staff       (20)      426 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-documentation-gh-pages.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)     1503 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-package-anaconda-org.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)      712 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)      548 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-conda-build.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)      440 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-poetry-build.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)      845 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-pre-commit-hooks.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)      775 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-pytest.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)     1009 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.gitignore
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091087 autora-core-3.0.0a3/.idea/
+-rw-r--r--   0 jholla10   (503) staff       (20)      176 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/.gitignore
+-rw-r--r--   0 jholla10   (503) staff       (20)     1654 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/autora-core.iml
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091248 autora-core-3.0.0a3/.idea/codeStyles/
+-rw-r--r--   0 jholla10   (503) staff       (20)      149 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      159 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/encodings.xml
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091795 autora-core-3.0.0a3/.idea/inspectionProfiles/
+-rw-r--r--   0 jholla10   (503) staff       (20)      716 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      228 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      310 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/misc.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      264 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/modules.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      186 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/other.xml
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091960 autora-core-3.0.0a3/.idea/runConfigurations/
+-rw-r--r--   0 jholla10   (503) staff       (20)     1011 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/runConfigurations/pytest_in_tests.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      180 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/vcs.xml
+-rw-r--r--   0 jholla10   (503) staff       (20)      796 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.pre-commit-config.yaml
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.092572 autora-core-3.0.0a3/.vscode/
+-rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/.gitignore
+-rw-r--r--   0 jholla10   (503) staff       (20)      112 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/extensions.json
+-rw-r--r--   0 jholla10   (503) staff       (20)      495 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/launch.json
+-rw-r--r--   0 jholla10   (503) staff       (20)     1100 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/LICENSE.md
+-rw-r--r--   0 jholla10   (503) staff       (20)    19467 2023-04-26 21:15:31.107296 autora-core-3.0.0a3/PKG-INFO
+-rw-r--r--   0 jholla10   (503) staff       (20)    18766 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/README.md
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.083509 autora-core-3.0.0a3/conda/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093117 autora-core-3.0.0a3/conda/autora/
+-rw-r--r--   0 jholla10   (503) staff       (20)     1315 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/conda/autora/meta.yaml
+-rw-r--r--   0 jholla10   (503) staff       (20)       26 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/conda/autora/run_test.sh
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084007 autora-core-3.0.0a3/docs/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093351 autora-core-3.0.0a3/docs/cycle/
+-rw-r--r--   0 jholla10   (503) staff       (20)   148488 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093795 autora-core-3.0.0a3/docs/experimentalists/
+-rw-r--r--   0 jholla10   (503) staff       (20)     2779 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/experimentalists/overview.md
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084264 autora-core-3.0.0a3/docs/theorist/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.095036 autora-core-3.0.0a3/docs/theorist/bms/
+-rw-r--r--   0 jholla10   (503) staff       (20)    13470 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/example.ipynb
+-rw-r--r--   0 jholla10   (503) staff       (20)     5203 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/search_space.ipynb
+-rw-r--r--   0 jholla10   (503) staff       (20)  1572980 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/weber.ipynb
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.099016 autora-core-3.0.0a3/docs/theorist/bsr/
+-rw-r--r--   0 jholla10   (503) staff       (20)     2231 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/how_it_works.md
+-rw-r--r--   0 jholla10   (503) staff       (20)    17622 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/img.png
+-rw-r--r--   0 jholla10   (503) staff       (20)      768 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/introduction.md
+-rw-r--r--   0 jholla10   (503) staff       (20)      951 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/meta_parameters.md
+-rw-r--r--   0 jholla10   (503) staff       (20)     1500 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/search_space.md
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.099495 autora-core-3.0.0a3/docs/theorist/darts/
+-rw-r--r--   0 jholla10   (503) staff       (20)    21418 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/darts/example.ipynb
+-rw-r--r--   0 jholla10   (503) staff       (20)   796078 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/darts/weber.ipynb
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084412 autora-core-3.0.0a3/mkdocs/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.100544 autora-core-3.0.0a3/mkdocs/overrides/
+-rw-r--r--   0 jholla10   (503) staff       (20)      660 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/mkdocs/overrides/main.html
+-rw-r--r--   0 jholla10   (503) staff       (20)     2602 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/mkdocs.yml
+-rw-r--r--   0 jholla10   (503) staff       (20)   178621 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/poetry.lock
+-rw-r--r--   0 jholla10   (503) staff       (20)     1465 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/pyproject.toml
+-rw-r--r--   0 jholla10   (503) staff       (20)       38 2023-04-26 21:15:31.107608 autora-core-3.0.0a3/setup.cfg
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.085443 autora-core-3.0.0a3/src/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.085360 autora-core-3.0.0a3/src/autora/
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.101332 autora-core-3.0.0a3/src/autora/cycle/
+-rw-r--r--   0 jholla10   (503) staff       (20)      197 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/__init__.py
+-rw-r--r--   0 jholla10   (503) staff       (20)    20109 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/plot_utils.py
+-rw-r--r--   0 jholla10   (503) staff       (20)    21619 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/simple.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.101852 autora-core-3.0.0a3/src/autora/experimentalist/
+-rw-r--r--   0 jholla10   (503) staff       (20)    18310 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.102305 autora-core-3.0.0a3/src/autora/experimentalist/pooler/
+-rw-r--r--   0 jholla10   (503) staff       (20)      620 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     1180 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pooler/random_.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103446 autora-core-3.0.0a3/src/autora/experimentalist/sampler/
+-rw-r--r--   0 jholla10   (503) staff       (20)     2383 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/assumption.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     2841 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/dissimilarity.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     2252 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/model_disagreement.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     1666 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/nearest_value.py
+-rw-r--r--   0 jholla10   (503) staff       (20)      497 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/random_.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     2052 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/uncertainty.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     4569 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103770 autora-core-3.0.0a3/src/autora/synthetic/
+-rw-r--r--   0 jholla10   (503) staff       (20)     2642 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/synthetic/__init__.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     7338 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/synthetic/inventory.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103927 autora-core-3.0.0a3/src/autora/theorist/
+-rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/theorist/.gitkeep
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.104162 autora-core-3.0.0a3/src/autora/utils/
+-rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/utils/__init__.py
+-rw-r--r--   0 jholla10   (503) staff       (20)      441 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/utils/dictionary.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.104486 autora-core-3.0.0a3/src/autora/variable/
+-rw-r--r--   0 jholla10   (503) staff       (20)     1866 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/variable/__init__.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     2511 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/variable/time.py
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.105561 autora-core-3.0.0a3/src/autora_core.egg-info/
+-rw-r--r--   0 jholla10   (503) staff       (20)    19467 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 jholla10   (503) staff       (20)     2449 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 jholla10   (503) staff       (20)        1 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 jholla10   (503) staff       (20)      350 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 jholla10   (503) staff       (20)        7 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.106917 autora-core-3.0.0a3/tests/
+-rw-r--r--   0 jholla10   (503) staff       (20)     1491 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/README.md
+-rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/__init__.py
+-rw-r--r--   0 jholla10   (503) staff       (20)    13298 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_cycle_plots.py
+-rw-r--r--   0 jholla10   (503) staff       (20)    10040 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 jholla10   (503) staff       (20)     4193 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_experimentalist_random.py
+-rw-r--r--   0 jholla10   (503) staff       (20)      862 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_synthetic_inventory.py
```

### Comparing `autora_core-3.0.0a2/LICENSE.md` & `autora-core-3.0.0a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/README.md` & `autora-core-3.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/cycle/plot_utils.py` & `autora-core-3.0.0a3/src/autora/cycle/plot_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib import rcParams
 from matplotlib.patches import Patch
 from matplotlib.ticker import MaxNLocator
+from numpy.typing import ArrayLike
 
 from .simple import SimpleCycle as Cycle
 
 # Change default plot styles
 rcParams["axes.spines.top"] = False
 rcParams["axes.spines.right"] = False
 rcParams["legend.frameon"] = False
@@ -84,15 +85,15 @@
         glob_min = np.min([s[idx] for s in l_mins])
         glob_max = np.max([s[idx] for s in l_maxs])
         l_return.append((glob_min, glob_max))
 
     return l_return
 
 
-def _generate_condition_space(cycle: Cycle, steps: int = 50) -> np.array:
+def _generate_condition_space(cycle: Cycle, steps: int = 50) -> ArrayLike:
     """
     Generates condition space based on the minimum and maximum of all observed data in AER Cycle.
     Args:
         cycle: AER Cycle object that has been run
         steps: Number of steps to define the condition space
 
     Returns: np.array
```

### Comparing `autora_core-3.0.0a2/autora/cycle/simple.py` & `autora-core-3.0.0a3/src/autora/cycle/simple.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/experimentalist/pipeline.py` & `autora-core-3.0.0a3/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/experimentalist/pooler/grid.py` & `autora-core-3.0.0a3/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/experimentalist/pooler/random.py` & `autora-core-3.0.0a3/src/autora/experimentalist/pooler/random_.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/experimentalist/sampler/nearest_value.py` & `autora-core-3.0.0a3/src/autora/experimentalist/sampler/nearest_value.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/experimentalist/utils.py` & `autora-core-3.0.0a3/src/autora/experimentalist/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 import collections
-from typing import Union
 
 import numpy as np
+import numpy.typing
 
 
 def sequence_to_array(iterable):
     """
     Converts a finite sequence of experimental conditions into a 2D numpy.array.
 
     See also: [array_to_sequence][autora.experimentalist.utils.array_to_sequence]
 
     Examples:
 
         A simple range object can be converted into an array of dimension 2:
-        >>> _sequence_to_array(range(5)) # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_array(range(5)) # doctest: +NORMALIZE_WHITESPACE
         array([[0], [1], [2], [3], [4]])
 
         For mixed datatypes, the highest-level type common to all the inputs will be used, so
         consider using [_sequence_to_recarray][autora.experimentalist.utils._sequence_to_recarray]
         instead.
-        >>> _sequence_to_array(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_array(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
         array([['0', 'a'], ['1', 'b'], ['2', 'c'], ['3', 'd'], ['4', 'e']],  dtype='<U21')
 
         Single strings are broken into characters:
         >>> sequence_to_array("abcde",array_type="numpy.array")  # doctest: +NORMALIZE_WHITESPACE
         array([['a'], ['b'], ['c'], ['d'], ['e']], dtype='<U1')
 
         Multiple strings are treated as individual entries:
@@ -44,42 +44,42 @@
     Converts a finite sequence of experimental conditions into a numpy recarray.
 
     See also: [array_to_sequence][autora.experimentalist.utils.array_to_sequence]
 
     Examples:
 
         A simple range object is converted into a recarray of dimension 2:
-        >>> _sequence_to_recarray(range(5)) # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_recarray(range(5)) # doctest: +NORMALIZE_WHITESPACE
         rec.array([(0,), (1,), (2,), (3,), (4,)], dtype=[('f0', '<i8')])
 
         Mixed datatypes lead to multiple output types:
-        >>> _sequence_to_recarray(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_recarray(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
         rec.array([(0, 'a'), (1, 'b'), (2, 'c'), (3, 'd'), (4, 'e')],
             dtype=[('f0', '<i8'), ('f1', '<U1')])
 
         Single strings are broken into characters:
-        >>> _sequence_to_recarray("abcde")  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_recarray("abcde")  # doctest: +NORMALIZE_WHITESPACE
         rec.array([('a',), ('b',), ('c',), ('d',), ('e',)], dtype=[('f0', '<U1')])
 
         Multiple strings are treated as individual entries:
-        >>> _sequence_to_recarray(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_recarray(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE
         rec.array([('abc',), ('de',)], dtype=[('f0', '<U3')])
 
     """
     deque = collections.deque(iterable)
 
     if isinstance(deque[0], (str, int, float, complex)):
         recarray = np.core.records.fromrecords([(d,) for d in deque])
     else:
         recarray = np.core.records.fromrecords(deque)
 
     return recarray
 
 
-def array_to_sequence(input: Union[np.array, np.recarray]):
+def array_to_sequence(input: numpy.typing.ArrayLike):
     """
     Convert an array of experimental conditions into an iterable of smaller arrays.
 
     See also:
         - [sequence_to_array][autora.experimentalist.utils.sequence_to_array]
         - [sequence_to_array][autora.experimentalist.utils.sequence_to_recarray]
```

### Comparing `autora_core-3.0.0a2/autora/synthetic/__init__.py` & `autora-core-3.0.0a3/src/autora/synthetic/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     ... against a fitted model if it exists:
     >>> from sklearn.linear_model import LinearRegression
     >>> model = LinearRegression().fit(x, y)
     >>> s.plotter(model)
 
     These can be used to run a full experimental cycle
     >>> from autora.experimentalist.pipeline import make_pipeline
-    >>> from autora.experimentalist.pooler.general_pool import grid_pool
-    >>> from autora.experimentalist.sampler.random import random_sampler
+    >>> from autora.experimentalist.pooler.grid import grid_pool
+    >>> from autora.experimentalist.sampler.random_ import random_sampler
     >>> from functools import partial
     >>> import random
     >>> metadata = s.metadata
     >>> pool = partial(grid_pool, ivs=metadata.independent_variables)
     >>> random.seed(181) # set the seed for the random sampler
     >>> sampler = partial(random_sampler, n=20)
     >>> experimentalist_pipeline = make_pipeline([pool, sampler])
```

### Comparing `autora_core-3.0.0a2/autora/synthetic/inventory.py` & `autora-core-3.0.0a3/src/autora/synthetic/inventory.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/variable/__init__.py` & `autora-core-3.0.0a3/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/autora/variable/time.py` & `autora-core-3.0.0a3/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora_core-3.0.0a2/PKG-INFO` & `autora-core-3.0.0a3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0a2
-Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. This framework implements tools for autonomously and iteratively generating 1) new theories to describe real-world data, and 2) experiments to invalidate those theories and seed a new cycle of theory-making. The experiments will be run online via crowd-sourcing platforms (MTurk, Prolific).
-Home-page: https://musslick.github.io/AER_website/Research.html
-Author: Sebastian Musslick
-Author-email: sebastian_musslick@brown.edu
-Requires-Python: >=3.8.10,<3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
-Requires-Dist: numpy (>=1.22.1)
-Requires-Dist: pandas (>=1.4.2,<3.0.0)
-Requires-Dist: scikit-learn (>=1.1.1,<2.0.0)
-Project-URL: Documentation, https://autoresearch.github.io/autora/
-Project-URL: Repository, https://github.com/AutoResearch/autora
+Version: 3.0.0a3
+Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
+Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
+Project-URL: homepage, https://www.empiricalresearch.ai
+Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
+Project-URL: documentation, https://autoresearch.github.io/autora/
+Requires-Python: <3.11,>=3.8.10
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: build
+Provides-Extra: notebook
+Provides-Extra: docs
+License-File: LICENSE.md
 
 # Autonomous Research Assistant
 Autonomous Research Assistant (AutoRA) is an open source AI-based system for automating each aspect of empirical research in the behavioral sciences, from the construction of a scientific hypothesis to conducting novel experiments. The documentation is here: [https://autoresearch.github.io/autora/](https://autoresearch.github.io/autora/)
 
 # Getting started
 
 You should be familiar with the command line for your operating system. The topics required are covered in:
@@ -438,8 +436,7 @@
     v1.3.0 and fixes a bugfix number v1.2.4. If necessary, modify the version number you've chosen to be consistent 
     with the content of the release.
   - Select whether this is a pre-release or a new "latest" release. It's a "pre-release" if there's an alpha, 
     beta, or release candidate number in the tag name, otherwise it's a new "latest" release.
   - Click on "Publish release"
 - GitHub actions will run to create and publish the PyPI and Anaconda packages, and publish the documentation. Check in 
   GitHub actions whether they run without errors and fix any errors which occur.
-
```

