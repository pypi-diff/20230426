# Comparing `tmp/shiny_mdc-1.5.1.tar.gz` & `tmp/shiny_mdc-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiny_mdc-1.5.1.tar", max compression
+gzip compressed data, was "shiny_mdc-1.5.2.tar", max compression
```

## Comparing `shiny_mdc-1.5.1.tar` & `shiny_mdc-1.5.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5210 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1082 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/LICENSE
--rw-r--r--   0        0        0       78 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/README.md
--rw-r--r--   0        0        0     2297 2023-04-20 04:57:43.432761 shiny_mdc-1.5.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/__init__.py
--rw-r--r--   0        0        0     1061 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_latexmk.py
--rw-r--r--   0        0        0     1867 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_liquid.py
--rw-r--r--   0        0        0     4643 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_pandoc.py
--rw-r--r--   0        0        0     5084 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/_templates.py
--rw-r--r--   0        0        0       64 2023-04-20 04:57:43.432761 shiny_mdc-1.5.1/shinymdc/_version.py
--rw-r--r--   0        0        0      410 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/addappendices.tex
--rw-r--r--   0        0        0      879 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetup.tex
--rw-r--r--   0        0        0      316 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetupshort.tex
--rw-r--r--   0        0        0      572 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/dynamic/dblfloatsetup.tex
--rw-r--r--   0        0        0      491 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibnonatsetup.tex
--rw-r--r--   0        0        0      324 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibnosupersetup.tex
--rw-r--r--   0        0        0      745 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/bibsupersetup.tex
--rw-r--r--   0        0        0     3359 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/floatsetup.tex
--rw-r--r--   0        0        0    19901 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/bibstyle.bst
--rw-r--r--   0        0        0     9433 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/esopic.sty
--rw-r--r--   0        0        0     3869 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/everyshi.sty
--rw-r--r--   0        0        0     8276 2023-04-20 04:57:19.084680 shiny_mdc-1.5.1/shinymdc/resources/static/iccv/iccv.sty
--rw-r--r--   0        0        0    26973 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/bibstyle.bst
--rw-r--r--   0        0        0     9153 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/iclr.sty
--rw-r--r--   0        0        0    12284 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/iclr/mathcommands.tex
--rw-r--r--   0        0        0    27146 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/icml/bibstyle.bst
--rw-r--r--   0        0        0    27887 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/icml/icml.sty
--rw-r--r--   0        0        0      735 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/mathsetup.tex
--rw-r--r--   0        0        0     1237 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/miscsetup.tex
--rw-r--r--   0        0        0    11306 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/neurips/neurips.sty
--rw-r--r--   0        0        0      406 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/resources/static/reqsetup.tex
--rw-r--r--   0        0        0    19208 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/shinymdc.py
--rw-r--r--   0        0        0      945 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/basic.tex
--rw-r--r--   0        0        0     1302 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/iccv.tex
--rw-r--r--   0        0        0     1423 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/iclr.tex
--rw-r--r--   0        0        0     2170 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/icml.tex
--rw-r--r--   0        0        0      916 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/neurips.tex
--rw-r--r--   0        0        0     3064 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/spacious.tex
--rw-r--r--   0        0        0      464 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/standalone.tex
--rw-r--r--   0        0        0     2281 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/shinymdc/templates/stylish.tex
--rw-r--r--   0        0        0    15953 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/anscombe.pdf
--rw-r--r--   0        0        0    40892 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/densities.pdf
--rw-r--r--   0        0        0    10736 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/diamonds.pdf
--rw-r--r--   0        0        0   197017 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/gaussian2d.pdf
--rw-r--r--   0        0        0    28282 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/figures/lines.png
--rw-r--r--   0        0        0     2971 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/main.md
--rwxr-xr-x   0        0        0      315 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/make.sh
--rw-r--r--   0        0        0     1166 2023-04-20 04:57:19.088681 shiny_mdc-1.5.1/test/references.bib
--rw-r--r--   0        0        0   690901 2023-04-20 04:57:19.092681 shiny_mdc-1.5.1/test/samples/basic.pdf
--rw-r--r--   0        0        0   414185 2023-04-20 04:57:19.096681 shiny_mdc-1.5.1/test/samples/iccv.pdf
--rw-r--r--   0        0        0   407653 2023-04-20 04:57:19.096681 shiny_mdc-1.5.1/test/samples/iclr.pdf
--rw-r--r--   0        0        0   446740 2023-04-20 04:57:19.100681 shiny_mdc-1.5.1/test/samples/icml.pdf
--rw-r--r--   0        0        0   451322 2023-04-20 04:57:19.100681 shiny_mdc-1.5.1/test/samples/neurips.pdf
--rw-r--r--   0        0        0   600276 2023-04-20 04:57:19.104681 shiny_mdc-1.5.1/test/samples/spacious.pdf
--rw-r--r--   0        0        0   555527 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/samples/standalone.pdf
--rw-r--r--   0        0        0   425326 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/samples/stylish.pdf
--rw-r--r--   0        0        0     1535 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/appendix1.md
--rw-r--r--   0        0        0     1624 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/appendix2.md
--rw-r--r--   0        0        0        0 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/empty.md
--rw-r--r--   0        0        0     2326 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/main1.md
--rw-r--r--   0        0        0     1351 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/sections/main2.md
--rw-r--r--   0        0        0      992 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/utils/commands.md
--rw-r--r--   0        0        0       41 2023-04-20 04:57:19.108682 shiny_mdc-1.5.1/test/utils/ext.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     5458 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1082 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/LICENSE
+-rw-r--r--   0        0        0       78 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/README.md
+-rw-r--r--   0        0        0     2297 2023-04-26 04:13:25.928233 shiny_mdc-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/__init__.py
+-rw-r--r--   0        0        0     1061 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/_latexmk.py
+-rw-r--r--   0        0        0     1867 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/_liquid.py
+-rw-r--r--   0        0        0     4643 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/_pandoc.py
+-rw-r--r--   0        0        0     5084 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/_templates.py
+-rw-r--r--   0        0        0       64 2023-04-26 04:13:25.928233 shiny_mdc-1.5.2/shinymdc/_version.py
+-rw-r--r--   0        0        0      410 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/dynamic/addappendices.tex
+-rw-r--r--   0        0        0      879 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/dynamic/authsetup.tex
+-rw-r--r--   0        0        0      316 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/dynamic/authsetupshort.tex
+-rw-r--r--   0        0        0      572 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/dynamic/dblfloatsetup.tex
+-rw-r--r--   0        0        0      491 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/static/bibnonatsetup.tex
+-rw-r--r--   0        0        0      324 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/static/bibnosupersetup.tex
+-rw-r--r--   0        0        0      745 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/static/bibsupersetup.tex
+-rw-r--r--   0        0        0     3359 2023-04-26 04:13:07.284060 shiny_mdc-1.5.2/shinymdc/resources/static/floatsetup.tex
+-rw-r--r--   0        0        0    19901 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iccv/bibstyle.bst
+-rw-r--r--   0        0        0     9433 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iccv/esopic.sty
+-rw-r--r--   0        0        0     3869 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iccv/everyshi.sty
+-rw-r--r--   0        0        0     8276 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iccv/iccv.sty
+-rw-r--r--   0        0        0    26973 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iclr/bibstyle.bst
+-rw-r--r--   0        0        0     9153 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iclr/iclr.sty
+-rw-r--r--   0        0        0    12284 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/iclr/mathcommands.tex
+-rw-r--r--   0        0        0    27146 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/icml/bibstyle.bst
+-rw-r--r--   0        0        0    27887 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/icml/icml.sty
+-rw-r--r--   0        0        0      735 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/mathsetup.tex
+-rw-r--r--   0        0        0     1237 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/miscsetup.tex
+-rw-r--r--   0        0        0    11306 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/neurips/neurips.sty
+-rw-r--r--   0        0        0      406 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/resources/static/reqsetup.tex
+-rw-r--r--   0        0        0    19326 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/shinymdc.py
+-rw-r--r--   0        0        0      945 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/basic.tex
+-rw-r--r--   0        0        0     1302 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/iccv.tex
+-rw-r--r--   0        0        0     1423 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/iclr.tex
+-rw-r--r--   0        0        0     2170 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/icml.tex
+-rw-r--r--   0        0        0      916 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/neurips.tex
+-rw-r--r--   0        0        0     3064 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/spacious.tex
+-rw-r--r--   0        0        0      464 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/standalone.tex
+-rw-r--r--   0        0        0     2281 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/shinymdc/templates/stylish.tex
+-rw-r--r--   0        0        0    15953 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/figures/anscombe.pdf
+-rw-r--r--   0        0        0    40892 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/figures/densities.pdf
+-rw-r--r--   0        0        0    10736 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/figures/diamonds.pdf
+-rw-r--r--   0        0        0   197017 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/figures/gaussian2d.pdf
+-rw-r--r--   0        0        0    28282 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/figures/lines.png
+-rw-r--r--   0        0        0     2971 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/main.md
+-rwxr-xr-x   0        0        0      315 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/make.sh
+-rw-r--r--   0        0        0     1166 2023-04-26 04:13:07.288060 shiny_mdc-1.5.2/test/references.bib
+-rw-r--r--   0        0        0   690901 2023-04-26 04:13:07.292060 shiny_mdc-1.5.2/test/samples/basic.pdf
+-rw-r--r--   0        0        0   414185 2023-04-26 04:13:07.296060 shiny_mdc-1.5.2/test/samples/iccv.pdf
+-rw-r--r--   0        0        0   407653 2023-04-26 04:13:07.296060 shiny_mdc-1.5.2/test/samples/iclr.pdf
+-rw-r--r--   0        0        0   446740 2023-04-26 04:13:07.300060 shiny_mdc-1.5.2/test/samples/icml.pdf
+-rw-r--r--   0        0        0   451322 2023-04-26 04:13:07.300060 shiny_mdc-1.5.2/test/samples/neurips.pdf
+-rw-r--r--   0        0        0   600276 2023-04-26 04:13:07.304060 shiny_mdc-1.5.2/test/samples/spacious.pdf
+-rw-r--r--   0        0        0   555527 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/samples/standalone.pdf
+-rw-r--r--   0        0        0   425326 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/samples/stylish.pdf
+-rw-r--r--   0        0        0     1535 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/sections/appendix1.md
+-rw-r--r--   0        0        0     1624 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/sections/appendix2.md
+-rw-r--r--   0        0        0        0 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/sections/empty.md
+-rw-r--r--   0        0        0     2326 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/sections/main1.md
+-rw-r--r--   0        0        0     1351 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/sections/main2.md
+-rw-r--r--   0        0        0      992 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/utils/commands.md
+-rw-r--r--   0        0        0       41 2023-04-26 04:13:07.308060 shiny_mdc-1.5.2/test/utils/ext.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 shiny_mdc-1.5.2/PKG-INFO
```

### Comparing `shiny_mdc-1.5.1/CHANGELOG.md` & `shiny_mdc-1.5.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 All notable changes to this project will be documented in this file. See [standard-version](https://github.com/conventional-changelog/standard-version) for commit guidelines.
 
+### [1.5.2](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.5.1...v1.5.2) (2023-04-26)
+
+
+### Bug Fixes
+
+* handle metadata being absent ([a2f61a8](https://github.com/jayanthkoushik/shiny-mdc/commit/a2f61a81fc16fe4a1b527fee4a0a971c43c1366a))
+
 ### [1.5.1](https://github.com/jayanthkoushik/shiny-mdc/compare/v1.5.0...v1.5.1) (2023-04-20)
 
 
 ### Bug Fixes
 
 * fix spacing for citations, footnotes, and super/sub-scripts ([db84c5d](https://github.com/jayanthkoushik/shiny-mdc/commit/db84c5de40db26594876f6b83293ea6149aad10a))
 * prevent output during cleanup when in quiet mode ([d1193f0](https://github.com/jayanthkoushik/shiny-mdc/commit/d1193f06255165db99fd430836a631f7dadd2b12))
```

### Comparing `shiny_mdc-1.5.1/LICENSE` & `shiny_mdc-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/pyproject.toml` & `shiny_mdc-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shiny-mdc"
-version = "1.5.1"  # managed by `poetry-dynamic-versioning`
+version = "1.5.2"  # managed by `poetry-dynamic-versioning`
 description = "Tool to compile markdown files to tex/pdf using pandoc, latexmk"
 readme = "README.md"
 authors = ["Jayanth Koushik <mail@jkoushik.me>"]
 license = "MIT"
 repository = "https://github.com/jayanthkoushik/shinymdc"
 packages = [
   { include = "shinymdc" }
```

### Comparing `shiny_mdc-1.5.1/shinymdc/_latexmk.py` & `shiny_mdc-1.5.2/shinymdc/_latexmk.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/_liquid.py` & `shiny_mdc-1.5.2/shinymdc/_liquid.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/_pandoc.py` & `shiny_mdc-1.5.2/shinymdc/_pandoc.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/_templates.py` & `shiny_mdc-1.5.2/shinymdc/_templates.py`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/dynamic/authsetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/dynamic/authsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/dynamic/dblfloatsetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/dynamic/dblfloatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/bibsupersetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/static/bibsupersetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/floatsetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/static/floatsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/bibstyle.bst` & `shiny_mdc-1.5.2/shinymdc/resources/static/iccv/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/esopic.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/iccv/esopic.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/everyshi.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/iccv/everyshi.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iccv/iccv.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/iccv/iccv.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/bibstyle.bst` & `shiny_mdc-1.5.2/shinymdc/resources/static/iclr/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/iclr.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/iclr/iclr.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/iclr/mathcommands.tex` & `shiny_mdc-1.5.2/shinymdc/resources/static/iclr/mathcommands.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/icml/bibstyle.bst` & `shiny_mdc-1.5.2/shinymdc/resources/static/icml/bibstyle.bst`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/icml/icml.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/icml/icml.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/mathsetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/static/mathsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/miscsetup.tex` & `shiny_mdc-1.5.2/shinymdc/resources/static/miscsetup.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/resources/static/neurips/neurips.sty` & `shiny_mdc-1.5.2/shinymdc/resources/static/neurips/neurips.sty`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/shinymdc.py` & `shiny_mdc-1.5.2/shinymdc/shinymdc.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,14 +230,16 @@
             raise ValueError from None
 
         # Rest of the input data is the main body.
         body_md = "\n".join(input_lines_iter).strip()
 
         # Parse metadata from header.
         metadata = yaml.safe_load(header)
+        if metadata is None:
+            metadata = {}
         try:
             bib_path = Path(metadata["bibliography"])
         except KeyError:
             bib_path = None
 
         # Link authors to institutes using institute IDs. This is for templates
         # which don't use superscripts for author affiliations.
@@ -261,22 +263,22 @@
         if metadata.get("skipequal", False) is False:
             metadata["skipequal"] = (
                 sum(int(author.get("equalcontrib", False)) for author in authors) < 2
             )
 
         # Get the longest author name, email, and institute name.
         # This can be used by templates to align the author list.
-        metadata["longest_author_name"] = max(
-            (_a.get("name", "") for _a in authors), key=len
+        metadata["longest_author_name"] = (
+            max((_a.get("name", "") for _a in authors), key=len) if authors else 0
         )
-        metadata["longest_email"] = max(
-            (_a.get("email", "") for _a in authors), key=len
+        metadata["longest_email"] = (
+            max((_a.get("email", "") for _a in authors), key=len) if authors else 0
         )
-        metadata["longest_inst_name"] = max(
-            (_i.get("name", "") for _i in institutes), key=len
+        metadata["longest_inst_name"] = (
+            max((_i.get("name", "") for _i in institutes), key=len) if institutes else 0
         )
 
         ############################################################
 
         ## 2. Prepare input for first stage processing.
 
         # Create combined input for first stage processing.
```

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/basic.tex` & `shiny_mdc-1.5.2/shinymdc/templates/basic.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/iccv.tex` & `shiny_mdc-1.5.2/shinymdc/templates/iccv.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/iclr.tex` & `shiny_mdc-1.5.2/shinymdc/templates/iclr.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/icml.tex` & `shiny_mdc-1.5.2/shinymdc/templates/icml.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/neurips.tex` & `shiny_mdc-1.5.2/shinymdc/templates/neurips.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/spacious.tex` & `shiny_mdc-1.5.2/shinymdc/templates/spacious.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/shinymdc/templates/stylish.tex` & `shiny_mdc-1.5.2/shinymdc/templates/stylish.tex`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/figures/anscombe.pdf` & `shiny_mdc-1.5.2/test/figures/anscombe.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/figures/densities.pdf` & `shiny_mdc-1.5.2/test/figures/densities.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/figures/diamonds.pdf` & `shiny_mdc-1.5.2/test/figures/diamonds.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/figures/gaussian2d.pdf` & `shiny_mdc-1.5.2/test/figures/gaussian2d.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/figures/lines.png` & `shiny_mdc-1.5.2/test/figures/lines.png`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/main.md` & `shiny_mdc-1.5.2/test/main.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/references.bib` & `shiny_mdc-1.5.2/test/references.bib`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/basic.pdf` & `shiny_mdc-1.5.2/test/samples/basic.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/iccv.pdf` & `shiny_mdc-1.5.2/test/samples/iccv.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/iclr.pdf` & `shiny_mdc-1.5.2/test/samples/iclr.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/icml.pdf` & `shiny_mdc-1.5.2/test/samples/icml.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/neurips.pdf` & `shiny_mdc-1.5.2/test/samples/neurips.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/spacious.pdf` & `shiny_mdc-1.5.2/test/samples/spacious.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/standalone.pdf` & `shiny_mdc-1.5.2/test/samples/standalone.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/samples/stylish.pdf` & `shiny_mdc-1.5.2/test/samples/stylish.pdf`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/sections/appendix1.md` & `shiny_mdc-1.5.2/test/sections/appendix1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/sections/appendix2.md` & `shiny_mdc-1.5.2/test/sections/appendix2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/sections/main1.md` & `shiny_mdc-1.5.2/test/sections/main1.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/sections/main2.md` & `shiny_mdc-1.5.2/test/sections/main2.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/test/utils/commands.md` & `shiny_mdc-1.5.2/test/utils/commands.md`

 * *Files identical despite different names*

### Comparing `shiny_mdc-1.5.1/PKG-INFO` & `shiny_mdc-1.5.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shiny-mdc
-Version: 1.5.1
+Version: 1.5.2
 Summary: Tool to compile markdown files to tex/pdf using pandoc, latexmk
 Home-page: https://github.com/jayanthkoushik/shinymdc
 License: MIT
 Author: Jayanth Koushik
 Author-email: mail@jkoushik.me
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

